# Comparing `tmp/prosimos-0.1.2.tar.gz` & `tmp/prosimos-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosimos-0.1.2.tar", max compression
+gzip compressed data, was "prosimos-1.2.3.tar", max compression
```

## Comparing `prosimos-0.1.2.tar` & `prosimos-1.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    14755 2023-05-10 17:42:38.843014 prosimos-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-12 15:53:47.578329 prosimos-0.1.2/bpdfr_discovery/__init__.py
--rw-r--r--   0        0        0     3478 2023-05-12 15:53:11.408033 prosimos-0.1.2/bpdfr_discovery/emd_metric.py
--rw-r--r--   0        0        0      489 2023-05-12 15:53:11.416500 prosimos-0.1.2/bpdfr_discovery/exceptions.py
--rw-r--r--   0        0        0     7248 2023-05-12 15:53:11.417547 prosimos-0.1.2/bpdfr_discovery/inter_arrival_cases_discovery.py
--rw-r--r--   0        0        0     5615 2023-05-12 15:54:39.777533 prosimos-0.1.2/bpdfr_discovery/log_comparison_metrics.py
--rw-r--r--   0        0        0    44018 2023-05-12 15:54:39.055764 prosimos-0.1.2/bpdfr_discovery/log_parser.py
--rw-r--r--   0        0        0        0 2023-05-12 15:21:53.261500 prosimos-0.1.2/cli/__init__.py
--rw-r--r--   0        0        0     3532 2023-05-12 15:54:39.055639 prosimos-0.1.2/cli/diff_res_bpsim.py
--rw-r--r--   0        0        0        0 2023-05-12 14:42:35.119495 prosimos-0.1.2/prosimos/__init__.py
--rw-r--r--   0        0        0    44562 2023-05-12 15:54:39.771171 prosimos-0.1.2/prosimos/batch_processing.py
--rw-r--r--   0        0        0     4383 2023-05-12 15:54:39.748936 prosimos-0.1.2/prosimos/batch_processing_parser.py
--rw-r--r--   0        0        0     2626 2023-05-12 15:54:39.771056 prosimos-0.1.2/prosimos/case_attributes.py
--rw-r--r--   0        0        0    48440 2023-05-12 15:54:39.748605 prosimos-0.1.2/prosimos/control_flow_manager.py
--rw-r--r--   0        0        0      487 2023-01-16 17:13:52.476673 prosimos-0.1.2/prosimos/exceptions.py
--rw-r--r--   0        0        0     7340 2023-05-12 15:54:39.749123 prosimos-0.1.2/prosimos/execution_info.py
--rw-r--r--   0        0        0     1109 2023-01-16 17:13:52.479840 prosimos-0.1.2/prosimos/file_manager.py
--rw-r--r--   0        0        0     3147 2023-05-12 15:54:39.748829 prosimos-0.1.2/prosimos/prioritisation.py
--rw-r--r--   0        0        0     1345 2023-05-12 15:54:39.771402 prosimos-0.1.2/prosimos/prioritisation_parser.py
--rw-r--r--   0        0        0     3009 2023-02-17 14:22:25.714177 prosimos-0.1.2/prosimos/prioritisation_rules.py
--rw-r--r--   0        0        0     8585 2023-05-09 14:34:59.262677 prosimos-0.1.2/prosimos/probability_distributions.py
--rw-r--r--   0        0        0    41729 2023-03-01 09:12:49.498726 prosimos-0.1.2/prosimos/resource_calendar.py
--rw-r--r--   0        0        0      467 2022-06-22 13:20:27.228747 prosimos-0.1.2/prosimos/resource_profile.py
--rw-r--r--   0        0        0    28588 2023-05-12 15:54:39.777377 prosimos-0.1.2/prosimos/simulation_engine.py
--rw-r--r--   0        0        0    22058 2023-05-12 15:54:39.776857 prosimos-0.1.2/prosimos/simulation_properties_parser.py
--rw-r--r--   0        0        0     6298 2023-02-17 14:22:25.717592 prosimos-0.1.2/prosimos/simulation_queues_ds.py
--rw-r--r--   0        0        0     6003 2023-05-12 15:54:39.748484 prosimos-0.1.2/prosimos/simulation_setup.py
--rw-r--r--   0        0        0    15565 2023-05-12 15:54:39.748727 prosimos-0.1.2/prosimos/simulation_stats.py
--rw-r--r--   0        0        0    14157 2023-05-12 15:54:38.365343 prosimos-0.1.2/prosimos/simulation_stats_calculator.py
--rw-r--r--   0        0        0     1714 2023-05-12 15:54:39.055703 prosimos-0.1.2/prosimos/weekday_helper.py
--rw-r--r--   0        0        0      612 2023-05-12 16:09:04.392646 prosimos-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    15464 1970-01-01 00:00:00.000000 prosimos-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    14755 2023-05-15 07:00:12.329363 prosimos-1.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 07:00:12.345364 prosimos-1.2.3/bpdfr_discovery/__init__.py
+-rw-r--r--   0        0        0     3478 2023-05-15 07:00:12.345364 prosimos-1.2.3/bpdfr_discovery/emd_metric.py
+-rw-r--r--   0        0        0      489 2023-05-15 07:00:12.345364 prosimos-1.2.3/bpdfr_discovery/exceptions.py
+-rw-r--r--   0        0        0     7248 2023-05-15 07:00:12.345364 prosimos-1.2.3/bpdfr_discovery/inter_arrival_cases_discovery.py
+-rw-r--r--   0        0        0     5615 2023-05-15 07:00:12.345364 prosimos-1.2.3/bpdfr_discovery/log_comparison_metrics.py
+-rw-r--r--   0        0        0    44018 2023-05-15 07:00:12.345364 prosimos-1.2.3/bpdfr_discovery/log_parser.py
+-rw-r--r--   0        0        0        0 2023-05-15 07:00:12.345364 prosimos-1.2.3/cli/__init__.py
+-rw-r--r--   0        0        0     3539 2023-05-15 07:00:12.345364 prosimos-1.2.3/cli/diff_res_bpsim.py
+-rw-r--r--   0        0        0        0 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/__init__.py
+-rw-r--r--   0        0        0    44562 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/batch_processing.py
+-rw-r--r--   0        0        0     4383 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/batch_processing_parser.py
+-rw-r--r--   0        0        0     2626 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/case_attributes.py
+-rw-r--r--   0        0        0    48440 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/control_flow_manager.py
+-rw-r--r--   0        0        0      487 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/exceptions.py
+-rw-r--r--   0        0        0     7340 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/execution_info.py
+-rw-r--r--   0        0        0     1109 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/file_manager.py
+-rw-r--r--   0        0        0     3147 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/prioritisation.py
+-rw-r--r--   0        0        0     1345 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/prioritisation_parser.py
+-rw-r--r--   0        0        0     3009 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/prioritisation_rules.py
+-rw-r--r--   0        0        0     8585 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/probability_distributions.py
+-rw-r--r--   0        0        0    41729 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/resource_calendar.py
+-rw-r--r--   0        0        0      467 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/resource_profile.py
+-rw-r--r--   0        0        0    28588 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/simulation_engine.py
+-rw-r--r--   0        0        0    22058 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/simulation_properties_parser.py
+-rw-r--r--   0        0        0     6298 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/simulation_queues_ds.py
+-rw-r--r--   0        0        0     6003 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/simulation_setup.py
+-rw-r--r--   0        0        0    15565 2023-05-15 07:00:12.453369 prosimos-1.2.3/prosimos/simulation_stats.py
+-rw-r--r--   0        0        0    14157 2023-05-15 07:00:12.453369 prosimos-1.2.3/prosimos/simulation_stats_calculator.py
+-rw-r--r--   0        0        0     1714 2023-05-15 07:00:12.453369 prosimos-1.2.3/prosimos/weekday_helper.py
+-rw-r--r--   0        0        0      612 2023-05-15 07:00:12.453369 prosimos-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0    15464 1970-01-01 00:00:00.000000 prosimos-1.2.3/PKG-INFO
```

### Comparing `prosimos-0.1.2/README.md` & `prosimos-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/bpdfr_discovery/emd_metric.py` & `prosimos-1.2.3/bpdfr_discovery/emd_metric.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/bpdfr_discovery/inter_arrival_cases_discovery.py` & `prosimos-1.2.3/bpdfr_discovery/inter_arrival_cases_discovery.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/bpdfr_discovery/log_comparison_metrics.py` & `prosimos-1.2.3/bpdfr_discovery/log_comparison_metrics.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/bpdfr_discovery/log_parser.py` & `prosimos-1.2.3/bpdfr_discovery/log_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/cli/diff_res_bpsim.py` & `prosimos-1.2.3/cli/diff_res_bpsim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import csv
 import os
 from pathlib import Path
 
 import click
 
-from prosimos.log_parser import preprocess_xes_log
+from bpdfr_discovery.log_parser import preprocess_xes_log
 from prosimos.simulation_engine import run_simulation
 from prosimos.simulation_setup import SimDiffSetup
 
 
 @click.group()
 def cli():
     pass
```

### Comparing `prosimos-0.1.2/prosimos/batch_processing.py` & `prosimos-1.2.3/prosimos/batch_processing.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/batch_processing_parser.py` & `prosimos-1.2.3/prosimos/batch_processing_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/case_attributes.py` & `prosimos-1.2.3/prosimos/case_attributes.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/control_flow_manager.py` & `prosimos-1.2.3/prosimos/control_flow_manager.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/execution_info.py` & `prosimos-1.2.3/prosimos/execution_info.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/file_manager.py` & `prosimos-1.2.3/prosimos/file_manager.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/prioritisation.py` & `prosimos-1.2.3/prosimos/prioritisation.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/prioritisation_parser.py` & `prosimos-1.2.3/prosimos/prioritisation_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/prioritisation_rules.py` & `prosimos-1.2.3/prosimos/prioritisation_rules.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/probability_distributions.py` & `prosimos-1.2.3/prosimos/probability_distributions.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/resource_calendar.py` & `prosimos-1.2.3/prosimos/resource_calendar.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/simulation_engine.py` & `prosimos-1.2.3/prosimos/simulation_engine.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/simulation_properties_parser.py` & `prosimos-1.2.3/prosimos/simulation_properties_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/simulation_queues_ds.py` & `prosimos-1.2.3/prosimos/simulation_queues_ds.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/simulation_setup.py` & `prosimos-1.2.3/prosimos/simulation_setup.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/simulation_stats.py` & `prosimos-1.2.3/prosimos/simulation_stats.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/simulation_stats_calculator.py` & `prosimos-1.2.3/prosimos/simulation_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/prosimos/weekday_helper.py` & `prosimos-1.2.3/prosimos/weekday_helper.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.2/pyproject.toml` & `prosimos-1.2.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prosimos"
-version = "0.1.2"
+version = "1.2.3"
 description = ""
 authors = ["Iryna Halenok, Orlenys López Pintado"]
 readme = "README.md"
 packages = [
     {include = "cli"},
     {include = "prosimos"},
     {include = "bpdfr_discovery"}
```

### Comparing `prosimos-0.1.2/PKG-INFO` & `prosimos-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosimos
-Version: 0.1.2
+Version: 1.2.3
 Summary: 
 Author: Iryna Halenok, Orlenys López Pintado
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

