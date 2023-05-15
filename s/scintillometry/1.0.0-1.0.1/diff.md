# Comparing `tmp/scintillometry-1.0.0.tar.gz` & `tmp/scintillometry-1.0.1.tar.gz`

## Comparing `scintillometry-1.0.0.tar` & `scintillometry-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.0/src/scintillometry/__init__.py
--rw-r--r--   0        0        0    13708 2020-02-02 00:00:00.000000 scintillometry-1.0.0/src/scintillometry/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.0/src/scintillometry/backend/__init__.py
--rw-r--r--   0        0        0     8355 2020-02-02 00:00:00.000000 scintillometry-1.0.0/src/scintillometry/backend/constants.py
--rw-r--r--   0        0        0    25120 2020-02-02 00:00:00.000000 scintillometry-1.0.0/src/scintillometry/backend/constructions.py
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 scintillometry-1.0.0/src/scintillometry/backend/derivations.py
--rw-r--r--   0        0        0    15745 2020-02-02 00:00:00.000000 scintillometry-1.0.0/src/scintillometry/backend/iterations.py
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 scintillometry-1.0.0/src/scintillometry/backend/transects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.0/src/scintillometry/metrics/__init__.py
--rwxr-xr-x   0        0        0    38547 2020-02-02 00:00:00.000000 scintillometry-1.0.0/src/scintillometry/metrics/calculations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.0/src/scintillometry/visuals/__init__.py
--rw-r--r--   0        0        0    31296 2020-02-02 00:00:00.000000 scintillometry-1.0.0/src/scintillometry/visuals/plotting.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.0/src/scintillometry/wrangler/__init__.py
--rw-r--r--   0        0        0    34245 2020-02-02 00:00:00.000000 scintillometry-1.0.0/src/scintillometry/wrangler/data_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0    27741 2020-02-02 00:00:00.000000 scintillometry-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0     6652 2020-02-02 00:00:00.000000 scintillometry-1.0.0/tests/test_backend_constants.py
--rw-r--r--   0        0        0    28643 2020-02-02 00:00:00.000000 scintillometry-1.0.0/tests/test_backend_constructions.py
--rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 scintillometry-1.0.0/tests/test_backend_derivations.py
--rw-r--r--   0        0        0    12610 2020-02-02 00:00:00.000000 scintillometry-1.0.0/tests/test_backend_iterations.py
--rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 scintillometry-1.0.0/tests/test_backend_transects.py
--rw-r--r--   0        0        0    44923 2020-02-02 00:00:00.000000 scintillometry-1.0.0/tests/test_metrics_calculations.py
--rw-r--r--   0        0        0    31374 2020-02-02 00:00:00.000000 scintillometry-1.0.0/tests/test_visuals_plotting.py
--rw-r--r--   0        0        0    48531 2020-02-02 00:00:00.000000 scintillometry-1.0.0/tests/test_wrangler_data_parser.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 scintillometry-1.0.0/tests/test_data/test_data_v7_empty.mat
--rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 scintillometry-1.0.0/tests/test_data/test_data_v7_results.mat
--rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 scintillometry-1.0.0/LICENSE
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 scintillometry-1.0.0/README.md
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 scintillometry-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    22490 2020-02-02 00:00:00.000000 scintillometry-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/__init__.py
+-rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/backend/__init__.py
+-rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/backend/constants.py
+-rw-r--r--   0        0        0    25114 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/backend/constructions.py
+-rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/backend/derivations.py
+-rw-r--r--   0        0        0    15739 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/backend/iterations.py
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/backend/transects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/metrics/__init__.py
+-rwxr-xr-x   0        0        0    38541 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/metrics/calculations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/visuals/__init__.py
+-rw-r--r--   0        0        0    31290 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/visuals/plotting.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/wrangler/__init__.py
+-rw-r--r--   0        0        0    34239 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/wrangler/data_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0    27735 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_backend_constants.py
+-rw-r--r--   0        0        0    28637 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_backend_constructions.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_backend_derivations.py
+-rw-r--r--   0        0        0    12604 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_backend_iterations.py
+-rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_backend_transects.py
+-rw-r--r--   0        0        0    44917 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_metrics_calculations.py
+-rw-r--r--   0        0        0    31368 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_visuals_plotting.py
+-rw-r--r--   0        0        0    48525 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_wrangler_data_parser.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_data/test_data_v7_empty.mat
+-rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_data/test_data_v7_results.mat
+-rw-r--r--   0        0        0    10813 2020-02-02 00:00:00.000000 scintillometry-1.0.1/LICENSE
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 scintillometry-1.0.1/README.md
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 scintillometry-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    22589 2020-02-02 00:00:00.000000 scintillometry-1.0.1/PKG-INFO
```

### Comparing `scintillometry-1.0.0/src/scintillometry/main.py` & `scintillometry-1.0.1/src/scintillometry/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2023 Scintillometry Tools Contributors.
+"""Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/src/scintillometry/backend/constants.py` & `scintillometry-1.0.1/src/scintillometry/backend/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2019-2023 Scintillometry-Tools Contributors.
+"""Copyright 2019-2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/src/scintillometry/backend/constructions.py` & `scintillometry-1.0.1/src/scintillometry/backend/constructions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2019-2023 Scintillometry-Tools Contributors.
+"""Copyright 2019-2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/src/scintillometry/backend/derivations.py` & `scintillometry-1.0.1/src/scintillometry/backend/derivations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2019-2023 Scintillometry-Tools Contributors.
+"""Copyright 2019-2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/src/scintillometry/backend/iterations.py` & `scintillometry-1.0.1/src/scintillometry/backend/iterations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2019-2023 Scintillometry-Tools Contributors.
+"""Copyright 2019-2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/src/scintillometry/backend/transects.py` & `scintillometry-1.0.1/src/scintillometry/backend/transects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2019-2023 Scintillometry-Tools Contributors.
+"""Copyright 2019-2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/src/scintillometry/metrics/calculations.py` & `scintillometry-1.0.1/src/scintillometry/metrics/calculations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2023 Scintillometry-Tools Contributors.
+"""Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/src/scintillometry/visuals/plotting.py` & `scintillometry-1.0.1/src/scintillometry/visuals/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2023 Scintillometry-Tools Contributors.
+"""Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/src/scintillometry/wrangler/data_parser.py` & `scintillometry-1.0.1/src/scintillometry/wrangler/data_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2023 Scintillometry-Tools Contributors.
+"""Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/tests/conftest.py` & `scintillometry-1.0.1/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2023 Scintillometry-Tools Contributors.
+"""Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/tests/test_backend_constants.py` & `scintillometry-1.0.1/tests/test_backend_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2023 Scintillometry-Tools Contributors.
+"""Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/tests/test_backend_constructions.py` & `scintillometry-1.0.1/tests/test_backend_constructions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2023 Scintillometry-Tools Contributors.
+"""Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/tests/test_backend_derivations.py` & `scintillometry-1.0.1/tests/test_backend_derivations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2023 Scintillometry-Tools Contributors.
+"""Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/tests/test_backend_iterations.py` & `scintillometry-1.0.1/tests/test_backend_iterations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2023 Scintillometry-Tools Contributors.
+"""Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/tests/test_backend_transects.py` & `scintillometry-1.0.1/tests/test_backend_transects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2023 Scintillometry-Tools Contributors.
+"""Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/tests/test_metrics_calculations.py` & `scintillometry-1.0.1/tests/test_metrics_calculations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2023 Scintillometry-Tools Contributors.
+"""Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/tests/test_visuals_plotting.py` & `scintillometry-1.0.1/tests/test_visuals_plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2023 Scintillometry-Tools Contributors.
+"""Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/tests/test_wrangler_data_parser.py` & `scintillometry-1.0.1/tests/test_wrangler_data_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright 2023 Scintillometry-Tools Contributors.
+"""Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/tests/test_data/test_data_v7_results.mat` & `scintillometry-1.0.1/tests/test_data/test_data_v7_results.mat`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.0/LICENSE` & `scintillometry-1.0.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
    Copyright 2019-2023 Nicolas Gampierakis, Josef Zink,
-   Scintillometry-Tools Contributors
+   Scintillometry Contributors
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `scintillometry-1.0.0/README.md` & `scintillometry-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,47 @@
-<!-- Copyright 2023 Scintillometry-Tools Contributors.
+<!-- Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License. -->
 
-# Scintillometry Tools
+# Scintillometry
 
-[![Pytest and Flake8](https://github.com/gampnico/scintillometry-tools/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/gampnico/scintillometry-tools/actions/workflows/python-app.yml)
+[![Pytest and Flake8](https://github.com/gampnico/scintillometry/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/gampnico/scintillometry/actions/workflows/python-app.yml)
 
 Analyse data & 2D flux footprints from Scintec's BLS scintillometers.
 
-This package started life as part of a field course. If you spot any missing citations or licenses please [open an issue](https://github.com/gampnico/scintillometry-tools/issues).
+This package started life as part of a field course. If you spot any missing citations or licenses please [open an issue](https://github.com/gampnico/scintillometry/issues).
+
+Comprehensive documentation is available [via ReadTheDocs](https://scintillometry.readthedocs.io/en/latest/).
 
 # Processing Scintillometry Data in Complex Terrain
 
-Scintillometry-Tools is configured for scintillometer experiments in Austria using public or local data (ZAMG, InnFLUX), but is easily modified to work with other data sources. Note that external data sources may have different licensing constraints.
+*Scintillometry* is configured for scintillometer experiments in Austria using public or local data (ZAMG, InnFLUX), but is easily modified to work with other data sources. Note that external data sources may have different licensing constraints.
 
 The package is currently in alpha and may change or break often. Support is only available for Python 3.8+ on debian-based Linux distros.
 
 ## Installation
 
-Scintillometry-Tools supports package installation with pip, or from source as an editable with pip or conda. **Installing as an editable is recommended**, as it allows you to call command line arguments directly on the package instead of writing a frontend.
+*Scintillometry* supports package installation with pip, or from source as an editable with pip or conda. **Installing as an editable is recommended**, as it allows you to call command line arguments directly on the package instead of writing a frontend.
 
 ### Install from Source with Conda/Mamba
 
 Create or activate your preferred conda environment and run:
 
 ```bash
-git clone https://github.com/gampnico/scintillometry-tools.git
+git clone https://github.com/gampnico/scintillometry.git
 make install
 ```
 
 That's it!
 
 Install the package with optional dependencies:
 
@@ -61,15 +63,15 @@
 ```
 
 Note that this installation method does not provide documentation or a Makefile, and you cannot easily use the package from the command line.
 
 To install from source (recommended):
 
 ```bash
-git clone https://github.com/gampnico/scintillometry-tools.git
+git clone https://github.com/gampnico/scintillometry.git
 pip install -e .
 ```
 
 Install the package with optional dependencies:
 
 ```bash
 pip install -e .[tests]
@@ -150,28 +152,28 @@
 
 ### Make Things Simple
 
 If you installed from source, the provided Makefile has many uses. View all the available commands:
 
 ```bash
 make help       # display help for Makefile targets
-make commands   # display help for scintillometry-tools
+make commands   # display help for scintillometry
 ```
 
 ### Run from Terminal
 
 From the package root, pass arguments like so:
 
 ```bash
 src/scintillometry/main.py [-h] [-i <input_data>] [-p <path_data>] [-d] [...] [-v]
 ```
 
 ### Import as Package
 
-Scintillometry-Tools and its submodules can be imported as Python modules:
+*Scintillometry* and its submodules can be imported as Python modules:
 
 ```python
 from scintillometry.wrangler.data_parser import WranglerParsing
 
 parser = WranglerParsing()
 dataframe = parser.scintillometer.parse_scintillometer(file_path="./data.mnd")
 weather = parser.weather.parse_weather(file_path="./weather.csv")
```

### Comparing `scintillometry-1.0.0/pyproject.toml` & `scintillometry-1.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scintillometry"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
-  { name="Scintillometry-Tools Contributors", email="" },
+  { name="Scintillometry Contributors", email="" },
 ]
 description = "Analyse data & 2D flux footprints from Scintec's BLS scintillometers."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 4 - Beta",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Environment :: Console",
     "Topic :: Scientific/Engineering :: Atmospheric Science",
@@ -51,14 +51,15 @@
   "pylint >= 2.16.1",
   "flake8 >= 6.0",
   "black >= 23.1",
   "isort",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/gampnico/scintillometry-tools"
-"Bug Tracker" = "https://github.com/gampnico/scintillometry-tools/issues"
+"Homepage" = "https://github.com/gampnico/scintillometry"
+"Bug Tracker" = "https://github.com/gampnico/scintillometry/issues"
+"Documentation" = "https://scintillometry.readthedocs.io/en/latest/"
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
```

### Comparing `scintillometry-1.0.0/PKG-INFO` & `scintillometry-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: scintillometry
-Version: 1.0.0
+Version: 1.0.1
 Summary: Analyse data & 2D flux footprints from Scintec's BLS scintillometers.
-Project-URL: Homepage, https://github.com/gampnico/scintillometry-tools
-Project-URL: Bug Tracker, https://github.com/gampnico/scintillometry-tools/issues
-Author: Scintillometry-Tools Contributors
+Project-URL: Homepage, https://github.com/gampnico/scintillometry
+Project-URL: Bug Tracker, https://github.com/gampnico/scintillometry/issues
+Project-URL: Documentation, https://scintillometry.readthedocs.io/en/latest/
+Author: Scintillometry Contributors
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -179,29 +180,29 @@
               defend, and hold each Contributor harmless for any liability
               incurred by, or claims asserted against, such Contributor by reason
               of your accepting any such warranty or additional liability.
         
            END OF TERMS AND CONDITIONS
         
            Copyright 2019-2023 Nicolas Gampierakis, Josef Zink,
-           Scintillometry-Tools Contributors
+           Scintillometry Contributors
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
 License-File: LICENSE
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -228,52 +229,54 @@
 Requires-Dist: sphinx-rtd-theme>=1.1; extra == 'docs'
 Provides-Extra: tests
 Requires-Dist: coverage>=7.1; extra == 'tests'
 Requires-Dist: pytest-dependency>=0.5; extra == 'tests'
 Requires-Dist: pytest>=7.0; extra == 'tests'
 Description-Content-Type: text/markdown
 
-<!-- Copyright 2023 Scintillometry-Tools Contributors.
+<!-- Copyright 2023 Scintillometry Contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License. -->
 
-# Scintillometry Tools
+# Scintillometry
 
-[![Pytest and Flake8](https://github.com/gampnico/scintillometry-tools/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/gampnico/scintillometry-tools/actions/workflows/python-app.yml)
+[![Pytest and Flake8](https://github.com/gampnico/scintillometry/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/gampnico/scintillometry/actions/workflows/python-app.yml)
 
 Analyse data & 2D flux footprints from Scintec's BLS scintillometers.
 
-This package started life as part of a field course. If you spot any missing citations or licenses please [open an issue](https://github.com/gampnico/scintillometry-tools/issues).
+This package started life as part of a field course. If you spot any missing citations or licenses please [open an issue](https://github.com/gampnico/scintillometry/issues).
+
+Comprehensive documentation is available [via ReadTheDocs](https://scintillometry.readthedocs.io/en/latest/).
 
 # Processing Scintillometry Data in Complex Terrain
 
-Scintillometry-Tools is configured for scintillometer experiments in Austria using public or local data (ZAMG, InnFLUX), but is easily modified to work with other data sources. Note that external data sources may have different licensing constraints.
+*Scintillometry* is configured for scintillometer experiments in Austria using public or local data (ZAMG, InnFLUX), but is easily modified to work with other data sources. Note that external data sources may have different licensing constraints.
 
 The package is currently in alpha and may change or break often. Support is only available for Python 3.8+ on debian-based Linux distros.
 
 ## Installation
 
-Scintillometry-Tools supports package installation with pip, or from source as an editable with pip or conda. **Installing as an editable is recommended**, as it allows you to call command line arguments directly on the package instead of writing a frontend.
+*Scintillometry* supports package installation with pip, or from source as an editable with pip or conda. **Installing as an editable is recommended**, as it allows you to call command line arguments directly on the package instead of writing a frontend.
 
 ### Install from Source with Conda/Mamba
 
 Create or activate your preferred conda environment and run:
 
 ```bash
-git clone https://github.com/gampnico/scintillometry-tools.git
+git clone https://github.com/gampnico/scintillometry.git
 make install
 ```
 
 That's it!
 
 Install the package with optional dependencies:
 
@@ -295,15 +298,15 @@
 ```
 
 Note that this installation method does not provide documentation or a Makefile, and you cannot easily use the package from the command line.
 
 To install from source (recommended):
 
 ```bash
-git clone https://github.com/gampnico/scintillometry-tools.git
+git clone https://github.com/gampnico/scintillometry.git
 pip install -e .
 ```
 
 Install the package with optional dependencies:
 
 ```bash
 pip install -e .[tests]
@@ -384,28 +387,28 @@
 
 ### Make Things Simple
 
 If you installed from source, the provided Makefile has many uses. View all the available commands:
 
 ```bash
 make help       # display help for Makefile targets
-make commands   # display help for scintillometry-tools
+make commands   # display help for scintillometry
 ```
 
 ### Run from Terminal
 
 From the package root, pass arguments like so:
 
 ```bash
 src/scintillometry/main.py [-h] [-i <input_data>] [-p <path_data>] [-d] [...] [-v]
 ```
 
 ### Import as Package
 
-Scintillometry-Tools and its submodules can be imported as Python modules:
+*Scintillometry* and its submodules can be imported as Python modules:
 
 ```python
 from scintillometry.wrangler.data_parser import WranglerParsing
 
 parser = WranglerParsing()
 dataframe = parser.scintillometer.parse_scintillometer(file_path="./data.mnd")
 weather = parser.weather.parse_weather(file_path="./weather.csv")
```

