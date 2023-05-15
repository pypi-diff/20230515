# Comparing `tmp/xtn-0.1.0.tar.gz` & `tmp/xtn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtn-0.1.0.tar", max compression
+gzip compressed data, was "xtn-0.1.1.tar", max compression
```

## Comparing `xtn-0.1.0.tar` & `xtn-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      458 2023-05-12 18:50:12.851964 xtn-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      505 2023-05-12 19:00:43.819253 xtn-0.1.0/README.md
--rw-r--r--   0        0        0      122 2023-05-12 15:09:11.486768 xtn-0.1.0/xtn/__init__.py
--rw-r--r--   0        0        0    12770 2023-05-12 14:35:04.885415 xtn-0.1.0/xtn/_xtn.py
--rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 xtn-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      458 2023-05-15 17:48:09.995708 xtn-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      575 2023-05-13 04:15:51.322967 xtn-0.1.1/README.md
+-rw-r--r--   0        0        0      122 2023-05-12 15:09:11.486768 xtn-0.1.1/xtn/__init__.py
+-rw-r--r--   0        0        0    13235 2023-05-15 17:54:47.956116 xtn-0.1.1/xtn/_xtn.py
+-rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 xtn-0.1.1/PKG-INFO
```

### Comparing `xtn-0.1.0/xtn/_xtn.py` & `xtn-0.1.1/xtn/_xtn.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     OBJECT_MUST_BE_ON_NEW_LINE = 1
     ARRAY_MUST_BE_ON_NEW_LINE = 2
     MULTILINE_MUST_BE_ON_NEW_LINE = 3
     LINE_MUST_NOT_START_WITH_COLON = 4
     PLUS_ENCOUNTERED_OUTSIDE_ARRAY = 5
     ARRAY_ELEMENT_MUST_START_WITH_PLUS = 6
     MULTILINE_MARKER_TOO_SHORT = 7
+    UNMATCHED_CLOSE_MARKER = 8
+    MISSING_CLOSE_MARKER = 9
 
 
 class XtnException(Exception):
     def __init__(self, code: XtnErrorCode, message: str, *args: object) -> None:
         super().__init__(message, *args)
         self.code = code
         self.message = message
@@ -56,17 +58,17 @@
 class XtnArray(XtnDataElement):
     def __init__(self, elements: list[XtnDataElement], comments: list[XtnComment] | None = None, trail_comments: list[XtnComment] | None = None) -> None:
         super().__init__(comments, trail_comments)
         self.elements = elements
 
 
 class XtnObject(XtnDataElement):
-    def __init__(self, elements: dict[str, XtnDataElement], comments: list[XtnComment] | None = None, trail_comments: list[XtnComment] | None = None) -> None:
+    def __init__(self, elements: dict[str, XtnDataElement] | None = None, comments: list[XtnComment] | None = None, trail_comments: list[XtnComment] | None = None) -> None:
         super().__init__(comments, trail_comments)
-        self.elements = elements
+        self.elements = {} if elements is None else elements
 
     @staticmethod
     def load(f: TextIO):
         obj = XtnObject({})
         _load(f, obj)
         return obj
 
@@ -110,15 +112,15 @@
                 if end:
                     write(indent, '----')
             elif isinstance(data, XtnText):
                 sv = data.value
                 lines = sv.splitlines()
                 if sv.endswith('\n'):
                     lines.append('')
-                if data.force_multiline or len(lines) > 1 or sv[0:1].isspace() or sv[-1:].isspace():
+                if data.force_multiline or len(lines) > 1 or sv[0:1].isspace() or sv[-1:].isspace() or any(m.group(0) != ' ' for m in re.finditer(r'\s', sv)):
                     marker_len = max((len(m.group(0)) for m in re.finditer(r'`+', sv)), default=0)
                     marker_len = min(marker_len, 4)
                     marker = (4 if marker_len < 3 else marker_len + (3 if marker_len % 2 == 1 else 4)) * "'"
                     write(indent, name, "'':")
                     child_indent = indent + '    '
                     write(child_indent, marker)
                     for line in lines:
@@ -232,14 +234,15 @@
             comments.clear()
 
     def attach_trailing_comments(target: XtnDataElement | None):
         if target is not None and comments is not None and len(comments) > 0:
             target.trail_comments = comments.copy()
             comments.clear()
 
+    i = -1
     for i, line in enumerate(f):
         state = stack[-1]
         if state.mode == _Mode.MULTILINE:
             if len(state.marker) == 0:
                 state.indent = len(line)
                 line = line.lstrip()
                 state.indent -= len(line)
@@ -318,13 +321,17 @@
                 child_target = state.set(left, right, raise_error)
                 attach_comments(child_target)
             else:
                 if state.mode == _Mode.OBJECT and state.in_array:
                     stack.pop()
                 attach_trailing_comments(stack[-1].target)
                 stack.pop()
-
+                if len(stack) == 0:
+                    raise_error(XtnErrorCode.UNMATCHED_CLOSE_MARKER, "The close marker ---- does not match any open object or array")
+    i += 1
+    if len(stack) > 1:
+        raise_error(XtnErrorCode.MISSING_CLOSE_MARKER, "A close marker ---- was expected")
     return top_level
 
 
 def load(f: TextIO):
     return _load(f, None)
```

### Comparing `xtn-0.1.0/PKG-INFO` & `xtn-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: xtn
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for working with the xtn format
 Home-page: https://github.com/koustubhmoharir/xtn
 License: MIT
 Author: Koustubh Moharir
 Author-email: koustubhmoharir@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
-# xtn
+## xtn Repository
 
-Sample code
+[On Github](https://github.com/koustubhmoharir/xtn)
+
+## Sample code
 ```
 import xtn
 
 # reads the data in the file (without comments) into a dict with key value pairs, the values can be dict, list, str
 with open(r'path/to/file.xtn', 'r') as f:
     data = xtn.load(f)
```

