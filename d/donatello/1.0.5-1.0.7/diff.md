# Comparing `tmp/donatello-1.0.5.tar.gz` & `tmp/donatello-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donatello-1.0.5.tar", last modified: Tue Jan  3 19:38:14 2023, max compression
+gzip compressed data, was "donatello-1.0.7.tar", last modified: Mon May 15 20:24:35 2023, max compression
```

## Comparing `donatello-1.0.5.tar` & `donatello-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-01-03 19:38:14.895304 donatello-1.0.5/
--rw-rw-rw-   0        0        0     1069 2022-11-07 08:36:06.000000 donatello-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     3739 2023-01-03 19:38:14.896303 donatello-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2572 2023-01-03 19:30:14.000000 donatello-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-01-03 19:38:14.871045 donatello-1.0.5/donatello/
--rw-rw-rw-   0        0        0      198 2023-01-03 19:17:45.000000 donatello-1.0.5/donatello/__init__.py
--rw-rw-rw-   0        0        0      106 2022-11-07 08:36:06.000000 donatello-1.0.5/donatello/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-01-03 19:38:14.891316 donatello-1.0.5/donatello.egg-info/
--rw-rw-rw-   0        0        0     3739 2023-01-03 19:38:14.000000 donatello-1.0.5/donatello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-01-03 19:38:14.000000 donatello-1.0.5/donatello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-03 19:38:14.000000 donatello-1.0.5/donatello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-01-03 19:38:14.000000 donatello-1.0.5/donatello.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-03 19:38:14.000000 donatello-1.0.5/donatello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      982 2023-01-03 19:37:38.000000 donatello-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      111 2023-01-03 19:38:14.900296 donatello-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1593 2023-01-03 19:23:53.000000 donatello-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 20:24:35.429831 donatello-1.0.7/
+-rw-rw-rw-   0        0        0     1069 2022-11-07 08:36:06.000000 donatello-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3127 2023-05-15 20:24:35.429831 donatello-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2202 2023-04-13 18:03:11.000000 donatello-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 20:24:35.211042 donatello-1.0.7/donatello/
+drwxrwxrwx   0        0        0        0 2023-05-15 20:24:35.289232 donatello-1.0.7/donatello/client/
+-rw-rw-rw-   0        0        0      269 2023-01-03 19:17:01.000000 donatello-1.0.7/donatello/client/__init__.py
+-rw-rw-rw-   0        0        0     1992 2023-01-03 19:18:31.000000 donatello-1.0.7/donatello/client/async_client.py
+-rw-rw-rw-   0        0        0     1429 2023-01-03 19:04:27.000000 donatello-1.0.7/donatello/client/base.py
+-rw-rw-rw-   0        0        0     1879 2023-01-03 19:17:45.000000 donatello-1.0.7/donatello/client/client.py
+drwxrwxrwx   0        0        0        0 2023-05-15 20:24:35.320392 donatello-1.0.7/donatello/donatello.egg-info/
+-rw-rw-rw-   0        0        0     3127 2023-05-15 20:24:35.000000 donatello-1.0.7/donatello/donatello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      706 2023-05-15 20:24:35.000000 donatello-1.0.7/donatello/donatello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 20:24:35.000000 donatello-1.0.7/donatello/donatello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-15 20:24:35.000000 donatello-1.0.7/donatello/donatello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-15 20:24:35.000000 donatello-1.0.7/donatello/donatello.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 20:24:35.351725 donatello-1.0.7/donatello/driver/
+-rw-rw-rw-   0        0        0      114 2023-04-13 18:28:22.000000 donatello-1.0.7/donatello/driver/__init__.py
+-rw-rw-rw-   0        0        0      673 2023-04-13 18:30:14.000000 donatello-1.0.7/donatello/driver/api_driver.py
+-rw-rw-rw-   0        0        0      792 2023-04-13 18:30:14.000000 donatello-1.0.7/donatello/driver/async_api_driver.py
+-rw-rw-rw-   0        0        0      586 2023-04-13 18:29:35.000000 donatello-1.0.7/donatello/driver/base.py
+drwxrwxrwx   0        0        0        0 2023-05-15 20:24:35.429831 donatello-1.0.7/donatello/models/
+-rw-rw-rw-   0        0        0      193 2023-04-13 18:17:09.000000 donatello-1.0.7/donatello/models/__init__.py
+-rw-rw-rw-   0        0        0      589 2023-04-13 18:23:36.000000 donatello-1.0.7/donatello/models/client.py
+-rw-rw-rw-   0        0        0      756 2023-04-13 18:23:36.000000 donatello-1.0.7/donatello/models/client_list.py
+-rw-rw-rw-   0        0        0     1073 2023-04-13 18:23:36.000000 donatello-1.0.7/donatello/models/donate.py
+-rw-rw-rw-   0        0        0     1030 2023-04-13 18:23:36.000000 donatello-1.0.7/donatello/models/donate_list.py
+-rw-rw-rw-   0        0        0      967 2023-04-13 18:23:36.000000 donatello-1.0.7/donatello/models/user.py
+-rw-rw-rw-   0        0        0      572 2023-04-13 18:23:36.000000 donatello-1.0.7/donatello/models/user_donates.py
+-rw-rw-rw-   0        0        0     1383 2023-05-15 20:22:41.000000 donatello-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      612 2023-05-15 20:24:35.429831 donatello-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1613 2023-05-15 20:18:35.000000 donatello-1.0.7/setup.py
```

### Comparing `donatello-1.0.5/LICENSE` & `donatello-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `donatello-1.0.5/PKG-INFO` & `donatello-1.0.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,40 @@
 Metadata-Version: 2.1
 Name: donatello
-Version: 1.0.5
+Version: 1.0.7
 Summary: 🐍 Python API wrapper for Ukrainian donate service Donatello
 Home-page: https://github.com/selfkilla666/donatello
-Download-URL: https://github.com/selfkilla666/donatello/blob/main/dist/donatello-1.0.5.tar.gz
+Download-URL: https://github.com/selfkilla666/donatello/blob/main/dist/donatello-1.0.7.tar.gz
 Author: selfkilla666 & Beengoo
 Author-email: selfkilla666 <selfkilla666@yahoo.com>, Beengoo <olddft@gmail.com>
 License: MIT License (MIT)
 Project-URL: Homepage, https://github.com/selfkilla666/donatello/
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Requires-Python: >=3.7.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Donatello.py
 
 
 ![Made with Python](https://img.shields.io/badge/Made%20with-Python-%23FFD242?logo=python&logoColor=white)
 ![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)
-![Version: 1.0.5](https://img.shields.io/badge/version-1.0.5-white)
-![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
+![Version: 1.0.7](https://img.shields.io/badge/version-1.0.7-red)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/donatello?color=succeses&logo=Pypi&logoColor=white)
-![Python version: 3.7 | 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/pypi/pyversions/donatello_api?color=blue&label=Python%20version)
 
 🐍 Unofficial Python wrapper for working with the API of the Ukrainian service for donations [Donatello](https://donatello.to/)
 
 [GitHub](https://github.com/selfkilla666/donatello/) | [PyPI](https://pypi.org/project/donatello/) | [Discord server](https://discord.gg/donatello-498101952333479956)
 <br>
-[Українська версія](https://github.com/selfkilla666/donatello/blob/main/README_UK.md)
 
 ---
 
 ## Quickstart
 
 Before you start, you need to take a couple of steps
 1) First you need to create a Donatello token and enable the API functionality, all this can be done in your account on the API page
@@ -58,15 +50,15 @@
 
 
 token = "<YOUR TOKEN HERE>"
 client = Donatello(token)
 
 me = client.get_me()
 
-# print your account nickname
+# Print your account nickname
 print(me.nickname)
 
 ```
 
 ### Get donations
 
 You may need to get a list of your donations, and there is a `get_donates()` method specifically for this, which will return you a convenient list of them
@@ -75,16 +67,15 @@
 
 from donatello import Donatello
 
 
 token = "<YOUR TOKEN HERE>"
 client = Donatello(token)
 
-# size = 5 - get 5 last donates
-donates = client.get_donates(size = 5)
+donates = client.get_donates(size = 5) # "size = 5" - Get 5 last donates
 
 for donate in donates:
     print(f"{donate.client_name}: {donate.message}")
 
 ```
     
 ### Get top donators
@@ -110,8 +101,7 @@
 ---
 
 ## In future
 
 - [ ] Add async API driver
 - [ ] Add docs
 - [ ] Longpolling / Events
-- [ ] Support new features in Donatello API
```

### Comparing `donatello-1.0.5/README.md` & `donatello-1.0.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # Donatello.py
 
 
 ![Made with Python](https://img.shields.io/badge/Made%20with-Python-%23FFD242?logo=python&logoColor=white)
 ![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)
-![Version: 1.0.5](https://img.shields.io/badge/version-1.0.5-white)
-![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
+![Version: 1.0.7](https://img.shields.io/badge/version-1.0.7-red)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/donatello?color=succeses&logo=Pypi&logoColor=white)
-![Python version: 3.7 | 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/pypi/pyversions/donatello_api?color=blue&label=Python%20version)
 
 🐍 Unofficial Python wrapper for working with the API of the Ukrainian service for donations [Donatello](https://donatello.to/)
 
 [GitHub](https://github.com/selfkilla666/donatello/) | [PyPI](https://pypi.org/project/donatello/) | [Discord server](https://discord.gg/donatello-498101952333479956)
 <br>
-[Українська версія](https://github.com/selfkilla666/donatello/blob/main/README_UK.md)
 
 ---
 
 ## Quickstart
 
 Before you start, you need to take a couple of steps
 1) First you need to create a Donatello token and enable the API functionality, all this can be done in your account on the API page
@@ -32,15 +29,15 @@
 
 
 token = "<YOUR TOKEN HERE>"
 client = Donatello(token)
 
 me = client.get_me()
 
-# print your account nickname
+# Print your account nickname
 print(me.nickname)
 
 ```
 
 ### Get donations
 
 You may need to get a list of your donations, and there is a `get_donates()` method specifically for this, which will return you a convenient list of them
@@ -49,16 +46,15 @@
 
 from donatello import Donatello
 
 
 token = "<YOUR TOKEN HERE>"
 client = Donatello(token)
 
-# size = 5 - get 5 last donates
-donates = client.get_donates(size = 5)
+donates = client.get_donates(size = 5) # "size = 5" - Get 5 last donates
 
 for donate in donates:
     print(f"{donate.client_name}: {donate.message}")
 
 ```
     
 ### Get top donators
@@ -84,8 +80,7 @@
 ---
 
 ## In future
 
 - [ ] Add async API driver
 - [ ] Add docs
 - [ ] Longpolling / Events
-- [ ] Support new features in Donatello API
```

### Comparing `donatello-1.0.5/donatello.egg-info/PKG-INFO` & `donatello-1.0.7/donatello/donatello.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,40 @@
 Metadata-Version: 2.1
 Name: donatello
-Version: 1.0.5
+Version: 1.0.7
 Summary: 🐍 Python API wrapper for Ukrainian donate service Donatello
 Home-page: https://github.com/selfkilla666/donatello
-Download-URL: https://github.com/selfkilla666/donatello/blob/main/dist/donatello-1.0.5.tar.gz
+Download-URL: https://github.com/selfkilla666/donatello/blob/main/dist/donatello-1.0.7.tar.gz
 Author: selfkilla666 & Beengoo
 Author-email: selfkilla666 <selfkilla666@yahoo.com>, Beengoo <olddft@gmail.com>
 License: MIT License (MIT)
 Project-URL: Homepage, https://github.com/selfkilla666/donatello/
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Requires-Python: >=3.7.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Donatello.py
 
 
 ![Made with Python](https://img.shields.io/badge/Made%20with-Python-%23FFD242?logo=python&logoColor=white)
 ![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)
-![Version: 1.0.5](https://img.shields.io/badge/version-1.0.5-white)
-![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
+![Version: 1.0.7](https://img.shields.io/badge/version-1.0.7-red)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/donatello?color=succeses&logo=Pypi&logoColor=white)
-![Python version: 3.7 | 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/pypi/pyversions/donatello_api?color=blue&label=Python%20version)
 
 🐍 Unofficial Python wrapper for working with the API of the Ukrainian service for donations [Donatello](https://donatello.to/)
 
 [GitHub](https://github.com/selfkilla666/donatello/) | [PyPI](https://pypi.org/project/donatello/) | [Discord server](https://discord.gg/donatello-498101952333479956)
 <br>
-[Українська версія](https://github.com/selfkilla666/donatello/blob/main/README_UK.md)
 
 ---
 
 ## Quickstart
 
 Before you start, you need to take a couple of steps
 1) First you need to create a Donatello token and enable the API functionality, all this can be done in your account on the API page
@@ -58,15 +50,15 @@
 
 
 token = "<YOUR TOKEN HERE>"
 client = Donatello(token)
 
 me = client.get_me()
 
-# print your account nickname
+# Print your account nickname
 print(me.nickname)
 
 ```
 
 ### Get donations
 
 You may need to get a list of your donations, and there is a `get_donates()` method specifically for this, which will return you a convenient list of them
@@ -75,16 +67,15 @@
 
 from donatello import Donatello
 
 
 token = "<YOUR TOKEN HERE>"
 client = Donatello(token)
 
-# size = 5 - get 5 last donates
-donates = client.get_donates(size = 5)
+donates = client.get_donates(size = 5) # "size = 5" - Get 5 last donates
 
 for donate in donates:
     print(f"{donate.client_name}: {donate.message}")
 
 ```
     
 ### Get top donators
@@ -110,8 +101,7 @@
 ---
 
 ## In future
 
 - [ ] Add async API driver
 - [ ] Add docs
 - [ ] Longpolling / Events
-- [ ] Support new features in Donatello API
```

### Comparing `donatello-1.0.5/setup.py` & `donatello-1.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,100 +1,101 @@
 00000000: 0d0a 6672 6f6d 2073 6574 7570 746f 6f6c  ..from setuptool
-00000010: 7320 696d 706f 7274 2073 6574 7570 0d0a  s import setup..
-00000020: 0d0a 4e41 4d45 203d 2022 646f 6e61 7465  ..NAME = "donate
-00000030: 6c6c 6f22 0d0a 4445 5343 5249 5054 494f  llo"..DESCRIPTIO
-00000040: 4e20 3d20 22f0 9f90 8d20 5079 7468 6f6e  N = ".... Python
-00000050: 2041 5049 2077 7261 7070 6572 2066 6f72   API wrapper for
-00000060: 2055 6b72 6169 6e69 616e 2064 6f6e 6174   Ukrainian donat
-00000070: 6520 7365 7276 6963 6520 446f 6e61 7465  e service Donate
-00000080: 6c6c 6f22 0d0a 5552 4c20 3d20 2268 7474  llo"..URL = "htt
-00000090: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000000a0: 7365 6c66 6b69 6c6c 6136 3636 2f64 6f6e  selfkilla666/don
-000000b0: 6174 656c 6c6f 220d 0a45 4d41 494c 203d  atello"..EMAIL =
-000000c0: 2022 7365 6c66 6b69 6c6c 6136 3636 4079   "selfkilla666@y
-000000d0: 6168 6f6f 2e63 6f6d 2026 206f 6c64 6466  ahoo.com & olddf
-000000e0: 7440 676d 6169 6c2e 636f 6d22 0d0a 4155  t@gmail.com"..AU
-000000f0: 5448 4f52 203d 2022 7365 6c66 6b69 6c6c  THOR = "selfkill
-00000100: 6136 3636 2026 2042 6565 6e67 6f6f 220d  a666 & Beengoo".
-00000110: 0a50 5954 484f 4e5f 5245 5155 4952 4553  .PYTHON_REQUIRES
-00000120: 203d 2022 3e3d 332e 372e 3022 0d0a 5645   = ">=3.7.0"..VE
-00000130: 5253 494f 4e20 3d20 2231 2e30 2e35 220d  RSION = "1.0.5".
-00000140: 0a0d 0a52 4551 5549 5245 4420 3d20 5b22  ...REQUIRED = ["
-00000150: 6169 6f68 7474 7022 2c20 2272 6571 7565  aiohttp", "reque
-00000160: 7374 7322 2c20 2270 7964 616e 7469 6322  sts", "pydantic"
-00000170: 5d0d 0a0d 0a74 7279 3a0d 0a20 2020 2077  ]....try:..    w
-00000180: 6974 6820 6f70 656e 2822 5245 4144 4d45  ith open("README
-00000190: 2e6d 6422 2c20 656e 636f 6469 6e67 3d22  .md", encoding="
-000001a0: 7574 662d 3822 2920 6173 2066 696c 653a  utf-8") as file:
-000001b0: 0d0a 2020 2020 2020 2020 4c4f 4e47 5f44  ..        LONG_D
-000001c0: 4553 4352 4950 5449 4f4e 203d 2022 5c6e  ESCRIPTION = "\n
-000001d0: 2220 2b20 6669 6c65 2e72 6561 6428 290d  " + file.read().
-000001e0: 0a65 7863 6570 7420 4669 6c65 4e6f 7446  .except FileNotF
-000001f0: 6f75 6e64 4572 726f 723a 0d0a 2020 2020  oundError:..    
-00000200: 4c4f 4e47 5f44 4553 4352 4950 5449 4f4e  LONG_DESCRIPTION
-00000210: 203d 2044 4553 4352 4950 5449 4f4e 0d0a   = DESCRIPTION..
-00000220: 0d0a 7365 7475 7028 0d0a 2020 2020 6e61  ..setup(..    na
-00000230: 6d65 3d4e 414d 452c 0d0a 2020 2020 7665  me=NAME,..    ve
-00000240: 7273 696f 6e3d 5645 5253 494f 4e2c 0d0a  rsion=VERSION,..
-00000250: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-00000260: 4445 5343 5249 5054 494f 4e2c 0d0a 2020  DESCRIPTION,..  
-00000270: 2020 6c6f 6e67 5f64 6573 6372 6970 7469    long_descripti
-00000280: 6f6e 3d4c 4f4e 475f 4445 5343 5249 5054  on=LONG_DESCRIPT
-00000290: 494f 4e2c 0d0a 2020 2020 6c6f 6e67 5f64  ION,..    long_d
-000002a0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
-000002b0: 6e74 5f74 7970 653d 2274 6578 742f 6d61  nt_type="text/ma
-000002c0: 726b 646f 776e 222c 0d0a 2020 2020 6175  rkdown",..    au
-000002d0: 7468 6f72 3d41 5554 484f 522c 0d0a 2020  thor=AUTHOR,..  
-000002e0: 2020 6175 7468 6f72 5f65 6d61 696c 3d45    author_email=E
-000002f0: 4d41 494c 2c0d 0a20 2020 2070 7974 686f  MAIL,..    pytho
-00000300: 6e5f 7265 7175 6972 6573 3d50 5954 484f  n_requires=PYTHO
-00000310: 4e5f 5245 5155 4952 4553 2c0d 0a20 2020  N_REQUIRES,..   
-00000320: 2075 726c 3d55 524c 2c0d 0a20 2020 2064   url=URL,..    d
-00000330: 6f77 6e6c 6f61 645f 7572 6c3d 2268 7474  ownload_url="htt
-00000340: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000350: 7365 6c66 6b69 6c6c 6136 3636 2f64 6f6e  selfkilla666/don
-00000360: 6174 656c 6c6f 2f62 6c6f 622f 6d61 696e  atello/blob/main
-00000370: 2f64 6973 742f 646f 6e61 7465 6c6c 6f2d  /dist/donatello-
-00000380: 312e 302e 352e 7461 722e 677a 222c 0d0a  1.0.5.tar.gz",..
-00000390: 2020 2020 7061 636b 6167 6573 3d5b 2264      packages=["d
-000003a0: 6f6e 6174 656c 6c6f 225d 2c0d 0a20 2020  onatello"],..   
-000003b0: 2069 6e73 7461 6c6c 5f72 6571 7569 7265   install_require
-000003c0: 733d 5245 5155 4952 4544 2c0d 0a20 2020  s=REQUIRED,..   
-000003d0: 206c 6963 656e 7365 3d22 4d49 5420 4c69   license="MIT Li
-000003e0: 6365 6e73 6520 284d 4954 2922 2c0d 0a20  cense (MIT)",.. 
-000003f0: 2020 2063 6c61 7373 6966 6965 7273 3d5b     classifiers=[
-00000400: 0d0a 2020 2020 2020 2020 2250 726f 6772  ..        "Progr
-00000410: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000420: 3a3a 2050 7974 686f 6e22 2c0d 0a20 2020  :: Python",..   
-00000430: 2020 2020 2022 5072 6f67 7261 6d6d 696e       "Programmin
-00000440: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000450: 7468 6f6e 203a 3a20 3322 2c0d 0a20 2020  thon :: 3",..   
-00000460: 2020 2020 2022 5072 6f67 7261 6d6d 696e       "Programmin
-00000470: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000480: 7468 6f6e 203a 3a20 332e 3722 2c0d 0a20  thon :: 3.7",.. 
-00000490: 2020 2020 2020 2022 5072 6f67 7261 6d6d         "Programm
-000004a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000004b0: 5079 7468 6f6e 203a 3a20 332e 3822 2c0d  Python :: 3.8",.
-000004c0: 0a20 2020 2020 2020 2022 5072 6f67 7261  .        "Progra
-000004d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000004e0: 3a20 5079 7468 6f6e 203a 3a20 332e 3922  : Python :: 3.9"
-000004f0: 2c0d 0a20 2020 2020 2020 2022 5072 6f67  ,..        "Prog
-00000500: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000510: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000520: 3130 222c 0d0a 2020 2020 2020 2020 2250  10",..        "P
-00000530: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000540: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000550: 2033 2e31 3122 2c0d 0a09 0922 4f70 6572   3.11",...."Oper
-00000560: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000570: 4f53 2049 6e64 6570 656e 6465 6e74 222c  OS Independent",
-00000580: 0d0a 2020 2020 2020 2020 2254 6f70 6963  ..        "Topic
-00000590: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
-000005a0: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
-000005b0: 6172 6965 7322 2c0d 0a20 2020 2020 2020  aries",..       
-000005c0: 2022 546f 7069 6320 3a3a 2053 6f66 7477   "Topic :: Softw
-000005d0: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
-000005e0: 3a3a 204c 6962 7261 7269 6573 203a 3a20  :: Libraries :: 
-000005f0: 5079 7468 6f6e 204d 6f64 756c 6573 222c  Python Modules",
-00000600: 0d0a 0909 2254 6f70 6963 203a 3a20 5574  ...."Topic :: Ut
-00000610: 696c 6974 6965 7322 2c0d 0a09 0922 5479  ilities",...."Ty
-00000620: 7069 6e67 203a 3a20 5479 7065 6422 2c0d  ping :: Typed",.
-00000630: 0a20 2020 205d 0d0a 29                   .    ]..)
+00000010: 7320 696d 706f 7274 2073 6574 7570 2c20  s import setup, 
+00000020: 6669 6e64 5f70 6163 6b61 6765 730d 0a0d  find_packages...
+00000030: 0a4e 414d 4520 3d20 2264 6f6e 6174 656c  .NAME = "donatel
+00000040: 6c6f 220d 0a44 4553 4352 4950 5449 4f4e  lo"..DESCRIPTION
+00000050: 203d 2022 f09f 908d 2050 7974 686f 6e20   = ".... Python 
+00000060: 4150 4920 7772 6170 7065 7220 666f 7220  API wrapper for 
+00000070: 556b 7261 696e 6961 6e20 646f 6e61 7465  Ukrainian donate
+00000080: 2073 6572 7669 6365 2044 6f6e 6174 656c   service Donatel
+00000090: 6c6f 220d 0a55 524c 203d 2022 6874 7470  lo"..URL = "http
+000000a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+000000b0: 656c 666b 696c 6c61 3636 362f 646f 6e61  elfkilla666/dona
+000000c0: 7465 6c6c 6f22 0d0a 454d 4149 4c20 3d20  tello"..EMAIL = 
+000000d0: 2273 656c 666b 696c 6c61 3636 3640 7961  "selfkilla666@ya
+000000e0: 686f 6f2e 636f 6d20 2620 6f6c 6464 6674  hoo.com & olddft
+000000f0: 4067 6d61 696c 2e63 6f6d 220d 0a41 5554  @gmail.com"..AUT
+00000100: 484f 5220 3d20 2273 656c 666b 696c 6c61  HOR = "selfkilla
+00000110: 3636 3620 2620 4265 656e 676f 6f22 0d0a  666 & Beengoo"..
+00000120: 5059 5448 4f4e 5f52 4551 5549 5245 5320  PYTHON_REQUIRES 
+00000130: 3d20 223e 3d33 2e39 2e30 220d 0a56 4552  = ">=3.9.0"..VER
+00000140: 5349 4f4e 203d 2022 312e 302e 3722 0d0a  SION = "1.0.7"..
+00000150: 0d0a 5245 5155 4952 4544 203d 205b 2261  ..REQUIRED = ["a
+00000160: 696f 6874 7470 222c 2022 7265 7175 6573  iohttp", "reques
+00000170: 7473 222c 2022 7079 6461 6e74 6963 225d  ts", "pydantic"]
+00000180: 0d0a 0d0a 7472 793a 0d0a 2020 2020 7769  ....try:..    wi
+00000190: 7468 206f 7065 6e28 2252 4541 444d 452e  th open("README.
+000001a0: 6d64 222c 2065 6e63 6f64 696e 673d 2275  md", encoding="u
+000001b0: 7466 2d38 2229 2061 7320 6669 6c65 3a0d  tf-8") as file:.
+000001c0: 0a20 2020 2020 2020 204c 4f4e 475f 4445  .        LONG_DE
+000001d0: 5343 5249 5054 494f 4e20 3d20 225c 6e22  SCRIPTION = "\n"
+000001e0: 202b 2066 696c 652e 7265 6164 2829 0d0a   + file.read()..
+000001f0: 6578 6365 7074 2046 696c 654e 6f74 466f  except FileNotFo
+00000200: 756e 6445 7272 6f72 3a0d 0a20 2020 204c  undError:..    L
+00000210: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
+00000220: 3d20 4445 5343 5249 5054 494f 4e0d 0a0d  = DESCRIPTION...
+00000230: 0a73 6574 7570 280d 0a20 2020 206e 616d  .setup(..    nam
+00000240: 653d 4e41 4d45 2c0d 0a20 2020 2076 6572  e=NAME,..    ver
+00000250: 7369 6f6e 3d56 4552 5349 4f4e 2c0d 0a20  sion=VERSION,.. 
+00000260: 2020 2064 6573 6372 6970 7469 6f6e 3d44     description=D
+00000270: 4553 4352 4950 5449 4f4e 2c0d 0a20 2020  ESCRIPTION,..   
+00000280: 206c 6f6e 675f 6465 7363 7269 7074 696f   long_descriptio
+00000290: 6e3d 4c4f 4e47 5f44 4553 4352 4950 5449  n=LONG_DESCRIPTI
+000002a0: 4f4e 2c0d 0a20 2020 206c 6f6e 675f 6465  ON,..    long_de
+000002b0: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
+000002c0: 745f 7479 7065 3d22 7465 7874 2f6d 6172  t_type="text/mar
+000002d0: 6b64 6f77 6e22 2c0d 0a20 2020 2061 7574  kdown",..    aut
+000002e0: 686f 723d 4155 5448 4f52 2c0d 0a20 2020  hor=AUTHOR,..   
+000002f0: 2061 7574 686f 725f 656d 6169 6c3d 454d   author_email=EM
+00000300: 4149 4c2c 0d0a 2020 2020 7079 7468 6f6e  AIL,..    python
+00000310: 5f72 6571 7569 7265 733d 5059 5448 4f4e  _requires=PYTHON
+00000320: 5f52 4551 5549 5245 532c 0d0a 2020 2020  _REQUIRES,..    
+00000330: 7572 6c3d 5552 4c2c 0d0a 2020 2020 646f  url=URL,..    do
+00000340: 776e 6c6f 6164 5f75 726c 3d22 6874 7470  wnload_url="http
+00000350: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000360: 656c 666b 696c 6c61 3636 362f 646f 6e61  elfkilla666/dona
+00000370: 7465 6c6c 6f2f 626c 6f62 2f6d 6169 6e2f  tello/blob/main/
+00000380: 6469 7374 2f64 6f6e 6174 656c 6c6f 2d31  dist/donatello-1
+00000390: 2e30 2e37 2e74 6172 2e67 7a22 2c0d 0a20  .0.7.tar.gz",.. 
+000003a0: 2020 2070 6163 6b61 6765 5f64 6972 3d7b     package_dir={
+000003b0: 2222 3a22 646f 6e61 7465 6c6c 6f22 7d2c  "":"donatello"},
+000003c0: 0d0a 2020 2020 7061 636b 6167 6573 3d66  ..    packages=f
+000003d0: 696e 645f 7061 636b 6167 6573 2877 6865  ind_packages(whe
+000003e0: 7265 3d22 646f 6e61 7465 6c6c 6f22 292c  re="donatello"),
+000003f0: 0d0a 2020 2020 696e 7374 616c 6c5f 7265  ..    install_re
+00000400: 7175 6972 6573 3d52 4551 5549 5245 442c  quires=REQUIRED,
+00000410: 0d0a 2020 2020 6c69 6365 6e73 653d 224d  ..    license="M
+00000420: 4954 204c 6963 656e 7365 2028 4d49 5429  IT License (MIT)
+00000430: 222c 0d0a 2020 2020 636c 6173 7369 6669  ",..    classifi
+00000440: 6572 733d 5b0d 0a20 2020 2020 2020 2022  ers=[..        "
+00000450: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000460: 7561 6765 203a 3a20 5079 7468 6f6e 222c  uage :: Python",
+00000470: 0d0a 2020 2020 2020 2020 2250 726f 6772  ..        "Progr
+00000480: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000490: 3a3a 2050 7974 686f 6e20 3a3a 2033 222c  :: Python :: 3",
+000004a0: 0d0a 2020 2020 2020 2020 2250 726f 6772  ..        "Progr
+000004b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000004c0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
+000004d0: 222c 0d0a 2020 2020 2020 2020 2250 726f  ",..        "Pro
+000004e0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000004f0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000500: 2e31 3022 2c0d 0a20 2020 2020 2020 2022  .10",..        "
+00000510: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000520: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000530: 3a20 332e 3131 222c 0d0a 2020 2020 2020  : 3.11",..      
+00000540: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
+00000550: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000560: 6e20 3a3a 2033 2e31 3222 2c0d 0a09 0922  n :: 3.12",...."
+00000570: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000580: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+00000590: 6e74 222c 0d0a 2020 2020 2020 2020 2254  nt",..        "T
+000005a0: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+000005b0: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
+000005c0: 4c69 6272 6172 6965 7322 2c0d 0a20 2020  Libraries",..   
+000005d0: 2020 2020 2022 546f 7069 6320 3a3a 2053       "Topic :: S
+000005e0: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
+000005f0: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
+00000600: 203a 3a20 5079 7468 6f6e 204d 6f64 756c   :: Python Modul
+00000610: 6573 222c 0d0a 0909 2254 6f70 6963 203a  es",...."Topic :
+00000620: 3a20 5574 696c 6974 6965 7322 2c0d 0a09  : Utilities",...
+00000630: 0922 5479 7069 6e67 203a 3a20 5479 7065  ."Typing :: Type
+00000640: 6422 2c0d 0a20 2020 205d 0d0a 29         d",..    ]..)
```

