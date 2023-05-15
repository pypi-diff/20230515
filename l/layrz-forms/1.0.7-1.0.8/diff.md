# Comparing `tmp/layrz-forms-1.0.7.tar.gz` & `tmp/layrz-forms-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layrz-forms-1.0.7.tar", last modified: Wed May 10 00:46:44 2023, max compression
+gzip compressed data, was "layrz-forms-1.0.8.tar", last modified: Mon May 15 05:43:12 2023, max compression
```

## Comparing `layrz-forms-1.0.7.tar` & `layrz-forms-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 00:46:44.331884 layrz-forms-1.0.7/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-10 00:46:44.330884 layrz-forms-1.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 00:46:44.325883 layrz-forms-1.0.7/layrz/
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 00:46:44.326883 layrz-forms-1.0.7/layrz/forms/
--rw-rw-rw-   0 root         (0) root         (0)     5934 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 00:46:44.329884 layrz-forms-1.0.7/layrz/forms/fields/
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/base.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/boolean.py
--rw-rw-rw-   0 root         (0) root         (0)     2558 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/char.py
--rw-rw-rw-   0 root         (0) root         (0)     1508 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/email.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/id.py
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2203 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/number.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 00:46:44.330884 layrz-forms-1.0.7/layrz_forms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-10 00:46:44.000000 layrz-forms-1.0.7/layrz_forms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-10 00:46:44.000000 layrz-forms-1.0.7/layrz_forms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 00:46:44.000000 layrz-forms-1.0.7/layrz_forms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-10 00:46:44.000000 layrz-forms-1.0.7/layrz_forms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 00:46:44.331884 layrz-forms-1.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:12.513249 layrz-forms-1.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-15 05:43:02.000000 layrz-forms-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-15 05:43:12.512249 layrz-forms-1.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-15 05:43:02.000000 layrz-forms-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:12.507248 layrz-forms-1.0.8/layrz/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-15 05:43:02.000000 layrz-forms-1.0.8/layrz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:12.507248 layrz-forms-1.0.8/layrz/forms/
+-rw-rw-rw-   0 root         (0) root         (0)     5934 2023-05-15 05:43:02.000000 layrz-forms-1.0.8/layrz/forms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:12.510249 layrz-forms-1.0.8/layrz/forms/fields/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-15 05:43:02.000000 layrz-forms-1.0.8/layrz/forms/fields/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2023-05-15 05:43:02.000000 layrz-forms-1.0.8/layrz/forms/fields/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-05-15 05:43:02.000000 layrz-forms-1.0.8/layrz/forms/fields/boolean.py
+-rw-rw-rw-   0 root         (0) root         (0)     2558 2023-05-15 05:43:02.000000 layrz-forms-1.0.8/layrz/forms/fields/char.py
+-rw-rw-rw-   0 root         (0) root         (0)     1508 2023-05-15 05:43:02.000000 layrz-forms-1.0.8/layrz/forms/fields/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-05-15 05:43:02.000000 layrz-forms-1.0.8/layrz/forms/fields/id.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-15 05:43:02.000000 layrz-forms-1.0.8/layrz/forms/fields/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2023-05-15 05:43:02.000000 layrz-forms-1.0.8/layrz/forms/fields/number.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:12.512249 layrz-forms-1.0.8/layrz_forms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-15 05:43:12.000000 layrz-forms-1.0.8/layrz_forms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      510 2023-05-15 05:43:12.000000 layrz-forms-1.0.8/layrz_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 05:43:12.000000 layrz-forms-1.0.8/layrz_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-15 05:43:12.000000 layrz-forms-1.0.8/layrz_forms.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 05:43:12.000000 layrz-forms-1.0.8/layrz_forms.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-15 05:43:12.000000 layrz-forms-1.0.8/layrz_forms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 05:43:12.513249 layrz-forms-1.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-05-15 05:43:02.000000 layrz-forms-1.0.8/setup.py
```

### Comparing `layrz-forms-1.0.7/LICENSE` & `layrz-forms-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.7/PKG-INFO` & `layrz-forms-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-forms
-Version: 1.0.7
+Version: 1.0.8
 Summary: Layrz forms and tools for Python
 Author: Golden M
 Author-email: software@goldenmcorp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `layrz-forms-1.0.7/README.md` & `layrz-forms-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.7/layrz/forms/__init__.py` & `layrz-forms-1.0.8/layrz/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.7/layrz/forms/fields/base.py` & `layrz-forms-1.0.8/layrz/forms/fields/base.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.7/layrz/forms/fields/boolean.py` & `layrz-forms-1.0.8/layrz/forms/fields/boolean.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.7/layrz/forms/fields/char.py` & `layrz-forms-1.0.8/layrz/forms/fields/char.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.7/layrz/forms/fields/email.py` & `layrz-forms-1.0.8/layrz/forms/fields/email.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.7/layrz/forms/fields/id.py` & `layrz-forms-1.0.8/layrz/forms/fields/id.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.7/layrz/forms/fields/json.py` & `layrz-forms-1.0.8/layrz/forms/fields/json.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.7/layrz/forms/fields/number.py` & `layrz-forms-1.0.8/layrz/forms/fields/number.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.7/layrz_forms.egg-info/PKG-INFO` & `layrz-forms-1.0.8/layrz_forms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-forms
-Version: 1.0.7
+Version: 1.0.8
 Summary: Layrz forms and tools for Python
 Author: Golden M
 Author-email: software@goldenmcorp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `layrz-forms-1.0.7/setup.py` & `layrz-forms-1.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,23 @@
   """ Return long description """
   with open('README.md', 'r', encoding='utf-8') as fh:
     return fh.read()
 
 
 setuptools.setup(
   name="layrz-forms",
-  version="1.0.7",
+  version="1.0.8",
   author="Golden M",
   author_email="software@goldenmcorp.com",
   description="Layrz forms and tools for Python",
   long_description=long_description(),
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
+  namespace_packages=['layrz'],
+  zip_safe=False,
   classifiers=[
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
   ],
```

