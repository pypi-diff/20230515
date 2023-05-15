# Comparing `tmp/sleepytime-0.0.6.tar.gz` & `tmp/sleepytime-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepytime-0.0.6.tar", last modified: Mon May 15 04:49:42 2023, max compression
+gzip compressed data, was "sleepytime-0.0.7.tar", last modified: Mon May 15 04:52:43 2023, max compression
```

## Comparing `sleepytime-0.0.6.tar` & `sleepytime-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 04:49:42.966699 sleepytime-0.0.6/
--rw-rw-rw-   0        0        0     1094 2023-05-15 04:49:13.000000 sleepytime-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1166 2023-05-15 04:49:42.966699 sleepytime-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      661 2023-05-15 04:49:13.000000 sleepytime-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 04:49:42.966699 sleepytime-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1028 2023-05-15 04:49:13.000000 sleepytime-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 04:49:42.966699 sleepytime-0.0.6/sleepytime/
--rw-rw-rw-   0        0        0        0 2023-05-15 04:49:13.000000 sleepytime-0.0.6/sleepytime/__init__.py
--rw-rw-rw-   0        0        0      484 2023-05-15 04:49:13.000000 sleepytime-0.0.6/sleepytime/__main__.py
--rw-rw-rw-   0        0        0       23 2023-05-15 04:49:13.000000 sleepytime-0.0.6/sleepytime/__version__.py
--rw-rw-rw-   0        0        0     3510 2023-05-15 04:49:13.000000 sleepytime-0.0.6/sleepytime/gui.py
--rw-rw-rw-   0        0        0     2628 2023-05-15 04:49:13.000000 sleepytime-0.0.6/sleepytime/resume_watcher.py
-drwxrwxrwx   0        0        0        0 2023-05-15 04:49:42.966699 sleepytime-0.0.6/sleepytime.egg-info/
--rw-rw-rw-   0        0        0     1166 2023-05-15 04:49:42.000000 sleepytime-0.0.6/sleepytime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-05-15 04:49:42.000000 sleepytime-0.0.6/sleepytime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 04:49:42.000000 sleepytime-0.0.6/sleepytime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-15 04:49:42.000000 sleepytime-0.0.6/sleepytime.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-15 04:49:42.000000 sleepytime-0.0.6/sleepytime.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 04:52:43.598064 sleepytime-0.0.7/
+-rw-rw-rw-   0        0        0     1094 2023-05-15 04:52:20.000000 sleepytime-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1166 2023-05-15 04:52:43.598064 sleepytime-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-05-15 04:52:20.000000 sleepytime-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-15 04:52:43.598064 sleepytime-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1039 2023-05-15 04:52:20.000000 sleepytime-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 04:52:43.598064 sleepytime-0.0.7/sleepytime/
+-rw-rw-rw-   0        0        0        0 2023-05-15 04:52:20.000000 sleepytime-0.0.7/sleepytime/__init__.py
+-rw-rw-rw-   0        0        0      484 2023-05-15 04:52:20.000000 sleepytime-0.0.7/sleepytime/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-05-15 04:52:20.000000 sleepytime-0.0.7/sleepytime/__version__.py
+-rw-rw-rw-   0        0        0     3510 2023-05-15 04:52:20.000000 sleepytime-0.0.7/sleepytime/gui.py
+-rw-rw-rw-   0        0        0     2628 2023-05-15 04:52:20.000000 sleepytime-0.0.7/sleepytime/resume_watcher.py
+drwxrwxrwx   0        0        0        0 2023-05-15 04:52:43.598064 sleepytime-0.0.7/sleepytime.egg-info/
+-rw-rw-rw-   0        0        0     1166 2023-05-15 04:52:43.000000 sleepytime-0.0.7/sleepytime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-05-15 04:52:43.000000 sleepytime-0.0.7/sleepytime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 04:52:43.000000 sleepytime-0.0.7/sleepytime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-05-15 04:52:43.000000 sleepytime-0.0.7/sleepytime.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-15 04:52:43.000000 sleepytime-0.0.7/sleepytime.egg-info/top_level.txt
```

### Comparing `sleepytime-0.0.6/LICENSE` & `sleepytime-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepytime-0.0.6/PKG-INFO` & `sleepytime-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepytime
-Version: 0.0.6
+Version: 0.0.7
 Home-page: http://github.com/csm10495/sleepytime
 Author: csm10495
 Author-email: csm10495@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `sleepytime-0.0.6/README.md` & `sleepytime-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sleepytime-0.0.6/setup.py` & `sleepytime-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,10 +24,10 @@
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
     include_package_data=True,
-    install_requires=["PySimpleGUI", "psgtray", "tendo"],
+    install_requires=["PySimpleGUI", "psgtray", "pywin32", "tendo"],
     entry_points={},
 )
```

### Comparing `sleepytime-0.0.6/sleepytime/gui.py` & `sleepytime-0.0.7/sleepytime/gui.py`

 * *Files identical despite different names*

### Comparing `sleepytime-0.0.6/sleepytime/resume_watcher.py` & `sleepytime-0.0.7/sleepytime/resume_watcher.py`

 * *Files identical despite different names*

### Comparing `sleepytime-0.0.6/sleepytime.egg-info/PKG-INFO` & `sleepytime-0.0.7/sleepytime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepytime
-Version: 0.0.6
+Version: 0.0.7
 Home-page: http://github.com/csm10495/sleepytime
 Author: csm10495
 Author-email: csm10495@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
```

