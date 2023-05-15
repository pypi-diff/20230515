# Comparing `tmp/cognicept-shell-1.5.2.tar.gz` & `tmp/cognicept-shell-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognicept-shell-1.5.2.tar", last modified: Mon Dec 12 09:00:42 2022, max compression
+gzip compressed data, was "cognicept-shell-1.6.0.tar", last modified: Mon May 15 07:55:08 2023, max compression
```

## Comparing `cognicept-shell-1.5.2.tar` & `cognicept-shell-1.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-sr-x   0     1000     1000        0 2022-12-12 09:00:42.718516 cognicept-shell-1.5.2/
--rw-r--r--   0     1000     1000    11357 2021-06-29 07:13:53.000000 cognicept-shell-1.5.2/LICENSE.txt
--rw-r--r--   0     1000     1000    14056 2022-12-12 09:00:42.718516 cognicept-shell-1.5.2/PKG-INFO
--rw-r--r--   0     1000     1000    13192 2022-10-05 03:30:10.000000 cognicept-shell-1.5.2/README.md
-drwxr-sr-x   0     1000     1000        0 2022-12-12 09:00:42.714516 cognicept-shell-1.5.2/cognicept_shell.egg-info/
--rw-r--r--   0     1000     1000    14056 2022-12-12 09:00:42.000000 cognicept-shell-1.5.2/cognicept_shell.egg-info/PKG-INFO
--rw-r--r--   0     1000     1000      628 2022-12-12 09:00:42.000000 cognicept-shell-1.5.2/cognicept_shell.egg-info/SOURCES.txt
--rw-r--r--   0     1000     1000        1 2022-12-12 09:00:42.000000 cognicept-shell-1.5.2/cognicept_shell.egg-info/dependency_links.txt
--rw-r--r--   0     1000     1000       61 2022-12-12 09:00:42.000000 cognicept-shell-1.5.2/cognicept_shell.egg-info/entry_points.txt
--rw-r--r--   0     1000     1000       99 2022-12-12 09:00:42.000000 cognicept-shell-1.5.2/cognicept_shell.egg-info/requires.txt
--rw-r--r--   0     1000     1000       21 2022-12-12 09:00:42.000000 cognicept-shell-1.5.2/cognicept_shell.egg-info/top_level.txt
-drwxr-sr-x   0     1000     1000        0 2022-12-12 09:00:42.718516 cognicept-shell-1.5.2/cogniceptshell/
--rw-r--r--   0     1000     1000        0 2021-10-22 09:01:45.000000 cognicept-shell-1.5.2/cogniceptshell/__init__.py
--rw-r--r--   0     1000     1000    38357 2022-12-12 08:59:52.000000 cognicept-shell-1.5.2/cogniceptshell/agent_life_cycle.py
--rw-r--r--   0     1000     1000     2461 2021-06-29 07:13:53.000000 cognicept-shell-1.5.2/cogniceptshell/common.py
--rw-r--r--   0     1000     1000    23091 2022-10-05 03:30:10.000000 cognicept-shell-1.5.2/cogniceptshell/configuration.py
--rw-r--r--   0     1000     1000     8371 2022-10-05 03:30:10.000000 cognicept-shell-1.5.2/cogniceptshell/interface.py
--rw-r--r--   0     1000     1000    11482 2021-10-22 09:01:45.000000 cognicept-shell-1.5.2/cogniceptshell/pusher.py
--rw-r--r--   0     1000     1000    19344 2021-10-22 09:01:45.000000 cognicept-shell-1.5.2/cogniceptshell/rosbag_record.py
--rw-r--r--   0     1000     1000       38 2022-12-12 09:00:42.718516 cognicept-shell-1.5.2/setup.cfg
--rw-r--r--   0     1000     1000     1344 2022-12-12 08:59:52.000000 cognicept-shell-1.5.2/setup.py
-drwxr-sr-x   0     1000     1000        0 2022-12-12 09:00:42.718516 cognicept-shell-1.5.2/tests/
--rw-r--r--   0     1000     1000        0 2021-06-29 07:13:53.000000 cognicept-shell-1.5.2/tests/__init__.py
-drwxr-sr-x   0     1000     1000        0 2022-12-12 09:00:42.718516 cognicept-shell-1.5.2/tests/unit/
--rw-r--r--   0     1000     1000        0 2021-06-29 07:13:53.000000 cognicept-shell-1.5.2/tests/unit/__init__.py
--rw-r--r--   0     1000     1000     2423 2022-10-05 03:30:10.000000 cognicept-shell-1.5.2/tests/unit/mock_docker_client.py
--rw-r--r--   0     1000     1000     7031 2022-10-05 03:30:10.000000 cognicept-shell-1.5.2/tests/unit/test_config.py
--rw-r--r--   0     1000     1000     3485 2021-06-29 07:13:53.000000 cognicept-shell-1.5.2/tests/unit/test_keyrotate.py
--rw-r--r--   0     1000     1000    15158 2022-12-12 08:59:52.000000 cognicept-shell-1.5.2/tests/unit/test_lifecycle.py
+drwxr-sr-x   0     1000     1000        0 2023-05-15 07:55:08.592476 cognicept-shell-1.6.0/
+-rw-r--r--   0     1000     1000    11357 2021-06-29 07:13:53.000000 cognicept-shell-1.6.0/LICENSE.txt
+-rw-r--r--   0     1000     1000    16073 2023-05-15 07:55:08.592476 cognicept-shell-1.6.0/PKG-INFO
+-rw-r--r--   0     1000     1000    15209 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/README.md
+drwxr-sr-x   0     1000     1000        0 2023-05-15 07:55:08.588476 cognicept-shell-1.6.0/cognicept_shell.egg-info/
+-rw-r--r--   0     1000     1000    16073 2023-05-15 07:55:08.000000 cognicept-shell-1.6.0/cognicept_shell.egg-info/PKG-INFO
+-rw-r--r--   0     1000     1000      628 2023-05-15 07:55:08.000000 cognicept-shell-1.6.0/cognicept_shell.egg-info/SOURCES.txt
+-rw-r--r--   0     1000     1000        1 2023-05-15 07:55:08.000000 cognicept-shell-1.6.0/cognicept_shell.egg-info/dependency_links.txt
+-rw-r--r--   0     1000     1000       61 2023-05-15 07:55:08.000000 cognicept-shell-1.6.0/cognicept_shell.egg-info/entry_points.txt
+-rw-r--r--   0     1000     1000      141 2023-05-15 07:55:08.000000 cognicept-shell-1.6.0/cognicept_shell.egg-info/requires.txt
+-rw-r--r--   0     1000     1000       21 2023-05-15 07:55:08.000000 cognicept-shell-1.6.0/cognicept_shell.egg-info/top_level.txt
+drwxr-sr-x   0     1000     1000        0 2023-05-15 07:55:08.588476 cognicept-shell-1.6.0/cogniceptshell/
+-rw-r--r--   0     1000     1000        0 2021-10-22 09:01:45.000000 cognicept-shell-1.6.0/cogniceptshell/__init__.py
+-rw-r--r--   0     1000     1000    48094 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/cogniceptshell/agent_life_cycle.py
+-rw-r--r--   0     1000     1000     2461 2021-06-29 07:13:53.000000 cognicept-shell-1.6.0/cogniceptshell/common.py
+-rw-r--r--   0     1000     1000    23787 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/cogniceptshell/configuration.py
+-rw-r--r--   0     1000     1000     8763 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/cogniceptshell/interface.py
+-rw-r--r--   0     1000     1000    11482 2021-10-22 09:01:45.000000 cognicept-shell-1.6.0/cogniceptshell/pusher.py
+-rw-r--r--   0     1000     1000    19344 2021-10-22 09:01:45.000000 cognicept-shell-1.6.0/cogniceptshell/rosbag_record.py
+-rw-r--r--   0     1000     1000       38 2023-05-15 07:55:08.592476 cognicept-shell-1.6.0/setup.cfg
+-rw-r--r--   0     1000     1000     1395 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/setup.py
+drwxr-sr-x   0     1000     1000        0 2023-05-15 07:55:08.588476 cognicept-shell-1.6.0/tests/
+-rw-r--r--   0     1000     1000        0 2021-06-29 07:13:53.000000 cognicept-shell-1.6.0/tests/__init__.py
+drwxr-sr-x   0     1000     1000        0 2023-05-15 07:55:08.588476 cognicept-shell-1.6.0/tests/unit/
+-rw-r--r--   0     1000     1000        0 2021-06-29 07:13:53.000000 cognicept-shell-1.6.0/tests/unit/__init__.py
+-rw-r--r--   0     1000     1000     2414 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/tests/unit/mock_docker_client.py
+-rw-r--r--   0     1000     1000     9247 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/tests/unit/test_config.py
+-rw-r--r--   0     1000     1000     3485 2021-06-29 07:13:53.000000 cognicept-shell-1.6.0/tests/unit/test_keyrotate.py
+-rw-r--r--   0     1000     1000    30840 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/tests/unit/test_lifecycle.py
```

### Comparing `cognicept-shell-1.5.2/LICENSE.txt` & `cognicept-shell-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.5.2/PKG-INFO` & `cognicept-shell-1.6.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: cognicept-shell
-Version: 1.5.2
-Summary: Shell utility to configure Cognicept tools.
-Home-page: https://kabam.ai
-Author: Jakub Tomasek
-License: Apache License 2.0
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 [![Build Status](https://jenkins.cognicept.systems/buildStatus/icon?job=cognicept-shell-pipeline)](https://jenkins.cognicept.systems/job/cognicept-shell-pipeline/)
 
 
 # COGNICEPT SHELL #
 
 This is a shell utility to manage Cognicept tools.
 
@@ -179,14 +156,20 @@
 
 
 To run update in detached mode:
 ```
 cognicept update -d
 ```
 In detached mode, printing of update statuses in muted. Update is run in a seperate process. Update will continue to run even if terminal session is closed.
+
+To update docker images in environment variable `COGNICEPT_EXTRA_IMAGES`
+```
+cognicept update --image <docker-images-repo>
+```
+
 #### `lastevent`: Display last event log reported by Cognicept agent
 
 Displays last event saved by `cgs_diagnostics_agent` from `~/.cognicept/logs`.
 
 #### `start`/`stop`/`restart`: start/stop/restart cognicept agents
 
 These commands are used to start/stop/restart containers specified in `COG_AGENT_CONTAINERS`/`COG_AGENT_IMAGES`. Certain container names are reserved for Cognicept agents and are preconfigured:
@@ -194,14 +177,21 @@
 * `cgs_diagnostics_agent`
 * `remote_intervention_agent`
 * `kriya_watchdog`
 * `cgs_diagnostics_ecs_api`
 * `cgs_diagnostics_streamer_api`
 * `cgs_bagger_server`
 * `health_aggregator`
+* `diagnostics_aggregator`
+* `kopilot`
+* `smartplus_sound`
+* `map_manager`
+* `computer_health_metrics`
+* `slamtec_adapter`
+* `cam_capture`
 
 Any agent name or image type can be put in the list as long as default command for the image is specified. All containers are started in `host` network mode.
 
 Following are examples for using `start`. `stop` follows same API as `start`. `restart` first calls `stop` and then `stop` .
 
 To start all listed agents `COG_AGENT_CONTAINERS` don't specify any argument:
 
@@ -225,14 +215,20 @@
 
 ```
 cognicept restart -d
 ```
 
 Detached mode is particularly useful for restarting a cognicept agent remotely. 
 In detached mode, progress of restart will not printed. 
+
+To restart and clearing logs
+```
+cognicept restart --prune
+```
+
 #### `keyrotate`: Rotate Cognicept cloud keys
 
 Updates temporary AWS credentials (`AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`, `AWS_SESSION_TOKEN`) using `COGNICEPT_ACCESS_KEY` from `COGNICEPT_API_URI`. The validity of the credentials is 12 hours. Internet access with HTTPS allowed is needed.
 
 #### `orbitty`: Run Orbitty
 
 TODO
@@ -310,14 +306,56 @@
 
 ```
 cognicept init --robot_id sample_robot --org_id sample_org
 Username: sample_username
 Password: sample_password (masked)
 ```
 
+### **Docker-Compose** 
+is supported in version `1.6` for cognicept-shell command below:
+```
+cognicept update/version/start/stop/restart
+```
+
+To make it work, you should added an enviroment variable `COG_COMPOSE_FILE` in `~/.cognicept/runtime.env` and specific the file directory of the docker-compose.yaml file, eg
+```
+COG_COMPOSE_FILE=~/.cognicept/docker-compose.yaml
+```
+
+Sample of docker-compose file:
+```yaml
+version: "3.9"
+services:
+  service_name:
+    container_name: service_name
+    network_mode: "host"
+    restart: unless-stopped
+    env_file:
+    - ${HOME}/.cognicept/runtime.env
+    image: image_repo
+    command: python3 example.py
+```
+Sample response after running `cognicept version`
+
+```Shell
+Cognicept Shell Version 1.6.0
++------------------------------+-----------+
+| Container Name               | Version   |
+|------------------------------+-----------|
+| remote_intervention_agent    | latest    |
+| kriya_watchdog               | latest    |
+| cgs_diagnostics_ecs_api      | dev       |
+| cgs_diagnostics_streamer_api | dev       |
+| cgs_diagnostics_agent        | dev       |
+| service_name                 |           |
++------------------------------+-----------+
+Runtime enviroment file directory: ~/.cognicept/
+```
+
+
 ## Building
 
 
 ### Tests
 
 `cognicept-shell` is using `pytest` as the test framework. Make sure you install manually:
 
@@ -395,14 +433,21 @@
 
 * Feature branch: /feature/name-of-the-feature
 * Bug fix branch: /fix/name-of-the-bug
 * Release branch: /release/name-of-the-release
 
 
 ## Version history
+* 1.6 [12/5/2023]
+  * `cognicept update/version/start/stop/restart` support of docker-compose with enviroment variable `COG_COMPOSE_FILE`
+  * `cognicept restart --prune` for clearing logs
+  * `cognicept update --image` to update docker images in environment variable `COGNICEPT_EXTRA_IMAGES`
+  * `cognicept update` will prompts msgs for users about the specific errors faced when trying to run `cognicept update`
+  * added camera_capture
+
 * 1.5 [23/9/2022]
     * Auto update shell on `cognicept update`
     * Allow container specific updates
     * Add support for kopilot, smartplus_sound_server, map_manager, kriya's friends
     * Audio config for sound devices
     * Backup runtime config before updating
 * 1.4 [16/12/2021]
@@ -436,9 +481,7 @@
     * Added support for Python 3.5
     * Added `lastevent` command to read last event 
     * Added ssh configuration for `remote_intervention_agent`
 
 * 0.1 [10/6/2020]
     * First version of the CLI utility able to configure, restart, and update agents 
 
-
-
```

### Comparing `cognicept-shell-1.5.2/README.md` & `cognicept-shell-1.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: cognicept-shell
+Version: 1.6.0
+Summary: Shell utility to configure Cognicept tools.
+Home-page: https://kabam.ai
+Author: Jakub Tomasek
+License: Apache License 2.0
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 [![Build Status](https://jenkins.cognicept.systems/buildStatus/icon?job=cognicept-shell-pipeline)](https://jenkins.cognicept.systems/job/cognicept-shell-pipeline/)
 
 
 # COGNICEPT SHELL #
 
 This is a shell utility to manage Cognicept tools.
 
@@ -156,14 +179,20 @@
 
 
 To run update in detached mode:
 ```
 cognicept update -d
 ```
 In detached mode, printing of update statuses in muted. Update is run in a seperate process. Update will continue to run even if terminal session is closed.
+
+To update docker images in environment variable `COGNICEPT_EXTRA_IMAGES`
+```
+cognicept update --image <docker-images-repo>
+```
+
 #### `lastevent`: Display last event log reported by Cognicept agent
 
 Displays last event saved by `cgs_diagnostics_agent` from `~/.cognicept/logs`.
 
 #### `start`/`stop`/`restart`: start/stop/restart cognicept agents
 
 These commands are used to start/stop/restart containers specified in `COG_AGENT_CONTAINERS`/`COG_AGENT_IMAGES`. Certain container names are reserved for Cognicept agents and are preconfigured:
@@ -171,14 +200,21 @@
 * `cgs_diagnostics_agent`
 * `remote_intervention_agent`
 * `kriya_watchdog`
 * `cgs_diagnostics_ecs_api`
 * `cgs_diagnostics_streamer_api`
 * `cgs_bagger_server`
 * `health_aggregator`
+* `diagnostics_aggregator`
+* `kopilot`
+* `smartplus_sound`
+* `map_manager`
+* `computer_health_metrics`
+* `slamtec_adapter`
+* `cam_capture`
 
 Any agent name or image type can be put in the list as long as default command for the image is specified. All containers are started in `host` network mode.
 
 Following are examples for using `start`. `stop` follows same API as `start`. `restart` first calls `stop` and then `stop` .
 
 To start all listed agents `COG_AGENT_CONTAINERS` don't specify any argument:
 
@@ -202,14 +238,20 @@
 
 ```
 cognicept restart -d
 ```
 
 Detached mode is particularly useful for restarting a cognicept agent remotely. 
 In detached mode, progress of restart will not printed. 
+
+To restart and clearing logs
+```
+cognicept restart --prune
+```
+
 #### `keyrotate`: Rotate Cognicept cloud keys
 
 Updates temporary AWS credentials (`AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`, `AWS_SESSION_TOKEN`) using `COGNICEPT_ACCESS_KEY` from `COGNICEPT_API_URI`. The validity of the credentials is 12 hours. Internet access with HTTPS allowed is needed.
 
 #### `orbitty`: Run Orbitty
 
 TODO
@@ -287,14 +329,56 @@
 
 ```
 cognicept init --robot_id sample_robot --org_id sample_org
 Username: sample_username
 Password: sample_password (masked)
 ```
 
+### **Docker-Compose** 
+is supported in version `1.6` for cognicept-shell command below:
+```
+cognicept update/version/start/stop/restart
+```
+
+To make it work, you should added an enviroment variable `COG_COMPOSE_FILE` in `~/.cognicept/runtime.env` and specific the file directory of the docker-compose.yaml file, eg
+```
+COG_COMPOSE_FILE=~/.cognicept/docker-compose.yaml
+```
+
+Sample of docker-compose file:
+```yaml
+version: "3.9"
+services:
+  service_name:
+    container_name: service_name
+    network_mode: "host"
+    restart: unless-stopped
+    env_file:
+    - ${HOME}/.cognicept/runtime.env
+    image: image_repo
+    command: python3 example.py
+```
+Sample response after running `cognicept version`
+
+```Shell
+Cognicept Shell Version 1.6.0
++------------------------------+-----------+
+| Container Name               | Version   |
+|------------------------------+-----------|
+| remote_intervention_agent    | latest    |
+| kriya_watchdog               | latest    |
+| cgs_diagnostics_ecs_api      | dev       |
+| cgs_diagnostics_streamer_api | dev       |
+| cgs_diagnostics_agent        | dev       |
+| service_name                 |           |
++------------------------------+-----------+
+Runtime enviroment file directory: ~/.cognicept/
+```
+
+
 ## Building
 
 
 ### Tests
 
 `cognicept-shell` is using `pytest` as the test framework. Make sure you install manually:
 
@@ -372,14 +456,21 @@
 
 * Feature branch: /feature/name-of-the-feature
 * Bug fix branch: /fix/name-of-the-bug
 * Release branch: /release/name-of-the-release
 
 
 ## Version history
+* 1.6 [12/5/2023]
+  * `cognicept update/version/start/stop/restart` support of docker-compose with enviroment variable `COG_COMPOSE_FILE`
+  * `cognicept restart --prune` for clearing logs
+  * `cognicept update --image` to update docker images in environment variable `COGNICEPT_EXTRA_IMAGES`
+  * `cognicept update` will prompts msgs for users about the specific errors faced when trying to run `cognicept update`
+  * added camera_capture
+
 * 1.5 [23/9/2022]
     * Auto update shell on `cognicept update`
     * Allow container specific updates
     * Add support for kopilot, smartplus_sound_server, map_manager, kriya's friends
     * Audio config for sound devices
     * Backup runtime config before updating
 * 1.4 [16/12/2021]
@@ -413,7 +504,9 @@
     * Added support for Python 3.5
     * Added `lastevent` command to read last event 
     * Added ssh configuration for `remote_intervention_agent`
 
 * 0.1 [10/6/2020]
     * First version of the CLI utility able to configure, restart, and update agents 
 
+
+
```

### Comparing `cognicept-shell-1.5.2/cognicept_shell.egg-info/PKG-INFO` & `cognicept-shell-1.6.0/cognicept_shell.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognicept-shell
-Version: 1.5.2
+Version: 1.6.0
 Summary: Shell utility to configure Cognicept tools.
 Home-page: https://kabam.ai
 Author: Jakub Tomasek
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -179,14 +179,20 @@
 
 
 To run update in detached mode:
 ```
 cognicept update -d
 ```
 In detached mode, printing of update statuses in muted. Update is run in a seperate process. Update will continue to run even if terminal session is closed.
+
+To update docker images in environment variable `COGNICEPT_EXTRA_IMAGES`
+```
+cognicept update --image <docker-images-repo>
+```
+
 #### `lastevent`: Display last event log reported by Cognicept agent
 
 Displays last event saved by `cgs_diagnostics_agent` from `~/.cognicept/logs`.
 
 #### `start`/`stop`/`restart`: start/stop/restart cognicept agents
 
 These commands are used to start/stop/restart containers specified in `COG_AGENT_CONTAINERS`/`COG_AGENT_IMAGES`. Certain container names are reserved for Cognicept agents and are preconfigured:
@@ -194,14 +200,21 @@
 * `cgs_diagnostics_agent`
 * `remote_intervention_agent`
 * `kriya_watchdog`
 * `cgs_diagnostics_ecs_api`
 * `cgs_diagnostics_streamer_api`
 * `cgs_bagger_server`
 * `health_aggregator`
+* `diagnostics_aggregator`
+* `kopilot`
+* `smartplus_sound`
+* `map_manager`
+* `computer_health_metrics`
+* `slamtec_adapter`
+* `cam_capture`
 
 Any agent name or image type can be put in the list as long as default command for the image is specified. All containers are started in `host` network mode.
 
 Following are examples for using `start`. `stop` follows same API as `start`. `restart` first calls `stop` and then `stop` .
 
 To start all listed agents `COG_AGENT_CONTAINERS` don't specify any argument:
 
@@ -225,14 +238,20 @@
 
 ```
 cognicept restart -d
 ```
 
 Detached mode is particularly useful for restarting a cognicept agent remotely. 
 In detached mode, progress of restart will not printed. 
+
+To restart and clearing logs
+```
+cognicept restart --prune
+```
+
 #### `keyrotate`: Rotate Cognicept cloud keys
 
 Updates temporary AWS credentials (`AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`, `AWS_SESSION_TOKEN`) using `COGNICEPT_ACCESS_KEY` from `COGNICEPT_API_URI`. The validity of the credentials is 12 hours. Internet access with HTTPS allowed is needed.
 
 #### `orbitty`: Run Orbitty
 
 TODO
@@ -310,14 +329,56 @@
 
 ```
 cognicept init --robot_id sample_robot --org_id sample_org
 Username: sample_username
 Password: sample_password (masked)
 ```
 
+### **Docker-Compose** 
+is supported in version `1.6` for cognicept-shell command below:
+```
+cognicept update/version/start/stop/restart
+```
+
+To make it work, you should added an enviroment variable `COG_COMPOSE_FILE` in `~/.cognicept/runtime.env` and specific the file directory of the docker-compose.yaml file, eg
+```
+COG_COMPOSE_FILE=~/.cognicept/docker-compose.yaml
+```
+
+Sample of docker-compose file:
+```yaml
+version: "3.9"
+services:
+  service_name:
+    container_name: service_name
+    network_mode: "host"
+    restart: unless-stopped
+    env_file:
+    - ${HOME}/.cognicept/runtime.env
+    image: image_repo
+    command: python3 example.py
+```
+Sample response after running `cognicept version`
+
+```Shell
+Cognicept Shell Version 1.6.0
++------------------------------+-----------+
+| Container Name               | Version   |
+|------------------------------+-----------|
+| remote_intervention_agent    | latest    |
+| kriya_watchdog               | latest    |
+| cgs_diagnostics_ecs_api      | dev       |
+| cgs_diagnostics_streamer_api | dev       |
+| cgs_diagnostics_agent        | dev       |
+| service_name                 |           |
++------------------------------+-----------+
+Runtime enviroment file directory: ~/.cognicept/
+```
+
+
 ## Building
 
 
 ### Tests
 
 `cognicept-shell` is using `pytest` as the test framework. Make sure you install manually:
 
@@ -395,14 +456,21 @@
 
 * Feature branch: /feature/name-of-the-feature
 * Bug fix branch: /fix/name-of-the-bug
 * Release branch: /release/name-of-the-release
 
 
 ## Version history
+* 1.6 [12/5/2023]
+  * `cognicept update/version/start/stop/restart` support of docker-compose with enviroment variable `COG_COMPOSE_FILE`
+  * `cognicept restart --prune` for clearing logs
+  * `cognicept update --image` to update docker images in environment variable `COGNICEPT_EXTRA_IMAGES`
+  * `cognicept update` will prompts msgs for users about the specific errors faced when trying to run `cognicept update`
+  * added camera_capture
+
 * 1.5 [23/9/2022]
     * Auto update shell on `cognicept update`
     * Allow container specific updates
     * Add support for kopilot, smartplus_sound_server, map_manager, kriya's friends
     * Audio config for sound devices
     * Backup runtime config before updating
 * 1.4 [16/12/2021]
```

### Comparing `cognicept-shell-1.5.2/cognicept_shell.egg-info/SOURCES.txt` & `cognicept-shell-1.6.0/cognicept_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.5.2/cogniceptshell/agent_life_cycle.py` & `cognicept-shell-1.6.0/cogniceptshell/agent_life_cycle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 # Copyright 2020 Cognicept Systems
 # Author: Jakub Tomasek (jakub@cognicept.systems)
 # --> AgentLifeCycle handles life cycle of Cognicept Agents
 
 import time
 import docker
 import boto3
+import getpass
 import base64
 import json
 import os
 import sys
 import subprocess
 import dateutil
 from datetime import datetime
+from ping3 import ping
 import re
+from docker.errors import DockerException
 import glob
 from multiprocessing import Process, Queue
 import requests
 import botocore
 import shutil
 import pkg_resources
 from tabulate import tabulate
 from cogniceptshell.common import bcolors
 from cogniceptshell.common import generate_progress_bar
 from cogniceptshell.common import permission_safe_docker_call
 from subprocess import DEVNULL
 from docker.types import LogConfig
+from compose.cli.main import TopLevelCommand, project_from_options
 
 class AgentLifeCycle:
     """
     A class to manage agent and Cognicept's docker container lifecycle
     ...
 
     Parameters
@@ -54,14 +58,15 @@
     run_orbitty(args):
         Starts Orbitty.
     """
 
     # default configuration of containers and images
     _docker_container_names = ["cgs_diagnostics_agent", "remote_intervention_agent",
                                "cgs_diagnostics_ecs_api", "cgs_diagnostics_streamer_api", "cgs_bagger_server"]
+    _docker_compose_container_name = []
     _docker_images = {}
     _docker_images["remote_intervention_agent"] = "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/remote_intervention_agent:latest"
     _docker_images["kriya_watchdog"] = "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/remote_intervention_agent:latest"
     _docker_images["cgs_diagnostics_agent"] = "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/cognicept_diagnostics_agent:latest"
     _docker_images["cgs_diagnostics_ecs_api"] = "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/cognicept_diagnostics_api:latest"
     _docker_images["cgs_diagnostics_streamer_api"] = "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/cognicept_diagnostics_api:latest"
     _docker_images["colab_master"] = "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/ros:master"
@@ -71,18 +76,19 @@
     _docker_images["cgs_bagger_server"] = "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/cognicept_rosbagger:latest"
     _docker_images["health_aggregator"] = "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/health_aggregator:dev"
     _docker_images["diagnostics_aggregator"] = "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/health_aggregator:dev"
     _docker_images["smartplus_sound"] = "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/smartplus_sound_server:latest"
     _docker_images["map_manager"] = "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/map_manager:latest"
     _docker_images["computer_health_metrics"] = "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/ros:computer_health_metrics"
     _docker_images["slamtec_adapter"] = "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/slamtec_adapter:latest"
+    _docker_images["cam_capture"] = "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/ros:camera_capture"
 
     def configure_containers(object, cfg):
         """
-        Loads agent configuration from `COG_AGENT_CONTAINERS` and `COG_AGENT_IMAGES`
+        Loads agent configuration from `COG_AGENT_CONTAINERS`, `COG_AGENT_IMAGES` and `COG_COMPOSE_FILE`
 
                 Parameters:
                         cfg (Configuration): Cognicept configuration
                 Returns:
                         None
         """
 
@@ -103,14 +109,26 @@
             if("COG_ORBITTY_ENABLED" in cfg.config and "COG_ORBITTY_IMAGE" in cfg.config):
                 if(bool(cfg.config["COG_ORBITTY_ENABLED"])):
                     object._docker_images["orbitty"] = cfg.config["COG_ORBITTY_IMAGE"]
         else:
             print(
                 "Undefined `COG_AGENT_CONTAINERS` or `COG_AGENT_IMAGES`. Using default.")
 
+        if "COG_COMPOSE_FILE" in cfg.config:
+            object._compose_dir = os.path.dirname(os.path.expanduser(cfg.config["COG_COMPOSE_FILE"]))
+            docker_compose_dict = cfg.get_docker_compose()
+
+            if docker_compose_dict == {}:
+                print(f"{bcolors.WARNING}Warning: failed to load docker compose file - {cfg.config['COG_COMPOSE_FILE']} {bcolors.ENDC}")
+            else:
+                for container_name in docker_compose_dict:
+                    object._docker_container_names.append(container_name)
+                    object._docker_compose_container_name.append(container_name)
+                object._docker_images.update(docker_compose_dict)
+
     def _get_latest_log_loc(object, args):
         """
         Retrieve path to the last log in `~/.cognicept/agent/logs/` relative to `~/.cognicept/` or `path` specified by args.
 
                 Parameters:
                         args: populated argument namespace returned by `argparse.parse_args()`
                 Returns:
@@ -161,15 +179,16 @@
                         data["message"].upper() + bcolors.ENDC
                 else:
                     cgs_agent_status = bcolors.WARNING + "STALE" + bcolors.ENDC
 
         except:
             cgs_agent_status = bcolors.FAIL + "Error" + bcolors.ENDC
 
-        for container_name in object._docker_container_names:
+        container_names = object._docker_container_names
+        for container_name in container_names:
             print(container_name, end=': ', flush=True)
             try:
                 container = client.containers.get(container_name)
                 if container.status != "running":
                     print(bcolors.WARNING + "OFFLINE" + bcolors.ENDC)
                 else:
                     if(container_name == "cgs_diagnostics_agent"):
@@ -327,14 +346,18 @@
             if args.detach:
                 result = True
                 print("Running restart in detached mode")
                 p = Process(target=object._detached_restart, args=(args,))
                 p.start()
             else:
                 result = object._restart_protocol(args)
+            if args.prune:
+                print("Clearing logs")
+                object.clear_logs(args)
+                            
         else:
             result = success_flag
             print(bcolors.FAIL + "Error: The following image(s) shown below cannot be found" + bcolors.ENDC)
             print(*missing_images, sep = "\n")
         return result
 
     def start(object, args):
@@ -356,18 +379,114 @@
         Stops the containers listed in `COG_AGENT_CONTAINERS`. If `args` has parameter `list`, stops only containers in the list.
 
                 Parameters:
                         args: populated argument namespace returned by `argparse.parse_args()`
                 Returns:
                         result (bool): True if succeeded
         """
-
         print("Stopping agents")
         result = object.remove_agents(args)
         return result
+    
+    def check_sudo_password(object, password):
+        '''
+        Checks if user entered password for clearing logs is correct. Runs a dummy sudo command to test input password.
+        '''
+        cmd = ["sudo","-kS","echo","test"]
+        
+        p = subprocess.run(cmd, capture_output=True, input=password, encoding="ascii")
+
+        if "incorrect password" in str(p):
+            return False
+        else:
+            return True
+        
+    
+    def clear_logs(object, args):
+        """
+        Remove all unused containers, networks, images (both dangling and unreferenced). Removes all .txt logs stored in /kriya_logs
+        and .json logs stored in /agents/logs
+                
+        """
+        log_list = ["sudo","-S","-k", "rm"]
+        kriya_log_count = 0
+        agent_folder_list = ["sudo","-S","-k","rm","-r"]
+        cognicept_dir_path = os.path.expanduser(args.path)
+        kriya_logs_dir = cognicept_dir_path + "kriya_logs/"
+        if os.path.exists(kriya_logs_dir):
+            kriya_logs = os.listdir(kriya_logs_dir)
+            for item in kriya_logs:
+                if item.endswith(".txt"):
+                    log_list.append(str(kriya_logs_dir + item))
+                    kriya_log_count += 1
+
+        agent_logs_dir = cognicept_dir_path + "agent/logs/"
+        if os.path.exists(agent_logs_dir):
+            agent_folders = os.listdir(agent_logs_dir)
+            
+            for folder in agent_folders:
+                folder_path = agent_logs_dir + folder
+                if os.path.isdir(folder_path) and folder != "bunched_logs" and folder != "unittest_logs":
+                    agent_folder_list.append(str(folder_path))
+                
+                elif folder == "bunched_logs":
+                    bunched_logs = os.listdir(folder_path)
+                    bunched_log_count = len(bunched_logs)
+                    for item in bunched_logs:
+                        log_list.append(str(folder_path + "/" + item))
+                
+                elif folder == "unittest_logs":
+                    unittest_logs = os.listdir(folder_path)
+                    unittest_log_count = len(unittest_logs)
+                    for item in unittest_logs:
+                        log_list.append(str(folder_path + "/" + item))
+
+        agent_folder_count = len(agent_folder_list)-4
+
+        print(f'\nClear File Summary: \n-Kriya: {kriya_log_count} Logs Found \n-Agent: {agent_folder_count} Folders Found \n-Bunched: {bunched_log_count} Logs Found \n-Unittest: {unittest_log_count} Logs Found')
+        if kriya_log_count + bunched_log_count + unittest_log_count + agent_folder_count == 0:
+            print("No detected Logs and Files to be cleared.")
+        else:
+            print("Do you wish to proceed?")
+            user_input = input("(Y/N)")
+            if user_input.lower() == "y":
+                
+                attempt = 0
+                success = False
+                while attempt < 3 and success == False:
+                    password = getpass.getpass("Enter sudo password: ")
+                    success = object.check_sudo_password(password)
+                    
+                    if not success:
+                        
+                        attempt += 1
+                
+                if success:
+                
+                    if kriya_log_count > 0:
+                        print("Successfully removed all kriya_folder")
+                    
+                    if agent_folder_count > 0:
+                        clear_agent_folder = subprocess.Popen(agent_folder_list, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+                        stdout, stderr = clear_agent_folder.communicate(input=(password + '\n').encode())
+                        print("Successfully removed all agent_folder")
+
+                    if bunched_log_count > 0:
+                        print("Successfully removed all bunched_logs")
+
+                    if unittest_log_count > 0:
+                        print("Successfully removed all unittest_logs")
+
+                    clear_logs = subprocess.Popen(log_list, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+                    stdout, stderr = clear_logs.communicate(input=(password + '\n').encode())
+
+                else:
+                    print("Logs and Files not cleared, Sudo Password Incorrect.")
+            else:
+                print("Logs and Files not cleared")
 
     def status(object, args):
         object.get_status(args)
         object.status_datadog(args)
         return True
 
     def remove_agents(object, args):
@@ -411,18 +530,18 @@
         Starts the containers listed in `args.list`.
 
                 Parameters:
                         args: populated argument namespace returned by `argparse.parse_args()`
                 Returns:
                         result (bool): True if succeeded
         """
-        # if list of agents is not specified, restart all
+        # if list of agents is not specified, restart all and run the docker-compose file
         if(not hasattr(args, 'list') or len(args.list) == 0):
             args.list = object._docker_container_names
-
+        
         object._agent_run_options = {}
 
         # diagnostics agent/API run config
         object._agent_run_options["cgs_diagnostics_agent"] = {"command": "rosrun error_resolution_diagnoser error_resolution_diagnoser", "volumes": {
             args.config.config_path + "agent/logs/": {"bind": "/root/.cognicept/agent/logs", "mode": "rw"}}, "network_mode": "host"}
         object._agent_run_options["cgs_diagnostics_ecs_api"] = {
             "command": "/src/ecs_endpoint.py", "network_mode": "host"}
@@ -478,14 +597,21 @@
             "/var/run/docker.sock/": {"bind": "/var/run/docker.sock/", "mode": "rw"}},
              "network_mode": "host"}
 
         # Slamware adapter run config
         object._agent_run_options["slamtec_adapter"] = {"volumes": {
             args.config.config_path + "slamware_maps/": {"bind": "/root/.cognicept/slamware_maps", "mode": "rw"}},
             "network_mode": "host"}
+        
+        # Camera capture run config 
+        object._agent_run_options["cam_capture"] = {"volumes": {
+            args.config.config_path + "inspect_images/" : {"bind": "/root/.cognicept/inspect_images/", "mode": "rw"},
+            args.config.config_path + "runtime.env" : {"bind": "/root/.cognicept/runtime.env", "mode": "rw"}},
+            "network_mode": "host"}
+        
 
         # Default other config
         object._agent_run_options["other"] = {
             "command": "", "network_mode": "host"}
         permission_docker_call_result = permission_safe_docker_call(
             docker.from_env)
         if permission_docker_call_result is None:
@@ -528,16 +654,23 @@
                 options["tty"] = True
                 options["log_config"] = LogConfig(
                     type=LogConfig.types.JSON, config={'max-size': '5m'})
                 if "command" in options:
                     command = options.pop("command")
                 else:
                     command = ""
-                container = client.containers.run(
-                    object._docker_images[container_name], command, **options)
+                
+                #if container name is within docker-compose service, trigger run function
+                # check whether the container's image is not found
+                if container_name in object._docker_compose_container_name:
+                    object._run_docker_compose_service(container_name)
+                else:
+                    container = client.containers.run(
+                        object._docker_images[container_name], command, **options)
+                
                 print(bcolors.OKBLUE + "DONE" + bcolors.ENDC)
             except docker.errors.ContainerError:
                 print(bcolors.WARNING + "ALREADY EXISTS" +
                       bcolors.ENDC + " (run `cognicept update`)")
             except docker.errors.ImageNotFound:
                 print(bcolors.WARNING + "IMAGE NOT FOUND" +
                       bcolors.ENDC + " (run `cognicept update`)")
@@ -620,106 +753,152 @@
         if latest_version != current_version:
             print(f"{package} current version {current_version} - Installing Version {latest_version}")
             os.system(f'pip3 install -q {package}=={latest_version}')
             print(f'Installation {package} to version {latest_version}:'+bcolors.OKBLUE + " DONE" + bcolors.ENDC)
         else:
             print(f"{package} already in latest version={latest_version}")
 
+    def pull_image(object,image_name,N,i):
+        """
+        Pulls a Docker image and displays a progress bar.
+
+            Parameters:
+                image_name : The name of the Docker image to pull.
+                N : The total number of images to pull.
+                i : index
+        """
+        image_name_short = image_name.replace("412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/", "cognicept/")
+        for status in object.docker_client.pull(image_name, stream=True, decode=True):
+            if("progress" not in status):
+                status["progress"] = ""
+            if("status" not in status):
+                status["status"] = "Error"
+            terminal_size = shutil.get_terminal_size().columns
+            progress = ""
+            if("progressDetail" in status and "total" in status["progressDetail"]):
+                progress = generate_progress_bar(
+                    status["progressDetail"]["current"], status["progressDetail"]["total"], 1, 10)
+                status = "[" + str(i) + "/" + str(N) + "] " + image_name_short + \
+                    " - " + status["status"] + " " + progress
+                if(terminal_size > 0):
+                    print('{:{terminal_size}.{terminal_size}}'.format(
+                        status, terminal_size=terminal_size), end="\r", flush=True)
+                else:
+                    print('{:{trm_sz}.{trm_sz}}'.format(
+                        status, trm_sz=80), end="\r", flush=True)
+        print("[" + str(i) + "/" + str(N) + "] " + image_name_short +
+            " - " + bcolors.OKBLUE + "OK" + bcolors.ENDC + "\033[K")
 
     def update_agents(object, args):
         """
         Starts the containers listed in `args.list` for the purpose of update.
 
                 Parameters:
                         args: populated argument namespace returned by `argparse.parse_args()`
                 Returns:
                         result (bool): True if succeeded
         """
-
+        
         # if list of agents is not specified, update all agents
-        if(not hasattr(args, 'list') or len(args.list) == 0): 
         
+        if((not hasattr(args, 'list') or not args.list) and (not hasattr(args, 'image') or not args.image)):
             images = set(object._docker_images.values())
             # load extra images to update
             if("COG_EXTRA_IMAGES" in args.config.config):
                 image_names = args.config.config["COG_EXTRA_IMAGES"].split(";")
                 if(len(image_names) > 0):
                     images = images.union(set(image_names))
             
             N = len(images)
             object.cognicept_version_update()
             print("Info: This may take a while depending on your connection.")
         # if list of agents is specified, update only that particular set of agents
         else: 
             images = set()
-            for container_name in args.list:
-                images.add(object._docker_images[container_name])
+            if args.list:
+                for container_name in args.list:
+                    if container_name in object._docker_container_names:
+                        images.add(object._docker_images[container_name])
+                    else:
+                        print(f"Error: Container {container_name} not found")
+                        success_flag = False
+
+            if args.image:
+                for image_name in args.image:
+                    images.add(image_name)
+
             N = len(images)
-            print("Info: Update " + str(N) + " agent_image(s)." )
+            print("Info: Update " + str(N) + " agent_image(s).")
 
         i = 0 # For indexing
         success_flag = True
 
         for image_name in images:
             i = i + 1
-
-            image_name_short = image_name.replace("412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/", "cognicept/")
-
             try:
-                for status in object.docker_client.pull(image_name, stream=True, decode=True):
-                    if("progress" not in status):
-                        status["progress"] = ""
-                    if("status" not in status):
-                        status["status"] = "Error"
-                    terminal_size = shutil.get_terminal_size().columns
-                    progress = ""
-                    if("progressDetail" in status and "total" in status["progressDetail"]):
-                        progress = generate_progress_bar(
-                            status["progressDetail"]["current"], status["progressDetail"]["total"], 1, 10)
-                        status = "[" + str(i) + "/" + str(N) + "] " + image_name_short + \
-                            " - " + status["status"] + " " + progress
-                        if(terminal_size > 0):
-                            print('{:{terminal_size}.{terminal_size}}'.format(
-                                status, terminal_size=terminal_size), end="\r", flush=True)
-                        else:
-                            print('{:{trm_sz}.{trm_sz}}'.format(
-                                status, trm_sz=80), end="\r", flush=True)
-                print("[" + str(i) + "/" + str(N) + "] " + image_name_short +
-                    " - " + bcolors.OKBLUE + "OK" + bcolors.ENDC + "\033[K")
-            except docker.errors.ImageNotFound:
-                print("[" + str(i) + "/" + str(N) + "] " + image_name_short +
-                    " - " + bcolors.FAIL + "FAILED" + bcolors.ENDC + "\033[K")
-                success_flag = False
+                if('412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/' in image_name):
+                    object.pull_image(image_name, N=N, i=i)
+                else:
+                    object.pull_image('412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/' + image_name, N=N, i=i)
+
+            except docker.errors.NotFound:
+                try:
+                    object.pull_image(image_name,N=N, i=i)
+                    
+                except docker.errors.NotFound:
+                    print(bcolors.FAIL + "Error: " + bcolors.ENDC + f"Image {image_name} can’t be accessed in ECR or Docker Hub.")
+                    print("[" + str(i) + "/" + str(N) + "] " + image_name +
+                        " - " + bcolors.FAIL + "FAILED" + bcolors.ENDC + "\033[K")
+                    success_flag = False
+                    
+                except DockerException as ex:
+                    print("[" + str(i) + "/" + str(N) + "] " + image_name +
+                        " - " + bcolors.FAIL + "FAILED" + bcolors.ENDC + "\033[K")
+                    print(f"Error: {ex}")
+                    success_flag = False
+                    continue  # skip the current image and continue with the next one
             except:
-                print("[" + str(i) + "/" + str(N) + "] " + image_name_short +
+                print("[" + str(i) + "/" + str(N) + "] " + image_name +
                     " - " + bcolors.FAIL + "FAILED" + bcolors.ENDC + "\033[K")
                 success_flag = False
+
+        if not success_flag:
+            print("There were errors while updating some images.")
         print("Info: Run `cognicept restart` to redeploy updated agents.")
-        
+
         return success_flag
-        
+    
     def _update_protocol(object, args):
         """
         Pulls docker images listed in `COG_AGENT_IMAGES`.
 
                 Parameters:
                         args: populated argument namespace returned by `argparse.parse_args()`
                 Returns:
                         result (bool): True if succeeded
         """
-        # Attempt to login to ECR client
-        login_success = object._ecr_login(args)
-
-        # If login failed, return false
-        if login_success is False:
-            print("Your update credentials may have expired. Run `cognicept keyrotate` to refresh credentials and try `cognicept update` again.")
+        #Check internet connection, if cannot connect, notify user and return false
+        response_time = ping('google.com')
+        if response_time == False:
+            print("No internet connection. Please check the internet connection and try 'cognicept update` again.")
             return False
-
-        return object.update_agents(args)
-
+        else:
+            login_success = object._ecr_login(args)
+            if login_success is False:
+                print("Your login has failed due to the error mentioned above. Please try again.")
+                return False
+            if object.update_agents(args) is False:
+                config_file_path = os.path.expanduser('~/.docker/config.json')
+                if os.path.exists(config_file_path):
+                    print(bcolors.WARNING + "There is a conflict in authentication file, run rm ~/.docker/config.json to remove conflicting file" + bcolors.ENDC)   
+                    return False
+                else:
+                    print(bcolors.WARNING + "Your update credentials may have expired. Run `cognicept keyrotate` to refresh credentials and try `cognicept update` again." + bcolors.ENDC)
+                    return False   
+        
     def _detached_update(object, args):
         """
         Runs the _update_protocol that pulls docker images listed in `COG_AGENT_IMAGES`.
 
                 Parameters:
                         args: populated argument namespace returned by `argparse.parse_args()`
                 Returns:
@@ -812,39 +991,63 @@
 
                 object.docker_client = docker_call_result
 
                 object.docker_client.login(username, password,
                                            registry=registry, reauth=True)
                 # Return true for successful login
                 return True
-            except (docker.errors.APIError, botocore.exceptions.ClientError):
+            except (docker.errors.APIError, botocore.exceptions.ClientError) as e:
                 # On failure, retry
                 print('Attempt #' + str(trial+1) + bcolors.FAIL +
                       " FAILED" + bcolors.ENDC + "\033[K")
+                error_message = str(e)
                 # Wait for 1 second before retrying
                 time.sleep(1.0)
         # If the loop is completed, login failed, so return false
+        print(bcolors.FAIL + error_message + bcolors.ENDC)
         return False
 
     def display_version(object, args):
         """
         Display Cognicept-Shell version and docker images version
 
         Parameters:
                         args: populated argument namespace returned by `argparse.parse_args()`
         """
         version = pkg_resources.require("cognicept-shell")[0].version
         data = {}
         images_version = []
         data['Container Name'] = object._docker_container_names
         # default value for version: "unknown/latest"
-        for x in object._docker_images:
-            image_data = object._docker_images[x].split(':')
-            if len(image_data) > 1:
-                images_version.append(image_data[1])
-                image_data = []
+        for x in data['Container Name']:
+            if x in object._docker_images:
+                image_data = object._docker_images[x].split(':')
+                if len(image_data) > 1:
+                    images_version.append(image_data[1])
+                    image_data = []
             else:
                 images_version.append("unknown/latest")
         data['Version'] = images_version
         print("Cognicept Shell Version "+version)
         print(tabulate(data, headers='keys', tablefmt='psql'))
-        print("Runtime enviroment file directory: " + args.path)
+        print("Runtime enviroment file directory: " +args.path)
+
+
+    def _run_docker_compose_service(object, container_name,):
+        option = {"--detach":True, 
+                "SERVICE" :[f"{container_name}"],
+                "--no-deps": "",
+                "--no-color":True,
+                "--no-recreate": True,
+                "--always-recreate-deps": "",
+                "--abort-on-container-exit": False,
+                "--remove-orphans": False,
+                "--force-recreate": False,
+                "--build": False,
+                "--no-build": True,
+                "--scale": [f'{container_name}=1'],
+                "--quiet-pull": True,
+                }
+        project = project_from_options(object._compose_dir,option)
+        compose_cmd = TopLevelCommand(project)
+        compose_cmd.up(option)
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cognicept-shell-1.5.2/cogniceptshell/common.py` & `cognicept-shell-1.6.0/cogniceptshell/common.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.5.2/cogniceptshell/configuration.py` & `cognicept-shell-1.6.0/cogniceptshell/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import os
 import re
 import jwt
 import requests
 import getpass
 import errno
 import shutil
+import yaml
 
 from cogniceptshell.common import bcolors
 
 
 class Configuration:
     """
     A class to manage agent and Cognicept's configuration
@@ -85,14 +86,29 @@
         if(len(object.config) == 0):
             print("Configuration file `" + object.env_path +
                   "` is empty or could not be parsed.")
             return False
         object._config_loaded = True
         return True
 
+    def get_docker_compose(object):
+        if "COG_COMPOSE_FILE" in object.config:
+            compose_file = os.path.expanduser(object.config["COG_COMPOSE_FILE"])
+            compose_images = {}
+            try:
+                with open(compose_file, 'r') as stream:
+                    docker_compose=yaml.safe_load(stream)
+                    for container_name in docker_compose['services']:
+                        compose_images[container_name] = docker_compose['services'][container_name]['image'] 
+                return compose_images
+            except (yaml.YAMLError,FileNotFoundError, IOError, TypeError):
+                return {}
+        else:
+            return {}
+
     def configure(object, args):
         """
         Manages cognicept configuration based on values in `args`:
             * If `args.read` is True, then it prints all configuration,
             * If `args.add` is True, then it will add or modify a single value inputed by user,
             * Otherwise it will iterate through all values and asks for modifications.
```

### Comparing `cognicept-shell-1.5.2/cogniceptshell/interface.py` & `cognicept-shell-1.6.0/cogniceptshell/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 local_cfg = Configuration()
 
 container_names = []
 
 #added in pull COG_AGENT_IMAGES from "~/.cognicept/"
 if(local_cfg.load_config("~/.cognicept/")):
     container_names = local_cfg.config["COG_AGENT_CONTAINERS"].split(";")
+    for container_name in local_cfg.get_docker_compose():
+        container_names.append(container_name)
     container_names.append([])
 
 #If container_names or agent_image_names cannot be pulled from runtime.env, label preset names for respective sets
 else:
     container_names = ["remote_intervention_agent","kriya_watchdog","cgs_diagnostics_ecs_api","cgs_diagnostics_streamer_api","cgs_diagnostics_agent", "colab_master", "colab_description", "cgs_mission_sys", "health_aggregator"]
 
 parser = argparse.ArgumentParser(
@@ -84,14 +86,17 @@
 
 parser_restart.add_argument('-d', '--detach', action='store_true',
                             help='sets restart to be run in a detached manner. Progress will not be printed')
 parser_restart.add_argument(
     '--path', help='Cognicept configuration directory (default: `' + DEFAULT_PATH + '`)', default=DEFAULT_PATH)
 parser_restart.add_argument(
     'list', help='List of agents to restart, leave empty to restart all agents', metavar='list', type=str, nargs='*',choices=container_names)
+parser_restart.add_argument('--prune', action='store_true',
+                            help='Clears the logs of in kriya_logs and agent logs')
+
 
 parser_start.add_argument(
     '--path', help='Cognicept configuration directory (default: `' + DEFAULT_PATH + '`)', default=DEFAULT_PATH)
 parser_start.add_argument(
     'list', help='List of agents to start, leave empty to start all agents', metavar='list', type=str, nargs='*',choices=container_names)
 
 
@@ -103,15 +108,19 @@
 parser_update.add_argument(
     '--path', help='Cognicept configuration directory (default: `' + DEFAULT_PATH + '`)', default=DEFAULT_PATH)
 parser_update.add_argument(
     '--reset', help='Triggers new login before update', action='store_true')
 parser_update.add_argument("-d", "--detach", help="Runs update in detached mode", action="store_true")
 
 """Adding an add_argument to parser_update"""
-parser_update.add_argument('list', help='List of agents to update, leave empty to start all agents', metavar='list', type=str, nargs='*',choices=container_names)  
+parser_update.add_argument(
+    '--image', '-i', dest ='image',help='List of docker images to update', metavar='flag', type=str, nargs='*')  
+parser_update.add_argument(
+    'list', help='List of agents to update, leave empty to start all agents', metavar='list', type=str, nargs='*',choices=container_names)
+
 
 parser_orbitty.add_argument(
     '--path', help='Cognicept configuration directory (default: `'
     + DEFAULT_PATH + '`)', default=DEFAULT_PATH)
 
 parser_record.add_argument(
     '--path', help='Cognicept configuration directory (default: `' + DEFAULT_PATH + '`)', default=DEFAULT_PATH)
@@ -142,15 +151,15 @@
 
 
 parser_init.add_argument(
     '--path', default=DEFAULT_PATH)
 parser_init.add_argument(
     '--robot_id', help='Input the robot ID', required=True)
 parser_init.add_argument(
-    '--org_id', help='Input the organisation ID', required=True)    
+    '--org_id', help='Input the organisation ID', required=True)
 
 argcomplete.autocomplete(parser)
 
 from cogniceptshell.agent_life_cycle import AgentLifeCycle
 from cogniceptshell.rosbag_record import RosbagRecord
 from cogniceptshell.pusher import Pusher
```

### Comparing `cognicept-shell-1.5.2/cogniceptshell/pusher.py` & `cognicept-shell-1.6.0/cogniceptshell/pusher.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.5.2/cogniceptshell/rosbag_record.py` & `cognicept-shell-1.6.0/cogniceptshell/rosbag_record.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.5.2/setup.py` & `cognicept-shell-1.6.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 import re
 import ast
 
 from setuptools import setup, find_packages
 
 
-requires = ['python-dotenv>=0.13.0', 'boto3>=1.14.0', 'docker>=5.0.0',  'PyCryptodome >=3.9.8', 'argcomplete>=1.12.3', 'tabulate']
+requires = ['python-dotenv>=0.13.0', 'boto3>=1.14.0', 'docker>=5.0.0',  'PyCryptodome >=3.9.8', 'argcomplete>=1.12.3', 'tabulate', 'ping3', 'docker-compose==1.29.2', 'PyJWT==1.7.1']
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup(
     name='cognicept-shell',
-    version='1.5.2',
+    version='1.6.0',
     description='Shell utility to configure Cognicept tools.',
     long_description_content_type="text/markdown",
     long_description=README,
     author='Jakub Tomasek',
     url='https://kabam.ai',
     packages=find_packages(),
     install_requires=requires,
```

### Comparing `cognicept-shell-1.5.2/tests/unit/mock_docker_client.py` & `cognicept-shell-1.6.0/tests/unit/mock_docker_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 
 import docker
 
-
 class MockDockerClient:
     """
     Class to mock docker client
     """
 
     def __init__(self):
         self.containers = MockDockerContainers()
@@ -54,32 +53,32 @@
         if(container_name in self._running_containers):
             def stop_function(timeout): return self._stop(container_name)
             def remove_function(): return self._remove(container_name)
             return MockContainer("running", stop_function, remove_function)
         else:
             raise docker.errors.NotFound("Container not found")
 
-
 class MockContainer:
     """
     Class to mock docker.containers API
     """
 
     def __init__(self, status, stop_function, remove_function):
         self.status = status
         self.stop = stop_function
         self.remove = remove_function
 
+
 class MockDockerImages:
     """
     Class to mock docker.images API
     """
 
     def __init__(self):
-        self._images = []        
+        self._images = []
 
     def get(self, image_name):
         """
         Mock get image api
         """
         if(image_name in self._images):
             return image_name
```

### Comparing `cognicept-shell-1.5.2/tests/unit/test_config.py` & `cognicept-shell-1.6.0/tests/unit/test_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -183,8 +183,64 @@
     result = object.load_config(str(tmpdir) + "/")
     # Mock shutil to succeed blindly to trigger 
     with patch('shutil.copyfile', new=mock_shutil_copy_success):
         with mock.patch("builtins.open", mock_file_write_fail):
             object.save_config()
             captured = capsys.readouterr()
     assert str(captured.out) == bcolors.OKBLUE + "Backed up runtime configuration to: " + str(tmpdir) + "/runtime.env.bk" + bcolors.ENDC + "\n" + \
-                                bcolors.FAIL + "Could not write into `" + str(tmpdir) + "/runtime.env" + "`. Please check write permission or run with `sudo`." + bcolors.ENDC + "\n"
+                                bcolors.FAIL + "Could not write into `" + str(tmpdir) + "/runtime.env" + "`. Please check write permission or run with `sudo`." + bcolors.ENDC + "\n"
+    
+def test_get_docker_compose(monkeypatch):
+    object = Configuration()
+    # Mock config dictionary with COG_COMPOSE_DIR key
+    object.config = {"COG_COMPOSE_FILE": "/path/to/docker-compose.yml"}
+    
+    # Mock yaml file contents
+    yaml_data = """
+    services:
+        camera_top:
+            image: 412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/ros:realsense
+        ip_cam_front:
+            image: 412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/ros:crystal
+    """
+    
+    # Mock the open() function to return yaml file contents
+    mock_file = mock.mock_open(read_data=yaml_data)
+    monkeypatch.setattr("builtins.open", mock_file)
+    # Call the function with the mock config
+    result = object.get_docker_compose()
+    
+    # Check that the expected dictionary was returned
+    expected_result = {"camera_top": "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/ros:realsense", "ip_cam_front": "412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/ros:crystal"}
+    assert result == expected_result
+
+def test_fail_get_docker_compose_(monkeypatch, capsys):
+    object = Configuration()
+    # Mock config dictionary with COG_COMPOSE_DIR key
+    object.config = {"COG_COMPOSE_FILE": "/path/to/docker-compose.yml"}
+    
+    # Call the function with the input directory but file not found
+    result = object.get_docker_compose()
+    assert result == {}
+
+    # Mock empty file contents
+    yaml_data = """"""
+    
+    # Mock the open() function to return yaml file contents
+    mock_file = mock.mock_open(read_data=yaml_data)
+    monkeypatch.setattr("builtins.open", mock_file)
+    # Call the function with the mock config with empty data
+    result = object.get_docker_compose()
+    assert result == {}
+    
+    # Test wrong try get data from invalid yaml format docker-compose file
+    yaml_data = """
+    services:
+    camera_top:
+            image: 412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/ros:realsense
+        ip_cam_front:
+            image: 412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/ros:crystal
+    """
+    mock_file1 = mock.mock_open(read_data=yaml_data)
+    monkeypatch.setattr("builtins.open", mock_file1)
+    result = object.get_docker_compose()
+    assert result == {}
```

### Comparing `cognicept-shell-1.5.2/tests/unit/test_keyrotate.py` & `cognicept-shell-1.6.0/tests/unit/test_keyrotate.py`

 * *Files identical despite different names*

