# Comparing `tmp/latestinfoearthquakeindonesia-0.0.1.tar.gz` & `tmp/latestinfoearthquakeindonesia-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latestinfoearthquakeindonesia-0.0.1.tar", last modified: Sat May 13 09:51:11 2023, max compression
+gzip compressed data, was "latestinfoearthquakeindonesia-0.0.3.tar", last modified: Mon May 15 11:48:17 2023, max compression
```

## Comparing `latestinfoearthquakeindonesia-0.0.1.tar` & `latestinfoearthquakeindonesia-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 09:51:11.551895 latestinfoearthquakeindonesia-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-05-10 11:57:41.000000 latestinfoearthquakeindonesia-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1052 2023-05-13 09:51:11.544883 latestinfoearthquakeindonesia-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-05-10 12:36:49.000000 latestinfoearthquakeindonesia-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 09:51:11.490803 latestinfoearthquakeindonesia-0.0.1/gempaterkini/
--rw-rw-rw-   0        0        0     2521 2023-05-12 12:16:43.000000 latestinfoearthquakeindonesia-0.0.1/gempaterkini/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 09:51:11.539880 latestinfoearthquakeindonesia-0.0.1/latestinfoearthquakeindonesia.egg-info/
--rw-rw-rw-   0        0        0     1052 2023-05-13 09:51:11.000000 latestinfoearthquakeindonesia-0.0.1/latestinfoearthquakeindonesia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-05-13 09:51:11.000000 latestinfoearthquakeindonesia-0.0.1/latestinfoearthquakeindonesia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 09:51:11.000000 latestinfoearthquakeindonesia-0.0.1/latestinfoearthquakeindonesia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-13 09:51:11.000000 latestinfoearthquakeindonesia-0.0.1/latestinfoearthquakeindonesia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 09:51:11.554910 latestinfoearthquakeindonesia-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      902 2023-05-13 09:07:55.000000 latestinfoearthquakeindonesia-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:48:17.176009 latestinfoearthquakeindonesia-0.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-05-10 11:57:41.000000 latestinfoearthquakeindonesia-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1052 2023-05-15 11:48:17.173005 latestinfoearthquakeindonesia-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-05-10 12:36:49.000000 latestinfoearthquakeindonesia-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 11:48:17.101898 latestinfoearthquakeindonesia-0.0.3/gempaterkini/
+-rw-rw-rw-   0        0        0     2521 2023-05-12 12:16:43.000000 latestinfoearthquakeindonesia-0.0.3/gempaterkini/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:48:17.147967 latestinfoearthquakeindonesia-0.0.3/latestinfoearthquakeindonesia.egg-info/
+-rw-rw-rw-   0        0        0     1052 2023-05-15 11:48:17.000000 latestinfoearthquakeindonesia-0.0.3/latestinfoearthquakeindonesia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-05-15 11:48:17.000000 latestinfoearthquakeindonesia-0.0.3/latestinfoearthquakeindonesia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 11:48:17.000000 latestinfoearthquakeindonesia-0.0.3/latestinfoearthquakeindonesia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-15 11:48:17.000000 latestinfoearthquakeindonesia-0.0.3/latestinfoearthquakeindonesia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 11:48:17.178011 latestinfoearthquakeindonesia-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      902 2023-05-15 11:46:26.000000 latestinfoearthquakeindonesia-0.0.3/setup.py
```

### Comparing `latestinfoearthquakeindonesia-0.0.1/LICENSE` & `latestinfoearthquakeindonesia-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `latestinfoearthquakeindonesia-0.0.1/PKG-INFO` & `latestinfoearthquakeindonesia-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latestinfoearthquakeindonesia
-Version: 0.0.1
+Version: 0.0.3
 Summary: This package will get the latest earthquake from BMKG | Meteorological, Climatological, and Geophysical Agency.
 Home-page: https://github.com/TOSS-ID/latest-indonesia-earthquake
 Author: Hendra Go
 Author-email: hendrago91@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `latestinfoearthquakeindonesia-0.0.1/gempaterkini/__init__.py` & `latestinfoearthquakeindonesia-0.0.3/gempaterkini/__init__.py`

 * *Files identical despite different names*

### Comparing `latestinfoearthquakeindonesia-0.0.1/latestinfoearthquakeindonesia.egg-info/PKG-INFO` & `latestinfoearthquakeindonesia-0.0.3/latestinfoearthquakeindonesia.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latestinfoearthquakeindonesia
-Version: 0.0.1
+Version: 0.0.3
 Summary: This package will get the latest earthquake from BMKG | Meteorological, Climatological, and Geophysical Agency.
 Home-page: https://github.com/TOSS-ID/latest-indonesia-earthquake
 Author: Hendra Go
 Author-email: hendrago91@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `latestinfoearthquakeindonesia-0.0.1/setup.py` & `latestinfoearthquakeindonesia-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="latestinfoearthquakeindonesia",
-    version="0.0.1",
+    version="0.0.3",
     author="Hendra Go",
     author_email="hendrago91@gmail.com",
     description="This package will get the latest earthquake from BMKG | Meteorological, Climatological, and "
                 "Geophysical Agency.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TOSS-ID/latest-indonesia-earthquake",
```

