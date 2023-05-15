# Comparing `tmp/hydroqc2mqtt-0.8.0.tar.gz` & `tmp/hydroqc2mqtt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydroqc2mqtt-0.8.0.tar", last modified: Tue Jan  3 02:29:47 2023, max compression
+gzip compressed data, was "hydroqc2mqtt-0.9.0.tar", last modified: Mon Jan 16 05:13:20 2023, max compression
```

## Comparing `hydroqc2mqtt-0.8.0.tar` & `hydroqc2mqtt-0.9.0.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.905937 hydroqc2mqtt-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     1851 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    12427 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1194 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    19948 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/.pypirc
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    34523 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2168 2023-01-03 02:29:47.905937 hydroqc2mqtt-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2925 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/config.sample.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/hydroqc2mqtt/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/hydroqc2mqtt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3557 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/hydroqc2mqtt/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/hydroqc2mqtt/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    45322 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/hydroqc2mqtt/contract_device.py
--rw-rw-rw-   0 root         (0) root         (0)    10101 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/hydroqc2mqtt/daemon.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/hydroqc2mqtt/error.py
--rw-rw-rw-   0 root         (0) root         (0)    23084 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/hydroqc2mqtt/sensors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/hydroqc2mqtt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-01-03 02:29:47.000000 hydroqc2mqtt-0.8.0/hydroqc2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1433 2023-01-03 02:29:47.000000 hydroqc2mqtt-0.8.0/hydroqc2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-03 02:29:47.000000 hydroqc2mqtt-0.8.0/hydroqc2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-01-03 02:29:47.000000 hydroqc2mqtt-0.8.0/hydroqc2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-01-03 02:29:47.000000 hydroqc2mqtt-0.8.0/hydroqc2mqtt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-01-03 02:29:47.000000 hydroqc2mqtt-0.8.0/hydroqc2mqtt.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3199 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/hydroqc2mqtt.svg
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2631 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/renovate.json
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/run.sample.sh
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-01-03 02:29:47.905937 hydroqc2mqtt-0.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/homeassistant/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/homeassistant/sensor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/homeassistant/sensor/4444444444-balance/
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/homeassistant/sensor/4444444444-balance/config
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/home/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/home/account/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/home/account/state/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/home/account/state/sensor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/home/account/state/sensor/balance/
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/home/account/state/sensor/balance/state
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/home/contract/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/home/contract/state/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/home/contract/state/binary_sensor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/home/contract/state/binary_sensor/current period epp enabled/
--rw-rw-rw-   0 root         (0) root         (0)        3 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/home/contract/state/binary_sensor/current period epp enabled/state
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/home/contract/state/sensor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.901937 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/home/contract/state/sensor/current billing period current day/
--rw-rw-rw-   0 root         (0) root         (0)        3 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/hydroqc/home/contract/state/sensor/current billing period current day/state
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 02:29:47.905937 hydroqc2mqtt-0.8.0/tests/input_http_data/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tests/input_http_data/calculerSommaireContractuel.json
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tests/input_http_data/contrats.json
--rw-rw-rw-   0 root         (0) root         (0)    11032 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tests/input_http_data/creditPointeCritique.json
--rw-rw-rw-   0 root         (0) root         (0)     4417 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tests/input_http_data/infoCompte.json
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tests/input_http_data/relations.json
--rw-rw-rw-   0 root         (0) root         (0)     6133 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tests/input_http_data/resourceObtenirDonneesConsommationHoraires.json
--rw-rw-rw-   0 root         (0) root         (0)    56115 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tests/input_http_data/resourceObtenirDonneesPeriodesConsommation.json
--rw-rw-rw-   0 root         (0) root         (0)     7057 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)    11077 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tests/test_base_sync_comsumption.py
--rw-rw-rw-   0 root         (0) root         (0)    10321 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tests/test_base_sync_comsumption_history.py
--rw-rw-rw-   0 root         (0) root         (0)     2766 2023-01-03 02:29:36.000000 hydroqc2mqtt-0.8.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.947131 hydroqc2mqtt-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    12447 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    19948 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/.pypirc
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    34523 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-01-16 05:13:20.947131 hydroqc2mqtt-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2925 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/config.sample.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.947131 hydroqc2mqtt-0.9.0/hydroqc2mqtt/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/hydroqc2mqtt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3557 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/hydroqc2mqtt/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/hydroqc2mqtt/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    45544 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/hydroqc2mqtt/contract_device.py
+-rw-rw-rw-   0 root         (0) root         (0)    10101 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/hydroqc2mqtt/daemon.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/hydroqc2mqtt/error.py
+-rw-rw-rw-   0 root         (0) root         (0)    23796 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/hydroqc2mqtt/sensors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.947131 hydroqc2mqtt-0.9.0/hydroqc2mqtt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-01-16 05:13:20.000000 hydroqc2mqtt-0.9.0/hydroqc2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-01-16 05:13:20.000000 hydroqc2mqtt-0.9.0/hydroqc2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-16 05:13:20.000000 hydroqc2mqtt-0.9.0/hydroqc2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-01-16 05:13:20.000000 hydroqc2mqtt-0.9.0/hydroqc2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-01-16 05:13:20.000000 hydroqc2mqtt-0.9.0/hydroqc2mqtt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-01-16 05:13:20.000000 hydroqc2mqtt-0.9.0/hydroqc2mqtt.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3199 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/hydroqc2mqtt.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/renovate.json
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/run.sample.sh
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-01-16 05:13:20.947131 hydroqc2mqtt-0.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.947131 hydroqc2mqtt-0.9.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.943131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.943131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/homeassistant/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.943131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/homeassistant/sensor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.947131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/homeassistant/sensor/4444444444-balance/
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/homeassistant/sensor/4444444444-balance/config
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.943131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.943131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/home/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.943131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/home/account/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.943131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/home/account/state/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.943131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/home/account/state/sensor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.947131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/home/account/state/sensor/balance/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/home/account/state/sensor/balance/state
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.943131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/home/contract/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.943131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/home/contract/state/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.943131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/home/contract/state/binary_sensor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.947131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/home/contract/state/binary_sensor/current period epp enabled/
+-rw-rw-rw-   0 root         (0) root         (0)        3 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/home/contract/state/binary_sensor/current period epp enabled/state
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.943131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/home/contract/state/sensor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.947131 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/home/contract/state/sensor/current billing period current day/
+-rw-rw-rw-   0 root         (0) root         (0)        3 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/hydroqc/home/contract/state/sensor/current billing period current day/state
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 05:13:20.947131 hydroqc2mqtt-0.9.0/tests/input_http_data/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/input_http_data/calculerSommaireContractuel.json
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/input_http_data/contrats.json
+-rw-rw-rw-   0 root         (0) root         (0)    11032 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/input_http_data/creditPointeCritique.json
+-rw-rw-rw-   0 root         (0) root         (0)     4417 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/input_http_data/infoCompte.json
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/input_http_data/outages.json
+-rw-rw-rw-   0 root         (0) root         (0)      724 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/input_http_data/relations.json
+-rw-rw-rw-   0 root         (0) root         (0)     6133 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/input_http_data/resourceObtenirDonneesConsommationHoraires.json
+-rw-rw-rw-   0 root         (0) root         (0)    56115 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/input_http_data/resourceObtenirDonneesPeriodesConsommation.json
+-rw-rw-rw-   0 root         (0) root         (0)     7209 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    11241 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/test_base_sync_comsumption.py
+-rw-rw-rw-   0 root         (0) root         (0)    10321 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tests/test_base_sync_comsumption_history.py
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-01-16 05:13:11.000000 hydroqc2mqtt-0.9.0/tox.ini
```

### Comparing `hydroqc2mqtt-0.8.0/.gitignore` & `hydroqc2mqtt-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/.gitlab-ci.yml` & `hydroqc2mqtt-0.9.0/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -39,26 +39,26 @@
     - name: eclipse-mosquitto:2.0.15
       alias: mosquitto
       entrypoint:
         - "/bin/sh"
       command:
         - -c
         - cp mosquitto-no-auth.conf /mosquitto/config/mosquitto.conf && cat /mosquitto/config/mosquitto.conf && /docker-entrypoint.sh mosquitto -c /mosquitto/config/mosquitto.conf
-    - name: homeassistant/home-assistant:2022.12.8
+    - name: homeassistant/home-assistant:2023.1.4
       alias: hass
       entrypoint:
         - bash
       command:
         - -c
         - |
           mkdir -p .storage && (echo ${HASS_AUTH} | base64 -d > .storage/auth) && (hass --script ensure_config -c /config 2>&1) && (echo 'homeassistant:' >> /config/configuration.yaml) && (echo '  time_zone: America/New_York' >> /config/configuration.yaml) && (echo '  latitude: 45.508888' >> /config/configuration.yaml) && (echo '  longitude: -73.561668' >> /config/configuration.yaml) && hass --script auth add admin password && sleep 1 && /init
   tags:
   - hydroqc
   image:
-    name: registry.gitlab.com/hydroqc/hydroqc-base-container/build:7ad943b
+    name: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20230111151303
   variables:
     MQTT_HOST: mosquitto
     MQTT_PORT: "1883"
   script:
     - cp /usr/share/zoneinfo/America/New_York /etc/localtime
     - echo echo "America/New_York " > /etc/timezone
     - tox --parallel auto
@@ -100,15 +100,15 @@
       command:
         - -c
         - |
           mkdir -p .storage && (echo ${HASS_AUTH} | base64 -d > .storage/auth) && (hass --script ensure_config -c /config 2>&1) && (echo 'homeassistant:' >> /config/configuration.yaml) && (echo '  time_zone: America/New_York' >> /config/configuration.yaml) && (echo '  latitude: 45.508888' >> /config/configuration.yaml) && (echo '  longitude: -73.561668' >> /config/configuration.yaml) && hass --script auth add admin password && sleep 1 && /init
   tags:
   - hydroqc
   image:
-    name: registry.gitlab.com/hydroqc/hydroqc-base-container/build:7ad943b
+    name: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20230111151303
   variables:
     MQTT_HOST: mosquitto
     MQTT_PORT: "1883"
   script:
     - cp /usr/share/zoneinfo/America/New_York /etc/localtime
     - echo echo "America/New_York " > /etc/timezone
     - tox --parallel auto
@@ -183,15 +183,15 @@
       when: on_success
     - when: never
 
 promote2pypi:
   stage: pypi
   tags:
   - hydroqc
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:7ad943b
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20230111151303
   script:
     - pip install --upgrade pip
     - pip install --upgrade build setuptools_scm twine
     - python3 -m build -o dist
     - python3 -m twine check --strict dist/*
     - twine upload --verbose --non-interactive --repository pypi dist/*
   rules:
```

### Comparing `hydroqc2mqtt-0.8.0/.pre-commit-config.yaml` & `hydroqc2mqtt-0.9.0/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -38,13 +38,13 @@
   hooks:
   - id: mypy
     args: [--strict, --pretty, --show-error-codes]
     additional_dependencies:
       - "types-PyYAML==6.0.12.2"
       - "pytest-stub==1.1.0"
       - "types-paho-mqtt==1.6.0.1"
-      - "homeassistant-stubs==2022.12.8"
-      - "Hydro_Quebec_API_Wrapper==2.2.0"
-      - "mqtt-hass-base==4.1.3"
+      - "homeassistant-stubs==2023.1.4"
+      - "Hydro_Quebec_API_Wrapper==2.3.3"
+      - "mqtt-hass-base==4.1.4"
       - "aioresponses==0.7.4"
       - "types-python-dateutil==2.8.19.5"
-      - "types-pytz==2022.7.0.0"
+      - "types-pytz==2022.7.1.0"
```

### Comparing `hydroqc2mqtt-0.8.0/.pylintrc` & `hydroqc2mqtt-0.9.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/Dockerfile` & `hydroqc2mqtt-0.9.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/LICENSE` & `hydroqc2mqtt-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/PKG-INFO` & `hydroqc2mqtt-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydroqc2mqtt
-Version: 0.8.0
+Version: 0.9.0
 Summary: Daemon managing hydroqc sensors through MQTT
 Home-page: https://hydroqc.ca
 Author-email: Hydroqc Team <info@hydroqc.ca>
 License: AGPL-3.0-or-later
 Project-URL: Source Code, https://gitlab.com/hydroqc/hydroqc2mqtt
 Project-URL: Bug Reports, https://gitlab.com/hydroqc/hydroqc2mqtt/-/issues
 Project-URL: Home-page, https://hydroqc.ca
```

### Comparing `hydroqc2mqtt-0.8.0/README.md` & `hydroqc2mqtt-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/config.sample.yaml` & `hydroqc2mqtt-0.9.0/config.sample.yaml`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/hydroqc2mqtt/__main__.py` & `hydroqc2mqtt-0.9.0/hydroqc2mqtt/__main__.py`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/hydroqc2mqtt/contract_device.py` & `hydroqc2mqtt-0.9.0/hydroqc2mqtt/contract_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -470,14 +470,16 @@
                     value = data_obj.isoformat()
                 elif (
                     isinstance(data_obj, (int, float))
                     and "device_class" in sensor_list[sensor_key]
                     and sensor_list[sensor_key]["device_class"] == "monetary"
                 ):
                     value = str(round(data_obj, 2))
+                elif isinstance(data_obj, datetime.timedelta):
+                    value = f"{data_obj.seconds / 60} minutes"
                 else:
                     value = data_obj
 
         if value is None and sensor_type != "ATTRIBUTES":
             if reason == "wc_sensor_not_in_season":
                 self.logger.info("Not in winter credit season, ignoring %s", sensor_key)
             elif reason == "data_not_available":
@@ -562,22 +564,24 @@
         """Update Home Assistant entities."""
         self.logger.info("Updating ...")
         # TODO if any api calls failed, we should NOT crash and set sensors to not_available
         # Fetch latest data
         self.logger.info("Fetching data...")
         customer, account, contract = await self.get_contract()
         await contract.get_periods_info()
+        await contract.refresh_outages()
 
         if contract.rate == "D" and contract.rate_option == "CPC":
             contract = cast(ContractDCPC, contract)
             contract.set_preheat_duration(self._preheat_duration)
             await contract.winter_credit.refresh_data()
         elif contract.rate == "DPC":
             contract = cast(ContractDPC, contract)
             await contract.get_dpc_data()
+            await contract.peak_handler.refresh_data()
         elif contract.rate == "DT":
             contract = cast(ContractDT, contract)
             await contract.get_annual_consumption()
 
         self.logger.info("Data fetched")
 
         # history
```

### Comparing `hydroqc2mqtt-0.8.0/hydroqc2mqtt/daemon.py` & `hydroqc2mqtt-0.9.0/hydroqc2mqtt/daemon.py`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/hydroqc2mqtt/sensors.py` & `hydroqc2mqtt-0.9.0/hydroqc2mqtt/sensors.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,14 +122,32 @@
         "icon": "mdi:currency-usd",
         "state_class": "measurement",
         "unit": "CAD",
         "sub_mqtt_topic": "account/state",
         "rates": ["ALL"],
     },
     # Contract
+    "outage": {
+        "name": "Next or current outage",
+        "data_source": "contract.next_outage.start_date",
+        "state_class": "measurement",
+        "device_class": "timestamp",
+        "expire_after": 0,
+        "force_update": False,
+        "icon": "mdi:calendar-start",
+        "sub_mqtt_topic": "contract/state",
+        "rates": ["ALL"],
+        "attributes": {
+            "end_date": "contract.next_outage.end_date",
+            "cause": "contract.next_outage.cause",
+            "planned_duration": "contract.next_outage.planned_duration",
+            "emergency_level": "contract.next_outage.emergency_level",
+            "is_planned": "contract.next_outage.is_planned",
+        },
+    },
     "current_billing_period_current_day": {
         "name": "Current billing period current day",
         "data_source": "contract.cp_current_day",
         "device_class": None,
         "expire_after": 0,
         "force_update": False,
         "icon": "mdi:calendar-start",
```

### Comparing `hydroqc2mqtt-0.8.0/hydroqc2mqtt.egg-info/PKG-INFO` & `hydroqc2mqtt-0.9.0/hydroqc2mqtt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydroqc2mqtt
-Version: 0.8.0
+Version: 0.9.0
 Summary: Daemon managing hydroqc sensors through MQTT
 Home-page: https://hydroqc.ca
 Author-email: Hydroqc Team <info@hydroqc.ca>
 License: AGPL-3.0-or-later
 Project-URL: Source Code, https://gitlab.com/hydroqc/hydroqc2mqtt
 Project-URL: Bug Reports, https://gitlab.com/hydroqc/hydroqc2mqtt/-/issues
 Project-URL: Home-page, https://hydroqc.ca
```

### Comparing `hydroqc2mqtt-0.8.0/hydroqc2mqtt.egg-info/SOURCES.txt` & `hydroqc2mqtt-0.9.0/hydroqc2mqtt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -36,10 +36,11 @@
 tests/expected_mqtt_data/hydroqc/home/account/state/sensor/balance/state
 tests/expected_mqtt_data/hydroqc/home/contract/state/binary_sensor/current period epp enabled/state
 tests/expected_mqtt_data/hydroqc/home/contract/state/sensor/current billing period current day/state
 tests/input_http_data/calculerSommaireContractuel.json
 tests/input_http_data/contrats.json
 tests/input_http_data/creditPointeCritique.json
 tests/input_http_data/infoCompte.json
+tests/input_http_data/outages.json
 tests/input_http_data/relations.json
 tests/input_http_data/resourceObtenirDonneesConsommationHoraires.json
 tests/input_http_data/resourceObtenirDonneesPeriodesConsommation.json
```

### Comparing `hydroqc2mqtt-0.8.0/hydroqc2mqtt.svg` & `hydroqc2mqtt-0.9.0/hydroqc2mqtt.svg`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/pyproject.toml` & `hydroqc2mqtt-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/renovate.json` & `hydroqc2mqtt-0.9.0/renovate.json`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/tests/expected_mqtt_data/homeassistant/sensor/4444444444-balance/config` & `hydroqc2mqtt-0.9.0/tests/expected_mqtt_data/homeassistant/sensor/4444444444-balance/config`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/tests/input_http_data/contrats.json` & `hydroqc2mqtt-0.9.0/tests/input_http_data/contrats.json`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/tests/input_http_data/creditPointeCritique.json` & `hydroqc2mqtt-0.9.0/tests/input_http_data/creditPointeCritique.json`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/tests/input_http_data/infoCompte.json` & `hydroqc2mqtt-0.9.0/tests/input_http_data/infoCompte.json`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/tests/input_http_data/relations.json` & `hydroqc2mqtt-0.9.0/tests/input_http_data/relations.json`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/tests/input_http_data/resourceObtenirDonneesConsommationHoraires.json` & `hydroqc2mqtt-0.9.0/tests/input_http_data/resourceObtenirDonneesConsommationHoraires.json`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/tests/input_http_data/resourceObtenirDonneesPeriodesConsommation.json` & `hydroqc2mqtt-0.9.0/tests/input_http_data/resourceObtenirDonneesPeriodesConsommation.json`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/tests/test_base.py` & `hydroqc2mqtt-0.9.0/tests/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     AUTH_URL,
     AUTHORIZE_URL,
     CONTRACT_LIST_URL,
     CONTRACT_SUMMARY_URL,
     CUSTOMER_INFO_URL,
     GET_WINTER_CREDIT_API_URL,
     LOGIN_URL_6,
+    OUTAGES,
     PERIOD_DATA_URL,
     PORTRAIT_URL,
     RELATION_URL,
     SECURITY_URL,
     SESSION_REFRESH_URL,
     SESSION_URL,
 )
@@ -75,15 +76,15 @@
     client.on_message = on_message
     client.connect_async(MQTT_HOST, MQTT_PORT, keepalive=60)
     client.loop_start()
 
     time.sleep(1)
 
     # Prepare http mocking
-    with aioresponses() as mres:  # type: ignore[no-untyped-call]
+    with aioresponses() as mres:
         # LOGIN
         mres.post(
             AUTH_URL,
             payload={
                 "callbacks": [
                     {"input": [{"value": "username"}]},
                     {"input": [{"value": "password"}]},
@@ -193,14 +194,18 @@
             payload_13 = json.load(fht)
         mres.get(GET_WINTER_CREDIT_API_URL, payload=payload_13)
 
         mres.get(
             f"{GET_WINTER_CREDIT_API_URL}?noContrat={CONTRACT_ID}", payload=payload_13
         )
 
+        with open("tests/input_http_data/outages.json", "rb") as fht:
+            payload_14 = json.load(fht)
+        mres.get(OUTAGES + "6666666666", payload=payload_14)
+
         # Run main loop once
         del sys.argv[1:]
         sys.argv.append("--run-once")
         main()
 
         # Check some data in MQTT
         time.sleep(1)
```

### Comparing `hydroqc2mqtt-0.8.0/tests/test_base_sync_comsumption.py` & `hydroqc2mqtt-0.9.0/tests/test_base_sync_comsumption.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     AUTHORIZE_URL,
     CONTRACT_LIST_URL,
     CONTRACT_SUMMARY_URL,
     CUSTOMER_INFO_URL,
     GET_WINTER_CREDIT_API_URL,
     HOURLY_CONSUMPTION_API_URL,
     LOGIN_URL_6,
+    OUTAGES,
     PERIOD_DATA_URL,
     PORTRAIT_URL,
     RELATION_URL,
     SECURITY_URL,
     SESSION_REFRESH_URL,
     SESSION_URL,
 )
@@ -143,15 +144,15 @@
         # os.environ["HQ2M_CONTRACTS_0_HOME_ASSISTANT_TOKEN"] = "fake_token"
 
         # await asyncio.sleep(1)
         time.sleep(1)
 
         # Prepare http mocking
         ws_server_url = os.environ["HQ2M_CONTRACTS_0_HOME_ASSISTANT_WEBSOCKET_URL"]
-        with aioresponses(passthrough=[ws_server_url]) as mres:  # type: ignore[no-untyped-call]
+        with aioresponses(passthrough=[ws_server_url]) as mres:
             # LOGIN
             mres.post(
                 AUTH_URL,
                 payload={
                     "callbacks": [
                         {"input": [{"value": "username"}]},
                         {"input": [{"value": "password"}]},
@@ -280,14 +281,18 @@
             mres.get(
                 f"{HOURLY_CONSUMPTION_API_URL}?date={YESTERDAY_STR}", payload=payload_12
             )
             mres.get(
                 f"{HOURLY_CONSUMPTION_API_URL}?date={TODAY_STR}", payload=payload_12
             )
 
+            with open("tests/input_http_data/outages.json", "rb") as fht:
+                payload_14 = json.load(fht)
+            mres.get(OUTAGES + "6666666666", payload=payload_14)
+
             del sys.argv[1:]
             sys.argv.append("--run-once")
             main()
 
             # Check some data in MQTT
             time.sleep(1)
             for topic, expected_value in expected_results.items():
```

### Comparing `hydroqc2mqtt-0.8.0/tests/test_base_sync_comsumption_history.py` & `hydroqc2mqtt-0.9.0/tests/test_base_sync_comsumption_history.py`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-0.8.0/tox.ini` & `hydroqc2mqtt-0.9.0/tox.ini`

 * *Files identical despite different names*

