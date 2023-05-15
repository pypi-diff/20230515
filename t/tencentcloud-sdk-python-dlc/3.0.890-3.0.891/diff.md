# Comparing `tmp/tencentcloud-sdk-python-dlc-3.0.890.tar.gz` & `tmp/tencentcloud-sdk-python-dlc-3.0.891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.890.tar", last modified: Fri May 12 02:06:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.891.tar", last modified: Mon May 15 03:01:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dlc-3.0.890.tar` & `tencentcloud-sdk-python-dlc-3.0.891.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/tencentcloud/dlc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/tencentcloud/dlc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/tencentcloud/dlc/v20210125/
--rw-r--r--   0 root         (0) root         (0)    78374 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/tencentcloud/dlc/v20210125/dlc_client.py
--rw-r--r--   0 root         (0) root         (0)    11538 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/tencentcloud/dlc/v20210125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/tencentcloud/dlc/v20210125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   323205 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/tencentcloud/dlc/v20210125/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/tencentcloud_sdk_python_dlc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 02:06:45.000000 tencentcloud-sdk-python-dlc-3.0.890/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/tencentcloud/dlc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/tencentcloud/dlc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/tencentcloud/dlc/v20210125/
+-rw-r--r--   0 root         (0) root         (0)    78374 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/tencentcloud/dlc/v20210125/dlc_client.py
+-rw-r--r--   0 root         (0) root         (0)    11538 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/tencentcloud/dlc/v20210125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/tencentcloud/dlc/v20210125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   324571 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/tencentcloud/dlc/v20210125/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/tencentcloud_sdk_python_dlc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 03:01:01.000000 tencentcloud-sdk-python-dlc-3.0.891/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.890/README.rst` & `tencentcloud-sdk-python-dlc-3.0.891/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.890/tencentcloud/dlc/v20210125/dlc_client.py` & `tencentcloud-sdk-python-dlc-3.0.891/tencentcloud/dlc/v20210125/dlc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.890/tencentcloud/dlc/v20210125/errorcodes.py` & `tencentcloud-sdk-python-dlc-3.0.891/tencentcloud/dlc/v20210125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.890/tencentcloud/dlc/v20210125/models.py` & `tencentcloud-sdk-python-dlc-3.0.891/tencentcloud/dlc/v20210125/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3226,14 +3226,38 @@
 
 
 class DataGovernPolicy(AbstractModel):
     """数据治理规则
 
     """
 
+    def __init__(self):
+        r"""
+        :param RuleType: 治理规则类型，Customize: 自定义；Intelligence: 智能治理
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RuleType: str
+        :param GovernEngine: 治理引擎
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GovernEngine: str
+        """
+        self.RuleType = None
+        self.GovernEngine = None
+
+
+    def _deserialize(self, params):
+        self.RuleType = params.get("RuleType")
+        self.GovernEngine = params.get("GovernEngine")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
 
 class DatabaseInfo(AbstractModel):
     """数据库对象
 
     """
 
     def __init__(self):
@@ -6029,19 +6053,22 @@
         :type TableBaseInfo: :class:`tencentcloud.dlc.v20210125.models.TableBaseInfo`
         :param Columns: 表字段信息
         :type Columns: list of TColumn
         :param Partitions: 表分区信息
         :type Partitions: list of TPartition
         :param Properties: 表属性信息
         :type Properties: list of Property
+        :param UpsertKeys: V2 upsert表 upsert键
+        :type UpsertKeys: list of str
         """
         self.TableBaseInfo = None
         self.Columns = None
         self.Partitions = None
         self.Properties = None
+        self.UpsertKeys = None
 
 
     def _deserialize(self, params):
         if params.get("TableBaseInfo") is not None:
             self.TableBaseInfo = TableBaseInfo()
             self.TableBaseInfo._deserialize(params.get("TableBaseInfo"))
         if params.get("Columns") is not None:
@@ -6058,14 +6085,15 @@
                 self.Partitions.append(obj)
         if params.get("Properties") is not None:
             self.Properties = []
             for item in params.get("Properties"):
                 obj = Property()
                 obj._deserialize(item)
                 self.Properties.append(obj)
+        self.UpsertKeys = params.get("UpsertKeys")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -7926,38 +7954,43 @@
         :type UserAlias: str
         :param UserSubUin: 建表用户ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type UserSubUin: str
         :param GovernPolicy: 数据治理配置项
 注意：此字段可能返回 null，表示取不到有效值。
         :type GovernPolicy: :class:`tencentcloud.dlc.v20210125.models.DataGovernPolicy`
+        :param DbGovernPolicyIsDisable: 库数据治理是否关闭，关闭：true，开启：false
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DbGovernPolicyIsDisable: str
         """
         self.DatabaseName = None
         self.TableName = None
         self.DatasourceConnectionName = None
         self.TableComment = None
         self.Type = None
         self.TableFormat = None
         self.UserAlias = None
         self.UserSubUin = None
         self.GovernPolicy = None
+        self.DbGovernPolicyIsDisable = None
 
 
     def _deserialize(self, params):
         self.DatabaseName = params.get("DatabaseName")
         self.TableName = params.get("TableName")
         self.DatasourceConnectionName = params.get("DatasourceConnectionName")
         self.TableComment = params.get("TableComment")
         self.Type = params.get("Type")
         self.TableFormat = params.get("TableFormat")
         self.UserAlias = params.get("UserAlias")
         self.UserSubUin = params.get("UserSubUin")
         if params.get("GovernPolicy") is not None:
             self.GovernPolicy = DataGovernPolicy()
             self.GovernPolicy._deserialize(params.get("GovernPolicy"))
+        self.DbGovernPolicyIsDisable = params.get("DbGovernPolicyIsDisable")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.890/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dlc-3.0.891/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dlc-3.0.890/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.891/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.890
+Version: 3.0.891
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.890/setup.py` & `tencentcloud-sdk-python-dlc-3.0.891/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.890/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.891/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.890
+Version: 3.0.891
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

