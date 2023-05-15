# Comparing `tmp/simmon-0.0.2.tar.gz` & `tmp/simmon-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simmon-0.0.2.tar", last modified: Sat May 13 17:50:22 2023, max compression
+gzip compressed data, was "simmon-0.0.3.tar", last modified: Mon May 15 05:05:35 2023, max compression
```

## Comparing `simmon-0.0.2.tar` & `simmon-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 17:50:22.074420 simmon-0.0.2/
--rw-rw-rw-   0        0        0     1086 2023-05-13 12:49:09.000000 simmon-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     6055 2023-05-13 17:50:22.074420 simmon-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5757 2023-05-13 17:49:08.000000 simmon-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-13 17:50:22.074420 simmon-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-05-13 17:50:12.000000 simmon-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:50:22.058811 simmon-0.0.2/simmon/
-drwxrwxrwx   0        0        0        0 2023-05-13 17:50:22.074420 simmon-0.0.2/simmon/simmon.egg-info/
--rw-rw-rw-   0        0        0     6055 2023-05-13 17:50:21.000000 simmon-0.0.2/simmon/simmon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-13 17:50:21.000000 simmon-0.0.2/simmon/simmon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 17:50:21.000000 simmon-0.0.2/simmon/simmon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-13 17:50:21.000000 simmon-0.0.2/simmon/simmon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-13 17:50:21.000000 simmon-0.0.2/simmon/simmon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    29858 2023-05-13 14:45:40.000000 simmon-0.0.2/simmon/simmon.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:05:35.056275 simmon-0.0.3/
+-rw-rw-rw-   0        0        0     1086 2023-05-13 12:49:09.000000 simmon-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6236 2023-05-15 05:05:35.056275 simmon-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5901 2023-05-15 04:55:07.000000 simmon-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-15 05:05:35.056275 simmon-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      693 2023-05-15 05:05:26.000000 simmon-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:05:35.056275 simmon-0.0.3/simmon/
+drwxrwxrwx   0        0        0        0 2023-05-15 05:05:35.056275 simmon-0.0.3/simmon/simmon.egg-info/
+-rw-rw-rw-   0        0        0     6236 2023-05-15 05:05:34.000000 simmon-0.0.3/simmon/simmon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-15 05:05:34.000000 simmon-0.0.3/simmon/simmon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 05:05:34.000000 simmon-0.0.3/simmon/simmon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-15 05:05:34.000000 simmon-0.0.3/simmon/simmon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-15 05:05:34.000000 simmon-0.0.3/simmon/simmon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    29858 2023-05-13 14:45:40.000000 simmon-0.0.3/simmon/simmon.py
```

### Comparing `simmon-0.0.2/LICENSE` & `simmon-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simmon-0.0.2/PKG-INFO` & `simmon-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,12 @@
-Metadata-Version: 2.1
-Name: simmon
-Version: 0.0.2
-Summary: A simple simulation monitor
-Author: Roie Zemel
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![Logo](https://raw.githubusercontent.com/roiezemel/simmon/main/assets/simmon_expanded_logo.png)
 
 [![PyPI version](https://badge.fury.io/py/simmon.svg)](https://badge.fury.io/py/simmon)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/roiezemel/simmon)
 
 # A simple monitor for simulations and other numeric processes
 
 ## Overview
 This project provides a simple tool for tracking simulations and 
 other numeric processes. It provides a Monitor class that has 
 all the following functionality:
```

### Comparing `simmon-0.0.2/README.md` & `simmon-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,24 @@
+Metadata-Version: 2.1
+Name: simmon
+Version: 0.0.3
+Summary: A simple simulation monitor
+Author: Roie Zemel
+Keywords: simulation, data tracking
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![Logo](https://raw.githubusercontent.com/roiezemel/simmon/main/assets/simmon_expanded_logo.png)
 
 [![PyPI version](https://badge.fury.io/py/simmon.svg)](https://badge.fury.io/py/simmon)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/roiezemel/simmon)
 
 # A simple monitor for simulations and other numeric processes
 
 ## Overview
 This project provides a simple tool for tracking simulations and 
 other numeric processes. It provides a Monitor class that has 
 all the following functionality:
```

### Comparing `simmon-0.0.2/simmon/simmon.egg-info/PKG-INFO` & `simmon-0.0.3/simmon/simmon.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: simmon
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple simulation monitor
 Author: Roie Zemel
+Keywords: simulation, data tracking
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Logo](https://raw.githubusercontent.com/roiezemel/simmon/main/assets/simmon_expanded_logo.png)
 
 [![PyPI version](https://badge.fury.io/py/simmon.svg)](https://badge.fury.io/py/simmon)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/roiezemel/simmon)
 
 # A simple monitor for simulations and other numeric processes
 
 ## Overview
 This project provides a simple tool for tracking simulations and 
 other numeric processes. It provides a Monitor class that has 
 all the following functionality:
```

### Comparing `simmon-0.0.2/simmon/simmon.py` & `simmon-0.0.3/simmon/simmon.py`

 * *Files identical despite different names*

