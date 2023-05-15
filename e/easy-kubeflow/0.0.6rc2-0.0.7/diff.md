# Comparing `tmp/easy-kubeflow-0.0.6rc2.tar.gz` & `tmp/easy-kubeflow-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy-kubeflow-0.0.6rc2.tar", last modified: Mon Dec  5 06:49:25 2022, max compression
+gzip compressed data, was "dist/easy-kubeflow-0.0.7.tar", last modified: Mon May 15 10:52:26 2023, max compression
```

## Comparing `easy-kubeflow-0.0.6rc2.tar` & `easy-kubeflow-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2022-12-05 06:49:25.000000 easy-kubeflow-0.0.6rc2/
--rw-r--r--   0 lwb        (501) staff       (20)      495 2022-12-05 06:49:25.000000 easy-kubeflow-0.0.6rc2/PKG-INFO
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2022-12-05 06:49:25.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow.egg-info/
--rw-r--r--   0 lwb        (501) staff       (20)      495 2022-12-05 06:49:25.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow.egg-info/PKG-INFO
--rw-r--r--   0 lwb        (501) staff       (20)      476 2022-12-05 06:49:25.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow.egg-info/SOURCES.txt
--rw-r--r--   0 lwb        (501) staff       (20)       52 2022-12-05 06:49:25.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow.egg-info/requires.txt
--rw-r--r--   0 lwb        (501) staff       (20)       14 2022-12-05 06:49:25.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow.egg-info/top_level.txt
--rw-r--r--   0 lwb        (501) staff       (20)        1 2022-12-05 06:49:25.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow.egg-info/dependency_links.txt
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2022-12-05 06:49:25.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow/
--rw-r--r--   0 lwb        (501) staff       (20)      122 2021-12-16 02:31:39.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow/__init__.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2022-12-05 06:49:25.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow/pipelines/
--rw-r--r--   0 lwb        (501) staff       (20)       69 2021-12-16 02:30:40.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow/pipelines/__init__.py
--rw-r--r--   0 lwb        (501) staff       (20)    20987 2022-07-18 10:13:06.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow/pipelines/pipelines_util.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2022-12-05 06:49:25.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow/utils/
--rw-r--r--   0 lwb        (501) staff       (20)     1140 2021-12-16 02:29:02.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow/utils/log_util.py
--rw-r--r--   0 lwb        (501) staff       (20)       31 2021-12-16 02:30:25.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow/utils/__init__.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2022-12-05 06:49:25.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow/examples/
--rw-r--r--   0 lwb        (501) staff       (20)        0 2021-12-16 08:21:23.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow/examples/__init__.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2022-12-05 06:49:25.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow/_docker/
--rw-r--r--   0 lwb        (501) staff       (20)       36 2021-12-16 02:30:53.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow/_docker/__init__.py
--rw-r--r--   0 lwb        (501) staff       (20)    22930 2022-12-05 06:17:57.000000 easy-kubeflow-0.0.6rc2/easy_kubeflow/_docker/docker_util.py
--rw-r--r--   0 lwb        (501) staff       (20)     7177 2022-04-19 03:38:05.000000 easy-kubeflow-0.0.6rc2/README.md
--rw-r--r--   0 lwb        (501) staff       (20)      839 2022-12-05 06:30:53.000000 easy-kubeflow-0.0.6rc2/setup.py
--rw-r--r--   0 lwb        (501) staff       (20)       38 2022-12-05 06:49:25.000000 easy-kubeflow-0.0.6rc2/setup.cfg
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/
+-rw-r--r--   0 lwb        (501) staff       (20)      492 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/PKG-INFO
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow.egg-info/
+-rw-r--r--   0 lwb        (501) staff       (20)      492 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow.egg-info/PKG-INFO
+-rw-r--r--   0 lwb        (501) staff       (20)      476 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow.egg-info/SOURCES.txt
+-rw-r--r--   0 lwb        (501) staff       (20)       52 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow.egg-info/requires.txt
+-rw-r--r--   0 lwb        (501) staff       (20)       14 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow.egg-info/top_level.txt
+-rw-r--r--   0 lwb        (501) staff       (20)        1 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow.egg-info/dependency_links.txt
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow/
+-rw-r--r--   0 lwb        (501) staff       (20)      122 2021-12-16 02:31:39.000000 easy-kubeflow-0.0.7/easy_kubeflow/__init__.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow/pipelines/
+-rw-r--r--   0 lwb        (501) staff       (20)       69 2021-12-16 02:30:40.000000 easy-kubeflow-0.0.7/easy_kubeflow/pipelines/__init__.py
+-rw-r--r--   0 lwb        (501) staff       (20)    21172 2023-05-15 10:39:18.000000 easy-kubeflow-0.0.7/easy_kubeflow/pipelines/pipelines_util.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow/utils/
+-rw-r--r--   0 lwb        (501) staff       (20)     1140 2021-12-16 02:29:02.000000 easy-kubeflow-0.0.7/easy_kubeflow/utils/log_util.py
+-rw-r--r--   0 lwb        (501) staff       (20)       31 2021-12-16 02:30:25.000000 easy-kubeflow-0.0.7/easy_kubeflow/utils/__init__.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow/examples/
+-rw-r--r--   0 lwb        (501) staff       (20)        0 2021-12-16 08:21:23.000000 easy-kubeflow-0.0.7/easy_kubeflow/examples/__init__.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow/_docker/
+-rw-r--r--   0 lwb        (501) staff       (20)       36 2021-12-16 02:30:53.000000 easy-kubeflow-0.0.7/easy_kubeflow/_docker/__init__.py
+-rw-r--r--   0 lwb        (501) staff       (20)    22930 2022-12-05 06:17:57.000000 easy-kubeflow-0.0.7/easy_kubeflow/_docker/docker_util.py
+-rw-r--r--   0 lwb        (501) staff       (20)     7231 2023-02-27 10:44:37.000000 easy-kubeflow-0.0.7/README.md
+-rw-r--r--   0 lwb        (501) staff       (20)      836 2023-05-15 10:45:09.000000 easy-kubeflow-0.0.7/setup.py
+-rw-r--r--   0 lwb        (501) staff       (20)       38 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/setup.cfg
```

### Comparing `easy-kubeflow-0.0.6rc2/easy_kubeflow/pipelines/pipelines_util.py` & `easy-kubeflow-0.0.7/easy_kubeflow/pipelines/pipelines_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,36 +243,44 @@
             _logger.error("at least, you need to add a component file !")
         return func
 
 
 class Component(object):
     """definition for pipelines component"""
 
-    def __init__(self, name: str = None, image: str = None, arguments: Optional[dict] = None,
-                 file_outputs: Optional[dict] = None, nfs_path: str = NFS_PATH,
+    def __init__(self, name: str = None, image: str = None,
+                 command: Optional[list] = None,
+                 arguments: Optional[dict] = None,
+                 file_outputs: Optional[dict] = None,
+                 nfs_path: str = NFS_PATH,
                  nfs_master_host: str = NFS_MASTER_HOST):
         """
         Component object
         :param name: name of component
         :param image: image for component container
+        :param command: [list] args to run component container, default None.
+                        the command to run in the container. If None, uses default CMD
+                        in defined in container.
         :param arguments: [dict] args to run component container, default None
         :param file_outputs: [dict] out put file of component container, default None
         :param nfs_path: default root path defined by cluster admin
         :param nfs_master_host: default host selected by cluster admin
         """
         self.name = name
         self.uuid = str(uuid4())
         self.image = image
+        self.command = command
         self.arguments = arguments
         self.file_outputs = file_outputs
         self.nfs_path = nfs_path
         self.nfs_master_host = nfs_master_host
         self.op = dsl.ContainerOp(
             name=self.name,
             image=self.image,
+            command=self.command,
             arguments=_dict2list(self.arguments),
             file_outputs=self.file_outputs
         )
 
     def default_op(self) -> 'dsl.ContainerOp':
         """
         default pipelines component containerOp
@@ -281,15 +289,15 @@
         _logger.info("Component op of `%s` init ..." % self.name)
         _logger.info("Container mount path is: %s" % self.nfs_path)
         self._pull_image_policy()
         self._add_volume()
         return self.op
 
     def udf_op(self, request_cpu: Optional[str] = None, request_mem: Optional[str] = None,
-               request_gpu: Optional[str] = '1',
+               request_gpu: Optional[str] = None,
                strategies: Optional[list] = None) -> 'dsl.ContainerOp':
         """
         user define pipelines component containerOp
         :param request_cpu: a string can be a number followed by "m", like `300m`, or `0.3` which equals `300m`
         :param request_mem: a string which can be a number or a number followed by one of "E", "P", "T", "G", "M", "K".
                             like `1Gi`, `1Mi`, `1Ki`
         :param request_gpu: str(number) like '1', '4', '8' means the amount of gpu you use
@@ -355,15 +363,15 @@
                 else:
                     _logger.error("strategy: %s not found in Strategies" % strategy)
         else:
             _logger.warning("Use default strategy")
 
     def _resource_limit(self, request_cpu: Optional[str] = None,
                         request_mem: Optional[str] = None,
-                        request_gpu: Optional[str] = '1'):
+                        request_gpu: Optional[str] = None):
         """
         resource: cpu, memory
         when user set resource, we recommend `request` equals to `limit`
         :param request_cpu: a string can be a number followed by "m", like `300m`, or `0.3` which equals `300m`
         :param request_mem: a string which can be an integer number or an integer number followed by one of "E",
                             "P", "T", "G", "M", "K". like `1Gi`, `1Mi`, `1Ki`
         :param request_gpu: str(number) like '1', '4', '8' means the amount of gpu you use
@@ -401,20 +409,19 @@
         # config for gpu
         if request_gpu:
             self.op.container.set_gpu_limit(
                 gpu=request_gpu)
             _logger.info("Set gpu request amount: %s" % request_gpu)
             _logger.info("Set gpu limit amount: %s" % request_gpu)
         else:
-            self.op.container.set_gpu_limit(
-                gpu=request_gpu)
-            _logger.warning("Use default gpu request: %s" % request_gpu)
-            _logger.warning("Use default gpu limit: %s" % request_gpu)
+            _logger.warning("Use default gpu request: 0")
+            _logger.warning("Use default gpu limit: 0")
 
 
+# TODO: ReuseComponent use command
 class ReuseComponent(object):
     """definition for reuse pipelines component"""
 
     def __init__(self, component_factory_func: Callable = None, arguments: Optional[dict] = None,
                  nfs_path: str = NFS_PATH,
                  nfs_master_host: str = NFS_MASTER_HOST):
         """
@@ -447,15 +454,15 @@
         _logger.info("ReuseComponent op of `%s` init ..." % self._uniform_name(self.factory_func.__name__))
         _logger.info("Container mount path is: %s" % self.nfs_path)
         self._pull_image_policy()
         self._add_volume()
         return self.op
 
     def udf_op(self, request_cpu: Optional[str] = None, request_mem: Optional[str] = None,
-               request_gpu: Optional[str] = '1',
+               request_gpu: Optional[str] = None,
                strategies: Optional[list] = None) -> 'dsl.ContainerOp':
         """
         user define pipelines component containerOp
         :param request_cpu: a string can be a number followed by "m", like `300m`, or `0.3` which equals `300m`
         :param request_mem: a string which can be a number or a number followed by one of "E", "P", "T", "G", "M", "K".
                             like `1Gi`, `1Mi`, `1Ki`
         :param request_gpu: str(number) like '1', '4', '8' means the amount of gpu you use
@@ -521,15 +528,15 @@
                 else:
                     _logger.error("strategy: %s not found in Strategies" % strategy)
         else:
             _logger.warning("Use default strategy")
 
     def _resource_limit(self, request_cpu: Optional[str] = None,
                         request_mem: Optional[str] = None,
-                        request_gpu: Optional[str] = '1'):
+                        request_gpu: Optional[str] = None):
         """
         resource: cpu, memory
         when user set resource, we recommend `request` equals to `limit`
         :param request_cpu: a string can be a number followed by "m", like `300m`, or `0.3` which equals `300m`
         :param request_mem: a string which can be an integer number or an integer number followed by one of "E",
                             "P", "T", "G", "M", "K". like `1Gi`, `1Mi`, `1Ki`
         :param request_gpu: str(number) like '1', '4', '8' means the amount of gpu you use
@@ -567,11 +574,9 @@
         # config for gpu
         if request_gpu:
             self.op.container.set_gpu_limit(
                 gpu=request_gpu)
             _logger.info("Set gpu request amount: %s" % request_gpu)
             _logger.info("Set gpu limit amount: %s" % request_gpu)
         else:
-            self.op.container.set_gpu_limit(
-                gpu=request_gpu)
-            _logger.warning("Use default gpu request: %s" % request_gpu)
-            _logger.warning("Use default gpu limit: %s" % request_gpu)
+            _logger.warning("Use default gpu request: 0")
+            _logger.warning("Use default gpu limit: 0")
```

### Comparing `easy-kubeflow-0.0.6rc2/easy_kubeflow/utils/log_util.py` & `easy-kubeflow-0.0.7/easy_kubeflow/utils/log_util.py`

 * *Files identical despite different names*

### Comparing `easy-kubeflow-0.0.6rc2/easy_kubeflow/_docker/docker_util.py` & `easy-kubeflow-0.0.7/easy_kubeflow/_docker/docker_util.py`

 * *Files identical despite different names*

### Comparing `easy-kubeflow-0.0.6rc2/README.md` & `easy-kubeflow-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # easy-kubeflow
 
 python sdk for kubeflow platform. use following func in .ipynb file
 
+## install 
+```bash
+pip install -U easy-kubeflow
+```
+
 ## docker
 
 examples for use of docker
 
 ### initial
 
 init docker client
```

### Comparing `easy-kubeflow-0.0.6rc2/setup.py` & `easy-kubeflow-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = None
 
 setuptools.setup(
     name="easy-kubeflow",  # Replace with your own name
-    version="0.0.6rc2",
+    version="0.0.7",
     author="CrazyBean",
     author_email="liuweibin@stonewise.cn",
     description="sdk help users for a better use of kubeflow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://service.stonewise.cn:8029/liuweibin/easy-kubeflow.git",
     install_requires=[
```

