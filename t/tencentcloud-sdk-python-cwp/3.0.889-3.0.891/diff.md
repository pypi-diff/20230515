# Comparing `tmp/tencentcloud-sdk-python-cwp-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-cwp-3.0.891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.889.tar", last modified: Thu May 11 02:37:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.891.tar", last modified: Mon May 15 02:53:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cwp-3.0.889.tar` & `tencentcloud-sdk-python-cwp-3.0.891.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/tencentcloud/cwp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/tencentcloud/cwp/v20180228/
--rw-r--r--   0 root         (0) root         (0)     3900 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/tencentcloud/cwp/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   250541 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/tencentcloud/cwp/v20180228/cwp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/tencentcloud/cwp/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)   903526 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/tencentcloud/cwp/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/tencentcloud/cwp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/tencentcloud_sdk_python_cwp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 02:37:35.000000 tencentcloud-sdk-python-cwp-3.0.889/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/tencentcloud/cwp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/tencentcloud/cwp/v20180228/
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/tencentcloud/cwp/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   250541 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/tencentcloud/cwp/v20180228/cwp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/tencentcloud/cwp/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   905394 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/tencentcloud/cwp/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/tencentcloud/cwp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/tencentcloud_sdk_python_cwp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 02:53:57.000000 tencentcloud-sdk-python-cwp-3.0.891/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.889/README.rst` & `tencentcloud-sdk-python-cwp-3.0.891/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.889/tencentcloud/cwp/v20180228/errorcodes.py` & `tencentcloud-sdk-python-cwp-3.0.891/tencentcloud/cwp/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.889/tencentcloud/cwp/v20180228/cwp_client.py` & `tencentcloud-sdk-python-cwp-3.0.891/tencentcloud/cwp/v20180228/cwp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.889/tencentcloud/cwp/v20180228/models.py` & `tencentcloud-sdk-python-cwp-3.0.891/tencentcloud/cwp/v20180228/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -12153,33 +12153,37 @@
 <li>Uuids- String - 是否必填：否 - 主机uuid</li>
 <li>IsSupportDefense - int- 是否必填：否 - 是否支持防御 0:不支持 1:支持</li>
         :type Filters: list of Filters
         :param Order: 排序方式 desc , asc
         :type Order: str
         :param By: 排序字段 PublishDate  LastScanTime HostCount
         :type By: str
+        :param HotspotAttack: 是否热点漏洞
+        :type HotspotAttack: bool
         """
         self.Limit = None
         self.Offset = None
         self.Filters = None
         self.Order = None
         self.By = None
+        self.HotspotAttack = None
 
 
     def _deserialize(self, params):
         self.Limit = params.get("Limit")
         self.Offset = params.get("Offset")
         if params.get("Filters") is not None:
             self.Filters = []
             for item in params.get("Filters"):
                 obj = Filters()
                 obj._deserialize(item)
                 self.Filters.append(obj)
         self.Order = params.get("Order")
         self.By = params.get("By")
+        self.HotspotAttack = params.get("HotspotAttack")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -17747,14 +17751,19 @@
 <li>Status - String - 是否必填：否 - 处理状态  0 -- 待处理 1 -- 已加白 2 -- 已删除 3 - 已忽略</li>
 <li>ModifyTime - String - 是否必填：否 - 最近发生时间</li>
 <li>Uuid- String - 是否必填：否 - 主机uuid查询</li>
 <li>VulName- string -</li>
 <li>VulCategory- string - 是否必填：否 - 漏洞类别 1: web-cms漏洞 2:应用漏洞  4: Linux软件漏洞 5: Windows系统漏洞</li>
 <li>IsSupportDefense - int- 是否必填：否 - 是否支持防御 0:不支持 1:支持</li>
 <li>Labels- string- 是否必填：否 - 标签搜索</li>
+<li>IsSupportAutoFix- string- 是否必填：否 - 是否支持自动修复 0:不支持 1:支持</li>
+<li>CvssScore- string- 是否必填：否 - CvssScore大于多少</li>
+<li>AttackLevel- string- 是否必填：否 - 攻击热度大于多少</li>
+
+
         :type Filters: list of Filters
         :param By: 可选排序字段 Level，LastTime，HostCount
         :type By: str
         :param Order: 排序顺序：desc  默认asc
         :type Order: str
         """
         self.Limit = None
@@ -18495,14 +18504,23 @@
         :type HostCount: int
         :param IsSupportDefense: 是否支持防御， 0:不支持 1:支持
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsSupportDefense: int
         :param DefenseAttackCount: 已防御的攻击次数
 注意：此字段可能返回 null，表示取不到有效值。
         :type DefenseAttackCount: int
+        :param Method: 检测规则 0 - 版本比对, 1 - POC验证
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Method: int
+        :param AttackLevel: 攻击热度级别
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AttackLevel: int
+        :param DefenseState: 是否有漏洞主机开启漏洞防御
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DefenseState: bool
         """
         self.VulId = None
         self.Level = None
         self.VulName = None
         self.PublishDate = None
         self.Category = None
         self.Status = None
@@ -18510,14 +18528,17 @@
         self.Progress = None
         self.CveId = None
         self.CvssScore = None
         self.Labels = None
         self.HostCount = None
         self.IsSupportDefense = None
         self.DefenseAttackCount = None
+        self.Method = None
+        self.AttackLevel = None
+        self.DefenseState = None
 
 
     def _deserialize(self, params):
         self.VulId = params.get("VulId")
         self.Level = params.get("Level")
         self.VulName = params.get("VulName")
         self.PublishDate = params.get("PublishDate")
@@ -18527,14 +18548,17 @@
         self.Progress = params.get("Progress")
         self.CveId = params.get("CveId")
         self.CvssScore = params.get("CvssScore")
         self.Labels = params.get("Labels")
         self.HostCount = params.get("HostCount")
         self.IsSupportDefense = params.get("IsSupportDefense")
         self.DefenseAttackCount = params.get("DefenseAttackCount")
+        self.Method = params.get("Method")
+        self.AttackLevel = params.get("AttackLevel")
+        self.DefenseState = params.get("DefenseState")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -26630,14 +26654,23 @@
         :type DefenseAttackCount: int
         :param FirstAppearTime: 首次出现时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type FirstAppearTime: str
         :param VulCategory: 漏洞类别 1: web-cms漏洞 2:应用漏洞  4: Linux软件漏洞 5: Windows系统漏洞
 注意：此字段可能返回 null，表示取不到有效值。
         :type VulCategory: int
+        :param AttackLevel: 攻击热度级别
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AttackLevel: int
+        :param FixNoNeedRestart: 漏洞修复后是否需要重启
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FixNoNeedRestart: bool
+        :param Method: 检测方式0 - 版本比对, 1 - POC验证
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Method: int
         """
         self.Ids = None
         self.Name = None
         self.Status = None
         self.VulId = None
         self.PublishTime = None
         self.LastTime = None
@@ -26654,14 +26687,17 @@
         self.Labels = None
         self.FixSwitch = None
         self.TaskId = None
         self.IsSupportDefense = None
         self.DefenseAttackCount = None
         self.FirstAppearTime = None
         self.VulCategory = None
+        self.AttackLevel = None
+        self.FixNoNeedRestart = None
+        self.Method = None
 
 
     def _deserialize(self, params):
         self.Ids = params.get("Ids")
         self.Name = params.get("Name")
         self.Status = params.get("Status")
         self.VulId = params.get("VulId")
@@ -26680,14 +26716,17 @@
         self.Labels = params.get("Labels")
         self.FixSwitch = params.get("FixSwitch")
         self.TaskId = params.get("TaskId")
         self.IsSupportDefense = params.get("IsSupportDefense")
         self.DefenseAttackCount = params.get("DefenseAttackCount")
         self.FirstAppearTime = params.get("FirstAppearTime")
         self.VulCategory = params.get("VulCategory")
+        self.AttackLevel = params.get("AttackLevel")
+        self.FixNoNeedRestart = params.get("FixNoNeedRestart")
+        self.Method = params.get("Method")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cwp-3.0.891/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cwp-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.891/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.889/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.891/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.889/setup.py` & `tencentcloud-sdk-python-cwp-3.0.891/setup.py`

 * *Files identical despite different names*

