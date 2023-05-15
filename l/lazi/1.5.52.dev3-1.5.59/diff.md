# Comparing `tmp/lazi-1.5.52.dev3.tar.gz` & `tmp/lazi-1.5.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazi-1.5.52.dev3.tar", max compression
+gzip compressed data, was "lazi-1.5.59.tar", max compression
```

## Comparing `lazi-1.5.52.dev3.tar` & `lazi-1.5.59.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.5.52.dev3/LICENSE
--rw-r--r--   0        0        0     1917 2023-05-15 07:59:50.478074 lazi-1.5.52.dev3/README.md
--rw-r--r--   0        0        0      197 2023-05-15 07:36:15.807454 lazi-1.5.52.dev3/lazi/auto.py
--rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.5.52.dev3/lazi/conf/auto.py
--rw-r--r--   0        0        0     1001 2023-05-15 19:51:29.591920 lazi-1.5.52.dev3/lazi/conf/base.py
--rw-r--r--   0        0        0     4738 2023-05-15 15:37:52.100153 lazi-1.5.52.dev3/lazi/conf/conf.py
--rw-r--r--   0        0        0       99 2023-05-15 15:35:10.790089 lazi-1.5.52.dev3/lazi/conf/test.py
--rw-r--r--   0        0        0      364 2023-05-15 07:36:15.807454 lazi-1.5.52.dev3/lazi/core/__init__.py
--rw-r--r--   0        0        0     3162 2023-05-15 19:51:00.219534 lazi-1.5.52.dev3/lazi/core/finder.py
--rw-r--r--   0        0        0     3655 2023-05-15 19:34:47.954749 lazi-1.5.52.dev3/lazi/core/loader.py
--rw-r--r--   0        0        0     3192 2023-05-15 19:48:21.985456 lazi-1.5.52.dev3/lazi/core/module.py
--rw-r--r--   0        0        0     1211 2023-05-15 19:47:25.048708 lazi-1.5.52.dev3/lazi/core/spec.py
--rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.5.52.dev3/lazi/util/__init__.py
--rw-r--r--   0        0        0      448 2023-05-15 19:22:20.692875 lazi-1.5.52.dev3/lazi/util/debug.py
--rw-r--r--   0        0        0      146 2023-05-15 19:51:00.223534 lazi-1.5.52.dev3/lazi/util/functional.py
--rw-r--r--   0        0        0      618 2023-05-11 20:06:44.097623 lazi-1.5.52.dev3/lazi/util/util.py
--rw-r--r--   0        0        0     1560 2023-05-15 19:04:55.642967 lazi-1.5.52.dev3/pyproject.toml
--rw-r--r--   0        0        0      273 2023-05-15 18:29:35.039325 lazi-1.5.52.dev3/tests/standalone/sa_pygments.py
--rw-r--r--   0        0        0      380 2023-05-15 15:58:12.284137 lazi-1.5.52.dev3/tests/test_array.py
--rw-r--r--   0        0        0      901 2023-05-15 15:52:23.767715 lazi-1.5.52.dev3/tests/test_django.py
--rw-r--r--   0        0        0      810 2023-05-15 17:48:17.171059 lazi-1.5.52.dev3/tests/test_pygments.py
--rw-r--r--   0        0        0      775 2023-05-15 15:54:31.125344 lazi-1.5.52.dev3/tests/test_requests.py
--rw-r--r--   0        0        0     2795 2023-05-15 19:40:10.903002 lazi-1.5.52.dev3/tests/test_rich.py
--rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 lazi-1.5.52.dev3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.5.59/LICENSE
+-rw-r--r--   0        0        0     1917 2023-05-15 07:59:50.478074 lazi-1.5.59/README.md
+-rw-r--r--   0        0        0      197 2023-05-15 07:36:15.807454 lazi-1.5.59/lazi/auto.py
+-rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.5.59/lazi/conf/auto.py
+-rw-r--r--   0        0        0     1001 2023-05-15 19:51:29.591920 lazi-1.5.59/lazi/conf/base.py
+-rw-r--r--   0        0        0     4738 2023-05-15 15:37:52.100153 lazi-1.5.59/lazi/conf/conf.py
+-rw-r--r--   0        0        0       99 2023-05-15 15:35:10.790089 lazi-1.5.59/lazi/conf/test.py
+-rw-r--r--   0        0        0      364 2023-05-15 07:36:15.807454 lazi-1.5.59/lazi/core/__init__.py
+-rw-r--r--   0        0        0     3162 2023-05-15 19:51:00.219534 lazi-1.5.59/lazi/core/finder.py
+-rw-r--r--   0        0        0     3655 2023-05-15 19:34:47.954749 lazi-1.5.59/lazi/core/loader.py
+-rw-r--r--   0        0        0     3192 2023-05-15 19:48:21.985456 lazi-1.5.59/lazi/core/module.py
+-rw-r--r--   0        0        0     1211 2023-05-15 19:47:25.048708 lazi-1.5.59/lazi/core/spec.py
+-rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.5.59/lazi/util/__init__.py
+-rw-r--r--   0        0        0      448 2023-05-15 19:22:20.692875 lazi-1.5.59/lazi/util/debug.py
+-rw-r--r--   0        0        0      146 2023-05-15 19:51:00.223534 lazi-1.5.59/lazi/util/functional.py
+-rw-r--r--   0        0        0      618 2023-05-11 20:06:44.097623 lazi-1.5.59/lazi/util/util.py
+-rw-r--r--   0        0        0     1555 2023-05-15 19:52:32.320744 lazi-1.5.59/pyproject.toml
+-rw-r--r--   0        0        0      273 2023-05-15 18:29:35.039325 lazi-1.5.59/tests/standalone/sa_pygments.py
+-rw-r--r--   0        0        0      380 2023-05-15 15:58:12.284137 lazi-1.5.59/tests/test_array.py
+-rw-r--r--   0        0        0      901 2023-05-15 15:52:23.767715 lazi-1.5.59/tests/test_django.py
+-rw-r--r--   0        0        0      810 2023-05-15 17:48:17.171059 lazi-1.5.59/tests/test_pygments.py
+-rw-r--r--   0        0        0      775 2023-05-15 15:54:31.125344 lazi-1.5.59/tests/test_requests.py
+-rw-r--r--   0        0        0     2795 2023-05-15 19:40:10.903002 lazi-1.5.59/tests/test_rich.py
+-rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 lazi-1.5.59/PKG-INFO
```

### Comparing `lazi-1.5.52.dev3/LICENSE` & `lazi-1.5.59/LICENSE`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52.dev3/README.md` & `lazi-1.5.59/README.md`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52.dev3/lazi/conf/base.py` & `lazi-1.5.59/lazi/conf/base.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52.dev3/lazi/conf/conf.py` & `lazi-1.5.59/lazi/conf/conf.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52.dev3/lazi/core/finder.py` & `lazi-1.5.59/lazi/core/finder.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52.dev3/lazi/core/loader.py` & `lazi-1.5.59/lazi/core/loader.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52.dev3/lazi/core/module.py` & `lazi-1.5.59/lazi/core/module.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52.dev3/lazi/core/spec.py` & `lazi-1.5.59/lazi/core/spec.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52.dev3/lazi/util/util.py` & `lazi-1.5.59/lazi/util/util.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52.dev3/pyproject.toml` & `lazi-1.5.59/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazi"
-version = "1.5.52-dev3"
+version = "1.5.59"
 description = "A lightweight and extensible way to implement lazy imports globally."
 authors = ["Phillip Sitbon <phillip.sitbon@gmail.com>"]
 readme = "README.md"
 license = "AGPLv3"
 repository = "https://github.com/sitbon/lazi"
 classifiers= [
     "Environment :: Web Environment",
```

### Comparing `lazi-1.5.52.dev3/tests/test_django.py` & `lazi-1.5.59/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52.dev3/tests/test_pygments.py` & `lazi-1.5.59/tests/test_pygments.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52.dev3/tests/test_requests.py` & `lazi-1.5.59/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52.dev3/tests/test_rich.py` & `lazi-1.5.59/tests/test_rich.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52.dev3/PKG-INFO` & `lazi-1.5.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazi
-Version: 1.5.52.dev3
+Version: 1.5.59
 Summary: A lightweight and extensible way to implement lazy imports globally.
 Home-page: https://github.com/sitbon/lazi
 License: AGPLv3
 Author: Phillip Sitbon
 Author-email: phillip.sitbon@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Environment :: Web Environment
```

