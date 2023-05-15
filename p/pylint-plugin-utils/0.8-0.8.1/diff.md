# Comparing `tmp/pylint_plugin_utils-0.8.tar.gz` & `tmp/pylint_plugin_utils-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint_plugin_utils-0.8.tar", max compression
+gzip compressed data, was "pylint_plugin_utils-0.8.1.tar", max compression
```

## Comparing `pylint_plugin_utils-0.8.tar` & `pylint_plugin_utils-0.8.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    18042 2023-05-14 11:45:57.812039 pylint_plugin_utils-0.8/LICENSE
--rw-r--r--   0        0        0     1913 2023-05-14 13:10:26.516666 pylint_plugin_utils-0.8/README.md
--rw-r--r--   0        0        0     6179 2023-05-14 12:12:48.419636 pylint_plugin_utils-0.8/pylint_plugin_utils/__init__.py
--rw-r--r--   0        0        0      983 2023-05-14 13:10:03.852795 pylint_plugin_utils-0.8/pyproject.toml
--rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 pylint_plugin_utils-0.8/setup.py
--rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 pylint_plugin_utils-0.8/PKG-INFO
+-rw-r--r--   0        0        0    18042 2023-05-14 11:45:57.812039 pylint_plugin_utils-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1913 2023-05-14 13:10:26.516666 pylint_plugin_utils-0.8.1/README.md
+-rw-r--r--   0        0        0     6179 2023-05-14 12:12:48.419636 pylint_plugin_utils-0.8.1/pylint_plugin_utils/__init__.py
+-rw-r--r--   0        0        0     1535 2023-05-15 02:15:08.367268 pylint_plugin_utils-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3343 1970-01-01 00:00:00.000000 pylint_plugin_utils-0.8.1/PKG-INFO
```

### Comparing `pylint_plugin_utils-0.8/LICENSE` & `pylint_plugin_utils-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylint_plugin_utils-0.8/README.md` & `pylint_plugin_utils-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pylint_plugin_utils-0.8/pylint_plugin_utils/__init__.py` & `pylint_plugin_utils-0.8.1/pylint_plugin_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint_plugin_utils-0.8/PKG-INFO` & `pylint_plugin_utils-0.8.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 Metadata-Version: 2.1
 Name: pylint-plugin-utils
-Version: 0.8
+Version: 0.8.1
 Summary: Utilities and helpers for writing Pylint plugins
 Home-page: https://github.com/PyCQA/pylint-plugin-utils
-License: GPLv2
+License: GPL-2.0-or-later
 Keywords: pylint,plugin,helpers
 Author: Carl Crowder
 Author-email: git@carlcrowder.com
 Requires-Python: >=3.7,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: pylint (>=1.7)
 Project-URL: Repository, https://github.com/PyCQA/pylint-plugin-utils
 Description-Content-Type: text/markdown
 
 # pylint-plugin-utils
 
 ## Status
```

