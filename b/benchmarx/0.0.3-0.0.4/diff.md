# Comparing `tmp/benchmarx-0.0.3.tar.gz` & `tmp/benchmarx-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchmarx-0.0.3.tar", last modified: Sun May 14 21:27:36 2023, max compression
+gzip compressed data, was "benchmarx-0.0.4.tar", last modified: Sun May 14 22:02:07 2023, max compression
```

## Comparing `benchmarx-0.0.3.tar` & `benchmarx-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,32 @@
-drwxr-xr-x   0 aleksandrtrisin   (501) staff       (20)        0 2023-05-14 21:27:36.699464 benchmarx-0.0.3/
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)     1074 2023-05-12 10:09:01.000000 benchmarx-0.0.3/LICENSE
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      601 2023-05-14 21:27:36.699318 benchmarx-0.0.3/PKG-INFO
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)       12 2023-05-13 21:44:46.000000 benchmarx-0.0.3/README.md
-drwxr-xr-x   0 aleksandrtrisin   (501) staff       (20)        0 2023-05-14 21:27:36.697655 benchmarx-0.0.3/benchmarx/
-drwxr-xr-x   0 aleksandrtrisin   (501) staff       (20)        0 2023-05-14 21:27:36.699107 benchmarx-0.0.3/benchmarx/benchmarx.egg-info/
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      601 2023-05-14 21:27:36.000000 benchmarx-0.0.3/benchmarx/benchmarx.egg-info/PKG-INFO
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      255 2023-05-14 21:27:36.000000 benchmarx-0.0.3/benchmarx/benchmarx.egg-info/SOURCES.txt
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)        1 2023-05-14 21:27:36.000000 benchmarx-0.0.3/benchmarx/benchmarx.egg-info/dependency_links.txt
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      117 2023-05-14 21:27:36.000000 benchmarx-0.0.3/benchmarx/benchmarx.egg-info/requires.txt
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)        1 2023-05-14 21:27:36.000000 benchmarx-0.0.3/benchmarx/benchmarx.egg-info/top_level.txt
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      572 2023-05-14 21:26:34.000000 benchmarx-0.0.3/pyproject.toml
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)       38 2023-05-14 21:27:36.699513 benchmarx-0.0.3/setup.cfg
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      975 2023-05-14 21:27:34.000000 benchmarx-0.0.3/setup.py
+drwxr-xr-x   0 aleksandrtrisin   (501) staff       (20)        0 2023-05-14 22:02:07.248060 benchmarx-0.0.4/
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)     1074 2023-05-12 10:09:01.000000 benchmarx-0.0.4/LICENSE
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      601 2023-05-14 22:02:07.247898 benchmarx-0.0.4/PKG-INFO
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)       12 2023-05-13 21:44:46.000000 benchmarx-0.0.4/README.md
+drwxr-xr-x   0 aleksandrtrisin   (501) staff       (20)        0 2023-05-14 22:02:07.243349 benchmarx-0.0.4/benchmarx/
+drwxr-xr-x   0 aleksandrtrisin   (501) staff       (20)        0 2023-05-14 22:02:07.244929 benchmarx-0.0.4/benchmarx/benchmarx.egg-info/
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      601 2023-05-14 22:02:07.000000 benchmarx-0.0.4/benchmarx/benchmarx.egg-info/PKG-INFO
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      776 2023-05-14 22:02:07.000000 benchmarx-0.0.4/benchmarx/benchmarx.egg-info/SOURCES.txt
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)        1 2023-05-14 22:02:07.000000 benchmarx-0.0.4/benchmarx/benchmarx.egg-info/dependency_links.txt
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      127 2023-05-14 22:02:07.000000 benchmarx-0.0.4/benchmarx/benchmarx.egg-info/requires.txt
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)        4 2023-05-14 22:02:07.000000 benchmarx-0.0.4/benchmarx/benchmarx.egg-info/top_level.txt
+drwxr-xr-x   0 aleksandrtrisin   (501) staff       (20)        0 2023-05-14 22:02:07.247659 benchmarx-0.0.4/benchmarx/src/
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)    11189 2023-05-14 18:00:49.000000 benchmarx-0.0.4/benchmarx/src/NeuralNetworkTraining.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)     1543 2023-05-12 12:42:47.000000 benchmarx-0.0.4/benchmarx/src/ProxGD_custom_linesearch.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)        0 2023-05-14 21:58:35.000000 benchmarx-0.0.4/benchmarx/src/__init__.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)    21138 2023-05-14 18:10:22.000000 benchmarx-0.0.4/benchmarx/src/benchmark.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)     5271 2023-05-14 17:55:41.000000 benchmarx-0.0.4/benchmarx/src/benchmark_result.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)     1333 2023-04-27 19:34:58.000000 benchmarx-0.0.4/benchmarx/src/custom_optimizer.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)       46 2023-04-30 18:47:02.000000 benchmarx-0.0.4/benchmarx/src/defaults.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)     2073 2023-05-13 18:59:48.000000 benchmarx-0.0.4/benchmarx/src/log_loss.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)     2258 2023-05-13 18:59:53.000000 benchmarx-0.0.4/benchmarx/src/log_loss_l2_reg.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      495 2023-05-14 17:57:46.000000 benchmarx-0.0.4/benchmarx/src/methods.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)     1212 2023-05-14 17:54:18.000000 benchmarx-0.0.4/benchmarx/src/metrics.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)    20912 2023-05-14 21:08:08.000000 benchmarx-0.0.4/benchmarx/src/plotter.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      779 2023-05-13 20:00:22.000000 benchmarx-0.0.4/benchmarx/src/problem.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)     1402 2023-05-13 20:35:15.000000 benchmarx-0.0.4/benchmarx/src/qadratic_problem_real_data.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)     1916 2023-05-12 13:01:37.000000 benchmarx-0.0.4/benchmarx/src/quadratic_problem.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      831 2023-05-13 19:39:55.000000 benchmarx-0.0.4/benchmarx/src/rastrigin.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      810 2023-05-13 19:40:29.000000 benchmarx-0.0.4/benchmarx/src/rosenbrock.py
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      902 2023-05-14 22:00:56.000000 benchmarx-0.0.4/pyproject.toml
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)       38 2023-05-14 22:02:07.248103 benchmarx-0.0.4/setup.cfg
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      996 2023-05-14 22:00:53.000000 benchmarx-0.0.4/setup.py
```

### Comparing `benchmarx-0.0.3/LICENSE` & `benchmarx-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `benchmarx-0.0.3/PKG-INFO` & `benchmarx-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchmarx
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tools for benchmarking optimization methods
 Home-page: https://github.com/AlexToW/benchmarx
 Author: AlexToW
 Author-email: Salex <31salex31@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AlexToW/benchmarx
 Project-URL: Bug Tracker, https://github.com/AlexToW/benchmarx/issues
```

### Comparing `benchmarx-0.0.3/benchmarx/benchmarx.egg-info/PKG-INFO` & `benchmarx-0.0.4/benchmarx/benchmarx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchmarx
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tools for benchmarking optimization methods
 Home-page: https://github.com/AlexToW/benchmarx
 Author: AlexToW
 Author-email: Salex <31salex31@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AlexToW/benchmarx
 Project-URL: Bug Tracker, https://github.com/AlexToW/benchmarx/issues
```

### Comparing `benchmarx-0.0.3/pyproject.toml` & `benchmarx-0.0.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "jax", "jaxopt >= 0.6", "typing-extensions >= 4.5.0","wandb >= 0.14.2","pandas == 1.5.3","plotly >= 5.14.1","flax >= 0.6.10","tensorflow_datasets"]
 build-backend = "hatchling.build"
 
 [project]
+dependencies = ["hatchling", "jax", "jaxopt >= 0.6", "typing-extensions >= 4.5.0", "wandb >= 0.14.2", "pandas == 1.5.3", "plotly >= 5.14.1", "flax >= 0.6.10", "tensorflow_datasets"]
 name = "benchmarx"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Salex", email="31salex31@gmail.com" },
 ]
 description = "Tools for benchmarking optimization methods"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `benchmarx-0.0.3/setup.py` & `benchmarx-0.0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
     name="benchmarx",
-    version="0.0.3",
+    version="0.0.4",
     description="Tools for benchmarking optimization methods",
     package_dir={"" : "benchmarx"},
     packages=find_packages(where="benchmarx"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AlexToW/benchmarx",
     author="AlexToW",
@@ -19,14 +19,15 @@
     license="MIT",
     classifiers=[
         "Licanse :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Operating System :: OS Independent",
     ],
     install_requires=[
+        "hatchling",
         "jax",
         "jaxopt >= 0.6",
         "typing-extensions >= 4.5.0",
         "wandb >= 0.14.2",
         "pandas == 1.5.3",
         "plotly >= 5.14.1",
         "flax >= 0.6.10",
```

