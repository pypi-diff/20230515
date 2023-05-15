# Comparing `tmp/kubegpt-0.0.5.tar.gz` & `tmp/kubegpt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubegpt-0.0.5.tar", last modified: Mon May 15 18:52:34 2023, max compression
+gzip compressed data, was "kubegpt-0.0.6.tar", last modified: Mon May 15 18:55:50 2023, max compression
```

## Comparing `kubegpt-0.0.5.tar` & `kubegpt-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 noqcks     (501) staff       (20)        0 2023-05-15 18:52:34.385184 kubegpt-0.0.5/
--rw-r--r--   0 noqcks     (501) staff       (20)     1067 2023-05-15 18:18:26.000000 kubegpt-0.0.5/LICENSE
--rw-r--r--   0 noqcks     (501) staff       (20)     1701 2023-05-15 18:52:34.385020 kubegpt-0.0.5/PKG-INFO
--rw-r--r--   0 noqcks     (501) staff       (20)     1398 2023-05-15 18:42:53.000000 kubegpt-0.0.5/README.md
-drwxr-xr-x   0 noqcks     (501) staff       (20)        0 2023-05-15 18:52:34.383791 kubegpt-0.0.5/kubegpt/
--rw-r--r--   0 noqcks     (501) staff       (20)        0 2023-05-15 18:28:55.000000 kubegpt-0.0.5/kubegpt/__init__.py
--rw-r--r--   0 noqcks     (501) staff       (20)      691 2023-05-15 18:52:17.000000 kubegpt-0.0.5/kubegpt/__main__.py
--rw-r--r--   0 noqcks     (501) staff       (20)     1742 2023-05-15 18:52:12.000000 kubegpt-0.0.5/kubegpt/prompt.py
-drwxr-xr-x   0 noqcks     (501) staff       (20)        0 2023-05-15 18:52:34.384717 kubegpt-0.0.5/kubegpt.egg-info/
--rw-r--r--   0 noqcks     (501) staff       (20)     1701 2023-05-15 18:52:34.000000 kubegpt-0.0.5/kubegpt.egg-info/PKG-INFO
--rw-r--r--   0 noqcks     (501) staff       (20)      287 2023-05-15 18:52:34.000000 kubegpt-0.0.5/kubegpt.egg-info/SOURCES.txt
--rw-r--r--   0 noqcks     (501) staff       (20)        1 2023-05-15 18:52:34.000000 kubegpt-0.0.5/kubegpt.egg-info/dependency_links.txt
--rw-r--r--   0 noqcks     (501) staff       (20)       50 2023-05-15 18:52:34.000000 kubegpt-0.0.5/kubegpt.egg-info/entry_points.txt
--rw-r--r--   0 noqcks     (501) staff       (20)       17 2023-05-15 18:52:34.000000 kubegpt-0.0.5/kubegpt.egg-info/requires.txt
--rw-r--r--   0 noqcks     (501) staff       (20)        8 2023-05-15 18:52:34.000000 kubegpt-0.0.5/kubegpt.egg-info/top_level.txt
--rw-r--r--   0 noqcks     (501) staff       (20)       90 2023-05-15 18:18:29.000000 kubegpt-0.0.5/pyproject.toml
--rw-r--r--   0 noqcks     (501) staff       (20)       38 2023-05-15 18:52:34.385229 kubegpt-0.0.5/setup.cfg
--rw-r--r--   0 noqcks     (501) staff       (20)      604 2023-05-15 18:52:28.000000 kubegpt-0.0.5/setup.py
+drwxr-xr-x   0 noqcks     (501) staff       (20)        0 2023-05-15 18:55:50.192922 kubegpt-0.0.6/
+-rw-r--r--   0 noqcks     (501) staff       (20)     1067 2023-05-15 18:18:26.000000 kubegpt-0.0.6/LICENSE
+-rw-r--r--   0 noqcks     (501) staff       (20)     1701 2023-05-15 18:55:50.192747 kubegpt-0.0.6/PKG-INFO
+-rw-r--r--   0 noqcks     (501) staff       (20)     1398 2023-05-15 18:42:53.000000 kubegpt-0.0.6/README.md
+drwxr-xr-x   0 noqcks     (501) staff       (20)        0 2023-05-15 18:55:50.191355 kubegpt-0.0.6/kubegpt/
+-rw-r--r--   0 noqcks     (501) staff       (20)        0 2023-05-15 18:28:55.000000 kubegpt-0.0.6/kubegpt/__init__.py
+-rw-r--r--   0 noqcks     (501) staff       (20)      883 2023-05-15 18:55:25.000000 kubegpt-0.0.6/kubegpt/__main__.py
+-rw-r--r--   0 noqcks     (501) staff       (20)     1742 2023-05-15 18:52:12.000000 kubegpt-0.0.6/kubegpt/prompt.py
+drwxr-xr-x   0 noqcks     (501) staff       (20)        0 2023-05-15 18:55:50.192528 kubegpt-0.0.6/kubegpt.egg-info/
+-rw-r--r--   0 noqcks     (501) staff       (20)     1701 2023-05-15 18:55:50.000000 kubegpt-0.0.6/kubegpt.egg-info/PKG-INFO
+-rw-r--r--   0 noqcks     (501) staff       (20)      287 2023-05-15 18:55:50.000000 kubegpt-0.0.6/kubegpt.egg-info/SOURCES.txt
+-rw-r--r--   0 noqcks     (501) staff       (20)        1 2023-05-15 18:55:50.000000 kubegpt-0.0.6/kubegpt.egg-info/dependency_links.txt
+-rw-r--r--   0 noqcks     (501) staff       (20)       50 2023-05-15 18:55:50.000000 kubegpt-0.0.6/kubegpt.egg-info/entry_points.txt
+-rw-r--r--   0 noqcks     (501) staff       (20)       17 2023-05-15 18:55:50.000000 kubegpt-0.0.6/kubegpt.egg-info/requires.txt
+-rw-r--r--   0 noqcks     (501) staff       (20)        8 2023-05-15 18:55:50.000000 kubegpt-0.0.6/kubegpt.egg-info/top_level.txt
+-rw-r--r--   0 noqcks     (501) staff       (20)       90 2023-05-15 18:18:29.000000 kubegpt-0.0.6/pyproject.toml
+-rw-r--r--   0 noqcks     (501) staff       (20)       38 2023-05-15 18:55:50.192970 kubegpt-0.0.6/setup.cfg
+-rw-r--r--   0 noqcks     (501) staff       (20)      604 2023-05-15 18:55:30.000000 kubegpt-0.0.6/setup.py
```

### Comparing `kubegpt-0.0.5/LICENSE` & `kubegpt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kubegpt-0.0.5/PKG-INFO` & `kubegpt-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubegpt
-Version: 0.0.5
+Version: 0.0.6
 Summary: Using human language to interact with Kubernetes
 Home-page: https://github.com/xeol-io/kubegpt
 Author: Benji Visser
 Author-email: benji@xeol.io
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `kubegpt-0.0.5/README.md` & `kubegpt-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `kubegpt-0.0.5/kubegpt/__main__.py` & `kubegpt-0.0.6/kubegpt/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import argparse
 import warnings
 
 
 def setup_cli():
     parser = argparse.ArgumentParser(description="kubegpt")
     parser.add_argument("prompt", help="The question to ask your Kubernetes cluster")
+    parser.add_argument("--version", action="version", version="0.0.6", help="Print the version and exit")
     return parser.parse_args()
 
 
 def main():
     # supress the warning "The shell tool has no safeguards by default"
     warnings.filterwarnings("ignore")
     args = setup_cli()
@@ -20,9 +21,12 @@
     if "OPENAI_API_KEY" not in os.environ:
         raise ValueError(
             "Please set your OpenAI API key in the environment variable OPENAI_API_KEY"
         )
 
     openai.api_key = os.getenv("OPENAI_API_KEY")
 
+    if not args.prompt.strip():
+        raise ValueError("Prompt cannot be empty.")
+
     prompt(args.prompt)
```

### Comparing `kubegpt-0.0.5/kubegpt/prompt.py` & `kubegpt-0.0.6/kubegpt/prompt.py`

 * *Files identical despite different names*

### Comparing `kubegpt-0.0.5/kubegpt.egg-info/PKG-INFO` & `kubegpt-0.0.6/kubegpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubegpt
-Version: 0.0.5
+Version: 0.0.6
 Summary: Using human language to interact with Kubernetes
 Home-page: https://github.com/xeol-io/kubegpt
 Author: Benji Visser
 Author-email: benji@xeol.io
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `kubegpt-0.0.5/setup.py` & `kubegpt-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kubegpt",
     author="Benji Visser",
     author_email="benji@xeol.io",
-    version="0.0.5",
+    version="0.0.6",
     description="Using human language to interact with Kubernetes",
     license="MIT",
     packages=find_packages(),
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": ["kubegpt = kubegpt.__main__:main"],
```

