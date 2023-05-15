# Comparing `tmp/pulumi_docker-4.3.0a1683956242.tar.gz` & `tmp/pulumi_docker-4.3.0a1684184527.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_docker-4.3.0a1683956242.tar", last modified: Sat May 13 05:44:39 2023, max compression
+gzip compressed data, was "pulumi_docker-4.3.0a1684184527.tar", last modified: Mon May 15 21:07:30 2023, max compression
```

## Comparing `pulumi_docker-4.3.0a1683956242.tar` & `pulumi_docker-4.3.0a1684184527.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 05:44:39.687241 pulumi_docker-4.3.0a1683956242/
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-13 05:44:39.687241 pulumi_docker-4.3.0a1683956242/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 05:44:39.687241 pulumi_docker-4.3.0a1683956242/pulumi_docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)   153875 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 05:44:39.687241 pulumi_docker-4.3.0a1683956242/pulumi_docker/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)   155376 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/get_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/get_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/get_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/get_registry_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/get_remote_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15590 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    32844 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/network.py
--rw-r--r--   0 runner    (1001) docker     (123)   125340 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/registry_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/remote_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    25797 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 05:44:39.687241 pulumi_docker-4.3.0a1683956242/pulumi_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/pulumi_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 05:44:39.687241 pulumi_docker-4.3.0a1683956242/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-13 05:44:39.000000 pulumi_docker-4.3.0a1683956242/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:07:30.211718 pulumi_docker-4.3.0a1684184527/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-15 21:07:30.211718 pulumi_docker-4.3.0a1684184527/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:07:30.211718 pulumi_docker-4.3.0a1684184527/pulumi_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153875 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:07:30.211718 pulumi_docker-4.3.0a1684184527/pulumi_docker/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155250 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/get_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/get_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/get_registry_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/get_remote_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15590 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32844 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125340 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/registry_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/remote_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25797 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:07:30.211718 pulumi_docker-4.3.0a1684184527/pulumi_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/pulumi_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:07:30.211718 pulumi_docker-4.3.0a1684184527/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-15 21:07:30.000000 pulumi_docker-4.3.0a1684184527/setup.py
```

### Comparing `pulumi_docker-4.3.0a1683956242/PKG-INFO` & `pulumi_docker-4.3.0a1684184527/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_docker
-Version: 4.3.0a1683956242
+Version: 4.3.0a1684184527
 Summary: A Pulumi package for interacting with Docker in Pulumi programs
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-docker
 Keywords: pulumi docker
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_docker-4.3.0a1683956242/README.md` & `pulumi_docker-4.3.0a1684184527/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/__init__.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/_enums.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/_inputs.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/_utilities.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/config/outputs.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/config/vars.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/container.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,15 @@
         :param pulumi.Input[str] ipc_mode: IPC sharing mode for the container. Possible values are: `none`, `private`, `shareable`, `container:<name|id>` or `host`.
         :param pulumi.Input[Sequence[pulumi.Input['ContainerLabelArgs']]] labels: User-defined key/value metadata
         :param pulumi.Input[str] log_driver: The logging driver to use for the container.
         :param pulumi.Input[Mapping[str, Any]] log_opts: Key/value pairs to use as options for the logging driver.
         :param pulumi.Input[bool] logs: Save the container logs (`attach` must be enabled). Defaults to `false`.
         :param pulumi.Input[int] max_retry_count: The maximum amount of times to an attempt a restart when `restart` is set to 'on-failure'.
         :param pulumi.Input[int] memory: The memory limit for the container in MBs.
-        :param pulumi.Input[int] memory_swap: The total memory limit (memory + swap) for the container in MBs. This setting may compute to `-1` after `terraform
-               apply` if the target host doesn't support memory swap, when that is the case docker will use a soft limitation.
+        :param pulumi.Input[int] memory_swap: The total memory limit (memory + swap) for the container in MBs. This setting may compute to `-1` after `pulumi up` if the target host doesn't support memory swap, when that is the case docker will use a soft limitation.
         :param pulumi.Input[Sequence[pulumi.Input['ContainerMountArgs']]] mounts: Specification for mounts to be added to containers created as part of the service.
         :param pulumi.Input[bool] must_run: If `true`, then the Docker container will be kept running. If `false`, then as long as the container exists, Terraform
                assumes it is successful. Defaults to `true`.
         :param pulumi.Input[str] name: The name of the container.
         :param pulumi.Input[str] network_mode: Network mode of the container.
         :param pulumi.Input[Sequence[pulumi.Input['ContainerNetworksAdvancedArgs']]] networks_advanced: The networks the container is attached to
         :param pulumi.Input[str] pid_mode: he PID (Process) Namespace mode for the container. Either `container:<name|id>` or `host`.
@@ -617,16 +616,15 @@
     def memory(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "memory", value)
 
     @property
     @pulumi.getter(name="memorySwap")
     def memory_swap(self) -> Optional[pulumi.Input[int]]:
         """
-        The total memory limit (memory + swap) for the container in MBs. This setting may compute to `-1` after `terraform
-        apply` if the target host doesn't support memory swap, when that is the case docker will use a soft limitation.
+        The total memory limit (memory + swap) for the container in MBs. This setting may compute to `-1` after `pulumi up` if the target host doesn't support memory swap, when that is the case docker will use a soft limitation.
         """
         return pulumi.get(self, "memory_swap")
 
     @memory_swap.setter
     def memory_swap(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "memory_swap", value)
 
@@ -1115,16 +1113,15 @@
         :param pulumi.Input[str] ipc_mode: IPC sharing mode for the container. Possible values are: `none`, `private`, `shareable`, `container:<name|id>` or `host`.
         :param pulumi.Input[Sequence[pulumi.Input['ContainerLabelArgs']]] labels: User-defined key/value metadata
         :param pulumi.Input[str] log_driver: The logging driver to use for the container.
         :param pulumi.Input[Mapping[str, Any]] log_opts: Key/value pairs to use as options for the logging driver.
         :param pulumi.Input[bool] logs: Save the container logs (`attach` must be enabled). Defaults to `false`.
         :param pulumi.Input[int] max_retry_count: The maximum amount of times to an attempt a restart when `restart` is set to 'on-failure'.
         :param pulumi.Input[int] memory: The memory limit for the container in MBs.
-        :param pulumi.Input[int] memory_swap: The total memory limit (memory + swap) for the container in MBs. This setting may compute to `-1` after `terraform
-               apply` if the target host doesn't support memory swap, when that is the case docker will use a soft limitation.
+        :param pulumi.Input[int] memory_swap: The total memory limit (memory + swap) for the container in MBs. This setting may compute to `-1` after `pulumi up` if the target host doesn't support memory swap, when that is the case docker will use a soft limitation.
         :param pulumi.Input[Sequence[pulumi.Input['ContainerMountArgs']]] mounts: Specification for mounts to be added to containers created as part of the service.
         :param pulumi.Input[bool] must_run: If `true`, then the Docker container will be kept running. If `false`, then as long as the container exists, Terraform
                assumes it is successful. Defaults to `true`.
         :param pulumi.Input[str] name: The name of the container.
         :param pulumi.Input[Sequence[pulumi.Input['ContainerNetworkDataArgs']]] network_datas: The data of the networks the container is connected to.
         :param pulumi.Input[str] network_mode: Network mode of the container.
         :param pulumi.Input[Sequence[pulumi.Input['ContainerNetworksAdvancedArgs']]] networks_advanced: The networks the container is attached to
@@ -1673,16 +1670,15 @@
     def memory(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "memory", value)
 
     @property
     @pulumi.getter(name="memorySwap")
     def memory_swap(self) -> Optional[pulumi.Input[int]]:
         """
-        The total memory limit (memory + swap) for the container in MBs. This setting may compute to `-1` after `terraform
-        apply` if the target host doesn't support memory swap, when that is the case docker will use a soft limitation.
+        The total memory limit (memory + swap) for the container in MBs. This setting may compute to `-1` after `pulumi up` if the target host doesn't support memory swap, when that is the case docker will use a soft limitation.
         """
         return pulumi.get(self, "memory_swap")
 
     @memory_swap.setter
     def memory_swap(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "memory_swap", value)
 
@@ -2221,16 +2217,15 @@
         :param pulumi.Input[str] ipc_mode: IPC sharing mode for the container. Possible values are: `none`, `private`, `shareable`, `container:<name|id>` or `host`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ContainerLabelArgs']]]] labels: User-defined key/value metadata
         :param pulumi.Input[str] log_driver: The logging driver to use for the container.
         :param pulumi.Input[Mapping[str, Any]] log_opts: Key/value pairs to use as options for the logging driver.
         :param pulumi.Input[bool] logs: Save the container logs (`attach` must be enabled). Defaults to `false`.
         :param pulumi.Input[int] max_retry_count: The maximum amount of times to an attempt a restart when `restart` is set to 'on-failure'.
         :param pulumi.Input[int] memory: The memory limit for the container in MBs.
-        :param pulumi.Input[int] memory_swap: The total memory limit (memory + swap) for the container in MBs. This setting may compute to `-1` after `terraform
-               apply` if the target host doesn't support memory swap, when that is the case docker will use a soft limitation.
+        :param pulumi.Input[int] memory_swap: The total memory limit (memory + swap) for the container in MBs. This setting may compute to `-1` after `pulumi up` if the target host doesn't support memory swap, when that is the case docker will use a soft limitation.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ContainerMountArgs']]]] mounts: Specification for mounts to be added to containers created as part of the service.
         :param pulumi.Input[bool] must_run: If `true`, then the Docker container will be kept running. If `false`, then as long as the container exists, Terraform
                assumes it is successful. Defaults to `true`.
         :param pulumi.Input[str] name: The name of the container.
         :param pulumi.Input[str] network_mode: Network mode of the container.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ContainerNetworksAdvancedArgs']]]] networks_advanced: The networks the container is attached to
         :param pulumi.Input[str] pid_mode: he PID (Process) Namespace mode for the container. Either `container:<name|id>` or `host`.
@@ -2574,16 +2569,15 @@
         :param pulumi.Input[str] ipc_mode: IPC sharing mode for the container. Possible values are: `none`, `private`, `shareable`, `container:<name|id>` or `host`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ContainerLabelArgs']]]] labels: User-defined key/value metadata
         :param pulumi.Input[str] log_driver: The logging driver to use for the container.
         :param pulumi.Input[Mapping[str, Any]] log_opts: Key/value pairs to use as options for the logging driver.
         :param pulumi.Input[bool] logs: Save the container logs (`attach` must be enabled). Defaults to `false`.
         :param pulumi.Input[int] max_retry_count: The maximum amount of times to an attempt a restart when `restart` is set to 'on-failure'.
         :param pulumi.Input[int] memory: The memory limit for the container in MBs.
-        :param pulumi.Input[int] memory_swap: The total memory limit (memory + swap) for the container in MBs. This setting may compute to `-1` after `terraform
-               apply` if the target host doesn't support memory swap, when that is the case docker will use a soft limitation.
+        :param pulumi.Input[int] memory_swap: The total memory limit (memory + swap) for the container in MBs. This setting may compute to `-1` after `pulumi up` if the target host doesn't support memory swap, when that is the case docker will use a soft limitation.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ContainerMountArgs']]]] mounts: Specification for mounts to be added to containers created as part of the service.
         :param pulumi.Input[bool] must_run: If `true`, then the Docker container will be kept running. If `false`, then as long as the container exists, Terraform
                assumes it is successful. Defaults to `true`.
         :param pulumi.Input[str] name: The name of the container.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ContainerNetworkDataArgs']]]] network_datas: The data of the networks the container is connected to.
         :param pulumi.Input[str] network_mode: Network mode of the container.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ContainerNetworksAdvancedArgs']]]] networks_advanced: The networks the container is attached to
@@ -2943,16 +2937,15 @@
         """
         return pulumi.get(self, "memory")
 
     @property
     @pulumi.getter(name="memorySwap")
     def memory_swap(self) -> pulumi.Output[Optional[int]]:
         """
-        The total memory limit (memory + swap) for the container in MBs. This setting may compute to `-1` after `terraform
-        apply` if the target host doesn't support memory swap, when that is the case docker will use a soft limitation.
+        The total memory limit (memory + swap) for the container in MBs. This setting may compute to `-1` after `pulumi up` if the target host doesn't support memory swap, when that is the case docker will use a soft limitation.
         """
         return pulumi.get(self, "memory_swap")
 
     @property
     @pulumi.getter
     def mounts(self) -> pulumi.Output[Optional[Sequence['outputs.ContainerMount']]]:
         """
```

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/get_logs.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/get_logs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/get_network.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/get_plugin.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/get_plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/get_registry_image.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/get_registry_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/get_remote_image.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/get_remote_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/image.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/network.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/outputs.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/plugin.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/provider.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/registry_image.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/registry_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/remote_image.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/remote_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/secret.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/service.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/service_config.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/service_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/tag.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker/volume.py` & `pulumi_docker-4.3.0a1684184527/pulumi_docker/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker.egg-info/PKG-INFO` & `pulumi_docker-4.3.0a1684184527/pulumi_docker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-docker
-Version: 4.3.0a1683956242
+Version: 4.3.0a1684184527
 Summary: A Pulumi package for interacting with Docker in Pulumi programs
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-docker
 Keywords: pulumi docker
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_docker-4.3.0a1683956242/pulumi_docker.egg-info/SOURCES.txt` & `pulumi_docker-4.3.0a1684184527/pulumi_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1683956242/setup.py` & `pulumi_docker-4.3.0a1684184527/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.3.0a1683956242"
-PLUGIN_VERSION = "4.3.0-alpha.1683956242+9bbe6145"
+VERSION = "4.3.0a1684184527"
+PLUGIN_VERSION = "4.3.0-alpha.1684184527+62725329"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'docker', PLUGIN_VERSION])
         except OSError as error:
```

