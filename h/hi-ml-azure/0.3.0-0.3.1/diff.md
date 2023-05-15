# Comparing `tmp/hi-ml-azure-0.3.0.tar.gz` & `tmp/hi-ml-azure-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hi-ml-azure-0.3.0.tar", last modified: Fri May  5 17:32:48 2023, max compression
+gzip compressed data, was "dist/hi-ml-azure-0.3.1.tar", last modified: Mon May 15 10:15:22 2023, max compression
```

## Comparing `hi-ml-azure-0.3.0.tar` & `hi-ml-azure-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/package_description.md
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/run_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/health_azure/
--rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4174 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/amulet.py
--rw-r--r--   0 runner    (1001) docker     (122)    20546 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/argparsing.py
--rw-r--r--   0 runner    (1001) docker     (122)    30389 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/health_azure/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1323 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/examples/elevate_this.py
--rw-r--r--   0 runner    (1001) docker     (122)    61721 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/himl.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2115 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/himl_download.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5570 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/himl_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     5550 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     1825 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/mlflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/package_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2884 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/paths.py
--rw-r--r--   0 runner    (1001) docker     (122)    11400 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/traverse.py
--rw-r--r--   0 runner    (1001) docker     (122)    95134 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:15:22.000000 hi-ml-azure-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-05-15 10:15:22.000000 hi-ml-azure-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/package_description.md
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/run_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 10:15:22.000000 hi-ml-azure-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:15:22.000000 hi-ml-azure-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:15:22.000000 hi-ml-azure-0.3.1/src/health_azure/
+-rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/src/health_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4174 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/src/health_azure/amulet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20546 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/src/health_azure/argparsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30389 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/src/health_azure/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:15:22.000000 hi-ml-azure-0.3.1/src/health_azure/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     1323 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/src/health_azure/examples/elevate_this.py
+-rw-r--r--   0 runner    (1001) docker     (122)    62003 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/src/health_azure/himl.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2115 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/src/health_azure/himl_download.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5570 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/src/health_azure/himl_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5550 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/src/health_azure/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1825 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/src/health_azure/mlflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/src/health_azure/package_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2884 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/src/health_azure/paths.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11400 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/src/health_azure/traverse.py
+-rw-r--r--   0 runner    (1001) docker     (122)    95140 2023-05-15 10:15:01.000000 hi-ml-azure-0.3.1/src/health_azure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:15:22.000000 hi-ml-azure-0.3.1/src/hi_ml_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-05-15 10:15:21.000000 hi-ml-azure-0.3.1/src/hi_ml_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-05-15 10:15:21.000000 hi-ml-azure-0.3.1/src/hi_ml_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 10:15:21.000000 hi-ml-azure-0.3.1/src/hi_ml_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-15 10:15:21.000000 hi-ml-azure-0.3.1/src/hi_ml_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-05-15 10:15:21.000000 hi-ml-azure-0.3.1/src/hi_ml_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-15 10:15:21.000000 hi-ml-azure-0.3.1/src/hi_ml_azure.egg-info/top_level.txt
```

### Comparing `hi-ml-azure-0.3.0/LICENSE` & `hi-ml-azure-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/PKG-INFO` & `hi-ml-azure-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml-azure
-Version: 0.3.0
+Version: 0.3.1
 Summary: Microsoft Health Futures package to elevate and monitor scripts to an AzureML workspace
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Description: # Microsoft Health Intelligence Machine Learning Azure Toolbox
```

### Comparing `hi-ml-azure-0.3.0/package_description.md` & `hi-ml-azure-0.3.1/package_description.md`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/setup.py` & `hi-ml-azure-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/src/health_azure/__init__.py` & `hi-ml-azure-0.3.1/src/health_azure/__init__.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/src/health_azure/amulet.py` & `hi-ml-azure-0.3.1/src/health_azure/amulet.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/src/health_azure/argparsing.py` & `hi-ml-azure-0.3.1/src/health_azure/argparsing.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/src/health_azure/datasets.py` & `hi-ml-azure-0.3.1/src/health_azure/datasets.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/src/health_azure/examples/elevate_this.py` & `hi-ml-azure-0.3.1/src/health_azure/examples/elevate_this.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/src/health_azure/himl.py` & `hi-ml-azure-0.3.1/src/health_azure/himl.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,14 +440,15 @@
     assert cleaned_value is not None, "Expecting an actual string"
     return cleaned_value
 
 
 def submit_run_v2(
     workspace: Optional[Workspace],
     environment: EnvironmentV2,
+    environment_variables: Optional[Dict[str, str]] = None,
     experiment_name: Optional[str] = None,
     input_datasets_v2: Optional[Dict[str, Input]] = None,
     output_datasets_v2: Optional[Dict[str, Output]] = None,
     snapshot_root_directory: Optional[Path] = None,
     entry_script: Optional[PathOrString] = None,
     script_params: Optional[List[str]] = None,
     compute_target: Optional[str] = None,
@@ -463,14 +464,15 @@
     display_name: Optional[str] = None,
 ) -> Job:
     """
     Starts a v2 AML Job on a given workspace by submitting a command
 
     :param workspace: The AzureML workspace to use.
     :param environment: An AML v2 Environment object.
+    :param environment_variables: The environment variables that should be set when running in AzureML.
     :param experiment_name: The name of the experiment that will be used or created. If the experiment name contains
         characters that are not valid in Azure, those will be removed.
     :param input_datasets_v2: An optional dictionary of Inputs to pass in to the command.
     :param output_datasets_v2: An optional dictionary of Outputs to pass in to the command.
     :param snapshot_root_directory: The directory that contains all code that should be packaged and sent to AzureML.
         All Python code that the script uses must be copied over.
     :param entry_script: The script that should be run in AzureML.
@@ -543,14 +545,15 @@
             distribution = PyTorchDistribution(process_count_per_instance=pytorch_processes_per_node)
         return command(
             code=str(snapshot_root_directory),
             command=cmd,
             inputs=input_datasets_v2,
             outputs=output_datasets_v2,
             environment=environment.name + "@latest",
+            environment_variables=environment_variables,
             compute=compute_target,
             experiment_name=experiment_name,
             tags=tags or {},
             shm_size=docker_shm_size,
             display_name=display_name,
             instance_count=num_nodes,
             distribution=distribution,
@@ -991,14 +994,15 @@
 
             job = submit_run_v2(
                 workspace=workspace,
                 input_datasets_v2=input_datasets_v2,
                 output_datasets_v2=output_datasets_v2,
                 experiment_name=experiment_name,
                 environment=registered_env,
+                environment_variables=environment_variables,
                 snapshot_root_directory=snapshot_root_directory,
                 entry_script=entry_script,
                 script_params=script_params,
                 compute_target=compute_cluster_name,
                 tags=tags,
                 display_name=display_name,
                 docker_shm_size=docker_shm_size,
```

### Comparing `hi-ml-azure-0.3.0/src/health_azure/himl_download.py` & `hi-ml-azure-0.3.1/src/health_azure/himl_download.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/src/health_azure/himl_tensorboard.py` & `hi-ml-azure-0.3.1/src/health_azure/himl_tensorboard.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/src/health_azure/logging.py` & `hi-ml-azure-0.3.1/src/health_azure/logging.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/src/health_azure/mlflow_utils.py` & `hi-ml-azure-0.3.1/src/health_azure/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/src/health_azure/package_setup.py` & `hi-ml-azure-0.3.1/src/health_azure/package_setup.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/src/health_azure/paths.py` & `hi-ml-azure-0.3.1/src/health_azure/paths.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/src/health_azure/traverse.py` & `hi-ml-azure-0.3.1/src/health_azure/traverse.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.0/src/health_azure/utils.py` & `hi-ml-azure-0.3.1/src/health_azure/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -468,24 +468,24 @@
     if not value and not allow_missing:
         raise ValueError(f"There is no value stored for the secret named '{name}'")
     return value
 
 
 def to_azure_friendly_string(x: Optional[str]) -> Optional[str]:
     """
-    Given a string, ensure it can be used in Azure by replacing everything apart from a-z, A-Z, 0-9, or _ with _,
+    Given a string, ensure it can be used in Azure by replacing everything apart from a-z, A-Z, 0-9, - or _ with _,
     and replace multiple _ with a single _.
 
     :param x: Optional string to be converted.
     :return: Converted string, if one supplied. None otherwise.
     """
     if x is None:
         return x
     else:
-        return re.sub("_+", "_", re.sub(r"\W+", "_", x))
+        return re.sub("_+", "_", re.sub(r"[^\w-]+", "_", x))
 
 
 def _log_conda_dependencies_stats(conda: CondaDependencies, message_prefix: str) -> None:
     """
     Write number of conda and pip packages to logs.
 
     :param conda: A conda dependencies object
```

### Comparing `hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/PKG-INFO` & `hi-ml-azure-0.3.1/src/hi_ml_azure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml-azure
-Version: 0.3.0
+Version: 0.3.1
 Summary: Microsoft Health Futures package to elevate and monitor scripts to an AzureML workspace
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Description: # Microsoft Health Intelligence Machine Learning Azure Toolbox
```

### Comparing `hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/SOURCES.txt` & `hi-ml-azure-0.3.1/src/hi_ml_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

