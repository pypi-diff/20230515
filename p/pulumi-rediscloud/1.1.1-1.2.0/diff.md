# Comparing `tmp/pulumi_rediscloud-1.1.1.tar.gz` & `tmp/pulumi_rediscloud-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rediscloud-1.1.1.tar", last modified: Wed May 10 12:24:38 2023, max compression
+gzip compressed data, was "pulumi_rediscloud-1.2.0.tar", last modified: Mon May 15 16:50:40 2023, max compression
```

## Comparing `pulumi_rediscloud-1.1.1.tar` & `pulumi_rediscloud-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:24:38.412462 pulumi_rediscloud-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-10 12:24:38.412462 pulumi_rediscloud-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:24:38.412462 pulumi_rediscloud-1.1.1/pulumi_rediscloud/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/active_active_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    46436 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/active_active_subscription_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    34875 2023-05-10 12:24:37.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/active_active_subscription_peering.py
--rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/active_active_subscription_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22233 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/cloud_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:24:38.412462 pulumi_rediscloud-1.1.1/pulumi_rediscloud/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_cloud_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)    14324 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_database_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_subscription_peerings.py
--rw-r--r--   0 runner    (1001) docker     (123)    52420 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    65203 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/subscription_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    31575 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud/subscription_peering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:24:38.412462 pulumi_rediscloud-1.1.1/pulumi_rediscloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/pulumi_rediscloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:24:38.412462 pulumi_rediscloud-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-10 12:24:38.000000 pulumi_rediscloud-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:50:40.863856 pulumi_rediscloud-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-15 16:50:40.859856 pulumi_rediscloud-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:50:40.855856 pulumi_rediscloud-1.2.0/pulumi_rediscloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40848 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47125 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34935 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription_peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22528 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/cloud_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:50:40.859856 pulumi_rediscloud-1.2.0/pulumi_rediscloud/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_cloud_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14314 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_database_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_subscription_peerings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53802 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65396 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/subscription_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31635 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud/subscription_peering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:50:40.859856 pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:50:40.863856 pulumi_rediscloud-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 16:50:40.000000 pulumi_rediscloud-1.2.0/setup.py
```

### Comparing `pulumi_rediscloud-1.1.1/PKG-INFO` & `pulumi_rediscloud-1.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,48 @@
-Metadata-Version: 2.1
-Name: pulumi_rediscloud
-Version: 1.1.1
-Summary: A Pulumi package for creating and managing rediscloud cloud resources.
-Home-page: https://www.pulumi.com
-License: Apache-2.0
-Project-URL: Repository, https://github.com/RedisLabs/pulumi-rediscloud
-Keywords: pulumi rediscloud category/cloud
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # Redis Cloud Resource Provider
 
-The Redis Cloud Resource Provider lets you manage [Redis Cloud](https://redislabs.com/redis-enterprise-cloud/overview) resources.
+The Redis Cloud Resource Provider lets you manage [Redis Cloud](https://redislabs.com/redis-enterprise-cloud/overview) resources. The provider is used to interact with the resources supported by Redis Enterprise Cloud. Please note that the provider is available only for Flexible or Annual subscriptions. It is not supported for Fixed or Free subscriptions.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @RedisLabs/pulumi-rediscloud
+npm install @rediscloud/pulumi-rediscloud
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @RedisLabs/pulumi-rediscloud
+yarn add @rediscloud/pulumi-rediscloud
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
-pip install redislabs_pulumi_rediscloud
+pip install pulumi_rediscloud
 ```
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library:
 
 ```bash
 go get github.com/RedisLabs/pulumi-rediscloud/sdk/go/...
 ```
 
-### .NET
-
-To use from .NET, install using `dotnet add package`:
-
-```bash
-dotnet add package RedisLabs.PulumiRedisCloud
-```
-
 ## Configuration
 
 The following configuration points are available for the `rediscloud` provider:
 
 - `apiKey` (environment: `REDISCLOUD_ACCESS_KEY`) - This is the Redis Enterprise Cloud API account key. It must be provided but can also be set by the environment variable.
 - `secretKey` (environment: `REDISCLOUD_SECRET_KEY`) - This is the Redis Enterprise Cloud API secret key. It must be provided but can also be set by the environment variable.
 
 ## Reference
 
 For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/rediscloud/api-docs/).
-
-
```

### Comparing `pulumi_rediscloud-1.1.1/README.md` & `pulumi_rediscloud-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,62 @@
+Metadata-Version: 2.1
+Name: pulumi_rediscloud
+Version: 1.2.0
+Summary: A Pulumi package for creating and managing rediscloud cloud resources.
+Home-page: https://www.pulumi.com
+License: Apache-2.0
+Project-URL: Repository, https://github.com/RedisLabs/pulumi-rediscloud
+Keywords: pulumi rediscloud category/cloud
+Platform: UNKNOWN
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # Redis Cloud Resource Provider
 
-The Redis Cloud Resource Provider lets you manage [Redis Cloud](https://redislabs.com/redis-enterprise-cloud/overview) resources.
+The Redis Cloud Resource Provider lets you manage [Redis Cloud](https://redislabs.com/redis-enterprise-cloud/overview) resources. The provider is used to interact with the resources supported by Redis Enterprise Cloud. Please note that the provider is available only for Flexible or Annual subscriptions. It is not supported for Fixed or Free subscriptions.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @RedisLabs/pulumi-rediscloud
+npm install @rediscloud/pulumi-rediscloud
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @RedisLabs/pulumi-rediscloud
+yarn add @rediscloud/pulumi-rediscloud
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
-pip install redislabs_pulumi_rediscloud
+pip install pulumi_rediscloud
 ```
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library:
 
 ```bash
 go get github.com/RedisLabs/pulumi-rediscloud/sdk/go/...
 ```
 
-### .NET
-
-To use from .NET, install using `dotnet add package`:
-
-```bash
-dotnet add package RedisLabs.PulumiRedisCloud
-```
-
 ## Configuration
 
 The following configuration points are available for the `rediscloud` provider:
 
 - `apiKey` (environment: `REDISCLOUD_ACCESS_KEY`) - This is the Redis Enterprise Cloud API account key. It must be provided but can also be set by the environment variable.
 - `secretKey` (environment: `REDISCLOUD_SECRET_KEY`) - This is the Redis Enterprise Cloud API secret key. It must be provided but can also be set by the environment variable.
 
 ## Reference
 
 For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/rediscloud/api-docs/).
+
+
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/__init__.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/_inputs.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     def __init__(__self__, *,
                  memory_limit_in_gb: pulumi.Input[float],
                  quantity: pulumi.Input[int],
                  regions: pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionCreationPlanRegionArgs']]]):
         """
         :param pulumi.Input[float] memory_limit_in_gb: Maximum memory usage that will be used for your largest planned database, including replication and other overhead
         :param pulumi.Input[int] quantity: The planned number of databases in the subscription.
-        :param pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionCreationPlanRegionArgs']]] regions: Deployment region as defined by cloud provider
         """
         pulumi.set(__self__, "memory_limit_in_gb", memory_limit_in_gb)
         pulumi.set(__self__, "quantity", quantity)
         pulumi.set(__self__, "regions", regions)
 
     @property
     @pulumi.getter(name="memoryLimitInGb")
@@ -64,17 +63,14 @@
     @quantity.setter
     def quantity(self, value: pulumi.Input[int]):
         pulumi.set(self, "quantity", value)
 
     @property
     @pulumi.getter
     def regions(self) -> pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionCreationPlanRegionArgs']]]:
-        """
-        Deployment region as defined by cloud provider
-        """
         return pulumi.get(self, "regions")
 
     @regions.setter
     def regions(self, value: pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionCreationPlanRegionArgs']]]):
         pulumi.set(self, "regions", value)
 
 
@@ -147,25 +143,25 @@
 
 @pulumi.input_type
 class ActiveActiveSubscriptionDatabaseGlobalAlertArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  value: pulumi.Input[int]):
         """
-        :param pulumi.Input[str] name: Alert name
+        :param pulumi.Input[str] name: A meaningful name to identify the database
         :param pulumi.Input[int] value: Alert value
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
-        Alert name
+        A meaningful name to identify the database
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
@@ -187,15 +183,15 @@
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  override_global_alerts: Optional[pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionDatabaseOverrideRegionOverrideGlobalAlertArgs']]]] = None,
                  override_global_data_persistence: Optional[pulumi.Input[str]] = None,
                  override_global_password: Optional[pulumi.Input[str]] = None,
                  override_global_source_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        :param pulumi.Input[str] name: Alert name
+        :param pulumi.Input[str] name: Region name.
         :param pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionDatabaseOverrideRegionOverrideGlobalAlertArgs']]] override_global_alerts: A block defining Redis regional instance of an Active-Active database alert, documented below, can be specified multiple times
         :param pulumi.Input[str] override_global_data_persistence: Regional instance of an Active-Active database data persistence rate (in persistent storage)
         :param pulumi.Input[str] override_global_password: If specified, this regional instance of an Active-Active database password will be used to access the database
         :param pulumi.Input[Sequence[pulumi.Input[str]]] override_global_source_ips: List of regional instance of an Active-Active database source IP addresses or subnet masks. If specified, Redis clients will be able to connect to this database only from within the specified source IP addresses ranges (example: ['192.168.10.0/32', '192.168.12.0/24'] )
         """
         pulumi.set(__self__, "name", name)
         if override_global_alerts is not None:
@@ -207,15 +203,15 @@
         if override_global_source_ips is not None:
             pulumi.set(__self__, "override_global_source_ips", override_global_source_ips)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
-        Alert name
+        Region name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
@@ -513,15 +509,15 @@
 @pulumi.input_type
 class SubscriptionCloudProviderArgs:
     def __init__(__self__, *,
                  regions: pulumi.Input[Sequence[pulumi.Input['SubscriptionCloudProviderRegionArgs']]],
                  cloud_account_id: Optional[pulumi.Input[str]] = None,
                  provider: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['SubscriptionCloudProviderRegionArgs']]] regions: Deployment region as defined by cloud provider
+        :param pulumi.Input[Sequence[pulumi.Input['SubscriptionCloudProviderRegionArgs']]] regions: A region object, documented below
         :param pulumi.Input[str] cloud_account_id: Cloud account identifier. Default: Redis Labs internal cloud account
                (using Cloud Account ID = 1 implies using Redis Labs internal cloud account). Note that a GCP subscription can be created
                only with Redis Labs internal cloud account
         :param pulumi.Input[str] provider: The cloud provider to use with the subscription, (either `AWS` or `GCP`). Default: ‘AWS’
         """
         pulumi.set(__self__, "regions", regions)
         if cloud_account_id is not None:
@@ -529,15 +525,15 @@
         if provider is not None:
             pulumi.set(__self__, "provider", provider)
 
     @property
     @pulumi.getter
     def regions(self) -> pulumi.Input[Sequence[pulumi.Input['SubscriptionCloudProviderRegionArgs']]]:
         """
-        Deployment region as defined by cloud provider
+        A region object, documented below
         """
         return pulumi.get(self, "regions")
 
     @regions.setter
     def regions(self, value: pulumi.Input[Sequence[pulumi.Input['SubscriptionCloudProviderRegionArgs']]]):
         pulumi.set(self, "regions", value)
 
@@ -868,25 +864,25 @@
 
 @pulumi.input_type
 class SubscriptionDatabaseAlertArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  value: pulumi.Input[int]):
         """
-        :param pulumi.Input[str] name: Name of the Redis database module to enable
+        :param pulumi.Input[str] name: Alert name
         :param pulumi.Input[int] value: Alert value
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
-        Name of the Redis database module to enable
+        Alert name
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/_utilities.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/active_active_subscription.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/active_active_subscription_database.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,25 +28,25 @@
                  global_source_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  override_regions: Optional[pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionDatabaseOverrideRegionArgs']]]] = None,
                  support_oss_cluster_api: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ActiveActiveSubscriptionDatabase resource.
         :param pulumi.Input[float] memory_limit_in_gb: Maximum memory usage for this specific database, including replication and other overhead
-        :param pulumi.Input[int] subscription_id: Identifier of the subscription
+        :param pulumi.Input[int] subscription_id: The ID of the Active-Active subscription to create the database in
         :param pulumi.Input[str] client_ssl_certificate: SSL certificate to authenticate user connections.
         :param pulumi.Input[str] data_eviction: The data items eviction policy (either: 'allkeys-lru', 'allkeys-lfu', 'allkeys-random', 'volatile-lru', 'volatile-lfu', 'volatile-random', 'volatile-ttl' or 'noeviction'. Default: 'volatile-lru')
         :param pulumi.Input[bool] enable_tls: Use TLS for authentication. Default: ‘false’
         :param pulumi.Input[bool] external_endpoint_for_oss_cluster_api: Should use the external endpoint for open-source (OSS) Cluster API.
                Can only be enabled if OSS Cluster API support is enabled. Default: 'false'
         :param pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionDatabaseGlobalAlertArgs']]] global_alerts: A block defining Redis database alert of regions that dont override global settings, documented below, can be specified multiple times
         :param pulumi.Input[str] global_data_persistence: Global rate of database data persistence (in persistent storage) of regions that dont override global settings. Default: 'none'
         :param pulumi.Input[str] global_password: Password to access the database of regions that dont override global settings. If left empty, the password will be generated automatically
         :param pulumi.Input[Sequence[pulumi.Input[str]]] global_source_ips: List of source IP addresses or subnet masks of regions that dont override global settings. If specified, Redis clients will be able to connect to this database only from within the specified source IP addresses ranges (example: ['192.168.10.0/32', '192.168.12.0/24'])
-        :param pulumi.Input[str] name: Alert name
+        :param pulumi.Input[str] name: A meaningful name to identify the database
         :param pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionDatabaseOverrideRegionArgs']]] override_regions: Override region specific configuration, documented below
         :param pulumi.Input[bool] support_oss_cluster_api: Support Redis open-source (OSS) Cluster API. Default: ‘false’
         """
         pulumi.set(__self__, "memory_limit_in_gb", memory_limit_in_gb)
         pulumi.set(__self__, "subscription_id", subscription_id)
         if client_ssl_certificate is not None:
             pulumi.set(__self__, "client_ssl_certificate", client_ssl_certificate)
@@ -83,15 +83,15 @@
     def memory_limit_in_gb(self, value: pulumi.Input[float]):
         pulumi.set(self, "memory_limit_in_gb", value)
 
     @property
     @pulumi.getter(name="subscriptionId")
     def subscription_id(self) -> pulumi.Input[int]:
         """
-        Identifier of the subscription
+        The ID of the Active-Active subscription to create the database in
         """
         return pulumi.get(self, "subscription_id")
 
     @subscription_id.setter
     def subscription_id(self, value: pulumi.Input[int]):
         pulumi.set(self, "subscription_id", value)
 
@@ -192,15 +192,15 @@
     def global_source_ips(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "global_source_ips", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Alert name
+        A meaningful name to identify the database
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -257,19 +257,19 @@
         :param pulumi.Input[bool] external_endpoint_for_oss_cluster_api: Should use the external endpoint for open-source (OSS) Cluster API.
                Can only be enabled if OSS Cluster API support is enabled. Default: 'false'
         :param pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionDatabaseGlobalAlertArgs']]] global_alerts: A block defining Redis database alert of regions that dont override global settings, documented below, can be specified multiple times
         :param pulumi.Input[str] global_data_persistence: Global rate of database data persistence (in persistent storage) of regions that dont override global settings. Default: 'none'
         :param pulumi.Input[str] global_password: Password to access the database of regions that dont override global settings. If left empty, the password will be generated automatically
         :param pulumi.Input[Sequence[pulumi.Input[str]]] global_source_ips: List of source IP addresses or subnet masks of regions that dont override global settings. If specified, Redis clients will be able to connect to this database only from within the specified source IP addresses ranges (example: ['192.168.10.0/32', '192.168.12.0/24'])
         :param pulumi.Input[float] memory_limit_in_gb: Maximum memory usage for this specific database, including replication and other overhead
-        :param pulumi.Input[str] name: Alert name
+        :param pulumi.Input[str] name: A meaningful name to identify the database
         :param pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionDatabaseOverrideRegionArgs']]] override_regions: Override region specific configuration, documented below
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] private_endpoint: A map of which private endpoints can to access the database per region, uses region name as key.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] public_endpoint: A map of which public endpoints can to access the database per region, uses region name as key.
-        :param pulumi.Input[int] subscription_id: Identifier of the subscription
+        :param pulumi.Input[int] subscription_id: The ID of the Active-Active subscription to create the database in
         :param pulumi.Input[bool] support_oss_cluster_api: Support Redis open-source (OSS) Cluster API. Default: ‘false’
         """
         if client_ssl_certificate is not None:
             pulumi.set(__self__, "client_ssl_certificate", client_ssl_certificate)
         if data_eviction is not None:
             pulumi.set(__self__, "data_eviction", data_eviction)
         if db_id is not None:
@@ -422,15 +422,15 @@
     def memory_limit_in_gb(self, value: Optional[pulumi.Input[float]]):
         pulumi.set(self, "memory_limit_in_gb", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Alert name
+        A meaningful name to identify the database
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -470,15 +470,15 @@
     def public_endpoint(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "public_endpoint", value)
 
     @property
     @pulumi.getter(name="subscriptionId")
     def subscription_id(self) -> Optional[pulumi.Input[int]]:
         """
-        Identifier of the subscription
+        The ID of the Active-Active subscription to create the database in
         """
         return pulumi.get(self, "subscription_id")
 
     @subscription_id.setter
     def subscription_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "subscription_id", value)
 
@@ -535,17 +535,17 @@
         :param pulumi.Input[bool] external_endpoint_for_oss_cluster_api: Should use the external endpoint for open-source (OSS) Cluster API.
                Can only be enabled if OSS Cluster API support is enabled. Default: 'false'
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionDatabaseGlobalAlertArgs']]]] global_alerts: A block defining Redis database alert of regions that dont override global settings, documented below, can be specified multiple times
         :param pulumi.Input[str] global_data_persistence: Global rate of database data persistence (in persistent storage) of regions that dont override global settings. Default: 'none'
         :param pulumi.Input[str] global_password: Password to access the database of regions that dont override global settings. If left empty, the password will be generated automatically
         :param pulumi.Input[Sequence[pulumi.Input[str]]] global_source_ips: List of source IP addresses or subnet masks of regions that dont override global settings. If specified, Redis clients will be able to connect to this database only from within the specified source IP addresses ranges (example: ['192.168.10.0/32', '192.168.12.0/24'])
         :param pulumi.Input[float] memory_limit_in_gb: Maximum memory usage for this specific database, including replication and other overhead
-        :param pulumi.Input[str] name: Alert name
+        :param pulumi.Input[str] name: A meaningful name to identify the database
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionDatabaseOverrideRegionArgs']]]] override_regions: Override region specific configuration, documented below
-        :param pulumi.Input[int] subscription_id: Identifier of the subscription
+        :param pulumi.Input[int] subscription_id: The ID of the Active-Active subscription to create the database in
         :param pulumi.Input[bool] support_oss_cluster_api: Support Redis open-source (OSS) Cluster API. Default: ‘false’
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ActiveActiveSubscriptionDatabaseArgs,
@@ -602,28 +602,30 @@
 
             __props__.__dict__["client_ssl_certificate"] = client_ssl_certificate
             __props__.__dict__["data_eviction"] = data_eviction
             __props__.__dict__["enable_tls"] = enable_tls
             __props__.__dict__["external_endpoint_for_oss_cluster_api"] = external_endpoint_for_oss_cluster_api
             __props__.__dict__["global_alerts"] = global_alerts
             __props__.__dict__["global_data_persistence"] = global_data_persistence
-            __props__.__dict__["global_password"] = global_password
+            __props__.__dict__["global_password"] = None if global_password is None else pulumi.Output.secret(global_password)
             __props__.__dict__["global_source_ips"] = global_source_ips
             if memory_limit_in_gb is None and not opts.urn:
                 raise TypeError("Missing required property 'memory_limit_in_gb'")
             __props__.__dict__["memory_limit_in_gb"] = memory_limit_in_gb
             __props__.__dict__["name"] = name
             __props__.__dict__["override_regions"] = override_regions
             if subscription_id is None and not opts.urn:
                 raise TypeError("Missing required property 'subscription_id'")
             __props__.__dict__["subscription_id"] = subscription_id
             __props__.__dict__["support_oss_cluster_api"] = support_oss_cluster_api
             __props__.__dict__["db_id"] = None
             __props__.__dict__["private_endpoint"] = None
             __props__.__dict__["public_endpoint"] = None
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["globalPassword"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(ActiveActiveSubscriptionDatabase, __self__).__init__(
             'rediscloud:index/activeActiveSubscriptionDatabase:ActiveActiveSubscriptionDatabase',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -660,19 +662,19 @@
         :param pulumi.Input[bool] external_endpoint_for_oss_cluster_api: Should use the external endpoint for open-source (OSS) Cluster API.
                Can only be enabled if OSS Cluster API support is enabled. Default: 'false'
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionDatabaseGlobalAlertArgs']]]] global_alerts: A block defining Redis database alert of regions that dont override global settings, documented below, can be specified multiple times
         :param pulumi.Input[str] global_data_persistence: Global rate of database data persistence (in persistent storage) of regions that dont override global settings. Default: 'none'
         :param pulumi.Input[str] global_password: Password to access the database of regions that dont override global settings. If left empty, the password will be generated automatically
         :param pulumi.Input[Sequence[pulumi.Input[str]]] global_source_ips: List of source IP addresses or subnet masks of regions that dont override global settings. If specified, Redis clients will be able to connect to this database only from within the specified source IP addresses ranges (example: ['192.168.10.0/32', '192.168.12.0/24'])
         :param pulumi.Input[float] memory_limit_in_gb: Maximum memory usage for this specific database, including replication and other overhead
-        :param pulumi.Input[str] name: Alert name
+        :param pulumi.Input[str] name: A meaningful name to identify the database
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionDatabaseOverrideRegionArgs']]]] override_regions: Override region specific configuration, documented below
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] private_endpoint: A map of which private endpoints can to access the database per region, uses region name as key.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] public_endpoint: A map of which public endpoints can to access the database per region, uses region name as key.
-        :param pulumi.Input[int] subscription_id: Identifier of the subscription
+        :param pulumi.Input[int] subscription_id: The ID of the Active-Active subscription to create the database in
         :param pulumi.Input[bool] support_oss_cluster_api: Support Redis open-source (OSS) Cluster API. Default: ‘false’
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ActiveActiveSubscriptionDatabaseState.__new__(_ActiveActiveSubscriptionDatabaseState)
 
         __props__.__dict__["client_ssl_certificate"] = client_ssl_certificate
@@ -774,15 +776,15 @@
         """
         return pulumi.get(self, "memory_limit_in_gb")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Alert name
+        A meaningful name to identify the database
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="overrideRegions")
     def override_regions(self) -> pulumi.Output[Optional[Sequence['outputs.ActiveActiveSubscriptionDatabaseOverrideRegion']]]:
         """
@@ -806,15 +808,15 @@
         """
         return pulumi.get(self, "public_endpoint")
 
     @property
     @pulumi.getter(name="subscriptionId")
     def subscription_id(self) -> pulumi.Output[int]:
         """
-        Identifier of the subscription
+        The ID of the Active-Active subscription to create the database in
         """
         return pulumi.get(self, "subscription_id")
 
     @property
     @pulumi.getter(name="supportOssClusterApi")
     def support_oss_cluster_api(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/active_active_subscription_peering.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription_peering.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
         :param pulumi.Input[str] gcp_network_name: The name of the network to be peered
         :param pulumi.Input[str] gcp_peering_id: Identifier of the cloud peering
         :param pulumi.Input[str] gcp_project_id: GCP project ID that the VPC to be peered lives in
         :param pulumi.Input[str] gcp_redis_network_name: The name of the Redis Enterprise Cloud network to be peered
         :param pulumi.Input[str] gcp_redis_project_id: Identifier of the Redis Enterprise Cloud GCP project to be peered
         :param pulumi.Input[str] provider_name: The cloud provider to use with the vpc peering, (either `AWS` or `GCP`). Default: ‘AWS’
         :param pulumi.Input[str] source_region: Name of the region to create the VPC peering from
-        :param pulumi.Input[str] status: Current status of the account - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`
+        :param pulumi.Input[str] status: is set to the current status of the peering - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`.
         :param pulumi.Input[str] subscription_id: A valid Active-Active subscription predefined in the current account
         :param pulumi.Input[str] vpc_cidr: CIDR range of the VPC to be peered
         :param pulumi.Input[str] vpc_id: Identifier of the VPC to be peered
         """
         if aws_account_id is not None:
             pulumi.set(__self__, "aws_account_id", aws_account_id)
         if aws_peering_id is not None:
@@ -345,15 +345,15 @@
     def source_region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "source_region", value)
 
     @property
     @pulumi.getter
     def status(self) -> Optional[pulumi.Input[str]]:
         """
-        Current status of the account - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`
+        is set to the current status of the peering - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`.
         """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
@@ -635,15 +635,15 @@
         :param pulumi.Input[str] gcp_network_name: The name of the network to be peered
         :param pulumi.Input[str] gcp_peering_id: Identifier of the cloud peering
         :param pulumi.Input[str] gcp_project_id: GCP project ID that the VPC to be peered lives in
         :param pulumi.Input[str] gcp_redis_network_name: The name of the Redis Enterprise Cloud network to be peered
         :param pulumi.Input[str] gcp_redis_project_id: Identifier of the Redis Enterprise Cloud GCP project to be peered
         :param pulumi.Input[str] provider_name: The cloud provider to use with the vpc peering, (either `AWS` or `GCP`). Default: ‘AWS’
         :param pulumi.Input[str] source_region: Name of the region to create the VPC peering from
-        :param pulumi.Input[str] status: Current status of the account - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`
+        :param pulumi.Input[str] status: is set to the current status of the peering - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`.
         :param pulumi.Input[str] subscription_id: A valid Active-Active subscription predefined in the current account
         :param pulumi.Input[str] vpc_cidr: CIDR range of the VPC to be peered
         :param pulumi.Input[str] vpc_id: Identifier of the VPC to be peered
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ActiveActiveSubscriptionPeeringState.__new__(_ActiveActiveSubscriptionPeeringState)
@@ -744,15 +744,15 @@
         """
         return pulumi.get(self, "source_region")
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Output[str]:
         """
-        Current status of the account - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`
+        is set to the current status of the peering - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`.
         """
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter(name="subscriptionId")
     def subscription_id(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/active_active_subscription_regions.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/active_active_subscription_regions.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 class ActiveActiveSubscriptionRegionsArgs:
     def __init__(__self__, *,
                  regions: pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionRegionsRegionArgs']]],
                  subscription_id: pulumi.Input[str],
                  delete_regions: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ActiveActiveSubscriptionRegions resource.
-        :param pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionRegionsRegionArgs']]] regions: Region name
+        :param pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionRegionsRegionArgs']]] regions: Cloud networking details, per region, documented below
         :param pulumi.Input[str] subscription_id: ID of the subscription that the regions belong to
         :param pulumi.Input[bool] delete_regions: Flag required to be set when one or more regions is to be deleted, if the flag is not set an error will be thrown
         """
         pulumi.set(__self__, "regions", regions)
         pulumi.set(__self__, "subscription_id", subscription_id)
         if delete_regions is not None:
             pulumi.set(__self__, "delete_regions", delete_regions)
 
     @property
     @pulumi.getter
     def regions(self) -> pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionRegionsRegionArgs']]]:
         """
-        Region name
+        Cloud networking details, per region, documented below
         """
         return pulumi.get(self, "regions")
 
     @regions.setter
     def regions(self, value: pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionRegionsRegionArgs']]]):
         pulumi.set(self, "regions", value)
 
@@ -72,15 +72,15 @@
     def __init__(__self__, *,
                  delete_regions: Optional[pulumi.Input[bool]] = None,
                  regions: Optional[pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionRegionsRegionArgs']]]] = None,
                  subscription_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ActiveActiveSubscriptionRegions resources.
         :param pulumi.Input[bool] delete_regions: Flag required to be set when one or more regions is to be deleted, if the flag is not set an error will be thrown
-        :param pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionRegionsRegionArgs']]] regions: Region name
+        :param pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionRegionsRegionArgs']]] regions: Cloud networking details, per region, documented below
         :param pulumi.Input[str] subscription_id: ID of the subscription that the regions belong to
         """
         if delete_regions is not None:
             pulumi.set(__self__, "delete_regions", delete_regions)
         if regions is not None:
             pulumi.set(__self__, "regions", regions)
         if subscription_id is not None:
@@ -98,15 +98,15 @@
     def delete_regions(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "delete_regions", value)
 
     @property
     @pulumi.getter
     def regions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionRegionsRegionArgs']]]]:
         """
-        Region name
+        Cloud networking details, per region, documented below
         """
         return pulumi.get(self, "regions")
 
     @regions.setter
     def regions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionRegionsRegionArgs']]]]):
         pulumi.set(self, "regions", value)
 
@@ -177,15 +177,15 @@
         ```sh
          $ pulumi import rediscloud:index/activeActiveSubscriptionRegions:ActiveActiveSubscriptionRegions regions-resource 12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] delete_regions: Flag required to be set when one or more regions is to be deleted, if the flag is not set an error will be thrown
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionRegionsRegionArgs']]]] regions: Region name
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionRegionsRegionArgs']]]] regions: Cloud networking details, per region, documented below
         :param pulumi.Input[str] subscription_id: ID of the subscription that the regions belong to
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ActiveActiveSubscriptionRegionsArgs,
@@ -287,15 +287,15 @@
         Get an existing ActiveActiveSubscriptionRegions resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] delete_regions: Flag required to be set when one or more regions is to be deleted, if the flag is not set an error will be thrown
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionRegionsRegionArgs']]]] regions: Region name
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionRegionsRegionArgs']]]] regions: Cloud networking details, per region, documented below
         :param pulumi.Input[str] subscription_id: ID of the subscription that the regions belong to
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ActiveActiveSubscriptionRegionsState.__new__(_ActiveActiveSubscriptionRegionsState)
 
         __props__.__dict__["delete_regions"] = delete_regions
@@ -311,15 +311,15 @@
         """
         return pulumi.get(self, "delete_regions")
 
     @property
     @pulumi.getter
     def regions(self) -> pulumi.Output[Sequence['outputs.ActiveActiveSubscriptionRegionsRegion']]:
         """
-        Region name
+        Cloud networking details, per region, documented below
         """
         return pulumi.get(self, "regions")
 
     @property
     @pulumi.getter(name="subscriptionId")
     def subscription_id(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/cloud_account.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/cloud_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,29 +371,31 @@
             __props__ = CloudAccountArgs.__new__(CloudAccountArgs)
 
             if access_key_id is None and not opts.urn:
                 raise TypeError("Missing required property 'access_key_id'")
             __props__.__dict__["access_key_id"] = access_key_id
             if access_secret_key is None and not opts.urn:
                 raise TypeError("Missing required property 'access_secret_key'")
-            __props__.__dict__["access_secret_key"] = access_secret_key
+            __props__.__dict__["access_secret_key"] = None if access_secret_key is None else pulumi.Output.secret(access_secret_key)
             if console_password is None and not opts.urn:
                 raise TypeError("Missing required property 'console_password'")
-            __props__.__dict__["console_password"] = console_password
+            __props__.__dict__["console_password"] = None if console_password is None else pulumi.Output.secret(console_password)
             if console_username is None and not opts.urn:
                 raise TypeError("Missing required property 'console_username'")
             __props__.__dict__["console_username"] = console_username
             __props__.__dict__["name"] = name
             if provider_type is None and not opts.urn:
                 raise TypeError("Missing required property 'provider_type'")
             __props__.__dict__["provider_type"] = provider_type
             if sign_in_login_url is None and not opts.urn:
                 raise TypeError("Missing required property 'sign_in_login_url'")
             __props__.__dict__["sign_in_login_url"] = sign_in_login_url
             __props__.__dict__["status"] = None
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["accessSecretKey", "consolePassword"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(CloudAccount, __self__).__init__(
             'rediscloud:index/cloudAccount:CloudAccount',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/config/vars.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/config/vars.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 class _ExportableConfig(types.ModuleType):
     @property
     def api_key(self) -> Optional[str]:
         """
         This is the Redis Cloud API key. It must be provided but can also be set by the `REDISCLOUD_ACCESS_KEY` environment
         variable.
         """
-        return __config__.get('apiKey')
+        return __config__.get('apiKey') or _utilities.get_env('REDISCLOUD_API_KEY')
 
     @property
     def secret_key(self) -> Optional[str]:
         """
         This is the Redis Cloud API secret key. It must be provided but can also be set by the `REDISCLOUD_SECRET_KEY`
         environment variable.
         """
-        return __config__.get('secretKey')
+        return __config__.get('secretKey') or _utilities.get_env('REDISCLOUD_SECRET_KEY')
 
     @property
     def url(self) -> Optional[str]:
         """
         This is the URL of Redis Cloud and will default to `https://api.redislabs.com/v1`. This can also be set by the
         `REDISCLOUD_URL` environment variable.
         """
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_cloud_account.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_cloud_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,17 @@
         if provider_type and not isinstance(provider_type, str):
             raise TypeError("Expected argument 'provider_type' to be a str")
         pulumi.set(__self__, "provider_type", provider_type)
 
     @property
     @pulumi.getter(name="accessKeyId")
     def access_key_id(self) -> str:
+        """
+        The access key ID associated with the cloud account
+        """
         return pulumi.get(self, "access_key_id")
 
     @property
     @pulumi.getter(name="excludeInternalAccount")
     def exclude_internal_account(self) -> Optional[bool]:
         return pulumi.get(self, "exclude_internal_account")
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_data_persistence.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_data_persistence.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,17 @@
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
 
     @property
     @pulumi.getter(name="dataPersistences")
     def data_persistences(self) -> Sequence['outputs.GetDataPersistenceDataPersistenceResult']:
+        """
+        A list of data persistence option that can be applied to subscription databases
+        """
         return pulumi.get(self, "data_persistences")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_database.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     def modules(self) -> Sequence['outputs.GetDatabaseModuleResult']:
         return pulumi.get(self, "modules")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
-        The name of the database
+        The alert name
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> str:
         """
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_database_modules.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_database_modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,17 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def modules(self) -> Sequence['outputs.GetDatabaseModulesModuleResult']:
+        """
+        A list of database modules.
+        """
         return pulumi.get(self, "modules")
 
 
 class AwaitableGetDatabaseModulesResult(GetDatabaseModulesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_payment_method.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_payment_method.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_regions.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_regions.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,19 +40,25 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="providerName")
     def provider_name(self) -> Optional[str]:
+        """
+        The identifier of the owning cloud provider, (either `AWS` or `GCP`)
+        """
         return pulumi.get(self, "provider_name")
 
     @property
     @pulumi.getter
     def regions(self) -> Sequence['outputs.GetRegionsRegionResult']:
+        """
+        A list of regions from either a single or multiple cloud providers.
+        """
         return pulumi.get(self, "regions")
 
 
 class AwaitableGetRegionsResult(GetRegionsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_subscription.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/get_subscription_peerings.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/get_subscription_peerings.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,19 +43,25 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def peerings(self) -> Sequence['outputs.GetSubscriptionPeeringsPeeringResult']:
+        """
+        A list of subscription peerings.
+        """
         return pulumi.get(self, "peerings")
 
     @property
     @pulumi.getter
     def status(self) -> Optional[str]:
+        """
+        Current status of the peering - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`.
+        """
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter(name="subscriptionId")
     def subscription_id(self) -> str:
         return pulumi.get(self, "subscription_id")
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/outputs.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     def __init__(__self__, *,
                  memory_limit_in_gb: float,
                  quantity: int,
                  regions: Sequence['outputs.ActiveActiveSubscriptionCreationPlanRegion']):
         """
         :param float memory_limit_in_gb: Maximum memory usage that will be used for your largest planned database, including replication and other overhead
         :param int quantity: The planned number of databases in the subscription.
-        :param Sequence['ActiveActiveSubscriptionCreationPlanRegionArgs'] regions: Deployment region as defined by cloud provider
         """
         pulumi.set(__self__, "memory_limit_in_gb", memory_limit_in_gb)
         pulumi.set(__self__, "quantity", quantity)
         pulumi.set(__self__, "regions", regions)
 
     @property
     @pulumi.getter(name="memoryLimitInGb")
@@ -83,17 +82,14 @@
         The planned number of databases in the subscription.
         """
         return pulumi.get(self, "quantity")
 
     @property
     @pulumi.getter
     def regions(self) -> Sequence['outputs.ActiveActiveSubscriptionCreationPlanRegion']:
-        """
-        Deployment region as defined by cloud provider
-        """
         return pulumi.get(self, "regions")
 
 
 @pulumi.output_type
 class ActiveActiveSubscriptionCreationPlanRegion(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -167,25 +163,25 @@
 
 @pulumi.output_type
 class ActiveActiveSubscriptionDatabaseGlobalAlert(dict):
     def __init__(__self__, *,
                  name: str,
                  value: int):
         """
-        :param str name: Alert name
+        :param str name: A meaningful name to identify the database
         :param int value: Alert value
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
-        Alert name
+        A meaningful name to identify the database
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def value(self) -> int:
         """
@@ -222,15 +218,15 @@
     def __init__(__self__, *,
                  name: str,
                  override_global_alerts: Optional[Sequence['outputs.ActiveActiveSubscriptionDatabaseOverrideRegionOverrideGlobalAlert']] = None,
                  override_global_data_persistence: Optional[str] = None,
                  override_global_password: Optional[str] = None,
                  override_global_source_ips: Optional[Sequence[str]] = None):
         """
-        :param str name: Alert name
+        :param str name: Region name.
         :param Sequence['ActiveActiveSubscriptionDatabaseOverrideRegionOverrideGlobalAlertArgs'] override_global_alerts: A block defining Redis regional instance of an Active-Active database alert, documented below, can be specified multiple times
         :param str override_global_data_persistence: Regional instance of an Active-Active database data persistence rate (in persistent storage)
         :param str override_global_password: If specified, this regional instance of an Active-Active database password will be used to access the database
         :param Sequence[str] override_global_source_ips: List of regional instance of an Active-Active database source IP addresses or subnet masks. If specified, Redis clients will be able to connect to this database only from within the specified source IP addresses ranges (example: ['192.168.10.0/32', '192.168.12.0/24'] )
         """
         pulumi.set(__self__, "name", name)
         if override_global_alerts is not None:
@@ -242,15 +238,15 @@
         if override_global_source_ips is not None:
             pulumi.set(__self__, "override_global_source_ips", override_global_source_ips)
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
-        Alert name
+        Region name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="overrideGlobalAlerts")
     def override_global_alerts(self) -> Optional[Sequence['outputs.ActiveActiveSubscriptionDatabaseOverrideRegionOverrideGlobalAlert']]:
         """
@@ -552,15 +548,15 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  regions: Sequence['outputs.SubscriptionCloudProviderRegion'],
                  cloud_account_id: Optional[str] = None,
                  provider: Optional[str] = None):
         """
-        :param Sequence['SubscriptionCloudProviderRegionArgs'] regions: Deployment region as defined by cloud provider
+        :param Sequence['SubscriptionCloudProviderRegionArgs'] regions: A region object, documented below
         :param str cloud_account_id: Cloud account identifier. Default: Redis Labs internal cloud account
                (using Cloud Account ID = 1 implies using Redis Labs internal cloud account). Note that a GCP subscription can be created
                only with Redis Labs internal cloud account
         :param str provider: The cloud provider to use with the subscription, (either `AWS` or `GCP`). Default: ‘AWS’
         """
         pulumi.set(__self__, "regions", regions)
         if cloud_account_id is not None:
@@ -568,15 +564,15 @@
         if provider is not None:
             pulumi.set(__self__, "provider", provider)
 
     @property
     @pulumi.getter
     def regions(self) -> Sequence['outputs.SubscriptionCloudProviderRegion']:
         """
-        Deployment region as defined by cloud provider
+        A region object, documented below
         """
         return pulumi.get(self, "regions")
 
     @property
     @pulumi.getter(name="cloudAccountId")
     def cloud_account_id(self) -> Optional[str]:
         """
@@ -896,25 +892,25 @@
 
 @pulumi.output_type
 class SubscriptionDatabaseAlert(dict):
     def __init__(__self__, *,
                  name: str,
                  value: int):
         """
-        :param str name: Name of the Redis database module to enable
+        :param str name: Alert name
         :param int value: Alert value
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
-        Name of the Redis database module to enable
+        Alert name
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def value(self) -> int:
         """
@@ -973,14 +969,15 @@
 @pulumi.output_type
 class GetDatabaseAlertResult(dict):
     def __init__(__self__, *,
                  name: str,
                  value: int):
         """
         :param str name: The name of the database to filter returned databases
+        :param int value: The alert value
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def name(self) -> str:
@@ -988,14 +985,17 @@
         The name of the database to filter returned databases
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def value(self) -> int:
+        """
+        The alert value
+        """
         return pulumi.get(self, "value")
 
 
 @pulumi.output_type
 class GetDatabaseModuleResult(dict):
     def __init__(__self__, *,
                  name: str):
@@ -1014,42 +1014,56 @@
 
 
 @pulumi.output_type
 class GetDatabaseModulesModuleResult(dict):
     def __init__(__self__, *,
                  description: str,
                  name: str):
+        """
+        :param str description: A meaningful description of the database module
+        :param str name: The identifier assigned by the database module
+        """
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def description(self) -> str:
+        """
+        A meaningful description of the database module
+        """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def name(self) -> str:
+        """
+        The identifier assigned by the database module
+        """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
 class GetRegionsRegionResult(dict):
     def __init__(__self__, *,
                  name: str,
                  provider_name: str):
         """
+        :param str name: The identifier assigned by the cloud provider, (for example `eu-west-1` for `AWS`)
         :param str provider_name: The name of the cloud provider to filter returned regions, (accepted values are `AWS` or `GCP`).
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "provider_name", provider_name)
 
     @property
     @pulumi.getter
     def name(self) -> str:
+        """
+        The identifier assigned by the cloud provider, (for example `eu-west-1` for `AWS`)
+        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="providerName")
     def provider_name(self) -> str:
         """
         The name of the cloud provider to filter returned regions, (accepted values are `AWS` or `GCP`).
@@ -1212,20 +1226,27 @@
                  peering_id: int,
                  provider_name: str,
                  region: str,
                  status: str,
                  vpc_cidr: str,
                  vpc_id: str):
         """
+        :param str aws_account_id: AWS account id that the VPC to be peered lives in
+        :param str aws_peering_id: Identifier of the AWS cloud peering
+        :param str gcp_network_name: The name of the network to be peered
         :param str gcp_peering_id: Identifier of the cloud peering
+        :param str gcp_project_id: GCP project ID that the VPC to be peered lives in
         :param str gcp_redis_network_name: The name of the Redis Enterprise Cloud network to be peered
+        :param str gcp_redis_project_id: Identifier of the Redis Enterprise Cloud GCP project to be peered
         :param int peering_id: ID of the subscription peering
         :param str provider_name: The name of the cloud provider. (either `AWS` or `GCP`)
-               * `status` Current status of the peering - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`.
+        :param str region: AWS Region that the VPC to be peered lives in
         :param str status: Current status of the peering - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`.
+        :param str vpc_cidr: CIDR range of the VPC to be peered
+        :param str vpc_id: Identifier of the VPC to be peered
         """
         pulumi.set(__self__, "aws_account_id", aws_account_id)
         pulumi.set(__self__, "aws_peering_id", aws_peering_id)
         pulumi.set(__self__, "gcp_network_name", gcp_network_name)
         pulumi.set(__self__, "gcp_peering_id", gcp_peering_id)
         pulumi.set(__self__, "gcp_project_id", gcp_project_id)
         pulumi.set(__self__, "gcp_redis_network_name", gcp_redis_network_name)
@@ -1236,50 +1257,65 @@
         pulumi.set(__self__, "status", status)
         pulumi.set(__self__, "vpc_cidr", vpc_cidr)
         pulumi.set(__self__, "vpc_id", vpc_id)
 
     @property
     @pulumi.getter(name="awsAccountId")
     def aws_account_id(self) -> str:
+        """
+        AWS account id that the VPC to be peered lives in
+        """
         return pulumi.get(self, "aws_account_id")
 
     @property
     @pulumi.getter(name="awsPeeringId")
     def aws_peering_id(self) -> str:
+        """
+        Identifier of the AWS cloud peering
+        """
         return pulumi.get(self, "aws_peering_id")
 
     @property
     @pulumi.getter(name="gcpNetworkName")
     def gcp_network_name(self) -> str:
+        """
+        The name of the network to be peered
+        """
         return pulumi.get(self, "gcp_network_name")
 
     @property
     @pulumi.getter(name="gcpPeeringId")
     def gcp_peering_id(self) -> str:
         """
         Identifier of the cloud peering
         """
         return pulumi.get(self, "gcp_peering_id")
 
     @property
     @pulumi.getter(name="gcpProjectId")
     def gcp_project_id(self) -> str:
+        """
+        GCP project ID that the VPC to be peered lives in
+        """
         return pulumi.get(self, "gcp_project_id")
 
     @property
     @pulumi.getter(name="gcpRedisNetworkName")
     def gcp_redis_network_name(self) -> str:
         """
         The name of the Redis Enterprise Cloud network to be peered
         """
         return pulumi.get(self, "gcp_redis_network_name")
 
     @property
     @pulumi.getter(name="gcpRedisProjectId")
     def gcp_redis_project_id(self) -> str:
+        """
+        Identifier of the Redis Enterprise Cloud GCP project to be peered
+        """
         return pulumi.get(self, "gcp_redis_project_id")
 
     @property
     @pulumi.getter(name="peeringId")
     def peering_id(self) -> int:
         """
         ID of the subscription peering
@@ -1287,35 +1323,43 @@
         return pulumi.get(self, "peering_id")
 
     @property
     @pulumi.getter(name="providerName")
     def provider_name(self) -> str:
         """
         The name of the cloud provider. (either `AWS` or `GCP`)
-        * `status` Current status of the peering - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`.
         """
         return pulumi.get(self, "provider_name")
 
     @property
     @pulumi.getter
     def region(self) -> str:
+        """
+        AWS Region that the VPC to be peered lives in
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
     def status(self) -> str:
         """
         Current status of the peering - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`.
         """
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter(name="vpcCidr")
     def vpc_cidr(self) -> str:
+        """
+        CIDR range of the VPC to be peered
+        """
         return pulumi.get(self, "vpc_cidr")
 
     @property
     @pulumi.getter(name="vpcId")
     def vpc_id(self) -> str:
+        """
+        Identifier of the VPC to be peered
+        """
         return pulumi.get(self, "vpc_id")
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/provider.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,16 +22,20 @@
         :param pulumi.Input[str] api_key: This is the Redis Cloud API key. It must be provided but can also be set by the `REDISCLOUD_ACCESS_KEY` environment
                variable.
         :param pulumi.Input[str] secret_key: This is the Redis Cloud API secret key. It must be provided but can also be set by the `REDISCLOUD_SECRET_KEY`
                environment variable.
         :param pulumi.Input[str] url: This is the URL of Redis Cloud and will default to `https://api.redislabs.com/v1`. This can also be set by the
                `REDISCLOUD_URL` environment variable.
         """
+        if api_key is None:
+            api_key = _utilities.get_env('REDISCLOUD_API_KEY')
         if api_key is not None:
             pulumi.set(__self__, "api_key", api_key)
+        if secret_key is None:
+            secret_key = _utilities.get_env('REDISCLOUD_SECRET_KEY')
         if secret_key is not None:
             pulumi.set(__self__, "secret_key", secret_key)
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter(name="apiKey")
@@ -132,17 +136,23 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
-            __props__.__dict__["api_key"] = api_key
-            __props__.__dict__["secret_key"] = secret_key
+            if api_key is None:
+                api_key = _utilities.get_env('REDISCLOUD_API_KEY')
+            __props__.__dict__["api_key"] = None if api_key is None else pulumi.Output.secret(api_key)
+            if secret_key is None:
+                secret_key = _utilities.get_env('REDISCLOUD_SECRET_KEY')
+            __props__.__dict__["secret_key"] = None if secret_key is None else pulumi.Output.secret(secret_key)
             __props__.__dict__["url"] = url
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["apiKey", "secretKey"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'rediscloud',
             resource_name,
             __props__,
             opts)
 
     @property
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/subscription.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/subscription_database.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/subscription_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         :param pulumi.Input[bool] enable_tls: Use TLS for authentication. Default: ‘false’
         :param pulumi.Input[bool] external_endpoint_for_oss_cluster_api: Should use the external endpoint for open-source (OSS) Cluster API.
                Can only be enabled if OSS Cluster API support is enabled. Default: 'false'
         :param pulumi.Input[Sequence[pulumi.Input[str]]] hashing_policies: List of regular expression rules to shard the database by. See
                [the documentation on clustering](https://docs.redislabs.com/latest/rc/concepts/clustering/) for more information on the
                hashing policy. This cannot be set when `support_oss_cluster_api` is set to true.
         :param pulumi.Input[Sequence[pulumi.Input['SubscriptionDatabaseModuleArgs']]] modules: A list of modules objects, documented below
-        :param pulumi.Input[str] name: Name of the Redis database module to enable
+        :param pulumi.Input[str] name: A meaningful name to identify the database
         :param pulumi.Input[str] password: Password to access the database. If omitted, a random 32 character long alphanumeric password will be automatically generated
         :param pulumi.Input[str] periodic_backup_path: Path that will be used to store database backup files
         :param pulumi.Input[Sequence[pulumi.Input[str]]] replica_ofs: Set of Redis database URIs, in the format `redis://user:password@host:port`, that this
                database will be a replica of. If the URI provided is Redis Labs Cloud instance, only host and port should be provided.
                Cannot be enabled when `support_oss_cluster_api` is enabled.
         :param pulumi.Input[bool] replication: Databases replication. Default: ‘true’
         :param pulumi.Input[Sequence[pulumi.Input[str]]] source_ips: List of source IP addresses or subnet masks. If specified, Redis clients will be able to connect to this database only from within the specified source IP addresses ranges (example: [‘192.168.10.0/32’, ‘192.168.12.0/24’])
@@ -277,15 +277,15 @@
     def modules(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SubscriptionDatabaseModuleArgs']]]]):
         pulumi.set(self, "modules", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the Redis database module to enable
+        A meaningful name to identify the database
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -404,15 +404,15 @@
         :param pulumi.Input[bool] external_endpoint_for_oss_cluster_api: Should use the external endpoint for open-source (OSS) Cluster API.
                Can only be enabled if OSS Cluster API support is enabled. Default: 'false'
         :param pulumi.Input[Sequence[pulumi.Input[str]]] hashing_policies: List of regular expression rules to shard the database by. See
                [the documentation on clustering](https://docs.redislabs.com/latest/rc/concepts/clustering/) for more information on the
                hashing policy. This cannot be set when `support_oss_cluster_api` is set to true.
         :param pulumi.Input[float] memory_limit_in_gb: Maximum memory usage for this specific database
         :param pulumi.Input[Sequence[pulumi.Input['SubscriptionDatabaseModuleArgs']]] modules: A list of modules objects, documented below
-        :param pulumi.Input[str] name: Name of the Redis database module to enable
+        :param pulumi.Input[str] name: A meaningful name to identify the database
         :param pulumi.Input[str] password: Password to access the database. If omitted, a random 32 character long alphanumeric password will be automatically generated
         :param pulumi.Input[str] periodic_backup_path: Path that will be used to store database backup files
         :param pulumi.Input[str] private_endpoint: Private endpoint to access the database
         :param pulumi.Input[str] protocol: The protocol that will be used to access the database, (either ‘redis’ or 'memcached’) Default: ‘redis’
         :param pulumi.Input[str] public_endpoint: Public endpoint to access the database
         :param pulumi.Input[Sequence[pulumi.Input[str]]] replica_ofs: Set of Redis database URIs, in the format `redis://user:password@host:port`, that this
                database will be a replica of. If the URI provided is Redis Labs Cloud instance, only host and port should be provided.
@@ -609,15 +609,15 @@
     def modules(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SubscriptionDatabaseModuleArgs']]]]):
         pulumi.set(self, "modules", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the Redis database module to enable
+        A meaningful name to identify the database
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -818,15 +818,15 @@
         :param pulumi.Input[bool] external_endpoint_for_oss_cluster_api: Should use the external endpoint for open-source (OSS) Cluster API.
                Can only be enabled if OSS Cluster API support is enabled. Default: 'false'
         :param pulumi.Input[Sequence[pulumi.Input[str]]] hashing_policies: List of regular expression rules to shard the database by. See
                [the documentation on clustering](https://docs.redislabs.com/latest/rc/concepts/clustering/) for more information on the
                hashing policy. This cannot be set when `support_oss_cluster_api` is set to true.
         :param pulumi.Input[float] memory_limit_in_gb: Maximum memory usage for this specific database
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SubscriptionDatabaseModuleArgs']]]] modules: A list of modules objects, documented below
-        :param pulumi.Input[str] name: Name of the Redis database module to enable
+        :param pulumi.Input[str] name: A meaningful name to identify the database
         :param pulumi.Input[str] password: Password to access the database. If omitted, a random 32 character long alphanumeric password will be automatically generated
         :param pulumi.Input[str] periodic_backup_path: Path that will be used to store database backup files
         :param pulumi.Input[str] protocol: The protocol that will be used to access the database, (either ‘redis’ or 'memcached’) Default: ‘redis’
         :param pulumi.Input[Sequence[pulumi.Input[str]]] replica_ofs: Set of Redis database URIs, in the format `redis://user:password@host:port`, that this
                database will be a replica of. If the URI provided is Redis Labs Cloud instance, only host and port should be provided.
                Cannot be enabled when `support_oss_cluster_api` is enabled.
         :param pulumi.Input[bool] replication: Databases replication. Default: ‘true’
@@ -907,15 +907,15 @@
             __props__.__dict__["external_endpoint_for_oss_cluster_api"] = external_endpoint_for_oss_cluster_api
             __props__.__dict__["hashing_policies"] = hashing_policies
             if memory_limit_in_gb is None and not opts.urn:
                 raise TypeError("Missing required property 'memory_limit_in_gb'")
             __props__.__dict__["memory_limit_in_gb"] = memory_limit_in_gb
             __props__.__dict__["modules"] = modules
             __props__.__dict__["name"] = name
-            __props__.__dict__["password"] = password
+            __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
             __props__.__dict__["periodic_backup_path"] = periodic_backup_path
             if protocol is None and not opts.urn:
                 raise TypeError("Missing required property 'protocol'")
             __props__.__dict__["protocol"] = protocol
             __props__.__dict__["replica_ofs"] = replica_ofs
             __props__.__dict__["replication"] = replication
             __props__.__dict__["source_ips"] = source_ips
@@ -928,14 +928,16 @@
             __props__.__dict__["throughput_measurement_by"] = throughput_measurement_by
             if throughput_measurement_value is None and not opts.urn:
                 raise TypeError("Missing required property 'throughput_measurement_value'")
             __props__.__dict__["throughput_measurement_value"] = throughput_measurement_value
             __props__.__dict__["db_id"] = None
             __props__.__dict__["private_endpoint"] = None
             __props__.__dict__["public_endpoint"] = None
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(SubscriptionDatabase, __self__).__init__(
             'rediscloud:index/subscriptionDatabase:SubscriptionDatabase',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -984,15 +986,15 @@
         :param pulumi.Input[bool] external_endpoint_for_oss_cluster_api: Should use the external endpoint for open-source (OSS) Cluster API.
                Can only be enabled if OSS Cluster API support is enabled. Default: 'false'
         :param pulumi.Input[Sequence[pulumi.Input[str]]] hashing_policies: List of regular expression rules to shard the database by. See
                [the documentation on clustering](https://docs.redislabs.com/latest/rc/concepts/clustering/) for more information on the
                hashing policy. This cannot be set when `support_oss_cluster_api` is set to true.
         :param pulumi.Input[float] memory_limit_in_gb: Maximum memory usage for this specific database
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SubscriptionDatabaseModuleArgs']]]] modules: A list of modules objects, documented below
-        :param pulumi.Input[str] name: Name of the Redis database module to enable
+        :param pulumi.Input[str] name: A meaningful name to identify the database
         :param pulumi.Input[str] password: Password to access the database. If omitted, a random 32 character long alphanumeric password will be automatically generated
         :param pulumi.Input[str] periodic_backup_path: Path that will be used to store database backup files
         :param pulumi.Input[str] private_endpoint: Private endpoint to access the database
         :param pulumi.Input[str] protocol: The protocol that will be used to access the database, (either ‘redis’ or 'memcached’) Default: ‘redis’
         :param pulumi.Input[str] public_endpoint: Public endpoint to access the database
         :param pulumi.Input[Sequence[pulumi.Input[str]]] replica_ofs: Set of Redis database URIs, in the format `redis://user:password@host:port`, that this
                database will be a replica of. If the URI provided is Redis Labs Cloud instance, only host and port should be provided.
@@ -1126,15 +1128,15 @@
         """
         return pulumi.get(self, "modules")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Name of the Redis database module to enable
+        A meaningful name to identify the database
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud/subscription_peering.py` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud/subscription_peering.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         :param pulumi.Input[str] gcp_network_name: The name of the network to be peered
         :param pulumi.Input[str] gcp_peering_id: Identifier of the cloud peering
         :param pulumi.Input[str] gcp_project_id: GCP project ID that the VPC to be peered lives in
         :param pulumi.Input[str] gcp_redis_network_name: The name of the Redis Enterprise Cloud network to be peered
         :param pulumi.Input[str] gcp_redis_project_id: Identifier of the Redis Enterprise Cloud GCP project to be peered
         :param pulumi.Input[str] provider_name: The cloud provider to use with the vpc peering, (either `AWS` or `GCP`). Default: ‘AWS’
         :param pulumi.Input[str] region: AWS Region that the VPC to be peered lives in
-        :param pulumi.Input[str] status: Current status of the account - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`
+        :param pulumi.Input[str] status: is set to the current status of the peering - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`.
         :param pulumi.Input[str] subscription_id: A valid subscription predefined in the current account
         :param pulumi.Input[str] vpc_cidr: CIDR range of the VPC to be peered
         :param pulumi.Input[str] vpc_id: Identifier of the VPC to be peered
         """
         if aws_account_id is not None:
             pulumi.set(__self__, "aws_account_id", aws_account_id)
         if aws_peering_id is not None:
@@ -313,15 +313,15 @@
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter
     def status(self) -> Optional[pulumi.Input[str]]:
         """
-        Current status of the account - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`
+        is set to the current status of the peering - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`.
         """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
@@ -595,15 +595,15 @@
         :param pulumi.Input[str] gcp_network_name: The name of the network to be peered
         :param pulumi.Input[str] gcp_peering_id: Identifier of the cloud peering
         :param pulumi.Input[str] gcp_project_id: GCP project ID that the VPC to be peered lives in
         :param pulumi.Input[str] gcp_redis_network_name: The name of the Redis Enterprise Cloud network to be peered
         :param pulumi.Input[str] gcp_redis_project_id: Identifier of the Redis Enterprise Cloud GCP project to be peered
         :param pulumi.Input[str] provider_name: The cloud provider to use with the vpc peering, (either `AWS` or `GCP`). Default: ‘AWS’
         :param pulumi.Input[str] region: AWS Region that the VPC to be peered lives in
-        :param pulumi.Input[str] status: Current status of the account - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`
+        :param pulumi.Input[str] status: is set to the current status of the peering - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`.
         :param pulumi.Input[str] subscription_id: A valid subscription predefined in the current account
         :param pulumi.Input[str] vpc_cidr: CIDR range of the VPC to be peered
         :param pulumi.Input[str] vpc_id: Identifier of the VPC to be peered
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SubscriptionPeeringState.__new__(_SubscriptionPeeringState)
@@ -695,15 +695,15 @@
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Output[str]:
         """
-        Current status of the account - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`
+        is set to the current status of the peering - `initiating-request`, `pending-acceptance`, `active`, `inactive` or `failed`.
         """
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter(name="subscriptionId")
     def subscription_id(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud.egg-info/PKG-INFO` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,57 @@
 Metadata-Version: 2.1
 Name: pulumi-rediscloud
-Version: 1.1.1
+Version: 1.2.0
 Summary: A Pulumi package for creating and managing rediscloud cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/RedisLabs/pulumi-rediscloud
 Keywords: pulumi rediscloud category/cloud
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Redis Cloud Resource Provider
 
-The Redis Cloud Resource Provider lets you manage [Redis Cloud](https://redislabs.com/redis-enterprise-cloud/overview) resources.
+The Redis Cloud Resource Provider lets you manage [Redis Cloud](https://redislabs.com/redis-enterprise-cloud/overview) resources. The provider is used to interact with the resources supported by Redis Enterprise Cloud. Please note that the provider is available only for Flexible or Annual subscriptions. It is not supported for Fixed or Free subscriptions.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @RedisLabs/pulumi-rediscloud
+npm install @rediscloud/pulumi-rediscloud
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @RedisLabs/pulumi-rediscloud
+yarn add @rediscloud/pulumi-rediscloud
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
-pip install redislabs_pulumi_rediscloud
+pip install pulumi_rediscloud
 ```
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library:
 
 ```bash
 go get github.com/RedisLabs/pulumi-rediscloud/sdk/go/...
 ```
 
-### .NET
-
-To use from .NET, install using `dotnet add package`:
-
-```bash
-dotnet add package RedisLabs.PulumiRedisCloud
-```
-
 ## Configuration
 
 The following configuration points are available for the `rediscloud` provider:
 
 - `apiKey` (environment: `REDISCLOUD_ACCESS_KEY`) - This is the Redis Enterprise Cloud API account key. It must be provided but can also be set by the environment variable.
 - `secretKey` (environment: `REDISCLOUD_SECRET_KEY`) - This is the Redis Enterprise Cloud API secret key. It must be provided but can also be set by the environment variable.
```

### Comparing `pulumi_rediscloud-1.1.1/pulumi_rediscloud.egg-info/SOURCES.txt` & `pulumi_rediscloud-1.2.0/pulumi_rediscloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.1.1/setup.py` & `pulumi_rediscloud-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.1.1"
-PLUGIN_VERSION = "1.1.1"
+VERSION = "1.2.0"
+PLUGIN_VERSION = "1.2.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'rediscloud', PLUGIN_VERSION, '--server', 'github://api.github.com/RedisLabs/pulumi-rediscloud'])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "rediscloud Pulumi Package - Development Version"
 
 
 setup(name='pulumi_rediscloud',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing rediscloud cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

