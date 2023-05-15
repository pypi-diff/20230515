# Comparing `tmp/my_python_serializer_release-0.2.0.tar.gz` & `tmp/my_python_serializer_release-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_python_serializer_release-0.2.0.tar", last modified: Mon May 15 21:13:46 2023, max compression
+gzip compressed data, was "my_python_serializer_release-0.2.1.tar", last modified: Mon May 15 21:16:11 2023, max compression
```

## Comparing `my_python_serializer_release-0.2.0.tar` & `my_python_serializer_release-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 egorbagrovets  (1000) egorbagrovets  (1000)        0 2023-05-15 21:13:46.642215 my_python_serializer_release-0.2.0/
--rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      114 2023-05-15 21:13:46.642215 my_python_serializer_release-0.2.0/PKG-INFO
-drwxr-xr-x   0 egorbagrovets  (1000) egorbagrovets  (1000)        0 2023-05-15 21:13:46.642215 my_python_serializer_release-0.2.0/my_python_serializer_release.egg-info/
--rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      114 2023-05-15 21:13:46.000000 my_python_serializer_release-0.2.0/my_python_serializer_release.egg-info/PKG-INFO
--rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      457 2023-05-15 21:13:46.000000 my_python_serializer_release-0.2.0/my_python_serializer_release.egg-info/SOURCES.txt
--rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)        1 2023-05-15 21:13:46.000000 my_python_serializer_release-0.2.0/my_python_serializer_release.egg-info/dependency_links.txt
--rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)       18 2023-05-15 21:13:46.000000 my_python_serializer_release-0.2.0/my_python_serializer_release.egg-info/requires.txt
--rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)       12 2023-05-15 21:13:46.000000 my_python_serializer_release-0.2.0/my_python_serializer_release.egg-info/top_level.txt
-drwxr-xr-x   0 egorbagrovets  (1000) egorbagrovets  (1000)        0 2023-05-15 21:13:46.642215 my_python_serializer_release-0.2.0/serializers/
--rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)     1404 2023-05-15 18:57:02.000000 my_python_serializer_release-0.2.0/serializers/constants.py
--rw-rw-r--   0 egorbagrovets  (1000) egorbagrovets  (1000)     6389 2023-05-15 18:52:51.000000 my_python_serializer_release-0.2.0/serializers/json.py
--rw-rw-r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      542 2023-05-15 18:54:17.000000 my_python_serializer_release-0.2.0/serializers/json_parser.py
--rw-rw-r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      430 2023-05-15 18:27:42.000000 my_python_serializer_release-0.2.0/serializers/parser.py
--rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      474 2023-05-15 18:32:02.000000 my_python_serializer_release-0.2.0/serializers/serializer_factory_method.py
--rw-rw-r--   0 egorbagrovets  (1000) egorbagrovets  (1000)     8969 2023-05-15 19:05:46.000000 my_python_serializer_release-0.2.0/serializers/xml.py
--rw-rw-r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      654 2023-05-15 18:54:35.000000 my_python_serializer_release-0.2.0/serializers/xml_parser.py
--rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)       38 2023-05-15 21:13:46.642215 my_python_serializer_release-0.2.0/setup.cfg
--rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      223 2023-05-15 21:13:44.000000 my_python_serializer_release-0.2.0/setup.py
+drwxr-xr-x   0 egorbagrovets  (1000) egorbagrovets  (1000)        0 2023-05-15 21:16:11.670002 my_python_serializer_release-0.2.1/
+-rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      114 2023-05-15 21:16:11.670002 my_python_serializer_release-0.2.1/PKG-INFO
+drwxr-xr-x   0 egorbagrovets  (1000) egorbagrovets  (1000)        0 2023-05-15 21:16:11.669002 my_python_serializer_release-0.2.1/my_python_serializer_release.egg-info/
+-rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      114 2023-05-15 21:16:11.000000 my_python_serializer_release-0.2.1/my_python_serializer_release.egg-info/PKG-INFO
+-rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      481 2023-05-15 21:16:11.000000 my_python_serializer_release-0.2.1/my_python_serializer_release.egg-info/SOURCES.txt
+-rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)        1 2023-05-15 21:16:11.000000 my_python_serializer_release-0.2.1/my_python_serializer_release.egg-info/dependency_links.txt
+-rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)       18 2023-05-15 21:16:11.000000 my_python_serializer_release-0.2.1/my_python_serializer_release.egg-info/requires.txt
+-rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)       12 2023-05-15 21:16:11.000000 my_python_serializer_release-0.2.1/my_python_serializer_release.egg-info/top_level.txt
+drwxr-xr-x   0 egorbagrovets  (1000) egorbagrovets  (1000)        0 2023-05-15 21:16:11.670002 my_python_serializer_release-0.2.1/serializers/
+-rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)       46 2023-05-15 19:33:11.000000 my_python_serializer_release-0.2.1/serializers/__init__.py
+-rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)     1404 2023-05-15 18:57:02.000000 my_python_serializer_release-0.2.1/serializers/constants.py
+-rw-rw-r--   0 egorbagrovets  (1000) egorbagrovets  (1000)     6389 2023-05-15 18:52:51.000000 my_python_serializer_release-0.2.1/serializers/json.py
+-rw-rw-r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      542 2023-05-15 18:54:17.000000 my_python_serializer_release-0.2.1/serializers/json_parser.py
+-rw-rw-r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      430 2023-05-15 18:27:42.000000 my_python_serializer_release-0.2.1/serializers/parser.py
+-rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      474 2023-05-15 18:32:02.000000 my_python_serializer_release-0.2.1/serializers/serializer_factory_method.py
+-rw-rw-r--   0 egorbagrovets  (1000) egorbagrovets  (1000)     8969 2023-05-15 19:05:46.000000 my_python_serializer_release-0.2.1/serializers/xml.py
+-rw-rw-r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      654 2023-05-15 18:54:35.000000 my_python_serializer_release-0.2.1/serializers/xml_parser.py
+-rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)       38 2023-05-15 21:16:11.670002 my_python_serializer_release-0.2.1/setup.cfg
+-rw-r--r--   0 egorbagrovets  (1000) egorbagrovets  (1000)      223 2023-05-15 21:16:10.000000 my_python_serializer_release-0.2.1/setup.py
```

### Comparing `my_python_serializer_release-0.2.0/serializers/constants.py` & `my_python_serializer_release-0.2.1/serializers/constants.py`

 * *Files identical despite different names*

### Comparing `my_python_serializer_release-0.2.0/serializers/json.py` & `my_python_serializer_release-0.2.1/serializers/json.py`

 * *Files identical despite different names*

### Comparing `my_python_serializer_release-0.2.0/serializers/json_parser.py` & `my_python_serializer_release-0.2.1/serializers/json_parser.py`

 * *Files identical despite different names*

### Comparing `my_python_serializer_release-0.2.0/serializers/xml.py` & `my_python_serializer_release-0.2.1/serializers/xml.py`

 * *Files identical despite different names*

### Comparing `my_python_serializer_release-0.2.0/serializers/xml_parser.py` & `my_python_serializer_release-0.2.1/serializers/xml_parser.py`

 * *Files identical despite different names*

