# Comparing `tmp/airlift-0.1.1.tar.gz` & `tmp/airlift-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airlift-0.1.1.tar", max compression
+gzip compressed data, was "airlift-0.1.2.tar", max compression
```

## Comparing `airlift-0.1.1.tar` & `airlift-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0     1062 2023-05-14 19:34:47.096484 airlift-0.1.1/LICENSE
--rw-r--r--   0        0        0     6286 2023-05-14 19:34:47.096484 airlift-0.1.1/README.md
--rw-r--r--   0        0        0      673 2023-05-14 19:34:47.108484 airlift-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/__init__.py
--rw-r--r--   0        0        0     1364 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/check.py
--rw-r--r--   0        0        0     1033 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/import_variables.py
--rw-r--r--   0        0        0      939 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/pause.py
--rw-r--r--   0        0        0     1161 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/remove.py
--rw-r--r--   0        0        0      826 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/run_dag.py
--rw-r--r--   0        0        0     6709 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/start.py
--rw-r--r--   0        0        0      896 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/status.py
--rw-r--r--   0        0        0        0 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/config/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/config/airlift/config.yaml
--rw-r--r--   0        0        0       71 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/config/airlift/required_software.yaml
--rw-r--r--   0        0        0      979 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/config/config.py
--rw-r--r--   0        0        0      176 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/config/docker/Dockerfile
--rw-r--r--   0        0        0        0 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/config/docker/final/.gitkeep
--rw-r--r--   0        0        0     1089 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/config/helm/final_values.yaml
--rw-r--r--   0        0        0     1482 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/config/helm/values.yaml
--rw-r--r--   0        0        0      975 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/config/kind/cluster.yaml
--rw-r--r--   0        0        0     3599 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/main.py
--rw-r--r--   0        0        0        0 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/__init__.py
--rw-r--r--   0        0        0     3676 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/airflow.py
--rw-r--r--   0        0        0      767 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/airlift.py
--rw-r--r--   0        0        0      677 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/command.py
--rw-r--r--   0        0        0     1989 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/docker.py
--rw-r--r--   0        0        0     3087 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/file.py
--rw-r--r--   0        0        0     1606 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/helm.py
--rw-r--r--   0        0        0     2306 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/kind.py
--rw-r--r--   0        0        0      815 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/kubernetes.py
--rw-r--r--   0        0        0     7020 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/parser.py
--rw-r--r--   0        0        0     7029 1970-01-01 00:00:00.000000 airlift-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-15 17:57:39.104413 airlift-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6509 2023-05-15 17:57:39.104413 airlift-0.1.2/README.md
+-rw-r--r--   0        0        0      673 2023-05-15 17:57:39.116413 airlift-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/__init__.py
+-rw-r--r--   0        0        0     1364 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/check.py
+-rw-r--r--   0        0        0     1033 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/import_variables.py
+-rw-r--r--   0        0        0      939 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/pause.py
+-rw-r--r--   0        0        0     1161 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/remove.py
+-rw-r--r--   0        0        0     1146 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/run_dag.py
+-rw-r--r--   0        0        0     6709 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/start.py
+-rw-r--r--   0        0        0     1179 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/status.py
+-rw-r--r--   0        0        0        0 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/airlift/config.yaml
+-rw-r--r--   0        0        0       71 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/airlift/required_software.yaml
+-rw-r--r--   0        0        0      979 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/config.py
+-rw-r--r--   0        0        0      176 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/docker/Dockerfile
+-rw-r--r--   0        0        0        0 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/docker/final/.gitkeep
+-rw-r--r--   0        0        0     1482 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/helm/values.yaml
+-rw-r--r--   0        0        0      975 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/kind/cluster.yaml
+-rw-r--r--   0        0        0     3600 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/main.py
+-rw-r--r--   0        0        0        0 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/__init__.py
+-rw-r--r--   0        0        0     3676 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/airflow.py
+-rw-r--r--   0        0        0      767 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/airlift.py
+-rw-r--r--   0        0        0      677 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/command.py
+-rw-r--r--   0        0        0     1989 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/docker.py
+-rw-r--r--   0        0        0     3087 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/file.py
+-rw-r--r--   0        0        0     1606 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/helm.py
+-rw-r--r--   0        0        0     2306 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/kind.py
+-rw-r--r--   0        0        0      815 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/kubernetes.py
+-rw-r--r--   0        0        0     8439 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/parser.py
+-rw-r--r--   0        0        0     7252 1970-01-01 00:00:00.000000 airlift-0.1.2/PKG-INFO
```

### Comparing `airlift-0.1.1/LICENSE` & `airlift-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/README.md` & `airlift-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   <a href="https://pypi.org/project/airlift/">
     <img alt="PyPI version" src="https://badge.fury.io/py/airlift.svg">
   </a>
 </p>
 
 ## Introduction
 
-Airlift is a Command Line Interface (CLI) tool designed to provide a flexible local development environment for Apache Airflow with simple defaults.
+Airlift is a Command Line Interface (CLI) tool designed to provide a local development environment for Apache Airflow with a simple but flexible interface.
 It is built on top of the official [Airflow Helm Chart](https://artifacthub.io/packages/helm/apache-airflow/airflow).
 <h3 align="center">
 <img src="./docs/images/start.gif"
         alt="demo"
         width=600,
         height=300,
         />
@@ -30,14 +30,16 @@
 
 1. Helm
 2. Docker
 3. Kind
 
 Below are the installation instructions for each of these tools on MacOS and Linux distributions.
 
+It is also recommended to allocate at least 4GB of RAM for Docker to run this service.
+
 ### Install Homebrew
 
 Homebrew is a package manager that we will use to install the necessary software. If you don't have Homebrew installed, you can install it by following these instructions:
 
 ```bash
 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
 ```
@@ -227,14 +229,20 @@
 helm_chart_version: '1.0.0'
 port: 8080
 post_start_dag_id: 'example_dag_id'
 ```
 
 In this example, `dag_path` in the yaml file overrides the `-d` setting, `plugin_path` overrides the `-p` setting, and so forth.
 
+Using this configuration, you can now start the service using:
+
+```bash
+airlift start -c $HOME/.config/airlift/config.yaml
+```
+
 ## Examples
 
 [See here for examples with common configuration modifications.](./docs/examples/)
 
 ## FAQ
 
 [See here for Frequently Asked Questions](./docs/faq.md)
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
                             **** [helicopter] ****
                              ****** Airlift ******
                                 [PyPI_version]
 ## Introduction Airlift is a Command Line Interface (CLI) tool designed to
-provide a flexible local development environment for Apache Airflow with simple
-defaults. It is built on top of the official [Airflow Helm Chart](https://
-artifacthub.io/packages/helm/apache-airflow/airflow).
+provide a local development environment for Apache Airflow with a simple but
+flexible interface. It is built on top of the official [Airflow Helm Chart]
+(https://artifacthub.io/packages/helm/apache-airflow/airflow).
                                **** [demo] ****
 ## Requirements Airlift requires the following software to be installed on your
 system: 1. Helm 2. Docker 3. Kind Below are the installation instructions for
-each of these tools on MacOS and Linux distributions. ### Install Homebrew
-Homebrew is a package manager that we will use to install the necessary
-software. If you don't have Homebrew installed, you can install it by following
-these instructions: ```bash /bin/bash -c "$(curl -fsSL https://
+each of these tools on MacOS and Linux distributions. It is also recommended to
+allocate at least 4GB of RAM for Docker to run this service. ### Install
+Homebrew Homebrew is a package manager that we will use to install the
+necessary software. If you don't have Homebrew installed, you can install it by
+following these instructions: ```bash /bin/bash -c "$(curl -fsSL https://
 raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)" ``` ### Install
 Software With Homebrew installed, you can now install Helm, Docker, and Kind.
 #### Helm ```bash brew install helm ``` #### Docker ```bash brew install --cask
 docker ``` -OR- use a tool like [Docker Desktop](https://www.docker.com/
 products/docker-desktop/) or [Rancher Desktop](https://rancherdesktop.io/) ####
 Kind ```bash brew install kind ``` ## Installation Airlift can be installed
 using pip: ```bash pip install airlift ``` ## Usage The general syntax for
@@ -63,18 +64,19 @@
 to/plugins requirements_file: /path/to/requirements.txt helm_values_file: /
 path/to/values.yaml airlift_config_file: /path/to/airlift/config.yaml
 extra_volume_mounts: - hostPath=/my/cool/path,containerPath=/my/mounted/
 path,name=a_unique_name cluster_config_file: /path/to/cluster/config.yaml
 image: 'apache/airflow:2.6.0' helm_chart_version: '1.0.0' port: 8080
 post_start_dag_id: 'example_dag_id' ``` In this example, `dag_path` in the yaml
 file overrides the `-d` setting, `plugin_path` overrides the `-p` setting, and
-so forth. ## Examples [See here for examples with common configuration
-modifications.](./docs/examples/) ## FAQ [See here for Frequently Asked
-Questions](./docs/faq.md) ## Motivation The motivation behind the creation of
-Airlift is to simplify the process of setting up a local development
-environment for Apache Airflow. It aims to be a flexible tool that allows
-developers to easily configure and manage their Airflow instances with
-unlimited flexibility. ## Support and Contribution If you encounter any issues
-or have suggestions for improvements, feel free to open an issue on the GitHub
-repository. Contributions to the project are also welcome. ## Contact If you
-have questions or feedback about Airlift, please reach out by opening an issue
-on the GitHub repository.
+so forth. Using this configuration, you can now start the service using:
+```bash airlift start -c $HOME/.config/airlift/config.yaml ``` ## Examples [See
+here for examples with common configuration modifications.](./docs/examples/
+) ## FAQ [See here for Frequently Asked Questions](./docs/faq.md) ## Motivation
+The motivation behind the creation of Airlift is to simplify the process of
+setting up a local development environment for Apache Airflow. It aims to be a
+flexible tool that allows developers to easily configure and manage their
+Airflow instances with unlimited flexibility. ## Support and Contribution If
+you encounter any issues or have suggestions for improvements, feel free to
+open an issue on the GitHub repository. Contributions to the project are also
+welcome. ## Contact If you have questions or feedback about Airlift, please
+reach out by opening an issue on the GitHub repository.
```

### Comparing `airlift-0.1.1/pyproject.toml` & `airlift-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airlift"
-version = "0.1.1"
+version = "0.1.2"
 description = "A CLI for creating a flexible Apache Airflow local development environment"
 authors = ["jered.little <jeredlittle1996@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "airlift", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `airlift-0.1.1/src/airlift/commands/check.py` & `airlift-0.1.2/src/airlift/commands/check.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/commands/import_variables.py` & `airlift-0.1.2/src/airlift/commands/import_variables.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/commands/pause.py` & `airlift-0.1.2/src/airlift/commands/pause.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/commands/remove.py` & `airlift-0.1.2/src/airlift/commands/remove.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/commands/start.py` & `airlift-0.1.2/src/airlift/commands/start.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/commands/status.py` & `airlift-0.1.2/src/airlift/commands/status.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,22 +11,30 @@
         args (): The command line args
         wait (): How long to sleep before checking the service
     """
     with Halo(
         text=f"Checking Webserver Status on Port {args.port}", spinner="dots"
     ) as spinner:
         spinner.start()
-        time.sleep(wait)
-        try:
-            AirflowUtils.check_webserver_status(port=args.port)
-        except RuntimeError as e:
+        retries = 0
+        error = None
+        while retries <= int(args.status_retries):
+            time.sleep(wait)
+            try:
+                AirflowUtils.check_webserver_status(port=args.port)
+                spinner.succeed()
+                return
+            except Exception as e:
+                error = e
+                logging.warning(str(e))
+                retries += 1
+        if retries >= int(args.status_retries):
             spinner.fail()
-            logging.error(str(e))
+            logging.error(str(error))
             exit(1)
-        spinner.succeed()
 
 
 def status(args, wait=10):
     """
     Checks the status
     Args:
         args (): The command line args
```

### Comparing `airlift-0.1.1/src/airlift/config/config.py` & `airlift-0.1.2/src/airlift/config/config.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/config/helm/final_values.yaml` & `airlift-0.1.2/src/airlift/config/helm/values.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -31,31 +31,39 @@
     failureThreshold: 10
     periodSeconds: 120
   extraVolumes:
     - name: dags
       hostPath:
         path: /mnt/airflow/dags
         type: Directory
-    
+    {% if plugin_path != None  %}
     - name: plugins
       hostPath:
         path: /mnt/airflow/plugins
         type: Directory
-    
-    
+    {% endif %}
+    {% for volume in extra_volume_mounts %}
+    - name: {{ volume['name'] }}
+      hostPath: 
+        path: {{ volume["containerPath"] }}
+        type: Directory
+    {% endfor %}
   extraVolumeMounts:
     - name: dags
       mountPath: /opt/airflow/dags
     - name: dags
       mountPath: /usr/local/airflow/dags/
-    
+    {% if plugin_path != None  %}
     - name: plugins
       mountPath: /opt/airflow/plugins
-     
-    
+    {% endif %} 
+    {% for volume in extra_volume_mounts %}
+    - name: {{ volume['name'] }} 
+      mountPath: {{ volume['containerPath'] }} 
+    {% endfor %}
 webserver:
   service:
     type: NodePort
     ports:
       - name: airflow-ui
         nodePort: 30080
-        port: 8080
+        port: 8080
```

### Comparing `airlift-0.1.1/src/airlift/config/kind/cluster.yaml` & `airlift-0.1.2/src/airlift/config/kind/cluster.yaml`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/main.py` & `airlift-0.1.2/src/airlift/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 This is the `airlift` CLI which can be used to spin up a local Airflow environment for development & testing.
 It uses Helm and Kind underneath the hood to spin up the service. run `airlift -h` to get started 
 """
 
 import sys
 import os
+
+current = os.path.dirname(os.path.realpath(__file__))
+parent = os.path.dirname(current)
+sys.path.append(parent)
 from airlift.commands.run_dag import run_dag
 from airlift.config.config import (
     DEFAULT_AIRLIFT_CONFIG_FILE,
     FINAL_CONFIG_VALUES_FILE_PATH,
     FINAL_DOCKERFILE_PATH,
     FINAL_HELM_VALUES_FILE_PATH,
     FINAL_CLUSTER_CONFIG_FILE_PATH,
 )
 
-current = os.path.dirname(os.path.realpath(__file__))
-parent = os.path.dirname(current)
-sys.path.append(parent)
 
 import argparse
 from airlift.commands.remove import remove
 from airlift.commands.status import status
 from airlift.commands.pause import pause, unpause
 from airlift.utils.parser import ParserUtils
 import logging
```

### Comparing `airlift-0.1.1/src/airlift/utils/airflow.py` & `airlift-0.1.2/src/airlift/utils/airflow.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/utils/airlift.py` & `airlift-0.1.2/src/airlift/utils/airlift.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/utils/command.py` & `airlift-0.1.2/src/airlift/utils/command.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/utils/docker.py` & `airlift-0.1.2/src/airlift/utils/docker.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/utils/file.py` & `airlift-0.1.2/src/airlift/utils/file.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/utils/helm.py` & `airlift-0.1.2/src/airlift/utils/helm.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/utils/kind.py` & `airlift-0.1.2/src/airlift/utils/kind.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/utils/kubernetes.py` & `airlift-0.1.2/src/airlift/utils/kubernetes.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.1/src/airlift/utils/parser.py` & `airlift-0.1.2/src/airlift/utils/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -117,14 +117,32 @@
             help=f"Override the default port exposed locally. Defaults to {DEFAULT_WEBSERVER_PORT}",
         )
         start.add_argument(
             "-D",
             "--post_start_dag_id",
             help="The DAG ID to run post service start. Helpful when you need to bootstrap the service with a DAG execution.",
         )
+        start.add_argument(
+            "-Dr",
+            "--dag_trigger_retries",
+            help="How many times to retry the DAG trigger operation. Time can vary between DAGs becoming available for execution in the UI. Defaults to 3.",
+            default=3,
+        )
+        start.add_argument(
+            "-Dw",
+            "--dag_trigger_retry_wait",
+            help="How long to wait before re-triggering the DAG in Airflow. Defaults to 10 seconds.",
+            default=10,
+        )
+        start.add_argument(
+            "-sr",
+            "--status_retries",
+            help="How many times to retry the service connection before failing. Defaults to 2.",
+            default=2,
+        )
 
     def __add_check_parser(self) -> None:
         self.subparser.add_parser(
             "check", description="Checks all pre-requisite software is installed"
         )
 
     def __add_pause_parser(self) -> None:
@@ -146,14 +164,20 @@
         )
         status.add_argument(
             "-P",
             "--port",
             default=DEFAULT_WEBSERVER_PORT,
             help=f"The port to check the webserver on. Defaults to {DEFAULT_WEBSERVER_PORT}",
         )
+        status.add_argument(
+            "-sr",
+            "--status_retries",
+            help="How many times to retry the service connection before failing. Defaults to 2.",
+            default=2,
+        )
 
     def __add_import_variables_parser(self) -> None:
         import_variables = self.subparser.add_parser(
             "import_variables",
             description="Imports a `variables.json` file to a running Airflow instance.",
         )
         import_variables.add_argument(
@@ -179,11 +203,23 @@
             help=f"The port the webserver is running on. Defaults to {DEFAULT_WEBSERVER_PORT}",
         )
         run_dag.add_argument(
             "-D",
             "--post_start_dag_id",
             help="The DAG ID to run.",
         )
+        run_dag.add_argument(
+            "-Dr",
+            "--dag_trigger_retries",
+            help="How many times to retry the DAG trigger operation. Time can vary between DAGs becoming available for execution in the UI. Defaults to 3.",
+            default=3,
+        )
+        run_dag.add_argument(
+            "-Dw",
+            "--dag_trigger_retry_wait",
+            help="How long to wait before re-triggering the DAG in Airflow. Defaults to 10 seconds.",
+            default=10,
+        )
 
     def get_parsed_args(self):
         args = self.parser.parse_args(self.args)
         return {tup[0]: tup[1] for tup in args._get_kwargs()}
```

### Comparing `airlift-0.1.1/PKG-INFO` & `airlift-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airlift
-Version: 0.1.1
+Version: 0.1.2
 Summary: A CLI for creating a flexible Apache Airflow local development environment
 Author: jered.little
 Author-email: jeredlittle1996@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -30,15 +30,15 @@
   <a href="https://pypi.org/project/airlift/">
     <img alt="PyPI version" src="https://badge.fury.io/py/airlift.svg">
   </a>
 </p>
 
 ## Introduction
 
-Airlift is a Command Line Interface (CLI) tool designed to provide a flexible local development environment for Apache Airflow with simple defaults.
+Airlift is a Command Line Interface (CLI) tool designed to provide a local development environment for Apache Airflow with a simple but flexible interface.
 It is built on top of the official [Airflow Helm Chart](https://artifacthub.io/packages/helm/apache-airflow/airflow).
 <h3 align="center">
 <img src="./docs/images/start.gif"
         alt="demo"
         width=600,
         height=300,
         />
@@ -50,14 +50,16 @@
 
 1. Helm
 2. Docker
 3. Kind
 
 Below are the installation instructions for each of these tools on MacOS and Linux distributions.
 
+It is also recommended to allocate at least 4GB of RAM for Docker to run this service.
+
 ### Install Homebrew
 
 Homebrew is a package manager that we will use to install the necessary software. If you don't have Homebrew installed, you can install it by following these instructions:
 
 ```bash
 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
 ```
@@ -247,14 +249,20 @@
 helm_chart_version: '1.0.0'
 port: 8080
 post_start_dag_id: 'example_dag_id'
 ```
 
 In this example, `dag_path` in the yaml file overrides the `-d` setting, `plugin_path` overrides the `-p` setting, and so forth.
 
+Using this configuration, you can now start the service using:
+
+```bash
+airlift start -c $HOME/.config/airlift/config.yaml
+```
+
 ## Examples
 
 [See here for examples with common configuration modifications.](./docs/examples/)
 
 ## FAQ
 
 [See here for Frequently Asked Questions](./docs/faq.md)
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: airlift Version: 0.1.1 Summary: A CLI for creating
+Metadata-Version: 2.1 Name: airlift Version: 0.1.2 Summary: A CLI for creating
 a flexible Apache Airflow local development environment Author: jered.little
 Author-email: jeredlittle1996@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: dotmap (>=1.3.30,<2.0.0) Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: hiyapyco (>=0.5.1,<0.6.0) Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests (>=2.30.0,<3.0.0)
 Description-Content-Type: text/markdown
                             **** [helicopter] ****
                              ****** Airlift ******
                                 [PyPI_version]
 ## Introduction Airlift is a Command Line Interface (CLI) tool designed to
-provide a flexible local development environment for Apache Airflow with simple
-defaults. It is built on top of the official [Airflow Helm Chart](https://
-artifacthub.io/packages/helm/apache-airflow/airflow).
+provide a local development environment for Apache Airflow with a simple but
+flexible interface. It is built on top of the official [Airflow Helm Chart]
+(https://artifacthub.io/packages/helm/apache-airflow/airflow).
                                **** [demo] ****
 ## Requirements Airlift requires the following software to be installed on your
 system: 1. Helm 2. Docker 3. Kind Below are the installation instructions for
-each of these tools on MacOS and Linux distributions. ### Install Homebrew
-Homebrew is a package manager that we will use to install the necessary
-software. If you don't have Homebrew installed, you can install it by following
-these instructions: ```bash /bin/bash -c "$(curl -fsSL https://
+each of these tools on MacOS and Linux distributions. It is also recommended to
+allocate at least 4GB of RAM for Docker to run this service. ### Install
+Homebrew Homebrew is a package manager that we will use to install the
+necessary software. If you don't have Homebrew installed, you can install it by
+following these instructions: ```bash /bin/bash -c "$(curl -fsSL https://
 raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)" ``` ### Install
 Software With Homebrew installed, you can now install Helm, Docker, and Kind.
 #### Helm ```bash brew install helm ``` #### Docker ```bash brew install --cask
 docker ``` -OR- use a tool like [Docker Desktop](https://www.docker.com/
 products/docker-desktop/) or [Rancher Desktop](https://rancherdesktop.io/) ####
 Kind ```bash brew install kind ``` ## Installation Airlift can be installed
 using pip: ```bash pip install airlift ``` ## Usage The general syntax for
@@ -73,18 +74,19 @@
 to/plugins requirements_file: /path/to/requirements.txt helm_values_file: /
 path/to/values.yaml airlift_config_file: /path/to/airlift/config.yaml
 extra_volume_mounts: - hostPath=/my/cool/path,containerPath=/my/mounted/
 path,name=a_unique_name cluster_config_file: /path/to/cluster/config.yaml
 image: 'apache/airflow:2.6.0' helm_chart_version: '1.0.0' port: 8080
 post_start_dag_id: 'example_dag_id' ``` In this example, `dag_path` in the yaml
 file overrides the `-d` setting, `plugin_path` overrides the `-p` setting, and
-so forth. ## Examples [See here for examples with common configuration
-modifications.](./docs/examples/) ## FAQ [See here for Frequently Asked
-Questions](./docs/faq.md) ## Motivation The motivation behind the creation of
-Airlift is to simplify the process of setting up a local development
-environment for Apache Airflow. It aims to be a flexible tool that allows
-developers to easily configure and manage their Airflow instances with
-unlimited flexibility. ## Support and Contribution If you encounter any issues
-or have suggestions for improvements, feel free to open an issue on the GitHub
-repository. Contributions to the project are also welcome. ## Contact If you
-have questions or feedback about Airlift, please reach out by opening an issue
-on the GitHub repository.
+so forth. Using this configuration, you can now start the service using:
+```bash airlift start -c $HOME/.config/airlift/config.yaml ``` ## Examples [See
+here for examples with common configuration modifications.](./docs/examples/
+) ## FAQ [See here for Frequently Asked Questions](./docs/faq.md) ## Motivation
+The motivation behind the creation of Airlift is to simplify the process of
+setting up a local development environment for Apache Airflow. It aims to be a
+flexible tool that allows developers to easily configure and manage their
+Airflow instances with unlimited flexibility. ## Support and Contribution If
+you encounter any issues or have suggestions for improvements, feel free to
+open an issue on the GitHub repository. Contributions to the project are also
+welcome. ## Contact If you have questions or feedback about Airlift, please
+reach out by opening an issue on the GitHub repository.
```

