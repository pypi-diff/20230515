# Comparing `tmp/vrplib-1.0.1.tar.gz` & `tmp/vrplib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vrplib-1.0.1.tar", max compression
+gzip compressed data, was "vrplib-1.1.0.tar", max compression
```

## Comparing `vrplib-1.0.1.tar` & `vrplib-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1065 2022-04-16 13:56:24.912717 vrplib-1.0.1/LICENSE
--rw-r--r--   0        0        0     5871 2023-02-07 11:27:41.270820 vrplib-1.0.1/README.md
--rw-r--r--   0        0        0     1108 2023-02-17 14:55:19.061863 vrplib-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      118 2023-02-06 13:16:48.597040 vrplib-1.0.1/vrplib/__init__.py
--rw-r--r--   0        0        0      133 2023-02-13 17:27:32.909102 vrplib-1.0.1/vrplib/download/__init__.py
--rw-r--r--   0        0        0      358 2023-02-13 16:45:49.189310 vrplib-1.0.1/vrplib/download/constants.py
--rw-r--r--   0        0        0      746 2023-02-13 16:50:33.818420 vrplib-1.0.1/vrplib/download/download_instance.py
--rw-r--r--   0        0        0      686 2023-02-13 16:50:33.819229 vrplib-1.0.1/vrplib/download/download_solution.py
--rw-r--r--   0        0        0     1263 2023-02-06 15:11:44.545798 vrplib-1.0.1/vrplib/download/download_utils.py
--rw-r--r--   0        0        0    18524 2023-02-06 13:16:48.598179 vrplib-1.0.1/vrplib/download/instance_data.csv
--rw-r--r--   0        0        0     1682 2023-02-06 13:16:48.598348 vrplib-1.0.1/vrplib/download/list_names.py
--rw-r--r--   0        0        0      123 2023-02-06 13:16:48.598476 vrplib-1.0.1/vrplib/parse/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 13:16:48.598565 vrplib-1.0.1/vrplib/parse/distances/__init__.py
--rw-r--r--   0        0        0     4281 2023-02-13 17:38:08.749038 vrplib-1.0.1/vrplib/parse/parse_distances.py
--rw-r--r--   0        0        0      914 2023-02-06 13:16:48.599196 vrplib-1.0.1/vrplib/parse/parse_solomon.py
--rw-r--r--   0        0        0     1069 2023-02-06 13:16:48.599418 vrplib-1.0.1/vrplib/parse/parse_solution.py
--rw-r--r--   0        0        0      424 2023-02-06 13:16:48.599632 vrplib-1.0.1/vrplib/parse/parse_utils.py
--rw-r--r--   0        0        0     3849 2023-02-13 16:50:33.820903 vrplib-1.0.1/vrplib/parse/parse_vrplib.py
--rw-r--r--   0        0        0       82 2023-02-06 13:16:48.601550 vrplib-1.0.1/vrplib/read/__init__.py
--rw-r--r--   0        0        0      658 2023-02-06 13:16:48.601852 vrplib-1.0.1/vrplib/read/read_instance.py
--rw-r--r--   0        0        0      369 2023-02-06 13:16:48.602001 vrplib-1.0.1/vrplib/read/read_solution.py
--rw-r--r--   0        0        0     6733 1970-01-01 00:00:00.000000 vrplib-1.0.1/setup.py
--rw-r--r--   0        0        0     6571 1970-01-01 00:00:00.000000 vrplib-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-04-16 13:56:24.912717 vrplib-1.1.0/LICENSE
+-rw-r--r--   0        0        0     8247 2023-05-02 14:33:26.191015 vrplib-1.1.0/README.md
+-rw-r--r--   0        0        0     1133 2023-05-15 09:50:28.677738 vrplib-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-02-06 13:16:48.597040 vrplib-1.1.0/vrplib/__init__.py
+-rw-r--r--   0        0        0      133 2023-04-18 19:36:43.150095 vrplib-1.1.0/vrplib/download/__init__.py
+-rw-r--r--   0        0        0      358 2023-02-13 16:45:49.189310 vrplib-1.1.0/vrplib/download/constants.py
+-rw-r--r--   0        0        0     1014 2023-04-26 17:05:13.976320 vrplib-1.1.0/vrplib/download/download_instance.py
+-rw-r--r--   0        0        0      952 2023-04-26 17:05:13.977912 vrplib-1.1.0/vrplib/download/download_solution.py
+-rw-r--r--   0        0        0     1263 2023-04-19 08:41:44.020458 vrplib-1.1.0/vrplib/download/download_utils.py
+-rw-r--r--   0        0        0    18524 2023-02-06 13:16:48.598179 vrplib-1.1.0/vrplib/download/instance_data.csv
+-rw-r--r--   0        0        0     1682 2023-04-19 08:31:58.419704 vrplib-1.1.0/vrplib/download/list_names.py
+-rw-r--r--   0        0        0      123 2023-02-06 13:16:48.598476 vrplib-1.1.0/vrplib/parse/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 13:16:48.598565 vrplib-1.1.0/vrplib/parse/distances/__init__.py
+-rw-r--r--   0        0        0     4282 2023-05-15 09:50:15.783042 vrplib-1.1.0/vrplib/parse/parse_distances.py
+-rw-r--r--   0        0        0     2084 2023-05-15 09:50:15.783357 vrplib-1.1.0/vrplib/parse/parse_solomon.py
+-rw-r--r--   0        0        0     1069 2023-05-15 09:50:15.783884 vrplib-1.1.0/vrplib/parse/parse_solution.py
+-rw-r--r--   0        0        0      424 2023-02-06 13:16:48.599632 vrplib-1.1.0/vrplib/parse/parse_utils.py
+-rw-r--r--   0        0        0     4045 2023-05-15 09:50:15.784353 vrplib-1.1.0/vrplib/parse/parse_vrplib.py
+-rw-r--r--   0        0        0       82 2023-02-06 13:16:48.601550 vrplib-1.1.0/vrplib/read/__init__.py
+-rw-r--r--   0        0        0     1070 2023-05-15 09:44:35.624203 vrplib-1.1.0/vrplib/read/read_instance.py
+-rw-r--r--   0        0        0      466 2023-05-15 09:44:35.624518 vrplib-1.1.0/vrplib/read/read_solution.py
+-rw-r--r--   0        0        0     9252 1970-01-01 00:00:00.000000 vrplib-1.1.0/setup.py
+-rw-r--r--   0        0        0     8993 1970-01-01 00:00:00.000000 vrplib-1.1.0/PKG-INFO
```

### Comparing `vrplib-1.0.1/LICENSE` & `vrplib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vrplib-1.0.1/README.md` & `vrplib-1.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,174 @@
 # VRPLIB
 [![PyPI version](https://badge.fury.io/py/vrplib.svg)](https://badge.fury.io/py/vrplib)
 [![vrplib](https://github.com/leonlan/vrplib/actions/workflows/vrplib.yaml/badge.svg)](https://github.com/leonlan/vrplib/actions/workflows/vrplib.yaml)
 [![codecov](https://codecov.io/gh/leonlan/VRPLIB/branch/master/graph/badge.svg?token=X0X66LBNZ7)](https://codecov.io/gh/leonlan/VRPLIB)
 
-`vrplib` is a Python package for reading Vehicle Routing Problem (VRP) instances. The main features are:
+`vrplib` is a Python package for working with Vehicle Routing Problem (VRP) instances. The main features are:
 - reading VRPLIB and Solomon instances and solutions, and
 - downloading instances and best known solutions from [CVRPLIB](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/).
 
-# Installation
-This library works with Python 3.8+ and only depends on `numpy`. Install the latest version of `vrplib`:
+## Installation
+`vrplib` works with Python 3.8+ and only depends on `numpy`.
 
 ```shell
 pip install vrplib
 ```
 
-# Example usage
-## Reading instances and solutions
+## Example usage
+### Reading instances and solutions
 ```python
 import vrplib
 
 # Read VRPLIB formatted instances (default)
 instance = vrplib.read_instance("/path/to/X-n101-k25.vrp")
 solution = vrplib.read_solution("/path/to/X-n101-k25.sol")
 
 # Read Solomon formatted instances
 instance = vrplib.read_instance("/path/to/C101.txt", instance_format="solomon")
 solution = vrplib.read_solution("/path/to/C101.sol") # only 1 solution format
 ```
 
 `instance` and `solution` are dictionaries that contain all parsed data. 
 ``` python
-instance.keys()
-# dict_keys(['name', 'comment', 'type', 'dimension', ..., 'edge_weight'])
+>>> instance.keys()
+dict_keys(['name', ..., 'edge_weight'])
 
-solutions.keys()
-# dict_keys(['routes', 'cost'])
+>>> solution.keys()
+dict_keys(['routes', 'cost'])
 ```
 
 
-## Downloading instances from CVRPLIB 
+### Downloading instances from CVRPLIB 
 ``` python
 import vrplib
 
-# Download the instance and solution to a local file
-vrplib.download_instance("X-n101-k25", "/path/to/X-n101-k25.vrp")
-vrplib.download_solution("X-n101-k25", "/path/to/X-n101-k25.sol")
+# Download an instance and a solution file 
+vrplib.download_instance("X-n101-k25", "/path/to/instances/")
+vrplib.download_solution("X-n101-k25", "/path/to/solutions/")
 
 # List all instance names that can be downloaded 
 vrplib.list_names()                      # All instance names
 vrplib.list_names(low=100, high=200)     # Instances with between [100, 200] customers
-vrplib.list_names(vrp_type='cvrp')       # Only CVRP instances
-vrplib.list_names(vrp_type='vrptw')      # Only VRPTW instances
+vrplib.list_names(vrp_type="cvrp")       # Only CVRP instances
+vrplib.list_names(vrp_type="vrptw")      # Only VRPTW instances
 ```
 
 
-# Notes
-This section contains additional notes about the `vrplib` package.
+## Documentation
+- [VRPLIB instance format](#vrplib-instance-format)
+- [Solomon instance format](#solomon-instance-format)
+- [Solution format](#solution-format)
+- [Other remarks](#other-remarks)
+
+### VRPLIB instance format
+The VRPLIB format is the standard format for the Capacitated Vehicle Routing Problem (CVRP). An example VRPLIB instance looks as follows:
+``` bash
+NAME: Example 
+EDGE_WEIGHT_TYPE: EUC_2D
+NODE_COORD_SECTION
+1 0 0
+2 5 5
+SERVICE_TIME_SECTION
+1 0
+2 3
+DEPOT_SECTION
+1
+EOF
+```
+
+A VRPLIB instance contains problem **specifications** and problem **data**. 
+- Specifications are key-value pairs separated by a colon. In the example above, `NAME` and `EDGE_WEIGHT_TYPE` are the two data specifications.
+- Data are explicit array-like values such as customer coordinates or service times. 
+Each data section should start with a header name that ends with `_SECTION`, e.g., `NODE_COORD_SECTION` and `SERVICE_TIME_SECTION`. It is then followed by rows of values and each row must start with an index representing the depot or customer. 
+There are two exceptions: values in `EDGE_WEIGHT_SECTION` and `DEPOT_SECTION` should not start with an index.
 
-## Instance formats
-Currently, two VRP instance formats are supported:
-- **VRPLIB**: this format is most commonly used for Capacitated Vehicle Routing Problem (CVRP) instances.  See the [X-n101-k25](http://vrp.atd-lab.inf.puc-rio.br/media/com_vrp/instances/X/X-n101-k25.vrp) instance for an example. VRPLIB is an extension of the [TSPLIB95](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/tsp95.pdf) format. Additional information about the VRPLIB format can be found [here]( http://webhotel4.ruc.dk/~keld/research/LKH-3/LKH-3_REPORT.pdf). 
-- **Solomon**: this format was used to introduce the Solomon instances for the Vehicle Routing Problem with Time Window (VRPTW) and also the extended instance set by Homberger and Gehring. See the [C101](http://vrp.atd-lab.inf.puc-rio.br/media/com_vrp/instances/Solomon/C101.txt) instance for an example.
+Besides the rules outlined above, `vrplib` is not strict about the naming of specifications or sections. 
+This means that you can use `vrplib` to read VRPLIB instances with custom specifications like `MY_SPECIFICATION: SOME_VALUE` and custom section names like `MY_SECTION`.
 
-## How instances are parsed
-`vrplib` parses an instance and returns a dictionary of keyword-value pairs. There are two types of instance data: 
-- Problem specifications, which may contain metadata or problem-specific information such as the max number of vehicles. 
-- Problem data, which are often arrays of values describing, for example, customer service times and time windows. 
+Reading the above example instance returns the following dictionary:
+``` python
+{'name': 'Example',
+ 'edge_weight_type': 'EUC_2D',
+ 'node_coord': array([[0, 0], [5, 5]]),
+ 'service_time': array([1, 3]),
+ 'depot': array([0]),
+ 'edge_weight': array([[0.  , 7.07106781], [7.07106781, 0.  ]])}
+```
 
-### On parsing distances 
-The `vrplib` library tries to follow the instance specifications as strictly as possible to compute the distances. 
+The depot section specifies which location index corresponds to the depot data. 
+The convention is to let index 1 represent the depot. 
+`vrplib` subtracts one from the depot value to make it easier to index.
+
+#### Computing edge weights 
+Note that the example instance did not include any explicit information about the edge weights, yet the output includes edge weights data.
+This is because `vrplib` automatically computes the edge weights based on the instance specifications, if applicable.
+In the example, the edge weight type specification and node coordinates data are used to compute the Euclidean distance.
+You can set the `compute_distances` argument in `read_instance` to disable this feature.
 
-For VRPLIB instances, the distances computation is determined by the `EDGE_WEIGHT_TYPE` and possibly the `EDGE_WEIGHT_FORMAT` specifications. We currently support two categories of edge weight types:
-- `*_2D`: compute the Euclidean distances using the node coordinate data.
+Following the VRPLIB conventions, the edge weights are computed based on the `EDGE_WEIGHT_TYPE` specification, and in some cases the `EDGE_WEIGHT_FORMAT` specification. `vrplib` currently supports two categories of edge weight types:
+- `*_2D`: Euclidean distances based on the node coordinates data.
     - `EUC_2D`: Double precision distances without rounding.
     - `FLOOR_2D`: Round down all distances to down to an integer.
     - `EXACT_2D`: Multiply the distances by 1000, round to the nearest integer.
-- `EXPLICIT`: the distance data is explicitly provided, in partial or full form. For explicit matrices, the `EDGE_WEIGHT_FORMAT` must be specified. We support the following two formats:
-  - `LOWER_ROW`: Lower row triangular matrix without diagonal entries.  
+- `EXPLICIT`: the distance data is explicitly provided, in partial or full form. The `EDGE_WEIGHT_FORMAT` specification must be present. We support the following two edge weight formats:
+  - `LOWER_ROW`: Lower row triangular matrix without diagonal entries.
   - `FULL_MATRIX`: Explicit full matrix representation.
   
-More information about how VRPLIB specifications can be found [here](  http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/tsp95.pdf) and [here]( http://webhotel4.ruc.dk/~keld/research/LKH-3/LKH-3_REPORT.pdf).
 
-Note that there are VRPLIB instances that use different rounding conventions in the literature, which may not be specified in the instance. For example, the X instance set proposed by [Uchoa et al. (2017)](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/new-instances) assumes that the distances are rounded to the nearest integer. When you use the `vrplib` package to read instances from the X set, it will return unrounded Euclidean distances because the instance specifies the `EUC_2D` edge weight type, i.e., no rouding. This can be easily solved by rounding the distances matrix manually.
+#### More information about VRPLIB
+The VRPLIB format is an extension of the [TSPLIB95](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/tsp95.pdf) format. 
+Additional information about the VRPLIB format can be found [here]( http://webhotel4.ruc.dk/~keld/research/LKH-3/LKH-3_REPORT.pdf).
+
+### Solomon instance format
+The Solomon format was used to introduce the Solomon instances for the Vehicle Routing Problem with Time Window (VRPTW) and also the extended instance set by Homberger and Gehring. A Solomon instance looks like this:
+``` bash
+Example
+
+VEHICLE
+NUMBER     CAPACITY
+  50          200
+
+CUSTOMER
+CUST NO.  XCOORD.    YCOORD.    DEMAND   READY TIME  DUE DATE   SERVICE TIME
+    0      70         70          0          0       1351          0
+    1      33         78         20        750        809         90
+```
 
-For Solomon-type instances, the distance computation is not specified in the instance file, hence we compute the Euclidean distances without rounding. A recent convention that was proposed during the [2021 DIMACS Vehicle Routing Implementation Challenge](http://dimacs.rutgers.edu/programs/challenge/vrp/vrptw/) is to truncate the Euclidean distances to one decimal. Similar to the X instance set, you can manually modify the distances matrix.
+Reading this Solomon instance returns the following dictionary:
+``` python
+{'name': 'Example',
+ 'vehicles': 50,
+ 'capacity': 200,
+ 'node_coord': array([[70, 70], [33, 78]]),
+ 'demand': array([ 0, 20]),
+ 'time_window': array([[ 0, 1351], [ 750,  809]]),
+ 'service_time': array([ 0, 90]),
+ 'edge_weight': array([[ 0.  , 37.85498646], [37.85498646,  0.  ]])}
+```
 
-## Additional remarks
-- Downloading instances may take up to a few seconds. 
-- The `XML100` benchmark set is not listed in `list_names` and cannot be downloaded through this package. You can download these instances directly from [CVRPLIB](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/).
+The edge weights are computed by default using the Euclidean distances. 
 
-    
+### Solution format
+Here's an example of a solution format:
+``` { .html } 
+Route #1: 1 2 3
+Route #2: 4 5
+Cost: 100
+```
+
+A solution is represented by a set of routes, where each route specifies the sequence of customers to visit. 
+Each route should start with "Route", followed by the route number, and followed by a colon. 
+The customers to be served on the route are then listed.
+The solution file can also include other keywords like `Cost`, which will be separated on the first colon or whitespace.
+
+The convention is that customer indices start counting from 1, but `vrplib` simply parses the file without strict requirements about those indices.
+
+Reading the above example solution returns the following dictionary:
+``` python
+{'routes': [[1, 2, 3], [4, 5]], 'cost': 100}
+```
+
+### Other remarks
+- The `XML100` benchmark set is not listed in `list_names` and cannot be downloaded through this package. You can download these instances directly from [CVRPLIB](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/).
+- In the literature, some instances use rounding conventions different from what is specified in the instance. For example, X instance set proposed by [Uchoa et al. (2017)](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/new-instances) assumes that the distances are rounded to the nearest integer. When you use the `vrplib` package to read this instance, it will return non-rounded Euclidean distances because the instance specifies the `EUC_2D` edge weight type which implies no rounding. To adhere to the convention used in the literature, you can manually round the distances matrix.
+- For large instances (>5000 customers) it's recommended to set the `compute_edge_weights` argument to `False` in `read_instance`.
```

### Comparing `vrplib-1.0.1/pyproject.toml` & `vrplib-1.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "vrplib"
-version = "1.0.1"
-description = "Python library for reading vehicle routing problem instances."
+version = "1.1.0"
+description = "Python library for working with vehicle routing problem instances."
 authors = ["Leon Lan <leon.lanyidong@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/leonlan/VRPLIB"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.19"
+codecov = "^2.1.13"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.9"
 pytest = "^7.1.2"
-codecov = "^2.1.12"
+codecov = "^2.1.13"
 pytest-cov = "^4.0.0"
 pre-commit = "^2.19.0"
 
 [pytest]
 pythonpath = [".", "vrplib"]
 
 [build-system]
```

### Comparing `vrplib-1.0.1/vrplib/download/download_instance.py` & `vrplib-1.1.0/vrplib/download/download_instance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,34 @@
+import os
+from pathlib import Path
+from typing import Union
 from urllib.request import urlopen
 
 from .constants import CVRPLIB_URL
 from .download_utils import find_set, is_vrptw
 
 
-def download_instance(name: str, path: str):
+def download_instance(name: str, path: Union[str, os.PathLike]):
     """
     Downloads an instance file from CVRPLIB and saves it at the specified path.
 
     Parameters
     ----------
     name
         The name of the instance to download. Should be one of the names
         listed in `vrplib.list_instances()`.
     path
-        The path where the instance file should be saved.
+        The path where the instance file should be saved. If a directory is
+        specified, the file will be saved in that directory with the original
+        file name.
     """
     ext = "txt" if is_vrptw(name) else "vrp"
     url = CVRPLIB_URL + f"{find_set(name)}/{name}.{ext}"
     response = urlopen(url, timeout=30)
 
     instance_text = response.read().decode("utf-8")
 
+    if os.path.isdir(path):
+        path = Path(path) / f"{name}.{ext}"
+
     with open(path, "w") as fi:
         fi.write(instance_text)
```

### Comparing `vrplib-1.0.1/vrplib/download/download_solution.py` & `vrplib-1.1.0/vrplib/download/download_solution.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,33 @@
+import os
+from pathlib import Path
+from typing import Union
 from urllib.request import urlopen
 
 from .constants import CVRPLIB_URL
 from .download_utils import find_set
 
 
-def download_solution(name: str, path: str):
+def download_solution(name: str, path: Union[str, os.PathLike]):
     """
     Downloads a solution file from CVRPLIB and saves it at the specified path.
 
     Parameters
     ----------
     name
         The name of the instance to download. Should be one of the names
         listed in `vrplib.list_instances`.
     path
-        The path where the solution file should be saved.
+        The path where the solution file should be saved. If a directory is
+        specified, the file will be saved in that directory with the original
+        file name.
     """
     url = CVRPLIB_URL + f"{find_set(name)}/{name}.sol"
     response = urlopen(url, timeout=30)
 
     solution_text = response.read().decode("utf-8")
 
+    if os.path.isdir(path):
+        path = Path(path) / f"{name}.sol"
+
     with open(path, "w") as fi:
         fi.write(solution_text)
```

### Comparing `vrplib-1.0.1/vrplib/download/download_utils.py` & `vrplib-1.1.0/vrplib/download/download_utils.py`

 * *Files identical despite different names*

### Comparing `vrplib-1.0.1/vrplib/download/instance_data.csv` & `vrplib-1.1.0/vrplib/download/instance_data.csv`

 * *Files identical despite different names*

### Comparing `vrplib-1.0.1/vrplib/download/list_names.py` & `vrplib-1.1.0/vrplib/download/list_names.py`

 * *Files identical despite different names*

### Comparing `vrplib-1.0.1/vrplib/parse/parse_distances.py` & `vrplib-1.1.0/vrplib/parse/parse_distances.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,20 @@
     Returns
     -------
     np.ndarray
         An n-by-n distances matrix.
     """
     if "2D" in edge_weight_type:  # Euclidean distance on node coordinates
         if node_coord is None:
-            raise ValueError(
-                "Node coordinates are required for Euclidean edge weight type."
+            msg = (
+                "Cannot compute Euclidean distances because node coordinates "
+                "are not provided."
             )
+            raise ValueError(msg)
+
         distance = pairwise_euclidean(node_coord)
 
         if edge_weight_type == "EUC_2D":
             return distance
 
         if edge_weight_type == "FLOOR_2D":
             return np.floor(distance)
@@ -80,15 +83,14 @@
 
     Returns
     -------
     np.ndarray
         An n-by-n Euclidean distances matrix.
 
     """
-    # Subtract each coordinate from every other coordinate
     diff = coords[:, np.newaxis, :] - coords
     square_diff = diff**2
     square_dist = np.sum(square_diff, axis=-1)
     return np.sqrt(square_dist)
 
 
 def from_lower_row(triangular: np.ndarray) -> np.ndarray:
```

### Comparing `vrplib-1.0.1/vrplib/parse/parse_solution.py` & `vrplib-1.1.0/vrplib/parse/parse_solution.py`

 * *Files identical despite different names*

### Comparing `vrplib-1.0.1/vrplib/parse/parse_vrplib.py` & `vrplib-1.1.0/vrplib/parse/parse_vrplib.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 
 from .parse_distances import parse_distances
 from .parse_utils import infer_type, text2lines
 
 Instance = Dict[str, Union[str, float, np.ndarray]]
 
 
-def parse_vrplib(text: str) -> Instance:
+def parse_vrplib(text: str, compute_edge_weights: bool = True) -> Instance:
     """
     Parses a VRPLIB instance. An instance consists of two parts:
     1) Specifications: single line of the form <KEY>:<VALUE>.
     2) Data sections: starts with <KEY>_SECTION, followed by rows of values.
 
     Each specification is parsed as keyword-value pair, where the keyword is
     given lowercase and the value is unmodified. From each data section the
     name is parsed in lower case without the "_SECTION". The data values are
     parsed as numpy arrays, where customer indices are removed (if applicable).
 
     Parameters
     ----------
     text
         The instance text.
+    compute_edge_weights
+        Whether to compute edge weights from the node coordinates.
+        Defaults to True.
 
     Returns
     -------
     dict
         The instance data.
     """
     instance = {}
@@ -38,15 +41,15 @@
         key, value = parse_specification(spec)
         instance[key] = value
 
     for section in sections:
         section, data = parse_section(section, instance)
         instance[section] = data
 
-    if instance and "edge_weight" not in instance:
+    if instance and compute_edge_weights and "edge_weight" not in instance:
         # Compute edge weights if there was no explicit edge weight section
         edge_weights = parse_distances([], **instance)  # type: ignore
         instance["edge_weight"] = edge_weights
 
     return instance
 
 
@@ -55,36 +58,36 @@
     Groups instance lines into specifications and section parts.
     """
     specs = []
     sections = []
 
     end_section = 0
     for idx, line in enumerate(lines):
-        if idx < end_section:  # Skip all lines of the current section
-            continue
-
         if "EOF" in line:
             break
-
-        if ":" in line:
+        elif idx < end_section:  # Skip all lines of the current section
+            continue
+        elif ":" in line:
             specs.append(line)
-
-        if "_SECTION" in line:
+        elif "_SECTION" in line:
             start = lines.index(line)
             end_section = start + 1
 
             for next_line in lines[start + 1 :]:
-                # The current section ends when a next section is found or
-                # when an EOF token is found.
+                # The current section ends when a next section or an EOF token
+                # is found.
                 if "_SECTION" in next_line or "EOF" in next_line:
                     break
 
                 end_section += 1
 
             sections.append(lines[start:end_section])
+        else:
+            msg = "Instance does not conform to the VRPLIB format."
+            raise RuntimeError(msg)
 
     return specs, sections
 
 
 def parse_specification(line: str) -> Tuple[str, Union[float, str]]:
     """
     Parses a specification line as keyword-value pair, split at the first colon
@@ -99,24 +102,21 @@
     Parses the data section into numpy arrays.
     """
     section = _remove_suffix(lines[0].strip(), "_SECTION").lower()
     data_ = [[infer_type(n) for n in line.split()] for line in lines[1:]]
 
     if section == "edge_weight":
         # Parse separately because it may require additional processing
-        return section, parse_distances(data_, **instance)
+        return section, parse_distances(data_, **instance)  # type: ignore
 
     data = np.array(data_)
 
     if section == "depot":
-        if len(data) < 2 or data[-1] != -1:
-            raise RuntimeError("Depot section does not end with -1.")
-
-        # Remove end token and renormalize depots to start at zero
-        data = data[:-1] - 1
+        # Remove -1 end token and renormalize depots to start at zero
+        data = data[data != -1] - 1
     else:
         # We remove the customer indices column from non-depot section
         data = data[:, 1:]
 
     # Squeeze data sections that contain only one column
     if data.ndim > 1 and data.shape[-1] == 1:
         data = data.squeeze(-1)
```

### Comparing `vrplib-1.0.1/PKG-INFO` & `vrplib-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,195 @@
 Metadata-Version: 2.1
 Name: vrplib
-Version: 1.0.1
-Summary: Python library for reading vehicle routing problem instances.
+Version: 1.1.0
+Summary: Python library for working with vehicle routing problem instances.
 Home-page: https://github.com/leonlan/VRPLIB
 License: MIT
 Author: Leon Lan
 Author-email: leon.lanyidong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: codecov (>=2.1.13,<3.0.0)
 Requires-Dist: numpy (>=1.19,<2.0)
 Project-URL: Repository, https://github.com/leonlan/VRPLIB
 Description-Content-Type: text/markdown
 
 # VRPLIB
 [![PyPI version](https://badge.fury.io/py/vrplib.svg)](https://badge.fury.io/py/vrplib)
 [![vrplib](https://github.com/leonlan/vrplib/actions/workflows/vrplib.yaml/badge.svg)](https://github.com/leonlan/vrplib/actions/workflows/vrplib.yaml)
 [![codecov](https://codecov.io/gh/leonlan/VRPLIB/branch/master/graph/badge.svg?token=X0X66LBNZ7)](https://codecov.io/gh/leonlan/VRPLIB)
 
-`vrplib` is a Python package for reading Vehicle Routing Problem (VRP) instances. The main features are:
+`vrplib` is a Python package for working with Vehicle Routing Problem (VRP) instances. The main features are:
 - reading VRPLIB and Solomon instances and solutions, and
 - downloading instances and best known solutions from [CVRPLIB](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/).
 
-# Installation
-This library works with Python 3.8+ and only depends on `numpy`. Install the latest version of `vrplib`:
+## Installation
+`vrplib` works with Python 3.8+ and only depends on `numpy`.
 
 ```shell
 pip install vrplib
 ```
 
-# Example usage
-## Reading instances and solutions
+## Example usage
+### Reading instances and solutions
 ```python
 import vrplib
 
 # Read VRPLIB formatted instances (default)
 instance = vrplib.read_instance("/path/to/X-n101-k25.vrp")
 solution = vrplib.read_solution("/path/to/X-n101-k25.sol")
 
 # Read Solomon formatted instances
 instance = vrplib.read_instance("/path/to/C101.txt", instance_format="solomon")
 solution = vrplib.read_solution("/path/to/C101.sol") # only 1 solution format
 ```
 
 `instance` and `solution` are dictionaries that contain all parsed data. 
 ``` python
-instance.keys()
-# dict_keys(['name', 'comment', 'type', 'dimension', ..., 'edge_weight'])
+>>> instance.keys()
+dict_keys(['name', ..., 'edge_weight'])
 
-solutions.keys()
-# dict_keys(['routes', 'cost'])
+>>> solution.keys()
+dict_keys(['routes', 'cost'])
 ```
 
 
-## Downloading instances from CVRPLIB 
+### Downloading instances from CVRPLIB 
 ``` python
 import vrplib
 
-# Download the instance and solution to a local file
-vrplib.download_instance("X-n101-k25", "/path/to/X-n101-k25.vrp")
-vrplib.download_solution("X-n101-k25", "/path/to/X-n101-k25.sol")
+# Download an instance and a solution file 
+vrplib.download_instance("X-n101-k25", "/path/to/instances/")
+vrplib.download_solution("X-n101-k25", "/path/to/solutions/")
 
 # List all instance names that can be downloaded 
 vrplib.list_names()                      # All instance names
 vrplib.list_names(low=100, high=200)     # Instances with between [100, 200] customers
-vrplib.list_names(vrp_type='cvrp')       # Only CVRP instances
-vrplib.list_names(vrp_type='vrptw')      # Only VRPTW instances
+vrplib.list_names(vrp_type="cvrp")       # Only CVRP instances
+vrplib.list_names(vrp_type="vrptw")      # Only VRPTW instances
 ```
 
 
-# Notes
-This section contains additional notes about the `vrplib` package.
+## Documentation
+- [VRPLIB instance format](#vrplib-instance-format)
+- [Solomon instance format](#solomon-instance-format)
+- [Solution format](#solution-format)
+- [Other remarks](#other-remarks)
+
+### VRPLIB instance format
+The VRPLIB format is the standard format for the Capacitated Vehicle Routing Problem (CVRP). An example VRPLIB instance looks as follows:
+``` bash
+NAME: Example 
+EDGE_WEIGHT_TYPE: EUC_2D
+NODE_COORD_SECTION
+1 0 0
+2 5 5
+SERVICE_TIME_SECTION
+1 0
+2 3
+DEPOT_SECTION
+1
+EOF
+```
+
+A VRPLIB instance contains problem **specifications** and problem **data**. 
+- Specifications are key-value pairs separated by a colon. In the example above, `NAME` and `EDGE_WEIGHT_TYPE` are the two data specifications.
+- Data are explicit array-like values such as customer coordinates or service times. 
+Each data section should start with a header name that ends with `_SECTION`, e.g., `NODE_COORD_SECTION` and `SERVICE_TIME_SECTION`. It is then followed by rows of values and each row must start with an index representing the depot or customer. 
+There are two exceptions: values in `EDGE_WEIGHT_SECTION` and `DEPOT_SECTION` should not start with an index.
 
-## Instance formats
-Currently, two VRP instance formats are supported:
-- **VRPLIB**: this format is most commonly used for Capacitated Vehicle Routing Problem (CVRP) instances.  See the [X-n101-k25](http://vrp.atd-lab.inf.puc-rio.br/media/com_vrp/instances/X/X-n101-k25.vrp) instance for an example. VRPLIB is an extension of the [TSPLIB95](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/tsp95.pdf) format. Additional information about the VRPLIB format can be found [here]( http://webhotel4.ruc.dk/~keld/research/LKH-3/LKH-3_REPORT.pdf). 
-- **Solomon**: this format was used to introduce the Solomon instances for the Vehicle Routing Problem with Time Window (VRPTW) and also the extended instance set by Homberger and Gehring. See the [C101](http://vrp.atd-lab.inf.puc-rio.br/media/com_vrp/instances/Solomon/C101.txt) instance for an example.
+Besides the rules outlined above, `vrplib` is not strict about the naming of specifications or sections. 
+This means that you can use `vrplib` to read VRPLIB instances with custom specifications like `MY_SPECIFICATION: SOME_VALUE` and custom section names like `MY_SECTION`.
 
-## How instances are parsed
-`vrplib` parses an instance and returns a dictionary of keyword-value pairs. There are two types of instance data: 
-- Problem specifications, which may contain metadata or problem-specific information such as the max number of vehicles. 
-- Problem data, which are often arrays of values describing, for example, customer service times and time windows. 
+Reading the above example instance returns the following dictionary:
+``` python
+{'name': 'Example',
+ 'edge_weight_type': 'EUC_2D',
+ 'node_coord': array([[0, 0], [5, 5]]),
+ 'service_time': array([1, 3]),
+ 'depot': array([0]),
+ 'edge_weight': array([[0.  , 7.07106781], [7.07106781, 0.  ]])}
+```
 
-### On parsing distances 
-The `vrplib` library tries to follow the instance specifications as strictly as possible to compute the distances. 
+The depot section specifies which location index corresponds to the depot data. 
+The convention is to let index 1 represent the depot. 
+`vrplib` subtracts one from the depot value to make it easier to index.
+
+#### Computing edge weights 
+Note that the example instance did not include any explicit information about the edge weights, yet the output includes edge weights data.
+This is because `vrplib` automatically computes the edge weights based on the instance specifications, if applicable.
+In the example, the edge weight type specification and node coordinates data are used to compute the Euclidean distance.
+You can set the `compute_distances` argument in `read_instance` to disable this feature.
 
-For VRPLIB instances, the distances computation is determined by the `EDGE_WEIGHT_TYPE` and possibly the `EDGE_WEIGHT_FORMAT` specifications. We currently support two categories of edge weight types:
-- `*_2D`: compute the Euclidean distances using the node coordinate data.
+Following the VRPLIB conventions, the edge weights are computed based on the `EDGE_WEIGHT_TYPE` specification, and in some cases the `EDGE_WEIGHT_FORMAT` specification. `vrplib` currently supports two categories of edge weight types:
+- `*_2D`: Euclidean distances based on the node coordinates data.
     - `EUC_2D`: Double precision distances without rounding.
     - `FLOOR_2D`: Round down all distances to down to an integer.
     - `EXACT_2D`: Multiply the distances by 1000, round to the nearest integer.
-- `EXPLICIT`: the distance data is explicitly provided, in partial or full form. For explicit matrices, the `EDGE_WEIGHT_FORMAT` must be specified. We support the following two formats:
-  - `LOWER_ROW`: Lower row triangular matrix without diagonal entries.  
+- `EXPLICIT`: the distance data is explicitly provided, in partial or full form. The `EDGE_WEIGHT_FORMAT` specification must be present. We support the following two edge weight formats:
+  - `LOWER_ROW`: Lower row triangular matrix without diagonal entries.
   - `FULL_MATRIX`: Explicit full matrix representation.
   
-More information about how VRPLIB specifications can be found [here](  http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/tsp95.pdf) and [here]( http://webhotel4.ruc.dk/~keld/research/LKH-3/LKH-3_REPORT.pdf).
 
-Note that there are VRPLIB instances that use different rounding conventions in the literature, which may not be specified in the instance. For example, the X instance set proposed by [Uchoa et al. (2017)](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/new-instances) assumes that the distances are rounded to the nearest integer. When you use the `vrplib` package to read instances from the X set, it will return unrounded Euclidean distances because the instance specifies the `EUC_2D` edge weight type, i.e., no rouding. This can be easily solved by rounding the distances matrix manually.
+#### More information about VRPLIB
+The VRPLIB format is an extension of the [TSPLIB95](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/tsp95.pdf) format. 
+Additional information about the VRPLIB format can be found [here]( http://webhotel4.ruc.dk/~keld/research/LKH-3/LKH-3_REPORT.pdf).
+
+### Solomon instance format
+The Solomon format was used to introduce the Solomon instances for the Vehicle Routing Problem with Time Window (VRPTW) and also the extended instance set by Homberger and Gehring. A Solomon instance looks like this:
+``` bash
+Example
+
+VEHICLE
+NUMBER     CAPACITY
+  50          200
+
+CUSTOMER
+CUST NO.  XCOORD.    YCOORD.    DEMAND   READY TIME  DUE DATE   SERVICE TIME
+    0      70         70          0          0       1351          0
+    1      33         78         20        750        809         90
+```
 
-For Solomon-type instances, the distance computation is not specified in the instance file, hence we compute the Euclidean distances without rounding. A recent convention that was proposed during the [2021 DIMACS Vehicle Routing Implementation Challenge](http://dimacs.rutgers.edu/programs/challenge/vrp/vrptw/) is to truncate the Euclidean distances to one decimal. Similar to the X instance set, you can manually modify the distances matrix.
+Reading this Solomon instance returns the following dictionary:
+``` python
+{'name': 'Example',
+ 'vehicles': 50,
+ 'capacity': 200,
+ 'node_coord': array([[70, 70], [33, 78]]),
+ 'demand': array([ 0, 20]),
+ 'time_window': array([[ 0, 1351], [ 750,  809]]),
+ 'service_time': array([ 0, 90]),
+ 'edge_weight': array([[ 0.  , 37.85498646], [37.85498646,  0.  ]])}
+```
 
-## Additional remarks
-- Downloading instances may take up to a few seconds. 
-- The `XML100` benchmark set is not listed in `list_names` and cannot be downloaded through this package. You can download these instances directly from [CVRPLIB](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/).
+The edge weights are computed by default using the Euclidean distances. 
 
-    
+### Solution format
+Here's an example of a solution format:
+``` { .html } 
+Route #1: 1 2 3
+Route #2: 4 5
+Cost: 100
+```
+
+A solution is represented by a set of routes, where each route specifies the sequence of customers to visit. 
+Each route should start with "Route", followed by the route number, and followed by a colon. 
+The customers to be served on the route are then listed.
+The solution file can also include other keywords like `Cost`, which will be separated on the first colon or whitespace.
+
+The convention is that customer indices start counting from 1, but `vrplib` simply parses the file without strict requirements about those indices.
+
+Reading the above example solution returns the following dictionary:
+``` python
+{'routes': [[1, 2, 3], [4, 5]], 'cost': 100}
+```
+
+### Other remarks
+- The `XML100` benchmark set is not listed in `list_names` and cannot be downloaded through this package. You can download these instances directly from [CVRPLIB](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/).
+- In the literature, some instances use rounding conventions different from what is specified in the instance. For example, X instance set proposed by [Uchoa et al. (2017)](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/new-instances) assumes that the distances are rounded to the nearest integer. When you use the `vrplib` package to read this instance, it will return non-rounded Euclidean distances because the instance specifies the `EUC_2D` edge weight type which implies no rounding. To adhere to the convention used in the literature, you can manually round the distances matrix.
+- For large instances (>5000 customers) it's recommended to set the `compute_edge_weights` argument to `False` in `read_instance`.
```

