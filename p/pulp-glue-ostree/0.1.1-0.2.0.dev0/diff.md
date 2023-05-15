# Comparing `tmp/pulp-glue-ostree-0.1.1.tar.gz` & `tmp/pulp-glue-ostree-0.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-glue-ostree-0.1.1.tar", last modified: Mon May 15 14:39:25 2023, max compression
+gzip compressed data, was "pulp-glue-ostree-0.2.0.dev0.tar", last modified: Mon Apr  3 11:54:53 2023, max compression
```

## Comparing `pulp-glue-ostree-0.1.1.tar` & `pulp-glue-ostree-0.2.0.dev0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:39:25.883053 pulp-glue-ostree-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-15 14:39:25.883053 pulp-glue-ostree-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-15 14:39:10.000000 pulp-glue-ostree-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:39:25.879053 pulp-glue-ostree-0.1.1/pulp_glue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:39:25.883053 pulp-glue-ostree-0.1.1/pulp_glue/ostree/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 14:39:10.000000 pulp-glue-ostree-0.1.1/pulp_glue/ostree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-15 14:39:10.000000 pulp-glue-ostree-0.1.1/pulp_glue/ostree/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:39:10.000000 pulp-glue-ostree-0.1.1/pulp_glue/ostree/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:39:25.883053 pulp-glue-ostree-0.1.1/pulp_glue_ostree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-15 14:39:25.000000 pulp-glue-ostree-0.1.1/pulp_glue_ostree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-15 14:39:25.000000 pulp-glue-ostree-0.1.1/pulp_glue_ostree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:39:25.000000 pulp-glue-ostree-0.1.1/pulp_glue_ostree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 14:39:25.000000 pulp-glue-ostree-0.1.1/pulp_glue_ostree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 14:39:25.000000 pulp-glue-ostree-0.1.1/pulp_glue_ostree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 14:39:10.000000 pulp-glue-ostree-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 14:39:25.883053 pulp-glue-ostree-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-15 14:39:10.000000 pulp-glue-ostree-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:53.808955 pulp-glue-ostree-0.2.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-03 11:54:53.808955 pulp-glue-ostree-0.2.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-03 11:54:44.000000 pulp-glue-ostree-0.2.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:53.804955 pulp-glue-ostree-0.2.0.dev0/pulp_glue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:53.804955 pulp-glue-ostree-0.2.0.dev0/pulp_glue/ostree/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-03 11:54:44.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue/ostree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-03 11:54:44.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue/ostree/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:44.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue/ostree/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:53.804955 pulp-glue-ostree-0.2.0.dev0/pulp_glue_ostree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-03 11:54:53.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue_ostree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-03 11:54:53.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue_ostree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 11:54:53.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue_ostree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-03 11:54:53.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue_ostree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-03 11:54:53.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue_ostree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-03 11:54:44.000000 pulp-glue-ostree-0.2.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 11:54:53.808955 pulp-glue-ostree-0.2.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-03 11:54:44.000000 pulp-glue-ostree-0.2.0.dev0/setup.py
```

### Comparing `pulp-glue-ostree-0.1.1/PKG-INFO` & `pulp-glue-ostree-0.2.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue-ostree
-Version: 0.1.1
+Version: 0.2.0.dev0
 Summary: Version agnostic glue library to talk to pulpcore's REST API.
 Home-page: https://github.com/pulp/pulp-cli-ostree
 Author: Pulp Team
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
```

### Comparing `pulp-glue-ostree-0.1.1/pulp_glue/ostree/context.py` & `pulp-glue-ostree-0.2.0.dev0/pulp_glue/ostree/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-ostree-0.1.1/pulp_glue_ostree.egg-info/PKG-INFO` & `pulp-glue-ostree-0.2.0.dev0/pulp_glue_ostree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue-ostree
-Version: 0.1.1
+Version: 0.2.0.dev0
 Summary: Version agnostic glue library to talk to pulpcore's REST API.
 Home-page: https://github.com/pulp/pulp-cli-ostree
 Author: Pulp Team
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
```

### Comparing `pulp-glue-ostree-0.1.1/setup.py` & `pulp-glue-ostree-0.2.0.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 setup(
     name="pulp-glue-ostree",
     description="Version agnostic glue library to talk to pulpcore's REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Pulp Team",
     url="https://github.com/pulp/pulp-cli-ostree",
-    version="0.1.1",
+    version="0.2.0.dev",
     packages=plugin_packages,
     package_data={"": ["py.typed"]},
     python_requires=">=3.6",
     install_requires=["pulp-glue>=0.18.0,<0.19"],
     license="GPLv2+",
     classifiers=[
         "Development Status :: 4 - Beta",
```

