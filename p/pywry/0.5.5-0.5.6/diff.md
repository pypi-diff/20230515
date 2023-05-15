# Comparing `tmp/pywry-0.5.5.tar.gz` & `tmp/pywry-0.5.6.tar.gz`

## Comparing `pywry-0.5.5.tar` & `pywry-0.5.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 pywry-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 pywry-0.5.5/rust_src/pywry/Cargo.toml
--rw-r--r--   0     1001      123     1063 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/LICENSE
--rw-r--r--   0     1001      123     4997 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/README.md
--rw-r--r--   0     1001      123     3954 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/constants.rs
--rw-r--r--   0     1001      123     8710 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/events.rs
--rw-r--r--   0     1001      123     5570 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/handlers.rs
--rw-r--r--   0     1001      123     7311 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/headless.rs
--rw-r--r--   0     1001      123     1762 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/lib.rs
--rw-r--r--   0     1001      123     1086 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/pipe.rs
--rw-r--r--   0     1001      123     9060 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/structs.rs
--rw-r--r--   0     1001      123     1663 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/utils.rs
--rw-r--r--   0     1001      123     7965 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/window.rs
--rw-r--r--   0     1001      123    60354 2023-05-11 09:41:22.000000 pywry-0.5.5/Cargo.lock
--rw-r--r--   0     1001      123     1155 2023-05-11 09:41:22.000000 pywry-0.5.5/python/pywry/backend.py
--rw-r--r--   0     1001      123        0 2023-05-11 09:41:22.000000 pywry-0.5.5/python/pywry/py.typed
--rw-r--r--   0     1001      123      180 2023-05-11 09:41:22.000000 pywry-0.5.5/python/pywry/__init__.py
--rw-r--r--   0     1001      123    14558 2023-05-11 09:41:22.000000 pywry-0.5.5/python/pywry/core.py
--rw-r--r--   0     1001      123      217 2023-05-11 09:41:22.000000 pywry-0.5.5/python/pywry/pywry.pyi
--rw-r--r--   0     1001      123      733 2023-05-11 09:41:22.000000 pywry-0.5.5/Cargo.toml
--rw-r--r--   0     1001      123     3954 2023-05-11 09:41:22.000000 pywry-0.5.5/src/constants.rs
--rw-r--r--   0     1001      123     8710 2023-05-11 09:41:22.000000 pywry-0.5.5/src/events.rs
--rw-r--r--   0     1001      123     5570 2023-05-11 09:41:22.000000 pywry-0.5.5/src/handlers.rs
--rw-r--r--   0     1001      123     7311 2023-05-11 09:41:22.000000 pywry-0.5.5/src/headless.rs
--rw-r--r--   0     1001      123     1762 2023-05-11 09:41:22.000000 pywry-0.5.5/src/lib.rs
--rw-r--r--   0     1001      123     1086 2023-05-11 09:41:22.000000 pywry-0.5.5/src/pipe.rs
--rw-r--r--   0     1001      123     9060 2023-05-11 09:41:22.000000 pywry-0.5.5/src/structs.rs
--rw-r--r--   0     1001      123     1663 2023-05-11 09:41:22.000000 pywry-0.5.5/src/utils.rs
--rw-r--r--   0     1001      123     7965 2023-05-11 09:41:22.000000 pywry-0.5.5/src/window.rs
--rw-r--r--   0        0        0     5599 1970-01-01 00:00:00.000000 pywry-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 pywry-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 pywry-0.5.6/rust_src/pywry/Cargo.toml
+-rw-r--r--   0     1001      123     1063 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/LICENSE
+-rw-r--r--   0     1001      123     4920 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/README.md
+-rw-r--r--   0     1001      123     3565 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/constants.rs
+-rw-r--r--   0     1001      123     6158 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/events.rs
+-rw-r--r--   0     1001      123     3733 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/handlers.rs
+-rw-r--r--   0     1001      123     5780 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/headless.rs
+-rw-r--r--   0     1001      123     1571 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/lib.rs
+-rw-r--r--   0     1001      123      975 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/pipe.rs
+-rw-r--r--   0     1001      123     7516 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/structs.rs
+-rw-r--r--   0     1001      123     1366 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/utils.rs
+-rw-r--r--   0     1001      123     6168 2023-05-15 19:22:25.000000 pywry-0.5.6/rust_src/pywry/src/window.rs
+-rw-r--r--   0     1001      123    63815 2023-05-15 19:22:25.000000 pywry-0.5.6/Cargo.lock
+-rw-r--r--   0     1001      123     1155 2023-05-15 19:22:25.000000 pywry-0.5.6/python/pywry/backend.py
+-rw-r--r--   0     1001      123        0 2023-05-15 19:22:25.000000 pywry-0.5.6/python/pywry/py.typed
+-rw-r--r--   0     1001      123      180 2023-05-15 19:22:25.000000 pywry-0.5.6/python/pywry/__init__.py
+-rw-r--r--   0     1001      123    14307 2023-05-15 19:22:25.000000 pywry-0.5.6/python/pywry/core.py
+-rw-r--r--   0     1001      123      217 2023-05-15 19:22:25.000000 pywry-0.5.6/python/pywry/pywry.pyi
+-rw-r--r--   0     1001      123      733 2023-05-15 19:22:25.000000 pywry-0.5.6/Cargo.toml
+-rw-r--r--   0     1001      123     3565 2023-05-15 19:22:25.000000 pywry-0.5.6/src/constants.rs
+-rw-r--r--   0     1001      123     6158 2023-05-15 19:22:25.000000 pywry-0.5.6/src/events.rs
+-rw-r--r--   0     1001      123     3733 2023-05-15 19:22:25.000000 pywry-0.5.6/src/handlers.rs
+-rw-r--r--   0     1001      123     5780 2023-05-15 19:22:25.000000 pywry-0.5.6/src/headless.rs
+-rw-r--r--   0     1001      123     1571 2023-05-15 19:22:25.000000 pywry-0.5.6/src/lib.rs
+-rw-r--r--   0     1001      123      975 2023-05-15 19:22:25.000000 pywry-0.5.6/src/pipe.rs
+-rw-r--r--   0     1001      123     7516 2023-05-15 19:22:25.000000 pywry-0.5.6/src/structs.rs
+-rw-r--r--   0     1001      123     1366 2023-05-15 19:22:25.000000 pywry-0.5.6/src/utils.rs
+-rw-r--r--   0     1001      123     6168 2023-05-15 19:22:25.000000 pywry-0.5.6/src/window.rs
+-rw-r--r--   0        0        0     5522 1970-01-01 00:00:00.000000 pywry-0.5.6/PKG-INFO
```

### Comparing `pywry-0.5.5/pyproject.toml` & `pywry-0.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pywry"
-version = "0.5.5"
-requires-python = ">=3.8"
+version = "0.5.6"
+requires-python = ">=3.9"
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
-target-version = "py38"
+target-version = "py39"
 
 [tool.ruff.isort]
 combine-as-imports = true
 force-wrap-aliases = true
 
 [tool.ruff.pylint]
 max-args=8
```

### Comparing `pywry-0.5.5/rust_src/pywry/Cargo.toml` & `pywry-0.5.6/rust_src/pywry/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.5"
+version = "0.5.6"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.5.5/rust_src/pywry/LICENSE` & `pywry-0.5.6/rust_src/pywry/LICENSE`

 * *Files identical despite different names*

### Comparing `pywry-0.5.5/rust_src/pywry/README.md` & `pywry-0.5.6/rust_src/pywry/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -58,22 +58,21 @@
 ## JSON Keys
 
 PyWry uses a JSON object to communicate between the python and rust backends and the javascript
 frontend. The following keys are available:
 
 | Key | Type | Description |
 | --- | --- | --- |
-| `html_str` | `str` | The HTML string to be rendered. |
-| `html_path` | `Union[str, Path]` | The path to the HTML file to be rendered. |
+| `html` | `Path | str` | The path to the HTML file to be loaded, or HTML string. |
 | `title` | `str` | The title of the window. |
-| `icon` | `Union[str, Path]` | The path to `png` icon to be used for the window. |
-| `json_data` | `Union[str, dict]` | A JSON string or dictionary to be passed to the javascript frontend. (see below) |
+| `icon` | `str | Path` | The path to `png` icon to be used for the window. |
+| `json_data` | `str | dict` | A JSON string or dictionary to be passed to the javascript frontend. (see below) |
 | `height` | `int` | The height of the window. |
 | `width` | `int` | The width of the window. |
-| `download_path` | `Union[str, Path]` | The path to the download directory. |
+| `download_path` | `str | Path` | The path to the download directory. |
 
 ## Javascript
 
 PyWry allows you to run javascript in the frontend. To do this, you can pass a dictionary
 of data to the `json_data` key in the `send_html` method. This dictionary will be converted
 to a JSON string and passed to the frontend. You can then access this data in the frontend
 by using the `window.json_data` object. For example:
@@ -84,15 +83,15 @@
 
 ```python
 from pathlib import Path
 # code from above ...
 
 # change send_html line to:
         handler.send_html(
-            html_path=Path(__file__).parent / "index.html", json_data={"name": "PyWry"}
+            html=Path(__file__).parent / "index.html", json_data={"name": "PyWry"}
         )
 ```
 
 ---------------------
 
 ### HTML
```

### Comparing `pywry-0.5.5/Cargo.lock` & `pywry-0.5.6/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.70"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "atk"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "39991bc421ddf72f70159011b323ff49b0f783cc676a7287c59453da2e2531cf"
 dependencies = [
@@ -133,19 +133,20 @@
 name = "cesu8"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d43a04d8753f35258c91f8ec639f792891f748a1edbd759cf1dcea3382ad83c"
 
 [[package]]
 name = "cfg-expr"
-version = "0.11.0"
+version = "0.15.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0357a6402b295ca3a86bc148e84df46c02e41f41fef186bda662557ef6328aa"
+checksum = "c8790cf1286da485c72cf5fc7aeba308438800036ec67d89425924c4807268c9"
 dependencies = [
  "smallvec",
+ "target-lexicon",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
@@ -211,17 +212,17 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "core-graphics"
 version = "0.22.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2581bbab3b8ffc6fcbd550bf46c355135d16e9ff2a6ea032ad6b9bf1d7efe4fb"
 dependencies = [
@@ -242,17 +243,17 @@
  "core-foundation",
  "foreign-types",
  "libc",
 ]
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -260,17 +261,17 @@
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.7"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf2b3e8478797446514c91ef04bafcb59faba183e621ad488df88983cc14128c"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
@@ -360,33 +361,42 @@
 checksum = "bde03329ae10e79ede66c9ce4dc930aa8599043b0743008548680f25b91502d6"
 dependencies = [
  "dtoa",
 ]
 
 [[package]]
 name = "dunce"
-version = "1.0.3"
+version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bd4b30a6560bbd9b4620f4de34c3f14f60848e58a9b7216801afcb4c7b31c3c"
+checksum = "56ce8c6da7551ec6c462cbaf3bfbc75131ebbfa1c944aeaa9dab51ca1c5f0c3b"
+
+[[package]]
+name = "fdeflate"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d329bdeac514ee06249dabc27877490f17f5d371ec693360768b838e19f3ae10"
+dependencies = [
+ "simd-adler32",
+]
 
 [[package]]
 name = "field-offset"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3cf3a800ff6e860c863ca6d4b16fd999db8b752819c1606884047b73e468535"
 dependencies = [
  "memoffset",
  "rustc_version",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.25"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -426,66 +436,66 @@
 dependencies = [
  "mac",
  "new_debug_unreachable",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "164713a5a0dcc3e7b4b1ed7d3b433cabc18025386f9339346e8daf15963cf7ac"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86d7a0c1aa76363dac491de0ee99faf6941128376f1cf96f07db7603b7de69dd"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1997dd9df74cdac935c76252744c1ed5794fac083242ea4fe77ef3ed60ba0f83"
+checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89d422fa3cbe3b40dca574ab087abb5bc98258ea57eea3fd6f1fa7162c778b91"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3eb14ed937631bd8b8b8977f2c198443447a8355b6e3ca599f38c975e5a963b6"
+checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "futures-task"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd65540d33b37b16542a0438c12e6aeead10d4ac5d05bd3f805b8f35ab592879"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-util"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ef6b17e481503ec85211fed8f39d1970f128935ca1f814cd32ac4a6842e84ab"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-core",
  "futures-macro",
  "futures-task",
  "pin-project-lite",
  "pin-utils",
  "slab",
@@ -584,17 +594,17 @@
  "libc",
  "system-deps",
  "x11",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
@@ -605,17 +615,17 @@
  "cfg-if",
  "libc",
  "wasi 0.9.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
@@ -818,31 +828,31 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "image"
-version = "0.24.5"
+version = "0.24.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69b7ea949b537b0fd0af141fff8c77690f2ce96f4f41f042ccb6c69c6c965945"
+checksum = "527909aa81e20ac3a44803521443a765550f09b5130c2c2fa1ea59c2f8f50a3a"
 dependencies = [
  "bytemuck",
  "byteorder",
  "color_quant",
  "num-rational",
  "num-traits",
  "png",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
@@ -856,14 +866,33 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "is-docker"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "928bae27f42bc99b60d9ac7334e3a21d10ad8f1835a4e12ec3ec0464765ed1b3"
+dependencies = [
+ "once_cell",
+]
+
+[[package]]
+name = "is-wsl"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "173609498df190136aa7dea1a91db051746d339e18476eed5ca40521f02d7aa5"
+dependencies = [
+ "is-docker",
+ "once_cell",
+]
+
+[[package]]
 name = "itoa"
 version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b71991ff56294aa922b450139ee08b3bfc70982c6b2c7562771375cf73542dd4"
 
 [[package]]
 name = "itoa"
@@ -930,17 +959,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -1021,31 +1050,32 @@
 dependencies = [
  "mime",
  "unicase",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.6.2"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
+ "simd-adler32",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
 dependencies = [
  "libc",
  "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "ndk"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2032c77e030ddee34a6787a64166008da93f6a352b629261d0fee232b8742dd4"
@@ -1177,18 +1207,19 @@
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "open"
-version = "4.0.1"
+version = "4.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "075c5203b3a2b698bc72c6c10b1f6263182135751d5013ea66e8a4b3d0562a43"
+checksum = "d16814a067484415fda653868c9be0ac5f2abd2ef5d951082a5f2fe1b3662944"
 dependencies = [
+ "is-wsl",
  "pathdiff",
 ]
 
 [[package]]
 name = "pango"
 version = "0.16.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1230,15 +1261,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "pathdiff"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8835116a5c179084a830efb3adc117ab007512b535bc1a21c991d3b32a6b44dd"
@@ -1332,26 +1363,27 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "png"
-version = "0.17.7"
+version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d708eaf860a19b19ce538740d2b4bdeeb8337fa53f7738455e706623ad5c638"
+checksum = "aaeebc51f9e7d2c150d3f3bfeb667f2aa985db5ef1e3d212847bdedb488beeaa"
 dependencies = [
  "bitflags",
  "crc32fast",
+ "fdeflate",
  "flate2",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
@@ -1402,76 +1434,76 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.52"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d0e1ae9e836cc3beddd63db0df682593d7e2d3d891ae8c9083d2113e1744224"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "python3-dll-a",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -1481,32 +1513,32 @@
 checksum = "a915bd72824962bf190bbd3e8a044cccb695d1409f73ff5493712eda5136c7a8"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pywry"
-version = "0.5.5"
+version = "0.5.6"
 dependencies = [
  "image",
  "mime_guess",
  "open",
  "pyo3",
  "serde",
  "serde_json",
  "tokio",
  "urlencoding",
  "wry",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.7.3"
@@ -1563,15 +1595,15 @@
 
 [[package]]
 name = "rand_core"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
- "getrandom 0.2.8",
+ "getrandom 0.2.9",
 ]
 
 [[package]]
 name = "rand_hc"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca3129af7b92a17112d59ad498c6f81eaf463253766b90396d39ea7a39d6613c"
@@ -1586,43 +1618,43 @@
 checksum = "16abd0c1b639e9eb4d7c50c0b8100b0d0f849be2349829c740fe8e6eb4816429"
 dependencies = [
  "rand_core 0.5.1",
 ]
 
 [[package]]
 name = "raw-window-handle"
-version = "0.5.1"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f851a03551ceefd30132e447f07f96cb7011d6b658374f3aed847333adb5559"
+checksum = "f2ff9a1f06a88b01621b7ae906ef0211290d1c8a168a15542486a8f61c0833b9"
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.2"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cce168fea28d3e05f158bda4576cf0c844d5045bc2cc3620fa0292ed5bb5814c"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
@@ -1674,44 +1706,53 @@
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
-version = "1.0.158"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "771d4d9c4163ee138805e12c710dd365e4f44be8be0503cb1bb9eb989425d9c9"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.158"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e801c1712f48475582b7696ac71e0ca34ebb30e09338425384269d9717c62cad"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.4",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.94"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa 1.0.6",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_spanned"
+version = "0.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0efd8caf556a6cebd3b285caf480045fcc1ac04f6bd786b09a6f11af30c4fcf4"
+dependencies = [
+ "serde",
+]
+
+[[package]]
 name = "servo_arc"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d98238b800e0d1576d8b6e3de32827c2d74bee68bb97748dcf5071fb53965432"
 dependencies = [
  "nodrop",
  "stable_deref_trait",
@@ -1734,14 +1775,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "simd-adler32"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "238abfbb77c1915110ad968465608b68e869e0772622c9656714e73e5a1a522f"
+
+[[package]]
 name = "siphasher"
 version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
 
 [[package]]
 name = "slab"
@@ -1837,28 +1884,28 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.4"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c622ae390c9302e214c31013517c2061ecb2699935882c60a9b37f82f8625ae"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "system-deps"
-version = "6.0.3"
+version = "6.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2955b1fe31e1fa2fbd1976b71cc69a606d7d4da16f6de3333d0c92d51419aeff"
+checksum = "e5fa6fb9ee296c0dc2df41a656ca7948546d061958115ddb0bcaae43ad0d17d2"
 dependencies = [
  "cfg-expr",
  "heck",
  "pkg-config",
  "toml",
  "version-compare",
 ]
@@ -1919,17 +1966,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tendril"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d24a120c5fc464a3458240ee02c299ebcb9d67b5249c8848b09d639dca8d7bb0"
 dependencies = [
@@ -1957,15 +2004,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.4",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
@@ -1977,65 +2024,72 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.26.0"
+version = "1.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03201d01c3c27a29c8a5cee5b55a93ddae1ccf6f08f65365c2c918f8c1b76f64"
+checksum = "0aa32867d44e6f2ce3385e89dceb990188b8bb0fb25b0cf576647a6f98ac5105"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
- "memchr",
  "mio",
  "num_cpus",
  "parking_lot",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "1.8.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d266c00fde287f55d3f1c3e96c500c362a2b8c695076ec180f27918820bc6df8"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "toml"
-version = "0.5.11"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
+checksum = "b403acf6f2bb0859c93c7f0d967cb4a75a7ac552100f9322faf64dc047669b21"
 dependencies = [
  "serde",
+ "serde_spanned",
+ "toml_datetime",
+ "toml_edit",
 ]
 
 [[package]]
 name = "toml_datetime"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3ab8ed2edee10b50132aed5f331333428b011c99402b5a534154ed15746f9622"
+dependencies = [
+ "serde",
+]
 
 [[package]]
 name = "toml_edit"
-version = "0.19.7"
+version = "0.19.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc18466501acd8ac6a3f615dd29a3438f8ca6bb3b19537138b3106e575621274"
+checksum = "239410c8609e8125456927e6707163a3b1fdb40561e4b803bc041f466ccfdc13"
 dependencies = [
  "indexmap",
+ "serde",
+ "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.16.0"
@@ -2105,19 +2159,19 @@
 name = "utf-8"
 version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "09cc8ee72d2a9becf2f2febe0205bbed8fc6615b7cb429ad062dc7b7ddd036a9"
 
 [[package]]
 name = "uuid"
-version = "1.3.0"
+version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1674845326ee10d37ca60470760d4288a6f80f304007d92e5c53bab78c9cfd79"
+checksum = "4dad5567ad0cf5b760e5665964bec1b47dfd077ba8a2544b513f3556d3d239a2"
 dependencies = [
- "getrandom 0.2.8",
+ "getrandom 0.2.9",
 ]
 
 [[package]]
 name = "version-compare"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "579a42fc0b8e0c63b76519a339be31bed574929511fa53c1a3acae26eb258f29"
@@ -2267,15 +2321,15 @@
 name = "windows"
 version = "0.44.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e745dab35a0c4c77aa3ce42d595e13d2003d6902d6b08c9ef5fc326d08da12b"
 dependencies = [
  "windows-implement",
  "windows-interface",
- "windows-targets",
+ "windows-targets 0.42.2",
 ]
 
 [[package]]
 name = "windows-bindgen"
 version = "0.44.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "222204ecf46521382a4d88b4a1bbefca9f8855697b4ab7d20803901425e061a3"
@@ -2314,30 +2368,54 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows-tokens"
 version = "0.44.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fa4251900975a0d10841c5d4bde79c56681543367ef811f3fabb8d1803b0959b"
@@ -2345,54 +2423,96 @@
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
 name = "winnow"
-version = "0.3.6"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23d020b441f92996c80d94ae9166e8501e59c7bb56121189dc9eab3bd8216966"
+checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "wry"
 version = "0.28.3"
```

### Comparing `pywry-0.5.5/python/pywry/backend.py` & `pywry-0.5.6/python/pywry/backend.py`

 * *Files identical despite different names*

### Comparing `pywry-0.5.5/python/pywry/core.py` & `pywry-0.5.6/python/pywry/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import asyncio
 import atexit
 import json
 import os
 import re
-import subprocess
 import sys
 import threading
 import traceback
 from asyncio.exceptions import CancelledError, IncompleteReadError, TimeoutError
 from pathlib import Path
 from queue import Queue
+from subprocess import PIPE
 from typing import List, Optional, Union
 
 import setproctitle
 
 from pywry import pywry
 
 __all__ = ["PyWry", "BackendFailedToStart"]
@@ -21,18 +21,25 @@
 AsyncioException = (
     CancelledError,
     IncompleteReadError,
     TimeoutError,
     ConnectionResetError,
 )
 
+# Ignore some messages from the backend that can be confusing to users
+# these messages are not errors, but they are not useful either
+IGNORE_REGEX = (
+    r"(Wayland|Compositor|webkit_download|"
+    r"NeedDebuggerBreak|GLib-GIO-CRITICAL|"
+    r"EGLDisplay|libEGL|Could not determine|"
+    r"Gtk-Message|WARNING|Gtk)"
+)
 
 ACCEPTED_KEYS_TYPES = {
-    "html_str": str,
-    "html_path": (str, Path),
+    "html": (str, Path),
     "title": str,
     "icon": (str, Path),
     "json_data": (dict, str),
     "height": int,
     "width": int,
     "download_path": (str, Path),
     "export_image": (str, Path),
@@ -47,40 +54,41 @@
 
 
 class PyWry:
     """This class handles the wry functionality, by spinning up a rust program that
     listens to pipes and shows windows with provided html and json data.
     """
 
-    _bootargs: List[str] = []
     __version__ = pywry.__version__
+    _bootargs: List[str] = []
+
+    daemon: bool = True
+    debug: bool = False
+    shell: bool = False
+    outgoing: List[str] = []
+    init_engine: List[str] = []
+    recv: Queue[dict] = Queue()
+    base: pywry.WindowManager = pywry.WindowManager()
 
     def __new__(cls, *args, **kwargs):  # pylint: disable=unused-argument
         "Makes the class a 'singleton' by only allowing one instance at a time"
         if not hasattr(cls, "instance"):
             cls.instance = super().__new__(cls)
         return cls.instance
 
     def __init__(
         self,
         daemon: bool = True,
         max_retries: int = 30,
         proc_name: str = "PyWry",
     ):
+        self.daemon: bool = daemon
         self.max_retries: int = max_retries
         self.proc_name: str = proc_name
 
-        self.outgoing: List[str] = []
-        self.recv: Queue[dict] = Queue()
-        self.init_engine: List[str] = []
-        self.daemon: bool = daemon
-        self.debug: bool = False
-        self.shell: bool = False
-        self.base = pywry.WindowManager()
-
         try:
             self.loop: asyncio.AbstractEventLoop = asyncio.get_event_loop()
         except RuntimeError:
             self.loop = asyncio.new_event_loop()
             asyncio.set_event_loop(self.loop)
 
         self.runner: Optional[asyncio.subprocess.Process] = None
@@ -96,53 +104,42 @@
 
     def __del__(self):
         if self._is_started.is_set():
             self.close()
 
     def send_html(
         self,
-        html_str: Optional[str] = None,
-        html_path: Optional[Union[str, Path]] = None,
+        html: Union[str, Path],
         json_data: Optional[dict] = None,
         title: str = "",
         width: int = 800,
         height: int = 600,
         **kwargs,
     ):
         """Send html to backend.
 
         Parameters
         ----------
-        html_str : str, optional
-            HTML string to send to backend.
-            If not provided, html_path must be provided, by default None
-        html_path : str, optional
-            Path to html file to send to backend, by default None
+        html: Union[str, Path]
+            HTML to send to backend.
         json_data : dict, optional
             JSON data to send to backend, by default None
         title : str, optional
             Title to display in the window, by default ""
         width : int, optional
             Width of the window, by default 800
         height : int, optional
             Height of the window, by default 600
         """
         self.loop.run_until_complete(self.check_backend())
-
         kwargs.update(
             dict(
-                html_str=html_str,
-                html_path=html_path,
-                json_data=json_data,
-                title=title,
-                width=width,
-                height=height,
+                html=html, json_data=json_data, title=title, width=width, height=height
             )
         )
-
         self.send_outgoing(kwargs)
 
     def send_outgoing(self, outgoing: dict):
         """Send outgoing data to backend.
 
         Parameters
         ----------
@@ -195,19 +192,24 @@
         return output
 
     def print_debug(self):
         """Print debug messages from the backend."""
         if self.debug:
             traceback.print_exc()
 
+    def clean_print(self, message: dict):
+        """Clean messages from the backend."""
+        if message and not re.search(IGNORE_REGEX, message, re.IGNORECASE):
+            print(message)
+
     async def check_backend(self):
         """Check if the backend is running."""
 
         if self.max_retries == 0:
-            # If the backend is not running and we have tried to connect
+            # If the backend is not running and we have retried
             # max_retries times, raise an error
             raise BackendFailedToStart("Exceededed max retries")
         try:
             if self.thread and not self.thread.is_alive():
                 self.start()
 
         except RuntimeError:
@@ -224,53 +226,34 @@
                     pass
 
                 with self.lock:
                     self.runner = None
                     self._is_started.clear()
                     self._is_closed.set()
 
-            kwargs = dict(
-                stdin=subprocess.PIPE,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-            )
+            kwargs = dict()
             cmd = [sys.executable, "-m", "pywry.backend", "--start"] + self._bootargs
 
-            # for pyinstaller builds
+            # For pyinstaller builds we need to get the path to the executable
             if hasattr(sys, "frozen"):
                 # pylint: disable=E1101,W0212
                 exec_name = os.environ.get("PYWRY_EXECUTABLE", "PyWry")
                 pywrypath = (Path(sys._MEIPASS) / exec_name).resolve()
-                cmd = f"{exec_name} --start{' '.join(self._bootargs)}"
+                cmd = f"{exec_name} --start {' '.join(self._bootargs)}"
                 if sys.platform == "darwin":
                     cmd = f"'{pywrypath}'"
 
-                kwargs.update(dict(cwd=str(pywrypath.parent)))
                 self.shell = True
+                kwargs.update(dict(cwd=str(pywrypath.parent)))
 
             env = os.environ.copy()
             env["PYWRY_PROCESS_NAME"] = self.proc_name
+            kwargs.update(dict(env=env))
 
-            runner = asyncio.create_subprocess_exec(
-                *cmd,
-                env=env,
-                limit=2**64,
-                **kwargs,
-            )
-
-            if self.shell:
-                if isinstance(cmd, list):
-                    cmd = " ".join(cmd)
-                runner = asyncio.create_subprocess_shell(
-                    cmd,
-                    env=env,
-                    **kwargs,
-                )
-
-            runner = await runner
+            runner = await self.create_subprocess(cmd=cmd, **kwargs)
 
             with self.lock:
                 self.runner = runner
                 self._is_started.set()
                 self._is_closed.clear()
 
             setproctitle.setproctitle(self.proc_name)
@@ -280,77 +263,68 @@
                 await asyncio.sleep(3)
 
         except Exception as proc_err:
             raise BackendFailedToStart("Could not start backend") from proc_err
 
     def print_message(self, message: dict):
         """Print messages from the backend."""
-        print_style = {
-            "error": "\033[91m",
-            "info": "\033[93m",
-            "debug": "\033[92m",
-        }
+        print_style = {"error": "\033[91m", "info": "\033[93m", "debug": "\033[92m"}
         if (
             key := re.search(r"error|info|debug", ",".join(message.keys()))
         ) is not None:
             return print(f"{print_style[key.group()]}{message[key.group()]}")
 
-        print(message)
+        return self.clean_print(message)
 
     async def recv_message(self, data: str):
         """Creates a new task to process messages from the stdout reader."""
         try:
             message: dict = json.loads(data)
             if message.get("result", None):
                 return self.recv.put(message, block=False)
             self.print_message(message)
         except (json.JSONDecodeError, AttributeError):
-            print(data)
+            self.clean_print(data)
 
     async def stdout_reader(self):
         """Read stdout from the backend."""
-
         try:
             while self._is_started.is_set():
                 if data := (await self.runner.stdout.readline()).decode().strip():
                     asyncio.create_task(self.recv_message(data))
-                await asyncio.sleep(0.02)
 
+                await asyncio.sleep(0.02)
         except Exception as proc_err:
             await self.exception_handler(proc_err)
 
     async def stderr_reader(self):
         """Read stderr from the backend."""
-        # Ignore some messages from the backend that can be confusing to users
-        # these messages are not errors, but they are not useful either
-        ignore_regex = r"(Wayland|Compositor|webkit_download|NeedDebuggerBreak)"
         try:
             while self._is_started.is_set():
                 if data := (await self.runner.stderr.readline()).decode().strip():
-                    if data and not re.search(ignore_regex, data):
-                        print(data)
+                    self.clean_print(data)
 
                 await asyncio.sleep(1)
-
         except Exception as proc_err:
             await self.exception_handler(proc_err)
 
     async def run_backend(self):
         """Runs the backend and starts the main loop."""
         await self.handle_start()
         with self.lock:
             self.subprocess_loop = asyncio.get_running_loop()
 
         # We need to create a new task for each reader, otherwise
         # the loop will not be able to run the main task
         self.subprocess_loop.create_task(self.stdout_reader())
-        self.subprocess_loop.create_task(self.stderr_reader())
 
-        while not self._is_started.is_set():
-            await asyncio.sleep(0.1)
+        # We only need to read stderr if we are in debug mode
+        if self.debug:
+            self.subprocess_loop.create_task(self.stderr_reader())
+
         try:
             if self.init_engine:
                 # if there is data in the init_engine list,
                 # we send it to the backend and clear the list
                 for msg in self.init_engine:
                     self.runner.stdin.write(f"{msg}\n".encode())
                     await self.runner.stdin.drain()
@@ -365,16 +339,16 @@
                         self.runner.stdin.write(f"{data}\n".encode())
                         await self.runner.stdin.drain()
 
                         self.init_engine = []
 
                     await asyncio.sleep(0.5)
 
-                except (BrokenPipeError, ConnectionResetError) as runtime_err:
-                    await self.exception_handler(runtime_err)
+                except (BrokenPipeError, ConnectionResetError) as pipe_err:
+                    await self.exception_handler(pipe_err)
                     await self.run_backend()
 
                 except AsyncioException as asyncio_err:
                     await self.exception_handler(asyncio_err, subtract=1)
                     await self.run_backend()
 
         except RuntimeError as runtime_err:
@@ -426,19 +400,32 @@
                 self.thread.join()
             self.thread = thread
 
         if headless:
             self.loop.run_until_complete(asyncio.sleep(3))
         self.loop.run_until_complete(self.check_backend())
 
-    def close(self, reset: bool = False):  # pylint: disable=unused-argument
+    def close(self):
         """Close the backend."""
         with self.lock:
             self._is_started.clear()
             self._is_closed.set()
 
         if self.runner:
             try:
                 self.subprocess_loop.call_soon_threadsafe(self.runner.terminate)
                 self.subprocess_loop.call_soon_threadsafe(self.runner.kill)
             except Exception:
                 pass
+
+    async def create_subprocess(self, cmd: Union[str, List[str]], **kwargs):
+        if self.shell:
+            if isinstance(cmd, list):
+                cmd = " ".join(cmd)
+
+            return await asyncio.create_subprocess_shell(
+                cmd, PIPE, PIPE, PIPE, 2**64, **kwargs
+            )
+
+        return await asyncio.create_subprocess_exec(
+            *cmd, stdin=PIPE, stdout=PIPE, stderr=PIPE, limit=2**64, **kwargs
+        )
```

### Comparing `pywry-0.5.5/Cargo.toml` & `pywry-0.5.6/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.5"
+version = "0.5.6"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.5.5/PKG-INFO` & `pywry-0.5.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pywry
-Version: 0.5.5
+Version: 0.5.6
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
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PyWry Web Viewer
 
 ![signal-2023-05-08-171646_002](https://github.com/OpenBB-finance/pywry/assets/25267873/a19338f7-0149-4ada-8fc7-389ae36c39fc)
 
 Easily create HTML webviewers in python utilizing the [wry](https://github.com/tauri-apps/wry) library. Unlike many HTML viewers that exist for Python - Pywry allows you to run javacsript. PyWry is also a ~2mb footprint for Mac and Windows - Linux will require a few more libraries which are listed below.
@@ -75,22 +75,21 @@
 ## JSON Keys
 
 PyWry uses a JSON object to communicate between the python and rust backends and the javascript
 frontend. The following keys are available:
 
 | Key | Type | Description |
 | --- | --- | --- |
-| `html_str` | `str` | The HTML string to be rendered. |
-| `html_path` | `Union[str, Path]` | The path to the HTML file to be rendered. |
+| `html` | `Path | str` | The path to the HTML file to be loaded, or HTML string. |
 | `title` | `str` | The title of the window. |
-| `icon` | `Union[str, Path]` | The path to `png` icon to be used for the window. |
-| `json_data` | `Union[str, dict]` | A JSON string or dictionary to be passed to the javascript frontend. (see below) |
+| `icon` | `str | Path` | The path to `png` icon to be used for the window. |
+| `json_data` | `str | dict` | A JSON string or dictionary to be passed to the javascript frontend. (see below) |
 | `height` | `int` | The height of the window. |
 | `width` | `int` | The width of the window. |
-| `download_path` | `Union[str, Path]` | The path to the download directory. |
+| `download_path` | `str | Path` | The path to the download directory. |
 
 ## Javascript
 
 PyWry allows you to run javascript in the frontend. To do this, you can pass a dictionary
 of data to the `json_data` key in the `send_html` method. This dictionary will be converted
 to a JSON string and passed to the frontend. You can then access this data in the frontend
 by using the `window.json_data` object. For example:
@@ -101,15 +100,15 @@
 
 ```python
 from pathlib import Path
 # code from above ...
 
 # change send_html line to:
         handler.send_html(
-            html_path=Path(__file__).parent / "index.html", json_data={"name": "PyWry"}
+            html=Path(__file__).parent / "index.html", json_data={"name": "PyWry"}
         )
 ```
 
 ---------------------
 
 ### HTML
```

