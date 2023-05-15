# Comparing `tmp/dictdot-1.4.0-py3-none-any.whl.zip` & `tmp/dictdot-1.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 15083 bytes, number of entries: 6
--rw-r--r--  2.0 unx     2600 b- defN 22-Feb-28 17:06 dictdot/__init__.py
--rw-r--r--  2.0 unx    35149 b- defN 22-Feb-28 17:08 dictdot-1.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1549 b- defN 22-Feb-28 17:08 dictdot-1.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Feb-28 17:08 dictdot-1.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 22-Feb-28 17:08 dictdot-1.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      462 b- defN 22-Feb-28 17:08 dictdot-1.4.0.dist-info/RECORD
-6 files, 39860 bytes uncompressed, 14249 bytes compressed:  64.3%
+Zip file size: 4250 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     5149 b- defN 23-May-14 23:50 dictdot/__init__.py
+-rw-r--r--  2.0 unx     1060 b- defN 23-May-15 00:02 dictdot-1.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1722 b- defN 23-May-15 00:02 dictdot-1.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 00:02 dictdot-1.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-15 00:02 dictdot-1.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      461 b- defN 23-May-15 00:02 dictdot-1.5.0.dist-info/RECORD
+6 files, 8492 bytes uncompressed, 3416 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dictdot/__init__.py
 Comment: 
 
-Filename: dictdot-1.4.0.dist-info/LICENSE
+Filename: dictdot-1.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: dictdot-1.4.0.dist-info/METADATA
+Filename: dictdot-1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: dictdot-1.4.0.dist-info/WHEEL
+Filename: dictdot-1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: dictdot-1.4.0.dist-info/top_level.txt
+Filename: dictdot-1.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dictdot-1.4.0.dist-info/RECORD
+Filename: dictdot-1.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dictdot/__init__.py

```diff
@@ -1,100 +1,175 @@
-"""Python dict accessible by dot."""
 import re
 
 
-class dictdot(dict):
-    """Usage:
+# Helper functions.
 
-    from dictdot import dictdot
 
-    d = dictdot()
+def _is_valid_dot_key(s):
+    """
+    Return True if `s` can be used to access a `dictdot` key by dot notation.
+    """
+    return (
+        s
+        and type(s) is str
+        and re.sub(r"\w", "", s) == ""
+        and not s[0].isdigit()
+        and s not in dictdot.__dict__
+    )
 
-    d["a"] = 1
-    assert d["a"] == d.a
 
-    d.b = 2
-    assert d["b"] == d.b
+def _build_path(*args):
+    """
+    Concatenate `args` to create a valid "path" to access a `dictdot` element.
+    """
+    result = ""
+    for x in args:
+        if isinstance(x, str):
+            if _is_valid_dot_key(x):
+                result += f".{x}"
+            else:
+                x = x.replace('"', r"\"")
+                result += f'["{x}"]'
+        else:
+            result += f"[{x}]"
+    return result
 
-    # builtin attributes are not overriden.
-    d.items = "foo"
-    assert d.items != d["items"]
-    assert hasattr(d.items, "__call__")
 
-    # d["NA"] will raise KeyError, but
-    assert d.NA is None
+def _true(x):
+    return True
 
-    # delete by attribute name.
-    del d.b
-    assert "b" not in d.keys()
 
-    # `copy` method returns a dictdot.
-    d2 = d.copy()
-    assert d2 == d
-    assert type(d2) is dictdot
+_func = type(_true)
 
-    # nested dicts are also dictdot.
-    d = dictdot(
-        a={"x": 0},
-        b=[{"y": 1}],
-    )
-    assert d.a.x == d.a["x"] == d["a"].x
-    assert d.b[0].y == d["b"][0]["y"]
 
-    # even when added after init. non-dict values are not modified.
-    d.c = [{"z": 2}, 2]
-    assert d.c[0].z == d.c[1]
-
-    # recursive dicts still work.
-    d.c.append(d)
-    assert d == d.c[-1] == d.c[-1].c[-1]
-
-    # keys with not allowed characters may still be found with "_".
-    d["test-key"] = "hyphen"
-    assert d.test_key == "hyphen"
-    # order matters.
-    d["test.key"] = "dot"
-    assert d.test_key == "hyphen"
-    # but verbatim keys always win.
-    d["test_key"] = "underscore"
-    assert d.test_key == "underscore"
-    """
+# Main class.
 
-    __delattr__ = dict.__delitem__
 
-    def __getattr__(self, name):
-        """
-        If `name` is not a verbatim key in `self`, try to find the first key
-        that matches a regex that considers "_"s in `name` as masking chars for
-        "." or "-", and "_" as well.
-        """
-        if name in self.keys():
-            return dict.get(self, name)
-        else:
-            pattern = re.compile(name.replace("_", r"[\.|\-|_]"))
-            keys = [k for k in self.keys() if pattern.findall(k)]
-            if len(keys) == 0:
-                return None
-            else:
-                return dict.get(self, keys[0])
+class dictdot(dict):
+    """
+    Python dict accessible by dot. For example:
 
-    def __setitem__(self, name, value):
-        return dict.__setitem__(self, name, self._add(value))
+        from dictdot import dictdot
 
-    def __setattr__(self, name, value):
-        return self.__setitem__(name, value)
+        d = dictdot({"foo": 1})
+        d.bar = 1
+        assert d.foo == d["bar"]
+
+    """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         for k, v in self.items():
             self[k] = self._add(v)
 
     def _add(self, value):
-        if type(value) is dict:
+        """Convert dicts nested in `value` into `dictdot`."""
+        if isinstance(value, dict):
             return self.__class__(value)
-        elif type(value) in [list, tuple]:
+        elif isinstance(value, (list, tuple)):
             return [self._add(v) for v in value]
         else:
             return value
 
     def copy(self):
-        return self.__class__(dict.copy(self))
+        return self.__class__(super().copy())
+
+    def as_dict(self):
+        """Convert `self` and nested `dictdot` objects into regular dicts."""
+        return self._as_dict_recursive(self)
+
+    @staticmethod
+    def _as_dict_recursive(value):
+        if isinstance(value, dictdot):
+            return {k: dictdot._as_dict_recursive(v) for k, v in value.items()}
+        elif isinstance(value, list):
+            return [dictdot._as_dict_recursive(v) for v in value]
+        else:
+            return value
+
+    @staticmethod
+    def find(it, *, max_depth=0, check_key=_true, check_value=_true, prev=None):
+        """
+        Recursively examine `it` and yield its (nested) paths that contain keys
+        and values that return True when passed as arguments to the functions
+        `check_key` and `check_value`, respectively. The "paths" found by this
+        function are returned as strings, hence they are not meant to be used
+        programatically.
+
+        By default `check_key` and `check_value` always return True.
+
+        If `check_key` (or `check_value`) is an explicit function, then it will
+        be applied to each key (or value).
+
+        If `check_key` (or `check_value`) is not a function, then it will be
+        replaced by a function that checks that the passed argument is equal to
+        the proived `check_key` (or `check_value`). Then, `check_key="3.14"` is
+        a shortcut for `check_key=lambda x: x == "3.14"`.
+        """
+        if prev is None:
+            prev = []
+        if max_depth and len(prev) >= max_depth:
+            return
+        if type(check_key) != _func:
+            _key = check_key
+            check_key = lambda x: x == _key
+        if type(check_value) != _func:
+            _value = check_value
+            check_value = lambda x: x == _value
+
+        if isinstance(it, dict):
+            for k, v in it.items():
+                if check_key(k) and check_value(v):
+                    yield _build_path(*prev, k)
+                yield from dictdot.find(
+                    v,
+                    check_key=check_key,
+                    check_value=check_value,
+                    prev=[*prev, k],
+                    max_depth=max_depth,
+                )
+        elif isinstance(it, (list, tuple)):
+            for i, x in enumerate(it):
+                if prev and check_key(prev[-1]) and check_value(x):
+                    yield _build_path(*prev, i)
+                yield from dictdot.find(
+                    x,
+                    check_key=check_key,
+                    check_value=check_value,
+                    prev=[*prev, i],
+                    max_depth=max_depth,
+                )
+
+    # Methods to handle items.
+
+    def __setitem__(self, name, value):
+        return super().__setitem__(name, self._add(value))
+
+    def __setattr__(self, name, value):
+        return self.__setitem__(name, value)
+
+    def __delattr__(self, name):
+        return super().__delitem__(name)
+
+    def __getattr__(self, name):
+        """
+        If `name` is not a verbatim key of `self`, try to find the first key
+        that matches the regex that uses "_"s in `name` as masking characters
+        for "." and "-".
+        """
+        if name in self:
+            return self[name]
+        else:
+            pattern = re.compile("^" + name.replace("_", r"[\.|\-]") + "$")
+            keys = [k for k in self.keys() if pattern.findall(k)]
+            if keys:
+                return self[keys[0]]
+            else:
+                return None
+
+    # For pickling.
+
+    def __getstate__(self):
+        return self.as_dict()
+
+    def __setstate__(self, state):
+        self.update(state)
```

