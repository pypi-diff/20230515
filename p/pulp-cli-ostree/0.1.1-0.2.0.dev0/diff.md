# Comparing `tmp/pulp-cli-ostree-0.1.1.tar.gz` & `tmp/pulp-cli-ostree-0.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-cli-ostree-0.1.1.tar", last modified: Mon May 15 14:39:31 2023, max compression
+gzip compressed data, was "pulp-cli-ostree-0.2.0.dev0.tar", last modified: Mon Apr  3 11:54:58 2023, max compression
```

## Comparing `pulp-cli-ostree-0.1.1.tar` & `pulp-cli-ostree-0.2.0.dev0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:39:31.039075 pulp-cli-ostree-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-15 14:39:31.035075 pulp-cli-ostree-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:39:31.035075 pulp-cli-ostree-0.1.1/pulp_cli_ostree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-15 14:39:30.000000 pulp-cli-ostree-0.1.1/pulp_cli_ostree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-15 14:39:31.000000 pulp-cli-ostree-0.1.1/pulp_cli_ostree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:39:30.000000 pulp-cli-ostree-0.1.1/pulp_cli_ostree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 14:39:30.000000 pulp-cli-ostree-0.1.1/pulp_cli_ostree.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 14:39:30.000000 pulp-cli-ostree-0.1.1/pulp_cli_ostree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 14:39:30.000000 pulp-cli-ostree-0.1.1/pulp_cli_ostree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:39:31.035075 pulp-cli-ostree-0.1.1/pulpcore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:39:31.035075 pulp-cli-ostree-0.1.1/pulpcore/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:39:31.035075 pulp-cli-ostree-0.1.1/pulpcore/cli/ostree/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-15 14:39:10.000000 pulp-cli-ostree-0.1.1/pulpcore/cli/ostree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-15 14:39:10.000000 pulp-cli-ostree-0.1.1/pulpcore/cli/ostree/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:39:10.000000 pulp-cli-ostree-0.1.1/pulpcore/cli/ostree/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-15 14:39:10.000000 pulp-cli-ostree-0.1.1/pulpcore/cli/ostree/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-05-15 14:39:10.000000 pulp-cli-ostree-0.1.1/pulpcore/cli/ostree/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-15 14:39:10.000000 pulp-cli-ostree-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 14:39:31.039075 pulp-cli-ostree-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-15 14:39:10.000000 pulp-cli-ostree-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:58.184807 pulp-cli-ostree-0.2.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-03 11:54:58.184807 pulp-cli-ostree-0.2.0.dev0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:58.184807 pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-03 11:54:58.000000 pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-03 11:54:58.000000 pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 11:54:58.000000 pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-03 11:54:58.000000 pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-03 11:54:58.000000 pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-03 11:54:58.000000 pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:58.184807 pulp-cli-ostree-0.2.0.dev0/pulpcore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:58.184807 pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:58.184807 pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-03 11:54:44.000000 pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-04-03 11:54:44.000000 pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:44.000000 pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-03 11:54:44.000000 pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-04-03 11:54:44.000000 pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-03 11:54:44.000000 pulp-cli-ostree-0.2.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 11:54:58.184807 pulp-cli-ostree-0.2.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-03 11:54:44.000000 pulp-cli-ostree-0.2.0.dev0/setup.py
```

### Comparing `pulp-cli-ostree-0.1.1/PKG-INFO` & `pulp-cli-ostree-0.2.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-cli-ostree
-Version: 0.1.1
+Version: 0.2.0.dev0
 Summary: Command line interface to talk to pulpcore's REST API. (OSTree plugin commands)
 Home-page: https://github.com/pulp/pulp-cli-ostree
 Author: Pulp Team
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
```

### Comparing `pulp-cli-ostree-0.1.1/pulp_cli_ostree.egg-info/PKG-INFO` & `pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-cli-ostree
-Version: 0.1.1
+Version: 0.2.0.dev0
 Summary: Command line interface to talk to pulpcore's REST API. (OSTree plugin commands)
 Home-page: https://github.com/pulp/pulp-cli-ostree
 Author: Pulp Team
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
```

### Comparing `pulp-cli-ostree-0.1.1/pulpcore/cli/ostree/__init__.py` & `pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import click
 from pulpcore.cli.common.generic import pulp_group
 
 from pulpcore.cli.ostree.distribution import distribution
 from pulpcore.cli.ostree.remote import remote
 from pulpcore.cli.ostree.repository import repository
 
-__version__ = "0.1.1"
+__version__ = "0.2.0.dev"
 
 
 @pulp_group("ostree")
 def ostree_group() -> None:
     pass
```

### Comparing `pulp-cli-ostree-0.1.1/pulpcore/cli/ostree/distribution.py` & `pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/distribution.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-ostree-0.1.1/pulpcore/cli/ostree/remote.py` & `pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/remote.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-ostree-0.1.1/pulpcore/cli/ostree/repository.py` & `pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/repository.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-ostree-0.1.1/pyproject.toml` & `pulp-cli-ostree-0.2.0.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulp-cli-ostree-0.1.1/setup.py` & `pulp-cli-ostree-0.2.0.dev0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 
 setup(
     name="pulp-cli-ostree",
     description="Command line interface to talk to pulpcore's REST API. (OSTree plugin commands)",
     author="Pulp Team",
     url="https://github.com/pulp/pulp-cli-ostree",
-    version="0.1.1",
+    version="0.2.0.dev",
     packages=plugin_packages,
     package_data={package: ["py.typed"] for package in plugin_packages},
     python_requires=">=3.6",
-    install_requires=["pulp-cli>=0.18.0", "pulp-glue-ostree==0.1.1"],
+    install_requires=["pulp-cli>=0.18.0", "pulp-glue-ostree==0.2.0.dev"],
     entry_points={
         "pulp_cli.plugins": [f"{name}={module}" for name, module in plugin_entry_points],
     },
     license="GPLv2+",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
```

