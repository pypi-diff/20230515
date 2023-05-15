# Comparing `tmp/FastSession-0.1.0.tar.gz` & `tmp/FastSession-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastSession-0.1.0.tar", last modified: Mon May 15 08:02:30 2023, max compression
+gzip compressed data, was "FastSession-0.1.1.tar", last modified: Mon May 15 08:20:08 2023, max compression
```

## Comparing `FastSession-0.1.0.tar` & `FastSession-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 08:02:30.971331 FastSession-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-05-15 08:02:30.954028 FastSession-0.1.0/FastSession.egg-info/
--rw-rw-rw-   0        0        0     3260 2023-05-15 08:02:30.000000 FastSession-0.1.0/FastSession.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-05-15 08:02:30.000000 FastSession-0.1.0/FastSession.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 08:02:30.000000 FastSession-0.1.0/FastSession.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-15 08:02:30.000000 FastSession-0.1.0/FastSession.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-15 08:02:30.000000 FastSession-0.1.0/FastSession.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11556 2023-05-05 05:02:46.000000 FastSession-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3260 2023-05-15 08:02:30.971331 FastSession-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2557 2023-05-15 07:54:01.000000 FastSession-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 08:02:30.957666 FastSession-0.1.0/fastsession/
--rw-rw-rw-   0        0        0      165 2023-05-15 04:03:26.000000 FastSession-0.1.0/fastsession/__init__.py
--rw-rw-rw-   0        0        0    10213 2023-05-15 07:50:50.000000 FastSession-0.1.0/fastsession/fast_session_middleware.py
--rw-rw-rw-   0        0        0     3703 2023-05-15 07:22:02.000000 FastSession-0.1.0/fastsession/memory_store.py
--rw-rw-rw-   0        0        0     3020 2023-05-15 03:33:44.000000 FastSession-0.1.0/fastsession/timed_signature_serializer.py
--rw-rw-rw-   0        0        0       42 2023-05-15 08:02:30.971331 FastSession-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      866 2023-05-14 08:12:12.000000 FastSession-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:02:30.969638 FastSession-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-05-14 08:02:49.000000 FastSession-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     8754 2023-05-15 07:00:42.000000 FastSession-0.1.0/tests/test_session_middleware.py
--rw-rw-rw-   0        0        0      636 2023-05-15 01:16:58.000000 FastSession-0.1.0/tests/test_store_memory.py
--rw-rw-rw-   0        0        0     1740 2023-05-15 07:44:41.000000 FastSession-0.1.0/tests/test_timed_signature_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:20:08.934772 FastSession-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-05-15 08:20:08.921948 FastSession-0.1.1/FastSession.egg-info/
+-rw-rw-rw-   0        0        0     3272 2023-05-15 08:20:08.000000 FastSession-0.1.1/FastSession.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-05-15 08:20:08.000000 FastSession-0.1.1/FastSession.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 08:20:08.000000 FastSession-0.1.1/FastSession.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-15 08:20:08.000000 FastSession-0.1.1/FastSession.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-15 08:20:08.000000 FastSession-0.1.1/FastSession.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11556 2023-05-05 05:02:46.000000 FastSession-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3272 2023-05-15 08:20:08.934772 FastSession-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2557 2023-05-15 07:54:01.000000 FastSession-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 08:20:08.924456 FastSession-0.1.1/fastsession/
+-rw-rw-rw-   0        0        0      165 2023-05-15 04:03:26.000000 FastSession-0.1.1/fastsession/__init__.py
+-rw-rw-rw-   0        0        0    10213 2023-05-15 07:50:50.000000 FastSession-0.1.1/fastsession/fast_session_middleware.py
+-rw-rw-rw-   0        0        0     3703 2023-05-15 07:22:02.000000 FastSession-0.1.1/fastsession/memory_store.py
+-rw-rw-rw-   0        0        0     3020 2023-05-15 03:33:44.000000 FastSession-0.1.1/fastsession/timed_signature_serializer.py
+-rw-rw-rw-   0        0        0       42 2023-05-15 08:20:08.934772 FastSession-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      932 2023-05-15 08:14:22.000000 FastSession-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:20:08.925454 FastSession-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-14 08:02:49.000000 FastSession-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     8754 2023-05-15 07:00:42.000000 FastSession-0.1.1/tests/test_session_middleware.py
+-rw-rw-rw-   0        0        0      636 2023-05-15 01:16:58.000000 FastSession-0.1.1/tests/test_store_memory.py
+-rw-rw-rw-   0        0        0     1740 2023-05-15 07:44:41.000000 FastSession-0.1.1/tests/test_timed_signature_serializer.py
```

### Comparing `FastSession-0.1.0/FastSession.egg-info/PKG-INFO` & `FastSession-0.1.1/FastSession.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: FastSession
-Version: 0.1.0
+Version: 0.1.1
 Summary: A session middleware for Starlette and FastAPI
 Home-page: https://github.com/riversun/FastSession
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `FastSession-0.1.0/LICENSE` & `FastSession-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FastSession-0.1.0/PKG-INFO` & `FastSession-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: FastSession
-Version: 0.1.0
+Version: 0.1.1
 Summary: A session middleware for Starlette and FastAPI
 Home-page: https://github.com/riversun/FastSession
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `FastSession-0.1.0/README.md` & `FastSession-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `FastSession-0.1.0/fastsession/fast_session_middleware.py` & `FastSession-0.1.1/fastsession/fast_session_middleware.py`

 * *Files identical despite different names*

### Comparing `FastSession-0.1.0/fastsession/memory_store.py` & `FastSession-0.1.1/fastsession/memory_store.py`

 * *Files identical despite different names*

### Comparing `FastSession-0.1.0/fastsession/timed_signature_serializer.py` & `FastSession-0.1.1/fastsession/timed_signature_serializer.py`

 * *Files identical despite different names*

### Comparing `FastSession-0.1.0/setup.py` & `FastSession-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="FastSession",
-    version="0.1.0",
+    version="0.1.1",
     author="Tom Misawa",
     author_email="riversun.org@gmail.com",
     description="A session middleware for Starlette and FastAPI",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/riversun/FastSession",
-    packages=find_packages(),
+    packages=find_packages(exclude=["tests.*", "tests", "examples.*", "examples"]),
     tests_require=["pytest","httpx"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     python_requires=">=3.8",
     install_requires=[
         "starlette",
```

### Comparing `FastSession-0.1.0/tests/test_session_middleware.py` & `FastSession-0.1.1/tests/test_session_middleware.py`

 * *Files identical despite different names*

### Comparing `FastSession-0.1.0/tests/test_store_memory.py` & `FastSession-0.1.1/tests/test_store_memory.py`

 * *Files identical despite different names*

### Comparing `FastSession-0.1.0/tests/test_timed_signature_serializer.py` & `FastSession-0.1.1/tests/test_timed_signature_serializer.py`

 * *Files identical despite different names*

