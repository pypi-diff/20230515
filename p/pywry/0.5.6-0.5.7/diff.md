# Comparing `tmp/pywry-0.5.6.tar.gz` & `tmp/pywry-0.5.7.tar.gz`

## Comparing `pywry-0.5.6.tar` & `pywry-0.5.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 pywry-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 pywry-0.5.6/rust_src/pywry/Cargo.toml
--rw-r--r--   0     1001      123     1063 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/LICENSE
--rw-r--r--   0     1001      123     4920 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/README.md
--rw-r--r--   0     1001      123     3565 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/constants.rs
--rw-r--r--   0     1001      123     6158 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/events.rs
--rw-r--r--   0     1001      123     3733 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/handlers.rs
--rw-r--r--   0     1001      123     5780 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/headless.rs
--rw-r--r--   0     1001      123     1571 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/lib.rs
--rw-r--r--   0     1001      123      975 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/pipe.rs
--rw-r--r--   0     1001      123     7516 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/structs.rs
--rw-r--r--   0     1001      123     1366 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/utils.rs
--rw-r--r--   0     1001      123     6168 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/window.rs
--rw-r--r--   0     1001      123    63815 2023-05-15 19:22:25.000000 pywry-0.5.6/Cargo.lock
--rw-r--r--   0     1001      123     1155 2023-05-15 19:22:25.000000 pywry-0.5.6/python/pywry/backend.py
--rw-r--r--   0     1001      123        0 2023-05-15 19:22:25.000000 pywry-0.5.6/python/pywry/py.typed
--rw-r--r--   0     1001      123      180 2023-05-15 19:22:25.000000 pywry-0.5.6/python/pywry/__init__.py
--rw-r--r--   0     1001      123    14307 2023-05-15 19:22:25.000000 pywry-0.5.6/python/pywry/core.py
--rw-r--r--   0     1001      123      217 2023-05-15 19:22:25.000000 pywry-0.5.6/python/pywry/pywry.pyi
--rw-r--r--   0     1001      123      733 2023-05-15 19:22:25.000000 pywry-0.5.6/Cargo.toml
--rw-r--r--   0     1001      123     3565 2023-05-15 19:22:25.000000 pywry-0.5.6/src/constants.rs
--rw-r--r--   0     1001      123     6158 2023-05-15 19:22:25.000000 pywry-0.5.6/src/events.rs
--rw-r--r--   0     1001      123     3733 2023-05-15 19:22:25.000000 pywry-0.5.6/src/handlers.rs
--rw-r--r--   0     1001      123     5780 2023-05-15 19:22:25.000000 pywry-0.5.6/src/headless.rs
--rw-r--r--   0     1001      123     1571 2023-05-15 19:22:25.000000 pywry-0.5.6/src/lib.rs
--rw-r--r--   0     1001      123      975 2023-05-15 19:22:25.000000 pywry-0.5.6/src/pipe.rs
--rw-r--r--   0     1001      123     7516 2023-05-15 19:22:25.000000 pywry-0.5.6/src/structs.rs
--rw-r--r--   0     1001      123     1366 2023-05-15 19:22:25.000000 pywry-0.5.6/src/utils.rs
--rw-r--r--   0     1001      123     6168 2023-05-15 19:22:25.000000 pywry-0.5.6/src/window.rs
--rw-r--r--   0        0        0     5522 1970-01-01 00:00:00.000000 pywry-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 pywry-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 pywry-0.5.7/rust_src/pywry/Cargo.toml
+-rw-r--r--   0     1001      123     1063 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/LICENSE
+-rw-r--r--   0     1001      123     4924 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/README.md
+-rw-r--r--   0     1001      123     3565 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/constants.rs
+-rw-r--r--   0     1001      123     6202 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/events.rs
+-rw-r--r--   0     1001      123     3733 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/handlers.rs
+-rw-r--r--   0     1001      123     5780 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/headless.rs
+-rw-r--r--   0     1001      123     1571 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/lib.rs
+-rw-r--r--   0     1001      123      975 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/pipe.rs
+-rw-r--r--   0     1001      123     7516 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/structs.rs
+-rw-r--r--   0     1001      123     1366 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/utils.rs
+-rw-r--r--   0     1001      123     6168 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/window.rs
+-rw-r--r--   0     1001      123    63815 2023-05-15 20:19:25.000000 pywry-0.5.7/Cargo.lock
+-rw-r--r--   0     1001      123     1155 2023-05-15 20:19:25.000000 pywry-0.5.7/python/pywry/backend.py
+-rw-r--r--   0     1001      123        0 2023-05-15 20:19:25.000000 pywry-0.5.7/python/pywry/py.typed
+-rw-r--r--   0     1001      123      180 2023-05-15 20:19:25.000000 pywry-0.5.7/python/pywry/__init__.py
+-rw-r--r--   0     1001      123    14417 2023-05-15 20:19:25.000000 pywry-0.5.7/python/pywry/core.py
+-rw-r--r--   0     1001      123      217 2023-05-15 20:19:25.000000 pywry-0.5.7/python/pywry/pywry.pyi
+-rw-r--r--   0     1001      123      733 2023-05-15 20:19:25.000000 pywry-0.5.7/Cargo.toml
+-rw-r--r--   0     1001      123     3565 2023-05-15 20:19:25.000000 pywry-0.5.7/src/constants.rs
+-rw-r--r--   0     1001      123     6202 2023-05-15 20:19:25.000000 pywry-0.5.7/src/events.rs
+-rw-r--r--   0     1001      123     3733 2023-05-15 20:19:25.000000 pywry-0.5.7/src/handlers.rs
+-rw-r--r--   0     1001      123     5780 2023-05-15 20:19:25.000000 pywry-0.5.7/src/headless.rs
+-rw-r--r--   0     1001      123     1571 2023-05-15 20:19:25.000000 pywry-0.5.7/src/lib.rs
+-rw-r--r--   0     1001      123      975 2023-05-15 20:19:25.000000 pywry-0.5.7/src/pipe.rs
+-rw-r--r--   0     1001      123     7516 2023-05-15 20:19:25.000000 pywry-0.5.7/src/structs.rs
+-rw-r--r--   0     1001      123     1366 2023-05-15 20:19:25.000000 pywry-0.5.7/src/utils.rs
+-rw-r--r--   0     1001      123     6168 2023-05-15 20:19:25.000000 pywry-0.5.7/src/window.rs
+-rw-r--r--   0        0        0     5526 1970-01-01 00:00:00.000000 pywry-0.5.7/PKG-INFO
```

### Comparing `pywry-0.5.6/pyproject.toml` & `pywry-0.5.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pywry"
-version = "0.5.6"
-requires-python = ">=3.9"
+version = "0.5.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: POSIX",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
@@ -29,15 +29,15 @@
 
 [project.optional-dependencies]
 dev = ["auditwheel", "wheel"]
 
 
 [tool.ruff]
 line-length = 122
-target-version = "py39"
+target-version = "py38"
 
 [tool.ruff.isort]
 combine-as-imports = true
 force-wrap-aliases = true
 
 [tool.ruff.pylint]
 max-args=8
```

### Comparing `pywry-0.5.6/rust_src/pywry/Cargo.toml` & `pywry-0.5.7/rust_src/pywry/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.6"
+version = "0.5.7"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.5.6/rust_src/pywry/LICENSE` & `pywry-0.5.7/rust_src/pywry/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 OpenBB
+Copyright (c) 2023 OpenBB
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pywry-0.5.6/rust_src/pywry/README.md` & `pywry-0.5.7/rust_src/pywry/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,21 +58,21 @@
 ## JSON Keys
 
 PyWry uses a JSON object to communicate between the python and rust backends and the javascript
 frontend. The following keys are available:
 
 | Key | Type | Description |
 | --- | --- | --- |
-| `html` | `Path | str` | The path to the HTML file to be loaded, or HTML string. |
+| `html` | `Path \| str` | The path to the HTML file to be loaded, or HTML string. |
 | `title` | `str` | The title of the window. |
-| `icon` | `str | Path` | The path to `png` icon to be used for the window. |
-| `json_data` | `str | dict` | A JSON string or dictionary to be passed to the javascript frontend. (see below) |
+| `icon` | `str \| Path` | The path to `png` icon to be used for the window. |
+| `json_data` | `str \| dict` | A JSON string or dictionary to be passed to the javascript frontend. (see below) |
 | `height` | `int` | The height of the window. |
 | `width` | `int` | The width of the window. |
-| `download_path` | `str | Path` | The path to the download directory. |
+| `download_path` | `str \| Path` | The path to the download directory. |
 
 ## Javascript
 
 PyWry allows you to run javascript in the frontend. To do this, you can pass a dictionary
 of data to the `json_data` key in the `send_html` method. This dictionary will be converted
 to a JSON string and passed to the frontend. You can then access this data in the frontend
 by using the `window.json_data` object. For example:
```

### Comparing `pywry-0.5.6/rust_src/pywry/src/constants.rs` & `pywry-0.5.7/rust_src/pywry/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/rust_src/pywry/src/events.rs` & `pywry-0.5.7/rust_src/pywry/src/events.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 use crate::{
 	structs::{ConsolePrinter, PlotData, UserEvent},
-	utils::decode_path,
 };
 
+#[cfg(not(target_os = "macos"))]
+use crate::utils::decode_path;
+
 use std::{
 	collections::HashMap,
 	io::{self, Write},
 	path::PathBuf,
 };
 
 #[cfg(not(target_os = "macos"))]
```

### Comparing `pywry-0.5.6/rust_src/pywry/src/handlers.rs` & `pywry-0.5.7/rust_src/pywry/src/handlers.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/rust_src/pywry/src/headless.rs` & `pywry-0.5.7/rust_src/pywry/src/headless.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/rust_src/pywry/src/lib.rs` & `pywry-0.5.7/rust_src/pywry/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/rust_src/pywry/src/pipe.rs` & `pywry-0.5.7/rust_src/pywry/src/pipe.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/rust_src/pywry/src/structs.rs` & `pywry-0.5.7/rust_src/pywry/src/structs.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/rust_src/pywry/src/utils.rs` & `pywry-0.5.7/rust_src/pywry/src/utils.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/rust_src/pywry/src/window.rs` & `pywry-0.5.7/rust_src/pywry/src/window.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/Cargo.lock` & `pywry-0.5.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1513,15 +1513,15 @@
 checksum = "a915bd72824962bf190bbd3e8a044cccb695d1409f73ff5493712eda5136c7a8"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pywry"
-version = "0.5.6"
+version = "0.5.7"
 dependencies = [
  "image",
  "mime_guess",
  "open",
  "pyo3",
  "serde",
  "serde_json",
```

### Comparing `pywry-0.5.6/python/pywry/backend.py` & `pywry-0.5.7/python/pywry/backend.py`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/python/pywry/core.py` & `pywry-0.5.7/python/pywry/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 
 import setproctitle
 
 from pywry import pywry
 
 __all__ = ["PyWry", "BackendFailedToStart"]
 
+if sys.version_info < (3, 9):
+    QueueT = Queue
+else:
+    QueueT = Queue[dict]
+
 AsyncioException = (
     CancelledError,
     IncompleteReadError,
     TimeoutError,
     ConnectionResetError,
 )
 
@@ -62,15 +67,15 @@
     _bootargs: List[str] = []
 
     daemon: bool = True
     debug: bool = False
     shell: bool = False
     outgoing: List[str] = []
     init_engine: List[str] = []
-    recv: Queue[dict] = Queue()
+    recv: QueueT = Queue()
     base: pywry.WindowManager = pywry.WindowManager()
 
     def __new__(cls, *args, **kwargs):  # pylint: disable=unused-argument
         "Makes the class a 'singleton' by only allowing one instance at a time"
         if not hasattr(cls, "instance"):
             cls.instance = super().__new__(cls)
         return cls.instance
@@ -105,27 +110,27 @@
     def __del__(self):
         if self._is_started.is_set():
             self.close()
 
     def send_html(
         self,
         html: Union[str, Path],
-        json_data: Optional[dict] = None,
+        json_data: Optional[Union[dict, str]] = None,
         title: str = "",
         width: int = 800,
         height: int = 600,
         **kwargs,
     ):
         """Send html to backend.
 
         Parameters
         ----------
         html: Union[str, Path]
             HTML to send to backend.
-        json_data : dict, optional
+        json_data : Optional[Union[dict, str]], optional
             JSON data to send to backend, by default None
         title : str, optional
             Title to display in the window, by default ""
         width : int, optional
             Width of the window, by default 800
         height : int, optional
             Height of the window, by default 600
```

### Comparing `pywry-0.5.6/Cargo.toml` & `pywry-0.5.7/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.6"
+version = "0.5.7"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.5.6/src/constants.rs` & `pywry-0.5.7/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/src/events.rs` & `pywry-0.5.7/src/events.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 use crate::{
 	structs::{ConsolePrinter, PlotData, UserEvent},
-	utils::decode_path,
 };
 
+#[cfg(not(target_os = "macos"))]
+use crate::utils::decode_path;
+
 use std::{
 	collections::HashMap,
 	io::{self, Write},
 	path::PathBuf,
 };
 
 #[cfg(not(target_os = "macos"))]
```

### Comparing `pywry-0.5.6/src/handlers.rs` & `pywry-0.5.7/src/handlers.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/src/headless.rs` & `pywry-0.5.7/src/headless.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/src/lib.rs` & `pywry-0.5.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/src/pipe.rs` & `pywry-0.5.7/src/pipe.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/src/structs.rs` & `pywry-0.5.7/src/structs.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/src/utils.rs` & `pywry-0.5.7/src/utils.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/src/window.rs` & `pywry-0.5.7/src/window.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.6/PKG-INFO` & `pywry-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pywry
-Version: 0.5.6
+Version: 0.5.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Requires-Dist: setproctitle
 Requires-Dist: auditwheel; extra == 'dev'
 Requires-Dist: wheel; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PyWry Web Viewer
 
 ![signal-2023-05-08-171646_002](https://github.com/OpenBB-finance/pywry/assets/25267873/a19338f7-0149-4ada-8fc7-389ae36c39fc)
 
 Easily create HTML webviewers in python utilizing the [wry](https://github.com/tauri-apps/wry) library. Unlike many HTML viewers that exist for Python - Pywry allows you to run javacsript. PyWry is also a ~2mb footprint for Mac and Windows - Linux will require a few more libraries which are listed below.
@@ -75,21 +75,21 @@
 ## JSON Keys
 
 PyWry uses a JSON object to communicate between the python and rust backends and the javascript
 frontend. The following keys are available:
 
 | Key | Type | Description |
 | --- | --- | --- |
-| `html` | `Path | str` | The path to the HTML file to be loaded, or HTML string. |
+| `html` | `Path \| str` | The path to the HTML file to be loaded, or HTML string. |
 | `title` | `str` | The title of the window. |
-| `icon` | `str | Path` | The path to `png` icon to be used for the window. |
-| `json_data` | `str | dict` | A JSON string or dictionary to be passed to the javascript frontend. (see below) |
+| `icon` | `str \| Path` | The path to `png` icon to be used for the window. |
+| `json_data` | `str \| dict` | A JSON string or dictionary to be passed to the javascript frontend. (see below) |
 | `height` | `int` | The height of the window. |
 | `width` | `int` | The width of the window. |
-| `download_path` | `str | Path` | The path to the download directory. |
+| `download_path` | `str \| Path` | The path to the download directory. |
 
 ## Javascript
 
 PyWry allows you to run javascript in the frontend. To do this, you can pass a dictionary
 of data to the `json_data` key in the `send_html` method. This dictionary will be converted
 to a JSON string and passed to the frontend. You can then access this data in the frontend
 by using the `window.json_data` object. For example:
```

