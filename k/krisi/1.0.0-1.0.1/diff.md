# Comparing `tmp/krisi-1.0.0.tar.gz` & `tmp/krisi-1.0.1.tar.gz`

## Comparing `krisi-1.0.0.tar` & `krisi-1.0.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-1.0.0/.flake8
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-1.0.0/.isort.cfg
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 krisi-1.0.0/mkdocs.yaml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-1.0.0/.vscode/launch.json
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 krisi-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 krisi-1.0.0/dev_utils/generate_from_examples.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 krisi-1.0.0/dev_utils/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/analyse/__init__.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/analyse/correlations.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/analyse/dataset.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/analyse/utils.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/evaluate/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/evaluate/assertions.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/evaluate/compare.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/evaluate/group.py
--rw-r--r--   0        0        0     8367 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/evaluate/metric.py
--rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/evaluate/score.py
--rw-r--r--   0        0        0    21324 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/evaluate/scorecard.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/evaluate/type.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/evaluate/utils.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/evaluate/library/__init__.py
--rw-r--r--   0        0        0     6642 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/evaluate/library/default_metrics_classification.py
--rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/evaluate/library/default_metrics_regression.py
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/evaluate/library/diagrams.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/evaluate/library/metric_wrappers.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/report/__init__.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/report/console.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/report/graph.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/report/interactive.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/report/pdf.py
--rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/report/report.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/report/type.py
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/report/vizualise.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/report/library/console/diagrams.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/report/library/pdf_layouts/scorecard/report.css
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/report/library/pdf_layouts/scorecard/report.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/utils/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/utils/console_plot.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/utils/data.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/utils/environment.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/utils/io.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/utils/iterable_helpers.py
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/utils/printing.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 krisi-1.0.0/src/krisi/utils/devutils/timing.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-1.0.0/.gitignore
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-1.0.0/LICENSE
--rw-r--r--   0        0        0    61743 2020-02-02 00:00:00.000000 krisi-1.0.0/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 krisi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    66529 2020-02-02 00:00:00.000000 krisi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-1.0.1/.flake8
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-1.0.1/.isort.cfg
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 krisi-1.0.1/mkdocs.yaml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-1.0.1/.vscode/launch.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 krisi-1.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 krisi-1.0.1/dev_utils/generate_from_examples.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 krisi-1.0.1/dev_utils/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/analyse/__init__.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/analyse/correlations.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/analyse/dataset.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/analyse/utils.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/assertions.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/compare.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/group.py
+-rw-r--r--   0        0        0     8367 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/metric.py
+-rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/score.py
+-rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/scorecard.py
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/type.py
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/utils.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/library/__init__.py
+-rw-r--r--   0        0        0     6642 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/library/default_metrics_classification.py
+-rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/library/default_metrics_regression.py
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/library/diagrams.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/library/metric_wrappers.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/__init__.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/console.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/graph.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/interactive.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/pdf.py
+-rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/report.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/type.py
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/vizualise.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/library/console/diagrams.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/library/pdf_layouts/scorecard/report.css
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/library/pdf_layouts/scorecard/report.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/console_plot.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/data.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/environment.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/io.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/iterable_helpers.py
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/printing.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/devutils/timing.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-1.0.1/.gitignore
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-1.0.1/LICENSE
+-rw-r--r--   0        0        0    61743 2020-02-02 00:00:00.000000 krisi-1.0.1/README.md
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 krisi-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    66529 2020-02-02 00:00:00.000000 krisi-1.0.1/PKG-INFO
```

### Comparing `krisi-1.0.0/mkdocs.yaml` & `krisi-1.0.1/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/.vscode/settings.json` & `krisi-1.0.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/analyse/correlations.py` & `krisi-1.0.1/src/krisi/analyse/correlations.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/analyse/dataset.py` & `krisi-1.0.1/src/krisi/analyse/dataset.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/evaluate/assertions.py` & `krisi-1.0.1/src/krisi/evaluate/assertions.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/evaluate/compare.py` & `krisi-1.0.1/src/krisi/evaluate/compare.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/evaluate/group.py` & `krisi-1.0.1/src/krisi/evaluate/group.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/evaluate/metric.py` & `krisi-1.0.1/src/krisi/evaluate/metric.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/evaluate/score.py` & `krisi-1.0.1/src/krisi/evaluate/score.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/evaluate/scorecard.py` & `krisi-1.0.1/src/krisi/evaluate/scorecard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import datetime
 import os
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Union
 
 import pandas as pd
-from IPython.display import display
 from rich import print
 from typing_extensions import Literal
 
 from krisi.evaluate.assertions import (
     check_valid_pred_target,
     is_dataset_classification_like,
 )
@@ -486,14 +485,16 @@
                 )
 
             elif mode is PrintMode.minimal:
                 to_display = get_minimal_summary(self, dataframe=frame_or_series)
             elif mode is PrintMode.minimal_table:
                 to_display = get_large_metric_summary(self, title)
             if isinstance(to_display, (pd.DataFrame, pd.Series)) and is_notebook():
+                from IPython.display import display
+
                 display(to_display)
             else:
                 print(to_display)
 
     def save(
         self,
         with_info: bool = False,
```

### Comparing `krisi-1.0.0/src/krisi/evaluate/type.py` & `krisi-1.0.1/src/krisi/evaluate/type.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/evaluate/utils.py` & `krisi-1.0.1/src/krisi/evaluate/utils.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/evaluate/library/default_metrics_classification.py` & `krisi-1.0.1/src/krisi/evaluate/library/default_metrics_classification.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/evaluate/library/default_metrics_regression.py` & `krisi-1.0.1/src/krisi/evaluate/library/default_metrics_regression.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/evaluate/library/diagrams.py` & `krisi-1.0.1/src/krisi/evaluate/library/diagrams.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/evaluate/library/metric_wrappers.py` & `krisi-1.0.1/src/krisi/evaluate/library/metric_wrappers.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/report/console.py` & `krisi-1.0.1/src/krisi/report/console.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/report/graph.py` & `krisi-1.0.1/src/krisi/report/graph.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/report/interactive.py` & `krisi-1.0.1/src/krisi/report/interactive.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/report/pdf.py` & `krisi-1.0.1/src/krisi/report/pdf.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/report/report.py` & `krisi-1.0.1/src/krisi/report/report.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/report/type.py` & `krisi-1.0.1/src/krisi/report/type.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/report/vizualise.py` & `krisi-1.0.1/src/krisi/report/vizualise.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/report/library/console/diagrams.py` & `krisi-1.0.1/src/krisi/report/library/console/diagrams.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/report/library/pdf_layouts/scorecard/report.css` & `krisi-1.0.1/src/krisi/report/library/pdf_layouts/scorecard/report.css`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/report/library/pdf_layouts/scorecard/report.html` & `krisi-1.0.1/src/krisi/report/library/pdf_layouts/scorecard/report.html`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/utils/console_plot.py` & `krisi-1.0.1/src/krisi/utils/console_plot.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/utils/data.py` & `krisi-1.0.1/src/krisi/utils/data.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/utils/environment.py` & `krisi-1.0.1/src/krisi/utils/environment.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/utils/io.py` & `krisi-1.0.1/src/krisi/utils/io.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/utils/iterable_helpers.py` & `krisi-1.0.1/src/krisi/utils/iterable_helpers.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/utils/printing.py` & `krisi-1.0.1/src/krisi/utils/printing.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/src/krisi/utils/devutils/timing.py` & `krisi-1.0.1/src/krisi/utils/devutils/timing.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/.gitignore` & `krisi-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/LICENSE` & `krisi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/README.md` & `krisi-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `krisi-1.0.0/pyproject.toml` & `krisi-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "krisi"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Mark Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 description = "Testing and Reporting framework for Time Series Analysis"
 readme = "README.md"
 license = { file="LICENSE" }
@@ -135,15 +135,15 @@
   "src",
   ".",
 ]
 testpaths = ["tests"] 
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `krisi-1.0.0/PKG-INFO` & `krisi-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krisi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Testing and Reporting framework for Time Series Analysis
 Project-URL: Documentation, https://dream-faster.github.io/krisi
 Project-URL: Issues, https://github.com/dream-faster/krisi/issues
 Project-URL: Source, https://github.com/dream-faster/krisi
 Author-email: Mark Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License: MIT License
```

