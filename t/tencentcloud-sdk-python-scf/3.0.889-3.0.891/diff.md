# Comparing `tmp/tencentcloud-sdk-python-scf-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-scf-3.0.891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.889.tar", last modified: Thu May 11 03:09:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.891.tar", last modified: Mon May 15 04:15:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-scf-3.0.889.tar` & `tencentcloud-sdk-python-scf-3.0.891.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/tencentcloud/scf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/tencentcloud/scf/v20180416/
--rw-r--r--   0 root         (0) root         (0)    42711 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/tencentcloud/scf/v20180416/scf_client.py
--rw-r--r--   0 root         (0) root         (0)    31630 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/tencentcloud/scf/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/tencentcloud/scf/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   191185 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/tencentcloud/scf/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/tencentcloud/scf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/tencentcloud_sdk_python_scf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:09:25.000000 tencentcloud-sdk-python-scf-3.0.889/tencentcloud_sdk_python_scf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/tencentcloud/scf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/tencentcloud/scf/v20180416/
+-rw-r--r--   0 root         (0) root         (0)    42711 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/tencentcloud/scf/v20180416/scf_client.py
+-rw-r--r--   0 root         (0) root         (0)    31630 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/tencentcloud/scf/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/tencentcloud/scf/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   191505 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/tencentcloud/scf/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/tencentcloud/scf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/tencentcloud_sdk_python_scf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 04:15:28.000000 tencentcloud-sdk-python-scf-3.0.891/tencentcloud_sdk_python_scf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-scf-3.0.889/README.rst` & `tencentcloud-sdk-python-scf-3.0.891/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.889/tencentcloud/scf/v20180416/scf_client.py` & `tencentcloud-sdk-python-scf-3.0.891/tencentcloud/scf/v20180416/scf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.889/tencentcloud/scf/v20180416/errorcodes.py` & `tencentcloud-sdk-python-scf-3.0.891/tencentcloud/scf/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.889/tencentcloud/scf/v20180416/models.py` & `tencentcloud-sdk-python-scf-3.0.891/tencentcloud/scf/v20180416/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -750,34 +750,38 @@
         :type Namespace: str
         :param Qualifier: 函数的版本，默认为 $LATEST，建议填写 [$DEFAULT](https://cloud.tencent.com/document/product/583/36149#.E9.BB.98.E8.AE.A4.E5.88.AB.E5.90.8D)方便后续进行版本的灰度发布。
         :type Qualifier: str
         :param Enable: 触发器的初始是能状态 OPEN表示开启 CLOSE表示关闭
         :type Enable: str
         :param CustomArgument: 用户自定义参数，仅支持timer触发器
         :type CustomArgument: str
+        :param Description: 触发器描述
+        :type Description: str
         """
         self.FunctionName = None
         self.TriggerName = None
         self.Type = None
         self.TriggerDesc = None
         self.Namespace = None
         self.Qualifier = None
         self.Enable = None
         self.CustomArgument = None
+        self.Description = None
 
 
     def _deserialize(self, params):
         self.FunctionName = params.get("FunctionName")
         self.TriggerName = params.get("TriggerName")
         self.Type = params.get("Type")
         self.TriggerDesc = params.get("TriggerDesc")
         self.Namespace = params.get("Namespace")
         self.Qualifier = params.get("Qualifier")
         self.Enable = params.get("Enable")
         self.CustomArgument = params.get("CustomArgument")
+        self.Description = params.get("Description")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4407,27 +4411,30 @@
         :type ResourceId: str
         :param BindStatus: 触发器和云函数绑定状态
         :type BindStatus: str
         :param TriggerAttribute: 触发器类型，双向表示两侧控制台均可操作，单向表示SCF控制台单向创建
         :type TriggerAttribute: str
         :param Qualifier: 触发器绑定的别名或版本
         :type Qualifier: str
+        :param Description: 触发器描述
+        :type Description: str
         """
         self.ModTime = None
         self.Type = None
         self.TriggerDesc = None
         self.TriggerName = None
         self.AddTime = None
         self.Enable = None
         self.CustomArgument = None
         self.AvailableStatus = None
         self.ResourceId = None
         self.BindStatus = None
         self.TriggerAttribute = None
         self.Qualifier = None
+        self.Description = None
 
 
     def _deserialize(self, params):
         self.ModTime = params.get("ModTime")
         self.Type = params.get("Type")
         self.TriggerDesc = params.get("TriggerDesc")
         self.TriggerName = params.get("TriggerName")
@@ -4435,14 +4442,15 @@
         self.Enable = params.get("Enable")
         self.CustomArgument = params.get("CustomArgument")
         self.AvailableStatus = params.get("AvailableStatus")
         self.ResourceId = params.get("ResourceId")
         self.BindStatus = params.get("BindStatus")
         self.TriggerAttribute = params.get("TriggerAttribute")
         self.Qualifier = params.get("Qualifier")
+        self.Description = params.get("Description")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-scf-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-scf-3.0.891/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.889'
+__version__ = '3.0.891'
```

### Comparing `tencentcloud-sdk-python-scf-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.891/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-scf-3.0.889/setup.py` & `tencentcloud-sdk-python-scf-3.0.891/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.889/tencentcloud_sdk_python_scf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.891/tencentcloud_sdk_python_scf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

