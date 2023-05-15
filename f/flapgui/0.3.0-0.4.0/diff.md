# Comparing `tmp/flapgui-0.3.0.tar.gz` & `tmp/flapgui-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flapgui-0.3.0.tar", last modified: Sat May 13 17:29:25 2023, max compression
+gzip compressed data, was "flapgui-0.4.0.tar", last modified: Mon May 15 17:41:21 2023, max compression
```

## Comparing `flapgui-0.3.0.tar` & `flapgui-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-13 17:29:25.847316 flapgui-0.3.0/
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     1073 2023-05-12 20:35:47.000000 flapgui-0.3.0/LICENSE
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     6747 2023-05-13 17:29:25.846739 flapgui-0.3.0/PKG-INFO
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     6206 2023-05-13 17:28:24.000000 flapgui-0.3.0/README.md
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)      614 2023-05-13 17:25:37.000000 flapgui-0.3.0/pyproject.toml
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)       38 2023-05-13 17:29:25.847452 flapgui-0.3.0/setup.cfg
-drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-13 17:29:25.832838 flapgui-0.3.0/src/
-drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-13 17:29:25.838279 flapgui-0.3.0/src/flapgui/
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     8608 2023-05-13 17:22:41.000000 flapgui-0.3.0/src/flapgui/__init__.py
-drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-13 17:29:25.845368 flapgui-0.3.0/src/flapgui.egg-info/
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     6747 2023-05-13 17:29:25.000000 flapgui-0.3.0/src/flapgui.egg-info/PKG-INFO
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)      196 2023-05-13 17:29:25.000000 flapgui-0.3.0/src/flapgui.egg-info/SOURCES.txt
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        1 2023-05-13 17:29:25.000000 flapgui-0.3.0/src/flapgui.egg-info/dependency_links.txt
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        8 2023-05-13 17:29:25.000000 flapgui-0.3.0/src/flapgui.egg-info/top_level.txt
+drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-15 17:41:21.221648 flapgui-0.4.0/
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     1073 2023-05-12 20:35:47.000000 flapgui-0.4.0/LICENSE
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     1221 2023-05-15 17:41:21.221023 flapgui-0.4.0/PKG-INFO
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)      680 2023-05-15 17:41:00.000000 flapgui-0.4.0/README.md
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)      614 2023-05-15 15:53:57.000000 flapgui-0.4.0/pyproject.toml
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)       38 2023-05-15 17:41:21.221852 flapgui-0.4.0/setup.cfg
+drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-15 17:41:21.147452 flapgui-0.4.0/src/
+drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-15 17:41:21.150807 flapgui-0.4.0/src/flapgui/
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)    14404 2023-05-15 17:32:37.000000 flapgui-0.4.0/src/flapgui/__init__.py
+drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-15 17:41:21.217641 flapgui-0.4.0/src/flapgui.egg-info/
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     1221 2023-05-15 17:41:21.000000 flapgui-0.4.0/src/flapgui.egg-info/PKG-INFO
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)      196 2023-05-15 17:41:21.000000 flapgui-0.4.0/src/flapgui.egg-info/SOURCES.txt
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        1 2023-05-15 17:41:21.000000 flapgui-0.4.0/src/flapgui.egg-info/dependency_links.txt
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        8 2023-05-15 17:41:21.000000 flapgui-0.4.0/src/flapgui.egg-info/top_level.txt
```

### Comparing `flapgui-0.3.0/LICENSE` & `flapgui-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flapgui-0.3.0/pyproject.toml` & `flapgui-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flapgui"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="WinFan3672", email="winfan3672@gmail.com" },
 ]
 description = "Easy-to-use and cross-platform GUI library for making functional GUI apps"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

