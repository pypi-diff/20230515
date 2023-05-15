# Comparing `tmp/ia_wumpus-0.2.2.tar.gz` & `tmp/ia_wumpus-0.2.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia_wumpus-0.2.2.tar", max compression
+gzip compressed data, was "ia_wumpus-0.2.21.tar", max compression
```

## Comparing `ia_wumpus-0.2.2.tar` & `ia_wumpus-0.2.21.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.2.2/LICENSE
--rw-r--r--   0        0        0     3921 2023-05-14 23:24:24.214729 ia_wumpus-0.2.2/README.md
--rw-r--r--   0        0        0       68 2023-05-13 02:13:49.858124 ia_wumpus-0.2.2/ia_mundo_do_wumpus/__init__.py
--rw-r--r--   0        0        0     4961 2023-05-13 02:13:49.858124 ia_wumpus-0.2.2/ia_mundo_do_wumpus/ambiente.py
--rw-r--r--   0        0        0      485 2023-05-14 23:23:49.390627 ia_wumpus-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 ia_wumpus-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.2.21/LICENSE
+-rw-r--r--   0        0        0     3921 2023-05-14 23:26:43.291386 ia_wumpus-0.2.21/README.md
+-rw-r--r--   0        0        0       68 2023-05-13 02:13:49.858124 ia_wumpus-0.2.21/ia_wumpus/__init__.py
+-rw-r--r--   0        0        0     4961 2023-05-13 02:13:49.858124 ia_wumpus-0.2.21/ia_wumpus/ambiente.py
+-rw-r--r--   0        0        0      477 2023-05-15 05:22:42.310310 ia_wumpus-0.2.21/pyproject.toml
+-rw-r--r--   0        0        0     4498 1970-01-01 00:00:00.000000 ia_wumpus-0.2.21/PKG-INFO
```

### Comparing `ia_wumpus-0.2.2/LICENSE` & `ia_wumpus-0.2.21/LICENSE`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.2.2/README.md` & `ia_wumpus-0.2.21/README.md`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.2.2/ia_mundo_do_wumpus/ambiente.py` & `ia_wumpus-0.2.21/ia_wumpus/ambiente.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.2.2/PKG-INFO` & `ia_wumpus-0.2.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ia-wumpus
-Version: 0.2.2
+Version: 0.2.21
 Summary: Projeto O Mundo do Wumpus - Anbiente para estudo da disciplina de Inteligencia Computacional.
 Author: Oseiasdfarias
 Author-email: oseias.dfarias@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

