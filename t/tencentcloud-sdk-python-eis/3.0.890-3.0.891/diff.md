# Comparing `tmp/tencentcloud-sdk-python-eis-3.0.890.tar.gz` & `tmp/tencentcloud-sdk-python-eis-3.0.891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-eis-3.0.890.tar", last modified: Fri May 12 02:10:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-eis-3.0.891.tar", last modified: Mon May 15 03:27:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-eis-3.0.890.tar` & `tencentcloud-sdk-python-eis-3.0.891.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20210601/
--rw-r--r--   0 root         (0) root         (0)     2977 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20210601/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     5846 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20210601/eis_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20210601/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24021 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20210601/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20200715/
--rw-r--r--   0 root         (0) root         (0)     1197 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20200715/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20200715/eis_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20200715/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13436 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20200715/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud_sdk_python_eis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud_sdk_python_eis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud_sdk_python_eis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/tencentcloud_sdk_python_eis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 02:10:11.000000 tencentcloud-sdk-python-eis-3.0.890/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20210601/
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20210601/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     5846 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20210601/eis_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20210601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24178 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20210601/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20200715/
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20200715/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20200715/eis_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20200715/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13436 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20200715/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud_sdk_python_eis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud_sdk_python_eis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud_sdk_python_eis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/tencentcloud_sdk_python_eis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 03:27:26.000000 tencentcloud-sdk-python-eis-3.0.891/setup.cfg
```

### Comparing `tencentcloud-sdk-python-eis-3.0.890/README.rst` & `tencentcloud-sdk-python-eis-3.0.891/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20210601/errorcodes.py` & `tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20210601/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20210601/eis_client.py` & `tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20210601/eis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20210601/models.py` & `tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20210601/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,20 +364,24 @@
 
     """
 
     def __init__(self):
         r"""
         :param RuntimeClass: 环境运行类型：0:运行时类型、1:api类型
         :type RuntimeClass: int
+        :param PlanType: 计划类型：0-pro 1-lite
+        :type PlanType: int
         """
         self.RuntimeClass = None
+        self.PlanType = None
 
 
     def _deserialize(self, params):
         self.RuntimeClass = params.get("RuntimeClass")
+        self.PlanType = params.get("PlanType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20200715/errorcodes.py` & `tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20200715/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20200715/eis_client.py` & `tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20200715/eis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.890/tencentcloud/eis/v20200715/models.py` & `tencentcloud-sdk-python-eis-3.0.891/tencentcloud/eis/v20200715/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.890/tencentcloud/__init__.py` & `tencentcloud-sdk-python-eis-3.0.891/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.890'
+__version__ = '3.0.891'
```

### Comparing `tencentcloud-sdk-python-eis-3.0.890/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-eis-3.0.891/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.890/tencentcloud_sdk_python_eis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-eis-3.0.891/tencentcloud_sdk_python_eis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eis
-Version: 3.0.890
+Version: 3.0.891
 Summary: Tencent Cloud Eis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eis-3.0.890/PKG-INFO` & `tencentcloud-sdk-python-eis-3.0.891/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eis
-Version: 3.0.890
+Version: 3.0.891
 Summary: Tencent Cloud Eis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eis-3.0.890/setup.py` & `tencentcloud-sdk-python-eis-3.0.891/setup.py`

 * *Files identical despite different names*

