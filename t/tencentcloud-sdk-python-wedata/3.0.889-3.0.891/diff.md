# Comparing `tmp/tencentcloud-sdk-python-wedata-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-wedata-3.0.891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.889.tar", last modified: Thu May 11 03:29:17 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.891.tar", last modified: Mon May 15 04:56:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wedata-3.0.889.tar` & `tencentcloud-sdk-python-wedata-3.0.891.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/tencentcloud/wedata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/tencentcloud/wedata/v20210820/
--rw-r--r--   0 root         (0) root         (0)     3323 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)   184325 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 root         (0) root         (0)   696922 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/tencentcloud_sdk_python_wedata.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:29:17.000000 tencentcloud-sdk-python-wedata-3.0.889/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:22.000000 tencentcloud-sdk-python-wedata-3.0.891/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 04:56:21.000000 tencentcloud-sdk-python-wedata-3.0.891/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:22.000000 tencentcloud-sdk-python-wedata-3.0.891/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:22.000000 tencentcloud-sdk-python-wedata-3.0.891/tencentcloud/wedata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:56:21.000000 tencentcloud-sdk-python-wedata-3.0.891/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:22.000000 tencentcloud-sdk-python-wedata-3.0.891/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 root         (0) root         (0)     3323 2023-05-15 04:56:21.000000 tencentcloud-sdk-python-wedata-3.0.891/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:56:21.000000 tencentcloud-sdk-python-wedata-3.0.891/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   184325 2023-05-15 04:56:21.000000 tencentcloud-sdk-python-wedata-3.0.891/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 root         (0) root         (0)   697134 2023-05-15 04:56:21.000000 tencentcloud-sdk-python-wedata-3.0.891/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 04:56:21.000000 tencentcloud-sdk-python-wedata-3.0.891/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:22.000000 tencentcloud-sdk-python-wedata-3.0.891/tencentcloud_sdk_python_wedata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 04:56:22.000000 tencentcloud-sdk-python-wedata-3.0.891/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-05-15 04:56:22.000000 tencentcloud-sdk-python-wedata-3.0.891/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-15 04:56:22.000000 tencentcloud-sdk-python-wedata-3.0.891/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 04:56:22.000000 tencentcloud-sdk-python-wedata-3.0.891/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-15 04:56:22.000000 tencentcloud-sdk-python-wedata-3.0.891/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-05-15 04:56:21.000000 tencentcloud-sdk-python-wedata-3.0.891/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 04:56:22.000000 tencentcloud-sdk-python-wedata-3.0.891/setup.cfg
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.889/README.rst` & `tencentcloud-sdk-python-wedata-3.0.891/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.889/tencentcloud/wedata/v20210820/errorcodes.py` & `tencentcloud-sdk-python-wedata-3.0.891/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.889/tencentcloud/wedata/v20210820/wedata_client.py` & `tencentcloud-sdk-python-wedata-3.0.891/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.889/tencentcloud/wedata/v20210820/models.py` & `tencentcloud-sdk-python-wedata-3.0.891/tencentcloud/wedata/v20210820/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3719,34 +3719,39 @@
         :type Region: str
         :param Type: 数据源类型:枚举值
 注意：此字段可能返回 null，表示取不到有效值。
         :type Type: str
         :param ClusterId: 数据源所属的集群id
 注意：此字段可能返回 null，表示取不到有效值。
         :type ClusterId: str
+        :param Version: 数据源版本信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Version: str
         """
         self.DatabaseNames = None
         self.Description = None
         self.ID = None
         self.Instance = None
         self.Name = None
         self.Region = None
         self.Type = None
         self.ClusterId = None
+        self.Version = None
 
 
     def _deserialize(self, params):
         self.DatabaseNames = params.get("DatabaseNames")
         self.Description = params.get("Description")
         self.ID = params.get("ID")
         self.Instance = params.get("Instance")
         self.Name = params.get("Name")
         self.Region = params.get("Region")
         self.Type = params.get("Type")
         self.ClusterId = params.get("ClusterId")
+        self.Version = params.get("Version")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wedata-3.0.891/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-wedata-3.0.889/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.891/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.891/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.889/setup.py` & `tencentcloud-sdk-python-wedata-3.0.891/setup.py`

 * *Files identical despite different names*

