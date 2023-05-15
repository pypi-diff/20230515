# Comparing `tmp/oss-python-sdk-1.0.1.tar.gz` & `tmp/oss-python-sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\oss-python-sdk-1.0.1.tar", last modified: Wed Apr 12 06:42:58 2023, max compression
+gzip compressed data, was "dist\oss-python-sdk-1.0.2.tar", last modified: Mon May 15 07:34:27 2023, max compression
```

## Comparing `oss-python-sdk-1.0.1.tar` & `oss-python-sdk-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 06:42:58.000000 oss-python-sdk-1.0.1/
--rw-rw-rw-   0        0        0      247 2023-04-12 06:42:58.000000 oss-python-sdk-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       20 2023-01-09 09:30:50.000000 oss-python-sdk-1.0.1/README.md
--rw-rw-rw-   0        0        0     1094 2023-01-10 02:34:59.000000 oss-python-sdk-1.0.1/license.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 06:42:58.000000 oss-python-sdk-1.0.1/oss/
--rw-rw-rw-   0        0        0      176 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.1/oss/__init__.py
--rw-rw-rw-   0        0        0    44863 2023-04-12 06:30:47.000000 oss-python-sdk-1.0.1/oss/api.py
--rw-rw-rw-   0        0        0     4328 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.1/oss/auth.py
--rw-rw-rw-   0        0        0     2326 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.1/oss/compat.py
--rw-rw-rw-   0        0        0     5097 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.1/oss/crc64_combine.py
--rw-rw-rw-   0        0        0     1449 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.1/oss/defaults.py
--rw-rw-rw-   0        0        0    20383 2023-01-10 00:59:04.000000 oss-python-sdk-1.0.1/oss/entity.py
--rw-rw-rw-   0        0        0     8253 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.1/oss/exceptions.py
--rw-rw-rw-   0        0        0     1791 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.1/oss/headers.py
--rw-rw-rw-   0        0        0     5880 2023-01-10 01:14:23.000000 oss-python-sdk-1.0.1/oss/http.py
--rw-rw-rw-   0        0        0     1237 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.1/oss/select_params.py
--rw-rw-rw-   0        0        0    10302 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.1/oss/select_response.py
--rw-rw-rw-   0        0        0    25152 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.1/oss/utils.py
--rw-rw-rw-   0        0        0    26073 2022-12-09 03:12:50.000000 oss-python-sdk-1.0.1/oss/xml_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 06:42:58.000000 oss-python-sdk-1.0.1/oss_python_sdk.egg-info/
--rw-rw-rw-   0        0        0      247 2023-04-12 06:42:58.000000 oss-python-sdk-1.0.1/oss_python_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-04-12 06:42:58.000000 oss-python-sdk-1.0.1/oss_python_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 06:42:58.000000 oss-python-sdk-1.0.1/oss_python_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-12 06:42:58.000000 oss-python-sdk-1.0.1/oss_python_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-12 06:42:58.000000 oss-python-sdk-1.0.1/oss_python_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 06:42:58.000000 oss-python-sdk-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      563 2023-04-12 06:26:39.000000 oss-python-sdk-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 07:34:27.000000 oss-python-sdk-1.0.2/
+-rw-rw-rw-   0        0        0      247 2023-05-15 07:34:27.000000 oss-python-sdk-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2023-01-09 09:30:50.000000 oss-python-sdk-1.0.2/README.md
+-rw-rw-rw-   0        0        0     1094 2023-01-10 02:34:59.000000 oss-python-sdk-1.0.2/license.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 07:34:27.000000 oss-python-sdk-1.0.2/oss/
+-rw-rw-rw-   0        0        0      176 2023-05-15 07:33:17.000000 oss-python-sdk-1.0.2/oss/__init__.py
+-rw-rw-rw-   0        0        0    44863 2023-04-12 06:30:47.000000 oss-python-sdk-1.0.2/oss/api.py
+-rw-rw-rw-   0        0        0     4328 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.2/oss/auth.py
+-rw-rw-rw-   0        0        0     2326 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.2/oss/compat.py
+-rw-rw-rw-   0        0        0     5097 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.2/oss/crc64_combine.py
+-rw-rw-rw-   0        0        0     1449 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.2/oss/defaults.py
+-rw-rw-rw-   0        0        0    20383 2023-01-10 00:59:04.000000 oss-python-sdk-1.0.2/oss/entity.py
+-rw-rw-rw-   0        0        0     8253 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.2/oss/exceptions.py
+-rw-rw-rw-   0        0        0     1791 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.2/oss/headers.py
+-rw-rw-rw-   0        0        0     5880 2023-01-10 01:14:23.000000 oss-python-sdk-1.0.2/oss/http.py
+-rw-rw-rw-   0        0        0     1237 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.2/oss/select_params.py
+-rw-rw-rw-   0        0        0    10302 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.2/oss/select_response.py
+-rw-rw-rw-   0        0        0    25152 2022-09-29 07:00:52.000000 oss-python-sdk-1.0.2/oss/utils.py
+-rw-rw-rw-   0        0        0    26073 2022-12-09 03:12:50.000000 oss-python-sdk-1.0.2/oss/xml_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 07:34:27.000000 oss-python-sdk-1.0.2/oss_python_sdk.egg-info/
+-rw-rw-rw-   0        0        0      247 2023-05-15 07:34:27.000000 oss-python-sdk-1.0.2/oss_python_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-05-15 07:34:27.000000 oss-python-sdk-1.0.2/oss_python_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 07:34:27.000000 oss-python-sdk-1.0.2/oss_python_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-15 07:34:27.000000 oss-python-sdk-1.0.2/oss_python_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-15 07:34:27.000000 oss-python-sdk-1.0.2/oss_python_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 07:34:27.000000 oss-python-sdk-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      563 2023-05-15 07:33:20.000000 oss-python-sdk-1.0.2/setup.py
```

### Comparing `oss-python-sdk-1.0.1/license.txt` & `oss-python-sdk-1.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `oss-python-sdk-1.0.1/oss/api.py` & `oss-python-sdk-1.0.2/oss/api.py`

 * *Files identical despite different names*

### Comparing `oss-python-sdk-1.0.1/oss/auth.py` & `oss-python-sdk-1.0.2/oss/auth.py`

 * *Files identical despite different names*

### Comparing `oss-python-sdk-1.0.1/oss/compat.py` & `oss-python-sdk-1.0.2/oss/compat.py`

 * *Files identical despite different names*

### Comparing `oss-python-sdk-1.0.1/oss/crc64_combine.py` & `oss-python-sdk-1.0.2/oss/crc64_combine.py`

 * *Files identical despite different names*

### Comparing `oss-python-sdk-1.0.1/oss/defaults.py` & `oss-python-sdk-1.0.2/oss/defaults.py`

 * *Files identical despite different names*

### Comparing `oss-python-sdk-1.0.1/oss/entity.py` & `oss-python-sdk-1.0.2/oss/entity.py`

 * *Files identical despite different names*

### Comparing `oss-python-sdk-1.0.1/oss/exceptions.py` & `oss-python-sdk-1.0.2/oss/exceptions.py`

 * *Files identical despite different names*

### Comparing `oss-python-sdk-1.0.1/oss/headers.py` & `oss-python-sdk-1.0.2/oss/headers.py`

 * *Files identical despite different names*

### Comparing `oss-python-sdk-1.0.1/oss/http.py` & `oss-python-sdk-1.0.2/oss/http.py`

 * *Files identical despite different names*

### Comparing `oss-python-sdk-1.0.1/oss/select_params.py` & `oss-python-sdk-1.0.2/oss/select_params.py`

 * *Files identical despite different names*

### Comparing `oss-python-sdk-1.0.1/oss/select_response.py` & `oss-python-sdk-1.0.2/oss/select_response.py`

 * *Files identical despite different names*

### Comparing `oss-python-sdk-1.0.1/oss/utils.py` & `oss-python-sdk-1.0.2/oss/utils.py`

 * *Files identical despite different names*

### Comparing `oss-python-sdk-1.0.1/oss/xml_utils.py` & `oss-python-sdk-1.0.2/oss/xml_utils.py`

 * *Files identical despite different names*

### Comparing `oss-python-sdk-1.0.1/setup.py` & `oss-python-sdk-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from distutils.core import setup
 
 with open('README.md', 'rb') as f:
     readme = f.read().decode('utf-8')
 
 setup(
     name='oss-python-sdk',
-    version='1.0.1',
+    version='1.0.2',
     description='OSS Python SDK',
     author='wangyingbin',
     author_email='869063218@qq.com',
     long_description=readme,
     packages=['oss'],
     install_requires=['requests!=2.9.0', 'crcmod>=1.7'],
     include_package_data=True,
```

