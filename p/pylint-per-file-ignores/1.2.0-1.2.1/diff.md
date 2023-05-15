# Comparing `tmp/pylint_per_file_ignores-1.2.0.tar.gz` & `tmp/pylint_per_file_ignores-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint_per_file_ignores-1.2.0.tar", max compression
+gzip compressed data, was "pylint_per_file_ignores-1.2.1.tar", max compression
```

## Comparing `pylint_per_file_ignores-1.2.0.tar` & `pylint_per_file_ignores-1.2.1.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     7718 2023-02-13 14:10:18.337986 pylint_per_file_ignores-1.2.0/pylint_per_file_ignores/__init__.py
--rw-r--r--   0        0        0      811 2023-02-13 14:11:22.570654 pylint_per_file_ignores-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      788 2023-02-13 14:10:18.337986 pylint_per_file_ignores-1.2.0/readme.md
--rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 pylint_per_file_ignores-1.2.0/setup.py
--rw-r--r--   0        0        0     1551 1970-01-01 00:00:00.000000 pylint_per_file_ignores-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     8823 2023-05-15 17:46:33.388506 pylint_per_file_ignores-1.2.1/pylint_per_file_ignores/__init__.py
+-rw-r--r--   0        0        0      811 2023-05-15 17:47:11.778774 pylint_per_file_ignores-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      788 2023-05-15 17:46:33.388506 pylint_per_file_ignores-1.2.1/readme.md
+-rw-r--r--   0        0        0     1551 1970-01-01 00:00:00.000000 pylint_per_file_ignores-1.2.1/PKG-INFO
```

### Comparing `pylint_per_file_ignores-1.2.0/pylint_per_file_ignores/__init__.py` & `pylint_per_file_ignores-1.2.1/pylint_per_file_ignores/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,14 +136,35 @@
         self.old_method = old_method
         self.node = node
 
     def __call__(self):
         self.old_method(self.node)
 
 
+def get_message_definitions(linter, message_id_or_symbol):
+    """
+    Lookup that onverts a symbol or message string into a unified message.
+    """
+    msgs_store = getattr(linter, "msgs_store", linter)
+
+    if hasattr(msgs_store, "check_message_id"):
+        return [msgs_store.check_message_id(message_id_or_symbol)]
+    # pylint 2.0 renamed check_message_id to get_message_definition in:
+    # https://github.com/PyCQA/pylint/commit/5ccbf9eaa54c0c302c9180bdfb745566c16e416d
+    if hasattr(msgs_store, "get_message_definition"):
+        return [msgs_store.get_message_definition(message_id_or_symbol)]
+    # pylint 2.3.0 renamed get_message_definition to get_message_definitions in:
+    # https://github.com/PyCQA/pylint/commit/da67a9da682e51844fbc674229ff6619eb9c816a
+    if hasattr(msgs_store, "get_message_definitions"):
+        return msgs_store.get_message_definitions(message_id_or_symbol)
+
+    msg = "pylint.utils.MessagesStore does not have a get_message_definition(s) method"
+    raise ValueError(msg)
+
+
 def augment_all_visit(linter, message_id_or_symbol, augmentation):
     """
     Augmenting a visit enables additional errors to be raised (although that case is
     better served using a new checker) or to suppress all warnings in certain
     circumstances.
     Augmenting functions should accept a 'chain' function, which runs the checker
     method and possibly any other augmentations, and secondly an Astroid node.
@@ -168,15 +189,17 @@
     checker = get_checker_by_msg(linter, message_id_or_symbol)
     if not hasattr(checker, "add_message"):
         return False
 
     add_message_method = getattr(checker, "add_message")
 
     def add_message(*args, **kwargs):
-        if test_func(None) and args[0] == message_id_or_symbol:
+        if test_func(None) and get_message_definitions(
+            linter, args[0]
+        ) == get_message_definitions(linter, message_id_or_symbol):
             return
         add_message_method(*args, **kwargs)
 
     setattr(checker, "add_message", add_message)
 
     return True
```

### Comparing `pylint_per_file_ignores-1.2.0/pyproject.toml` & `pylint_per_file_ignores-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [tool.poetry]
 authors = ["Christopher Pickering <christopher@going.bg>"]
 description = "A pylint plugin to ignore error codes per file."
 license = "MIT"
 name = "pylint-per-file-ignores"
 readme = "readme.md"
 repository = "https://github.com/christopherpickering/pylint-per-file-ignores.git"
-version = "1.2.0"
+version = "1.2.1"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 tomli = {version = "^2.0.1", python = "<3.11"}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.0.0"
```

### Comparing `pylint_per_file_ignores-1.2.0/readme.md` & `pylint_per_file_ignores-1.2.1/readme.md`

 * *Files identical despite different names*

### Comparing `pylint_per_file_ignores-1.2.0/PKG-INFO` & `pylint_per_file_ignores-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-per-file-ignores
-Version: 1.2.0
+Version: 1.2.1
 Summary: A pylint plugin to ignore error codes per file.
 Home-page: https://github.com/christopherpickering/pylint-per-file-ignores.git
 License: MIT
 Author: Christopher Pickering
 Author-email: christopher@going.bg
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

