# Comparing `tmp/tencentcloud-sdk-python-tcss-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-tcss-3.0.891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.889.tar", last modified: Thu May 11 03:18:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.891.tar", last modified: Mon May 15 04:40:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcss-3.0.889.tar` & `tencentcloud-sdk-python-tcss-3.0.891.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/tencentcloud/tcss/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/tencentcloud/tcss/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/tencentcloud/tcss/v20201101/
--rw-r--r--   0 root         (0) root         (0)   316128 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/tencentcloud/tcss/v20201101/tcss_client.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/tencentcloud/tcss/v20201101/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/tencentcloud/tcss/v20201101/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1015029 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/tencentcloud/tcss/v20201101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/tencentcloud_sdk_python_tcss.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:18:50.000000 tencentcloud-sdk-python-tcss-3.0.889/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/tencentcloud/tcss/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/tencentcloud/tcss/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/tencentcloud/tcss/v20201101/
+-rw-r--r--   0 root         (0) root         (0)   316128 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/tencentcloud/tcss/v20201101/tcss_client.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/tencentcloud/tcss/v20201101/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/tencentcloud/tcss/v20201101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1015233 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/tencentcloud/tcss/v20201101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/tencentcloud_sdk_python_tcss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 04:40:58.000000 tencentcloud-sdk-python-tcss-3.0.891/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.889/README.rst` & `tencentcloud-sdk-python-tcss-3.0.891/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcss-3.0.891/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcss-3.0.889/tencentcloud/tcss/v20201101/tcss_client.py` & `tencentcloud-sdk-python-tcss-3.0.891/tencentcloud/tcss/v20201101/tcss_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.889/tencentcloud/tcss/v20201101/errorcodes.py` & `tencentcloud-sdk-python-tcss-3.0.891/tencentcloud/tcss/v20201101/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.889/tencentcloud/tcss/v20201101/models.py` & `tencentcloud-sdk-python-tcss-3.0.891/tencentcloud/tcss/v20201101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -25085,36 +25085,41 @@
         :param OperationTime: 操作时间
         :type OperationTime: str
         :param AppId: 操作人appid
 注意：此字段可能返回 null，表示取不到有效值。
         :type AppId: int
         :param Uin: 操作人uin
         :type Uin: str
+        :param PolicyId: 策略id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PolicyId: int
         """
         self.ClusterId = None
         self.ClusterName = None
         self.Region = None
         self.Action = None
         self.Operation = None
         self.NetworkPolicyName = None
         self.OperationTime = None
         self.AppId = None
         self.Uin = None
+        self.PolicyId = None
 
 
     def _deserialize(self, params):
         self.ClusterId = params.get("ClusterId")
         self.ClusterName = params.get("ClusterName")
         self.Region = params.get("Region")
         self.Action = params.get("Action")
         self.Operation = params.get("Operation")
         self.NetworkPolicyName = params.get("NetworkPolicyName")
         self.OperationTime = params.get("OperationTime")
         self.AppId = params.get("AppId")
         self.Uin = params.get("Uin")
+        self.PolicyId = params.get("PolicyId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.889/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.891/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.891/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.889/setup.py` & `tencentcloud-sdk-python-tcss-3.0.891/setup.py`

 * *Files identical despite different names*

