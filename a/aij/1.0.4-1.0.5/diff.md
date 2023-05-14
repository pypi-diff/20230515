# Comparing `tmp/aij-1.0.4.tar.gz` & `tmp/aij-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.0.4.tar", last modified: Wed May 10 22:21:55 2023, max compression
+gzip compressed data, was "aij-1.0.5.tar", last modified: Sun May 14 22:23:05 2023, max compression
```

## Comparing `aij-1.0.4.tar` & `aij-1.0.5.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/
--rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     4137 2023-05-10 22:21:56.000000 aij-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-05-05 12:30:36.000000 aij-1.0.4/README.md
--rw-rw-rw-   0        0        0     6343 2023-05-10 22:21:42.000000 aij-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 22:21:56.000000 aij-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/src/aij.egg-info/
--rw-rw-rw-   0        0        0     4137 2023-05-10 22:21:56.000000 aij-1.0.4/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-05-10 22:21:56.000000 aij-1.0.4/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 22:21:56.000000 aij-1.0.4/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-05-10 22:21:56.000000 aij-1.0.4/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      197 2023-05-10 22:21:56.000000 aij-1.0.4/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-05-10 22:21:56.000000 aij-1.0.4/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/src/custom/
--rw-rw-rw-   0        0        0      440 2023-05-10 19:37:52.000000 aij-1.0.4/src/custom/__init__.py
--rw-rw-rw-   0        0        0     4531 2023-05-10 18:27:28.000000 aij-1.0.4/src/custom/generator.py
-drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/src/intro/
--rw-rw-rw-   0        0        0      440 2023-05-07 13:08:58.000000 aij-1.0.4/src/intro/__init__.py
--rw-rw-rw-   0        0        0     4524 2023-05-07 13:07:50.000000 aij-1.0.4/src/intro/intro.py
-drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/src/news/
--rw-rw-rw-   0        0        0      567 2023-05-07 13:07:50.000000 aij-1.0.4/src/news/__init__.py
--rw-rw-rw-   0        0        0     4492 2023-05-07 13:16:16.000000 aij-1.0.4/src/news/core.py
--rw-rw-rw-   0        0        0     1407 2023-05-07 13:18:00.000000 aij-1.0.4/src/news/publisher.py
--rw-rw-rw-   0        0        0     1196 2023-05-05 12:37:32.000000 aij-1.0.4/src/news/subscriber.py
-drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/src/setup/
--rw-rw-rw-   0        0        0     1162 2023-05-07 21:18:54.000000 aij-1.0.4/src/setup/__init__.py
--rw-rw-rw-   0        0        0     3739 2023-05-07 21:18:28.000000 aij-1.0.4/src/setup/install.py
-drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/src/webcam/
--rw-rw-rw-   0        0        0    17500 2023-05-06 19:32:44.000000 aij-1.0.4/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 22:23:04.000000 aij-1.0.5/
+-rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-14 22:23:06.000000 aij-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-10 22:39:42.000000 aij-1.0.5/README.md
+-rw-rw-rw-   0        0        0     6333 2023-05-14 22:22:48.000000 aij-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 22:23:06.000000 aij-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 22:23:04.000000 aij-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-14 22:23:04.000000 aij-1.0.5/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-14 22:23:04.000000 aij-1.0.5/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-05-14 22:23:04.000000 aij-1.0.5/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 22:23:04.000000 aij-1.0.5/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-05-14 22:23:04.000000 aij-1.0.5/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:23:04.000000 aij-1.0.5/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-05-14 22:23:04.000000 aij-1.0.5/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 22:23:04.000000 aij-1.0.5/src/custom/
+-rw-rw-rw-   0        0        0      440 2023-05-10 19:37:52.000000 aij-1.0.5/src/custom/__init__.py
+-rw-rw-rw-   0        0        0     4531 2023-05-10 18:27:28.000000 aij-1.0.5/src/custom/generator.py
+drwxrwxrwx   0        0        0        0 2023-05-14 22:23:04.000000 aij-1.0.5/src/intro/
+-rw-rw-rw-   0        0        0      440 2023-05-07 13:08:58.000000 aij-1.0.5/src/intro/__init__.py
+-rw-rw-rw-   0        0        0     4524 2023-05-07 13:07:50.000000 aij-1.0.5/src/intro/intro.py
+drwxrwxrwx   0        0        0        0 2023-05-14 22:23:04.000000 aij-1.0.5/src/news/
+-rw-rw-rw-   0        0        0      567 2023-05-07 13:07:50.000000 aij-1.0.5/src/news/__init__.py
+-rw-rw-rw-   0        0        0     4492 2023-05-07 13:16:16.000000 aij-1.0.5/src/news/core.py
+-rw-rw-rw-   0        0        0     1407 2023-05-07 13:18:00.000000 aij-1.0.5/src/news/publisher.py
+-rw-rw-rw-   0        0        0     1196 2023-05-05 12:37:32.000000 aij-1.0.5/src/news/subscriber.py
+drwxrwxrwx   0        0        0        0 2023-05-14 22:23:04.000000 aij-1.0.5/src/setup/
+-rw-rw-rw-   0        0        0     1162 2023-05-07 21:18:54.000000 aij-1.0.5/src/setup/__init__.py
+-rw-rw-rw-   0        0        0     3739 2023-05-07 21:18:28.000000 aij-1.0.5/src/setup/install.py
+drwxrwxrwx   0        0        0        0 2023-05-14 22:23:04.000000 aij-1.0.5/src/speech/
+-rw-rw-rw-   0        0        0      152 2023-05-14 22:21:56.000000 aij-1.0.5/src/speech/__init__.py
+-rw-rw-rw-   0        0        0     1052 2023-05-14 22:20:36.000000 aij-1.0.5/src/speech/talk.py
+-rw-rw-rw-   0        0        0      873 2023-05-14 22:05:06.000000 aij-1.0.5/src/speech/whisperx.py
+-rw-rw-rw-   0        0        0      579 2023-05-14 21:57:48.000000 aij-1.0.5/src/speech/whisperxx.py
+drwxrwxrwx   0        0        0        0 2023-05-14 22:23:04.000000 aij-1.0.5/src/webcam/
+-rw-rw-rw-   0        0        0    17500 2023-05-06 19:32:44.000000 aij-1.0.5/src/webcam/__init__.py
```

### Comparing `aij-1.0.4/LICENSE.txt` & `aij-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.0.4/pyproject.toml` & `aij-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.4"
+version = "1.0.5"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -146,17 +146,17 @@
 "Say Thanks!" = "http://saythanks.io/to/aij"
 "Source" = "https://github.com/codesapienbe/aij"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
 aij = "webcam:main"
-aijnews = "news:main"
-aijintro = "intro:main"
-aijsetup = "setup:main"
+aijn = "news:main"
+aiji = "intro:main"
+aijt = "speech:main"
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 package-data = { "db" = ["*.dat"] }
```

### Comparing `aij-1.0.4/src/custom/generator.py` & `aij-1.0.5/src/custom/generator.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.4/src/intro/intro.py` & `aij-1.0.5/src/intro/intro.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.4/src/news/__init__.py` & `aij-1.0.5/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.4/src/news/core.py` & `aij-1.0.5/src/news/core.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.4/src/news/publisher.py` & `aij-1.0.5/src/news/publisher.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.4/src/news/subscriber.py` & `aij-1.0.5/src/news/subscriber.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.4/src/setup/__init__.py` & `aij-1.0.5/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.4/src/setup/install.py` & `aij-1.0.5/src/setup/install.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.4/src/webcam/__init__.py` & `aij-1.0.5/src/webcam/__init__.py`

 * *Files identical despite different names*

