# Comparing `tmp/pierskarsenbarg_pulumi_ngrok-0.0.17.tar.gz` & `tmp/pierskarsenbarg_pulumi_ngrok-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pierskarsenbarg_pulumi_ngrok-0.0.17.tar", last modified: Fri May 12 14:22:11 2023, max compression
+gzip compressed data, was "dist/pierskarsenbarg_pulumi_ngrok-0.0.19.tar", last modified: Mon May 15 12:34:34 2023, max compression
```

## Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17.tar` & `pierskarsenbarg_pulumi_ngrok-0.0.19.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/
--rw-r--r--   0 runner    (1001) docker     (123)    23130 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19071 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95968 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    16890 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/agent_ingress.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    14843 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/certificate_authority.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    51929 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/endpoint_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/event_destination.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/event_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/ip_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/ip_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/ip_restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)    90020 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15848 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/reserved_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    34391 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/reserved_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/ssh_certificate_authority.py
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/ssh_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    28845 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/ssh_host_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    39372 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/ssh_user_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    24697 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/tls_certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23130 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-12 14:22:11.000000 pierskarsenbarg_pulumi_ngrok-0.0.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:34:34.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/
+-rw-r--r--   0 runner    (1001) docker     (123)    23130 2023-05-15 12:34:34.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19071 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:34:34.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95968 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16890 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/agent_ingress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14843 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/certificate_authority.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:34:34.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51929 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/endpoint_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/event_destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/event_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/ip_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/ip_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/ip_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90020 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15848 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/reserved_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34391 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/reserved_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/ssh_certificate_authority.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/ssh_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28845 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/ssh_host_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39372 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/ssh_user_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24697 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/tls_certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:34:34.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23130 2023-05-15 12:34:34.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-15 12:34:34.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:34:34.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:34:34.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 12:34:34.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 12:34:34.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:34:34.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-15 12:34:33.000000 pierskarsenbarg_pulumi_ngrok-0.0.19/setup.py
```

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/PKG-INFO` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pierskarsenbarg_pulumi_ngrok
-Version: 0.0.17
+Name: pierskarsenbarg-pulumi-ngrok
+Version: 0.0.19
 Summary: A Pulumi package for creating and managing ngrok cloud resources.
 Home-page: https://ngrok.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-ngrok
 Description: # Terraform Bridge Provider Boilerplate
         
         This repository contains boilerplate code for building a new Pulumi provider which wraps an existing Terraform provider.
```

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/README.md` & `pierskarsenbarg_pulumi_ngrok-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/__init__.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/__init__.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/_inputs.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/_inputs.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/_utilities.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/_utilities.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/agent_ingress.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/agent_ingress.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/api_key.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/api_key.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/certificate_authority.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/certificate_authority.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/config/vars.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/config/vars.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/credential.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/credential.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/endpoint_configuration.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/endpoint_configuration.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/event_destination.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/event_destination.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/event_subscription.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/event_subscription.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/ip_policy.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/ip_policy.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/ip_policy_rule.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/ip_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/ip_restriction.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/ip_restriction.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/outputs.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/outputs.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/provider.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/provider.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/reserved_address.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/reserved_address.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/reserved_domain.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/reserved_domain.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/ssh_certificate_authority.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/ssh_certificate_authority.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/ssh_credential.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/ssh_credential.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/ssh_host_certificate.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/ssh_host_certificate.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/ssh_user_certificate.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/ssh_user_certificate.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok/tls_certificate.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok.egg-info/PKG-INFO` & `pierskarsenbarg_pulumi_ngrok-0.0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pierskarsenbarg-pulumi-ngrok
-Version: 0.0.17
+Name: pierskarsenbarg_pulumi_ngrok
+Version: 0.0.19
 Summary: A Pulumi package for creating and managing ngrok cloud resources.
 Home-page: https://ngrok.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-ngrok
 Description: # Terraform Bridge Provider Boilerplate
         
         This repository contains boilerplate code for building a new Pulumi provider which wraps an existing Terraform provider.
```

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/pierskarsenbarg_pulumi_ngrok.egg-info/SOURCES.txt` & `pierskarsenbarg_pulumi_ngrok-0.0.19/pierskarsenbarg_pulumi_ngrok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_ngrok-0.0.17/setup.py` & `pierskarsenbarg_pulumi_ngrok-0.0.19/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.17"
-PLUGIN_VERSION = "0.0.17"
+VERSION = "0.0.19"
+PLUGIN_VERSION = "0.0.19"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'ngrok', PLUGIN_VERSION, '--server', 'github://api.github.com/pierskarsenbarg/pulumi-ngrok'])
         except OSError as error:
```

