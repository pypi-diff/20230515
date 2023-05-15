# Comparing `tmp/pulumi_rediscloud-1.2.0.tar.gz` & `tmp/pulumi_rediscloud-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rediscloud-1.2.0.tar", last modified: Mon May 15 16:50:40 2023, max compression
+gzip compressed data, was "pulumi_rediscloud-1.2.1.tar", last modified: Mon May 15 17:08:36 2023, max compression
```

## Comparing `pulumi_rediscloud-1.2.0.tar` & `pulumi_rediscloud-1.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:50:40.863856 pulumi_rediscloud-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-15 16:50:40.859856 pulumi_rediscloud-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:50:40.855856 pulumi_rediscloud-1.2.0/pulumi_rediscloud/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40848 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    47125 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    34935 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription_peering.py
--rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22528 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/cloud_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:50:40.859856 pulumi_rediscloud-1.2.0/pulumi_rediscloud/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_cloud_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)    14314 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_database_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_subscription_peerings.py
--rw-r--r--   0 runner    (1001) docker     (123)    53802 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    65396 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/subscription_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    31635 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/subscription_peering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:50:40.859856 pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:50:40.863856 pulumi_rediscloud-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:08:36.744519 pulumi_rediscloud-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-15 17:08:36.744519 pulumi_rediscloud-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:08:36.744519 pulumi_rediscloud-1.2.1/pulumi_rediscloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40848 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/active_active_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47125 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/active_active_subscription_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34935 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/active_active_subscription_peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/active_active_subscription_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22528 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/cloud_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:08:36.744519 pulumi_rediscloud-1.2.1/pulumi_rediscloud/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_cloud_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14314 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_database_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_subscription_peerings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53802 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65396 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/subscription_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31635 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud/subscription_peering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:08:36.744519 pulumi_rediscloud-1.2.1/pulumi_rediscloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/pulumi_rediscloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:08:36.744519 pulumi_rediscloud-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 17:08:36.000000 pulumi_rediscloud-1.2.1/setup.py
```

### Comparing `pulumi_rediscloud-1.2.0/PKG-INFO` & `pulumi_rediscloud-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rediscloud
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Pulumi package for creating and managing rediscloud cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/RedisLabs/pulumi-rediscloud
 Keywords: pulumi rediscloud category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_rediscloud-1.2.0/README.md` & `pulumi_rediscloud-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/__init__.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/_inputs.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/_utilities.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/active_active_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription_database.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/active_active_subscription_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription_peering.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/active_active_subscription_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription_regions.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/active_active_subscription_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/cloud_account.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/cloud_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/config/vars.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_cloud_account.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_cloud_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_data_persistence.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_data_persistence.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_database.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_database_modules.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_database_modules.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_payment_method.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_payment_method.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_regions.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_subscription.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_subscription_peerings.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/get_subscription_peerings.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/outputs.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/provider.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/subscription.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/subscription_database.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/subscription_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud/subscription_peering.py` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud/subscription_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/PKG-INFO` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-rediscloud
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Pulumi package for creating and managing rediscloud cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/RedisLabs/pulumi-rediscloud
 Keywords: pulumi rediscloud category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/SOURCES.txt` & `pulumi_rediscloud-1.2.1/pulumi_rediscloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.0/setup.py` & `pulumi_rediscloud-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.2.0"
-PLUGIN_VERSION = "1.2.0"
+VERSION = "1.2.1"
+PLUGIN_VERSION = "1.2.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'rediscloud', PLUGIN_VERSION, '--server', 'github://api.github.com/RedisLabs/pulumi-rediscloud'])
         except OSError as error:
```

