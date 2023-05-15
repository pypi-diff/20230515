# Comparing `tmp/jack_rhoas_sdks-0.0.4.tar.gz` & `tmp/jack_rhoas_sdks-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jack_rhoas_sdks-0.0.4.tar", max compression
+gzip compressed data, was "jack_rhoas_sdks-0.0.5.tar", max compression
```

## Comparing `jack_rhoas_sdks-0.0.4.tar` & `jack_rhoas_sdks-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,11 @@
--rw-r--r--   0        0        0      119 2023-05-11 10:10:18.275759 jack_rhoas_sdks-0.0.4/auth/constants.py
--rw-r--r--   0        0        0      739 2023-05-11 10:10:18.275759 jack_rhoas_sdks-0.0.4/auth/rhoas_auth.py
--rw-r--r--   0        0        0       25 2023-05-11 10:10:18.275759 jack_rhoas_sdks-0.0.4/docs/README.md
--rw-r--r--   0        0        0      974 2023-05-11 10:10:55.983498 jack_rhoas_sdks-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 jack_rhoas_sdks-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      119 2023-05-15 09:45:33.245202 jack_rhoas_sdks-0.0.5/auth/constants.py
+-rw-r--r--   0        0        0      739 2023-05-15 09:45:33.245202 jack_rhoas_sdks-0.0.5/auth/rhoas_auth.py
+-rw-r--r--   0        0        0       25 2023-05-15 09:45:33.245202 jack_rhoas_sdks-0.0.5/docs/README.md
+-rw-r--r--   0        0        0      109 2023-05-15 09:45:33.245202 jack_rhoas_sdks-0.0.5/kafka_instance_sdk/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-15 09:45:33.245202 jack_rhoas_sdks-0.0.5/kafka_mgmt_sdk/__init__.py
+-rw-r--r--   0        0        0      974 2023-05-15 09:46:02.241203 jack_rhoas_sdks-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-05-15 09:45:33.245202 jack_rhoas_sdks-0.0.5/registry_instance_sdk/__init__.py
+-rw-r--r--   0        0        0      106 2023-05-15 09:45:33.245202 jack_rhoas_sdks-0.0.5/registry_mgmt_sdk/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-15 09:45:33.245202 jack_rhoas_sdks-0.0.5/service_accounts_mgmt_sdk/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-15 09:45:33.245202 jack_rhoas_sdks-0.0.5/smart_events_mgmt_sdk/__init__.py
+-rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 jack_rhoas_sdks-0.0.5/PKG-INFO
```

### Comparing `jack_rhoas_sdks-0.0.4/auth/rhoas_auth.py` & `jack_rhoas_sdks-0.0.5/auth/rhoas_auth.py`

 * *Files identical despite different names*

### Comparing `jack_rhoas_sdks-0.0.4/pyproject.toml` & `jack_rhoas_sdks-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jack_rhoas_sdks"
-version = "0.0.4"
+version = "0.0.5"
 description = "A package which includes RHOAS SDKs"
 authors = ["jackdelahunt <jdelahun@redhat.com>"]
 license = "Apache License"
 readme = "docs/README.md"
 packages = [
     { include = "connector_mgmt_sdk/**/*.py" },
     { include = "kafka_instance_sdk/**/*.py"},
```

### Comparing `jack_rhoas_sdks-0.0.4/PKG-INFO` & `jack_rhoas_sdks-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jack-rhoas-sdks
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package which includes RHOAS SDKs
 License: Apache License
 Author: jackdelahunt
 Author-email: jdelahun@redhat.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

