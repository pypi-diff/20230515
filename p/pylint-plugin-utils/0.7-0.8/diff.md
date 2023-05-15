# Comparing `tmp/pylint-plugin-utils-0.7.tar.gz` & `tmp/pylint_plugin_utils-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint-plugin-utils-0.7.tar", last modified: Tue Dec 28 15:08:10 2021, max compression
+gzip compressed data, was "pylint_plugin_utils-0.8.tar", max compression
```

## Comparing `pylint-plugin-utils-0.7.tar` & `pylint_plugin_utils-0.8.tar`

### file list

```diff
@@ -1,15 +1,6 @@
-drwxrwxr-x   0 carl      (1000) carl      (1000)        0 2021-12-28 15:08:10.983898 pylint-plugin-utils-0.7/
--rw-rw-r--   0 carl      (1000) carl      (1000)    18042 2021-12-28 08:46:56.000000 pylint-plugin-utils-0.7/LICENSE
--rw-rw-r--   0 carl      (1000) carl      (1000)       16 2021-12-28 08:46:56.000000 pylint-plugin-utils-0.7/MANIFEST.in
--rw-rw-r--   0 carl      (1000) carl      (1000)     1006 2021-12-28 15:08:10.983898 pylint-plugin-utils-0.7/PKG-INFO
--rw-rw-r--   0 carl      (1000) carl      (1000)     1914 2021-12-28 14:25:55.000000 pylint-plugin-utils-0.7/README.md
-drwxrwxr-x   0 carl      (1000) carl      (1000)        0 2021-12-28 15:08:10.983898 pylint-plugin-utils-0.7/pylint_plugin_utils/
--rw-rw-r--   0 carl      (1000) carl      (1000)     6263 2021-12-28 08:48:02.000000 pylint-plugin-utils-0.7/pylint_plugin_utils/__init__.py
-drwxrwxr-x   0 carl      (1000) carl      (1000)        0 2021-12-28 15:08:10.983898 pylint-plugin-utils-0.7/pylint_plugin_utils.egg-info/
--rw-rw-r--   0 carl      (1000) carl      (1000)     1006 2021-12-28 15:08:10.000000 pylint-plugin-utils-0.7/pylint_plugin_utils.egg-info/PKG-INFO
--rw-rw-r--   0 carl      (1000) carl      (1000)      294 2021-12-28 15:08:10.000000 pylint-plugin-utils-0.7/pylint_plugin_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 carl      (1000) carl      (1000)        1 2021-12-28 15:08:10.000000 pylint-plugin-utils-0.7/pylint_plugin_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 carl      (1000) carl      (1000)       12 2021-12-28 15:08:10.000000 pylint-plugin-utils-0.7/pylint_plugin_utils.egg-info/requires.txt
--rw-rw-r--   0 carl      (1000) carl      (1000)       20 2021-12-28 15:08:10.000000 pylint-plugin-utils-0.7/pylint_plugin_utils.egg-info/top_level.txt
--rw-rw-r--   0 carl      (1000) carl      (1000)      147 2021-12-28 15:08:10.983898 pylint-plugin-utils-0.7/setup.cfg
--rw-rw-r--   0 carl      (1000) carl      (1000)     1253 2021-12-28 08:50:06.000000 pylint-plugin-utils-0.7/setup.py
+-rw-r--r--   0        0        0    18042 2023-05-14 11:45:57.812039 pylint_plugin_utils-0.8/LICENSE
+-rw-r--r--   0        0        0     1913 2023-05-14 13:10:26.516666 pylint_plugin_utils-0.8/README.md
+-rw-r--r--   0        0        0     6179 2023-05-14 12:12:48.419636 pylint_plugin_utils-0.8/pylint_plugin_utils/__init__.py
+-rw-r--r--   0        0        0      983 2023-05-14 13:10:03.852795 pylint_plugin_utils-0.8/pyproject.toml
+-rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 pylint_plugin_utils-0.8/setup.py
+-rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 pylint_plugin_utils-0.8/PKG-INFO
```

### Comparing `pylint-plugin-utils-0.7/LICENSE` & `pylint_plugin_utils-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pylint-plugin-utils-0.7/README.md` & `pylint_plugin_utils-0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # About
 
 Utilities and helpers for writing Pylint plugins. This is not a direct Pylint plugin, but rather a set of tools and functions used by other plugins such as [pylint-django](https://github.com/PyCQA/pylint-django) and [pylint-celery](https://github.com/PyCQA/pylint-celery).
 
 # Testing
 Create virtualenv:
 ```bash
-python3.8  -m venv .pylint-plugin-utils
+python3.8 -m venv .pylint-plugin-utils
 source .pylint-plugin-utils/bin/activate
 pip install --upgrade pip setuptools
 ```
 
 We use [tox](https://tox.readthedocs.io/en/latest/) for running the test suite. You should be able to install it with:
 ```bash
 pip install tox pytest
```

### Comparing `pylint-plugin-utils-0.7/pylint_plugin_utils/__init__.py` & `pylint_plugin_utils-0.8/pylint_plugin_utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,15 @@
     "chain()" can be called at any point to trigger the continuation of other
     checks, or not at all to prevent any further checking.
     """
 
     try:
         checker = get_checker(linter, checker_method.__self__.__class__)
     except AttributeError:
-        checker = get_checker(
-            linter, get_class(checker_method.__module__, checker_method.__qualname__)
-        )
+        checker = get_checker(linter, get_class(checker_method.__module__, checker_method.__qualname__))
 
     old_method = getattr(checker, checker_method.__name__)
     setattr(checker, checker_method.__name__, AugmentFunc(old_method, augmentation))
 
 
 class AugmentFunc:
     def __init__(self, old_method, augmentation_func):
@@ -97,17 +95,15 @@
 
 def suppress_message(linter: PyLinter, checker_method, message_id_or_symbol, test_func):
     """
     This wrapper allows the suppression of a message if the supplied test function
     returns True. It is useful to prevent one particular message from being raised
     in one particular case, while leaving the rest of the messages intact.
     """
-    augment_visit(
-        linter, checker_method, DoSuppress(linter, message_id_or_symbol, test_func)
-    )
+    augment_visit(linter, checker_method, DoSuppress(linter, message_id_or_symbol, test_func))
 
 
 class DoSuppress:
     def __init__(self, linter: PyLinter, message_id_or_symbol, test_func):
         self.linter = linter
         self.message_id_or_symbol = message_id_or_symbol
         self.test_func = test_func
@@ -157,12 +153,9 @@
         elif hasattr(msgs_store, "get_message_definition"):
             return [msgs_store.get_message_definition(message_id_or_symbol)]
         # pylint 2.3.0 renamed get_message_definition to get_message_definitions in:
         # https://github.com/PyCQA/pylint/commit/da67a9da682e51844fbc674229ff6619eb9c816a
         elif hasattr(msgs_store, "get_message_definitions"):
             return msgs_store.get_message_definitions(message_id_or_symbol)
         else:
-            msg = (
-                "pylint.utils.MessagesStore does not have a "
-                "get_message_definition(s) method"
-            )
+            msg = "pylint.utils.MessagesStore does not have a " "get_message_definition(s) method"
             raise ValueError(msg)
```

