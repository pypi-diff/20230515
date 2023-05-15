# Comparing `tmp/robotcode_core-0.37.1.tar.gz` & `tmp/robotcode_core-0.38.0.tar.gz`

## Comparing `robotcode_core-0.37.1.tar` & `robotcode_core-0.38.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/__version__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/async_cache.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/async_itertools.py
--rw-r--r--   0        0        0    21484 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/async_tools.py
--rw-r--r--   0        0        0    15625 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/dataclasses.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/event.py
--rw-r--r--   0        0        0    15842 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/logging.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/py.typed
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/types.py
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/uri.py
--rw-r--r--   0        0        0   233349 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/lsp/types.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/utils/debugpy.py
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/utils/glob_path.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/utils/inspect.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/utils/net.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/utils/path.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/utils/safe_eval.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/src/robotcode/core/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/LICENSE.txt
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/README.md
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/pyproject.toml
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 robotcode_core-0.37.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/__version__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/async_cache.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/async_itertools.py
+-rw-r--r--   0        0        0    21626 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/async_tools.py
+-rw-r--r--   0        0        0    15597 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/dataclasses.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/event.py
+-rw-r--r--   0        0        0    15831 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/logging.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/py.typed
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/types.py
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/uri.py
+-rw-r--r--   0        0        0   233349 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/lsp/types.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/utils/debugpy.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/utils/glob_path.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/utils/inspect.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/utils/net.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/utils/path.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/utils/safe_eval.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/src/robotcode/core/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/LICENSE.txt
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/README.md
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/pyproject.toml
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 robotcode_core-0.38.0/PKG-INFO
```

### Comparing `robotcode_core-0.37.1/src/robotcode/core/async_cache.py` & `robotcode_core-0.38.0/src/robotcode/core/async_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.37.1/src/robotcode/core/async_itertools.py` & `robotcode_core-0.38.0/src/robotcode/core/async_itertools.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.37.1/src/robotcode/core/async_tools.py` & `robotcode_core-0.38.0/src/robotcode/core/async_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import asyncio
+import atexit
 import concurrent.futures
 import contextvars
 import functools
 import inspect
 import threading
 import time
 import warnings
@@ -264,14 +265,21 @@
         raise asyncio.CancelledError
     return True
 
 
 __executor = ThreadPoolExecutor(thread_name_prefix="global_sub_asyncio")
 
 
+def shutdown_thread_pool_executor() -> None:
+    __executor.shutdown(wait=False)
+
+
+atexit.register(shutdown_thread_pool_executor)
+
+
 def run_in_thread(func: Callable[..., _T], /, *args: Any, **kwargs: Any) -> asyncio.Future[_T]:
     loop = asyncio.get_running_loop()
 
     ctx = contextvars.copy_context()
     func_call = functools.partial(ctx.run, func, *args, **kwargs)
 
     return cast(
@@ -519,15 +527,15 @@
                     while not done.is_set():
                         if time.monotonic() - start > 120:
                             warnings.warn("Can't set future result.")
                             break
 
                         time.sleep(0.001)
         else:
-            warnings.warn(f"Future {repr(fut)} loop is closed")
+            warnings.warn(f"Future {fut!r} loop is closed")
             self._waiters.remove(fut)
             self._wake_up_first()
 
 
 class RLock(Lock):
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `robotcode_core-0.37.1/src/robotcode/core/dataclasses.py` & `robotcode_core-0.38.0/src/robotcode/core/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             if value is not None or field.default == dataclasses.MISSING
         }
     if isinstance(o, enum.Enum):
         return o.value
     if isinstance(o, Set):
         return list(o)
 
-    raise TypeError(f"Cant' get default value for {type(o)} with value {repr(o)}")
+    raise TypeError(f"Cant' get default value for {type(o)} with value {o!r}")
 
 
 def as_json(obj: Any, indent: Optional[bool] = None, compact: Optional[bool] = None) -> str:
     return json.dumps(
         obj,
         default=__default,
         indent=4 if indent else None,
@@ -294,15 +294,15 @@
                 match_same_keys = same_keys
                 match_ = t
                 match_value = cased_value
                 match_signature = signature
                 match_type_hints = type_hints
             elif match_same_keys is not None and len(match_same_keys) == len(same_keys):
                 raise TypeError(
-                    f"Value {repr(value)} matches to more then one types of "
+                    f"Value {value!r} matches to more then one types of "
                     f"{repr(types[0].__name__) if len(types)==1 else ' | '.join(repr(e.__name__) for e in types)}."
                 )
 
         if (
             match_ is not None
             and match_value is not None
             and match_signature is not None
@@ -313,30 +313,30 @@
                 for k, v in match_value.items()
                 if k in match_type_hints
             }
 
             try:
                 return match_(**params)
             except TypeError as ex:
-                raise TypeError(f"Can't initialize class {repr(match_)} with parameters {repr(params)}.") from ex
+                raise TypeError(f"Can't initialize class {match_!r} with parameters {params!r}.") from ex
 
     for t in types:
         args = get_args(t)
         origin = get_origin(t)
 
         if (origin or t) is Literal:
             continue
 
         if issubclass(origin or t, enum.Enum):
             for v in cast(Iterable[Any], t):
                 if v.value == value:
                     return cast(_T, v)
 
     raise TypeError(
-        f"Cant convert value {repr(value)} of type {type(value).__name__} to type(s) "
+        f"Cant convert value {value!r} of type {type(value).__name__} to type(s) "
         + (
             repr(types[0])
             if len(types) == 1
             else " | ".join(
                 (
                     (getattr(e, "__name__", None) or str(e) if e is not type(None) else "None")
                     if get_origin(e) is not Literal
@@ -411,21 +411,21 @@
         self.class_ = target.__class__
         self.errors = errors
 
     def __repr__(self) -> str:
         cls = self.class_
         cls_name = f"{cls.__module__}.{cls.__name__}" if cls.__module__ != "__main__" else cls.__name__
         attrs = ", ".join([repr(v) for v in self.args])
-        return f"{cls_name}({attrs}, errors={repr(self.errors)})"
+        return f"{cls_name}({attrs}, errors={self.errors!r})"
 
     def __str__(self) -> str:
         cls = self.class_
         cls_name = f"{cls.__module__}.{cls.__name__}" if cls.__module__ != "__main__" else cls.__name__
         s = cls_name
-        return f"{s} (errors = {repr(self.errors)})"
+        return f"{s} (errors = {self.errors!r})"
 
 
 def validate_types(expected_types: Union[type, Tuple[type, ...], None], value: Any) -> List[str]:
     if expected_types is None:
         return []
 
     if not isinstance(expected_types, tuple):
```

### Comparing `robotcode_core-0.37.1/src/robotcode/core/event.py` & `robotcode_core-0.38.0/src/robotcode/core/event.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.37.1/src/robotcode/core/logging.py` & `robotcode_core-0.38.0/src/robotcode/core/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,15 @@
     @property
     def name(self) -> str:
         return self.logger.name
 
     def __repr__(self) -> str:
         logger = self.logger
         level = logging.getLevelName(logger.getEffectiveLevel())
-        return f"{self.__class__.__name__}(name={repr(logger.name)}, level={repr(level)})"
+        return f"{self.__class__.__name__}(name={logger.name!r}, level={level!r})"
 
     _call_tracing_enabled: ClassVar = (
         "ROBOT_CALL_TRACING_ENABLED" in os.environ and os.environ["ROBOT_CALL_TRACING_ENABLED"] != "0"
     )
     _call_tracing_default_level: ClassVar = (
         logging.getLevelName(os.environ["ROBOT_CALL_TRACING_LEVEL"])
         if "ROBOT_CALL_TRACING_LEVEL" in os.environ
@@ -434,15 +434,15 @@
                     message_args = wrapper_args[1:] if skip_first_arg else wrapper_args
 
                     return "{0}({1}{2}{3})".format(
                         func_name(),
                         ", ".join(_repr(a) for a in message_args),
                         (", " if len(message_args) > 0 and len(wrapper_kwargs) > 0 else ""),
                         (
-                            ", ".join(f"{str(k)}={_repr(v)}" for k, v in wrapper_kwargs.items())
+                            ", ".join(f"{k!s}={_repr(v)}" for k, v in wrapper_kwargs.items())
                             if len(wrapper_kwargs) > 0
                             else ""
                         ),
                     )
 
                 def build_exit_message(res: Any, duration: Optional[float]) -> str:
                     return "{0}(...) -> {1}{2}".format(
```

### Comparing `robotcode_core-0.37.1/src/robotcode/core/uri.py` & `robotcode_core-0.38.0/src/robotcode/core/uri.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
         self._path: Optional[Path] = None
 
     def __str__(self) -> str:
         return parse.urlunparse(tuple(self._parts))
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}({repr(parse.urlunparse(tuple(self._parts)))})"
+        return f"{type(self).__name__}({parse.urlunparse(tuple(self._parts))!r})"
 
     def to_path(self) -> Path:
         if self._path is None:
             self._path = Path(self._to_path_str())
 
         return self._path
 
@@ -108,15 +108,15 @@
         invalid characters and semantics. Will *not* look at the scheme of this URI.
         """
         # scheme://netloc/path;parameters?query#fragment
         netloc = parse.unquote(self.netloc)
         path = parse.unquote(self.path)
 
         if self._parts.scheme != "file":
-            raise InvalidUriError(f"Invalid URI scheme '{str(self)}'.")
+            raise InvalidUriError(f"Invalid URI scheme '{self!s}'.")
 
         if netloc and self._parts.scheme == "file":
             # unc path: file://shares/c$/far/boo
             value = "//{}{}".format(netloc, path or "")
 
         elif _RE_DRIVE_LETTER_PATH.match(path):
             # windows drive letter: file:///C:/far/boo
```

### Comparing `robotcode_core-0.37.1/src/robotcode/core/lsp/types.py` & `robotcode_core-0.38.0/src/robotcode/core/lsp/types.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.37.1/src/robotcode/core/utils/debugpy.py` & `robotcode_core-0.38.0/src/robotcode/core/utils/debugpy.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.37.1/src/robotcode/core/utils/glob_path.py` & `robotcode_core-0.38.0/src/robotcode/core/utils/glob_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             path = Path(path)
         return self._re_pattern.fullmatch(str(path).replace(os.sep, "/")) is not None
 
     def __str__(self) -> str:
         return self.pattern
 
     def __repr__(self) -> str:
-        return f"{type(self).__qualname__}(pattern={repr(self.pattern)}"
+        return f"{type(self).__qualname__}(pattern={self.pattern!r}"
 
 
 def globmatches(pattern: str, path: Union[Path, str, os.PathLike[Any]]) -> bool:
     return Pattern(pattern).matches(path)
 
 
 def iter_files(
```

### Comparing `robotcode_core-0.37.1/src/robotcode/core/utils/inspect.py` & `robotcode_core-0.38.0/src/robotcode/core/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.37.1/src/robotcode/core/utils/net.py` & `robotcode_core-0.38.0/src/robotcode/core/utils/net.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.37.1/src/robotcode/core/utils/safe_eval.py` & `robotcode_core-0.38.0/src/robotcode/core/utils/safe_eval.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.37.1/src/robotcode/core/utils/version.py` & `robotcode_core-0.38.0/src/robotcode/core/utils/version.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.37.1/.gitignore` & `robotcode_core-0.38.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.37.1/LICENSE.txt` & `robotcode_core-0.38.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.37.1/README.md` & `robotcode_core-0.38.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.37.1/pyproject.toml` & `robotcode_core-0.38.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.37.1/PKG-INFO` & `robotcode_core-0.38.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-core
-Version: 0.37.1
+Version: 0.38.0
 Summary: Some core classes for RobotCode
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
```

