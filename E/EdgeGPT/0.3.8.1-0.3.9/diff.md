# Comparing `tmp/EdgeGPT-0.3.8.1.tar.gz` & `tmp/EdgeGPT-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.3.8.1.tar", last modified: Sat May 13 12:54:23 2023, max compression
+gzip compressed data, was "EdgeGPT-0.3.9.tar", last modified: Mon May 15 02:33:30 2023, max compression
```

## Comparing `EdgeGPT-0.3.8.1.tar` & `EdgeGPT-0.3.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 12:54:23.450954 EdgeGPT-0.3.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-13 12:53:51.000000 EdgeGPT-0.3.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-13 12:54:23.450954 EdgeGPT-0.3.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-13 12:54:23.000000 EdgeGPT-0.3.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-13 12:54:23.450954 EdgeGPT-0.3.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-13 12:53:51.000000 EdgeGPT-0.3.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 12:54:23.446954 EdgeGPT-0.3.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 12:54:23.450954 EdgeGPT-0.3.8.1/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-13 12:54:23.000000 EdgeGPT-0.3.8.1/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-13 12:54:23.000000 EdgeGPT-0.3.8.1/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 12:54:23.000000 EdgeGPT-0.3.8.1/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-13 12:54:23.000000 EdgeGPT-0.3.8.1/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-13 12:54:23.000000 EdgeGPT-0.3.8.1/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 12:54:23.000000 EdgeGPT-0.3.8.1/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29710 2023-05-13 12:53:51.000000 EdgeGPT-0.3.8.1/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-13 12:53:51.000000 EdgeGPT-0.3.8.1/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 02:33:30.879199 EdgeGPT-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-15 02:32:54.000000 EdgeGPT-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-05-15 02:33:30.879199 EdgeGPT-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-05-15 02:33:30.000000 EdgeGPT-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-15 02:33:30.879199 EdgeGPT-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-15 02:32:54.000000 EdgeGPT-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 02:33:30.879199 EdgeGPT-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 02:33:30.879199 EdgeGPT-0.3.9/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-05-15 02:33:30.000000 EdgeGPT-0.3.9/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-15 02:33:30.000000 EdgeGPT-0.3.9/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 02:33:30.000000 EdgeGPT-0.3.9/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 02:33:30.000000 EdgeGPT-0.3.9/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-15 02:33:30.000000 EdgeGPT-0.3.9/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 02:33:30.000000 EdgeGPT-0.3.9/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29897 2023-05-15 02:32:54.000000 EdgeGPT-0.3.9/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-15 02:32:54.000000 EdgeGPT-0.3.9/src/ImageGen.py
```

### Comparing `EdgeGPT-0.3.8.1/LICENSE` & `EdgeGPT-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.8.1/PKG-INFO` & `EdgeGPT-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.8.1
+Version: 0.3.9
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -22,15 +22,15 @@
 
 # Edge GPT
 
 _The reverse engineering the chat feature of the new version of Bing_
 
 <a>English</a> -
 <a href="./README_zh-cn.md">简体中文</a> -
-<a href="./README_zh-tw.md">繁體中文 (中國臺灣)</a> -
+<a href="./README_zh-tw.md">繁體中文</a> -
 <a href="./README_es.md">Español</a> -
 <a href="./README_ja.md">日本語</a>
 
 </div>
 
 <p align="center">
   <a href="https://github.com/acheong08/EdgeGPT">
```

#### html2text {}

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.8.1 Summary: Reverse
-engineered Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT
-Author: Antonio Cheong Author-email: acheong@student.dalat.org License: GNU
-General Public License v2.0 Project-URL: Bug Report, https://github.com/
-acheong08/EdgeGPT/issues/new Classifier: License :: OSI Approved :: The
-Unlicense (Unlicense) Classifier: Intended Audience :: Developers Classifier:
-Topic :: Software Development :: Libraries :: Python Modules Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-License-File: LICENSE
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.9 Summary: Reverse engineered
+Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
+Cheong Author-email: acheong@student.dalat.org License: GNU General Public
+License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
+issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: Intended Audience :: Developers Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
-    version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ_(ä¸­åèºç£) -
-                             EspaÃ±ol - æ¥æ¬èª
+ version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ - EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
 --- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
 upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
 access to
 bing.com/chat> (Required) - Required in a supported country with New Bing
 (Chinese mainland VPN required)   ### Checking access (Required)  - Install the
 latest version of Microsoft Edge - Alternatively, you can use any browser and
```

### Comparing `EdgeGPT-0.3.8.1/README.md` & `EdgeGPT-0.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Edge GPT
 
 _The reverse engineering the chat feature of the new version of Bing_
 
 <a>English</a> -
 <a href="./README_zh-cn.md">简体中文</a> -
-<a href="./README_zh-tw.md">繁體中文 (中國臺灣)</a> -
+<a href="./README_zh-tw.md">繁體中文</a> -
 <a href="./README_es.md">Español</a> -
 <a href="./README_ja.md">日本語</a>
 
 </div>
 
 <p align="center">
   <a href="https://github.com/acheong08/EdgeGPT">
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
-    version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ_(ä¸­åèºç£) -
-                             EspaÃ±ol - æ¥æ¬èª
+ version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ - EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
 --- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
 upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
 access to
 bing.com/chat> (Required) - Required in a supported country with New Bing
 (Chinese mainland VPN required)   ### Checking access (Required)  - Install the
 latest version of Microsoft Edge - Alternatively, you can use any browser and
```

### Comparing `EdgeGPT-0.3.8.1/setup.py` & `EdgeGPT-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.3.8.1",
+    version="0.3.9",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.3.8.1/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.3.9/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.8.1
+Version: 0.3.9
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -22,15 +22,15 @@
 
 # Edge GPT
 
 _The reverse engineering the chat feature of the new version of Bing_
 
 <a>English</a> -
 <a href="./README_zh-cn.md">简体中文</a> -
-<a href="./README_zh-tw.md">繁體中文 (中國臺灣)</a> -
+<a href="./README_zh-tw.md">繁體中文</a> -
 <a href="./README_es.md">Español</a> -
 <a href="./README_ja.md">日本語</a>
 
 </div>
 
 <p align="center">
   <a href="https://github.com/acheong08/EdgeGPT">
```

#### html2text {}

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.8.1 Summary: Reverse
-engineered Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT
-Author: Antonio Cheong Author-email: acheong@student.dalat.org License: GNU
-General Public License v2.0 Project-URL: Bug Report, https://github.com/
-acheong08/EdgeGPT/issues/new Classifier: License :: OSI Approved :: The
-Unlicense (Unlicense) Classifier: Intended Audience :: Developers Classifier:
-Topic :: Software Development :: Libraries :: Python Modules Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-License-File: LICENSE
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.9 Summary: Reverse engineered
+Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
+Cheong Author-email: acheong@student.dalat.org License: GNU General Public
+License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
+issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: Intended Audience :: Developers Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
-    version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ_(ä¸­åèºç£) -
-                             EspaÃ±ol - æ¥æ¬èª
+ version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ - EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
 --- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
 upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
 access to
 bing.com/chat> (Required) - Required in a supported country with New Bing
 (Chinese mainland VPN required)   ### Checking access (Required)  - Install the
 latest version of Microsoft Edge - Alternatively, you can use any browser and
```

### Comparing `EdgeGPT-0.3.8.1/src/EdgeGPT.py` & `EdgeGPT-0.3.9/src/EdgeGPT.py`

 * *Files 1% similar despite different names*

```diff
@@ -540,14 +540,16 @@
                                         "adaptiveCards"
                                     ][0]["body"][0]["inlines"][0].get("text")
                                     + "\n"
                                 )
                         yield False, resp_txt
 
                 elif response.get("type") == 2:
+                    if response["item"]["result"].get("error"):
+                        raise Exception(f"{response['item']['result']['value']}: {response['item']['result']['message']}")
                     if draw:
                         cache = response["item"]["messages"][1]["adaptiveCards"][0][
                             "body"
                         ][0]["text"]
                         response["item"]["messages"][1]["adaptiveCards"][0]["body"][0][
                             "text"
                         ] = (cache + resp_txt)
```

