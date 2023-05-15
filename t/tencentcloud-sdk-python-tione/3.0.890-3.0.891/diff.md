# Comparing `tmp/tencentcloud-sdk-python-tione-3.0.890.tar.gz` & `tmp/tencentcloud-sdk-python-tione-3.0.891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.890.tar", last modified: Fri May 12 04:13:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.891.tar", last modified: Mon May 15 04:42:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tione-3.0.890.tar` & `tencentcloud-sdk-python-tione-3.0.891.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)    51024 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20211111/tione_client.py
--rw-r--r--   0 root         (0) root         (0)    11488 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   333554 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20211111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)    22010 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20191022/tione_client.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20191022/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91250 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud_sdk_python_tione.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 04:13:34.000000 tencentcloud-sdk-python-tione-3.0.890/tencentcloud_sdk_python_tione.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)    51024 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)    11488 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   334001 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)    22010 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91250 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud_sdk_python_tione.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud_sdk_python_tione.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tione-3.0.890/README.rst` & `tencentcloud-sdk-python-tione-3.0.891/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.890/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tione-3.0.891/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,18 +175,18 @@
         :type Uin: str
         :param SubUin: 子账号uin
         :type SubUin: str
         :param Region: 地域
         :type Region: str
         :param ChargeType: 计费模式
         :type ChargeType: str
-        :param ResourceGroupId: 预付费专用资源组id
+        :param ResourceGroupId: 包年包月资源组id
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResourceGroupId: str
-        :param ResourceGroupName: 预付费专用资源组名称
+        :param ResourceGroupName: 包年包月资源组名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResourceGroupName: str
         :param ResourceConfigInfo: 资源配置
         :type ResourceConfigInfo: :class:`tencentcloud.tione.v20211111.models.ResourceConfigInfo`
         :param Tags: 标签
 注意：此字段可能返回 null，表示取不到有效值。
         :type Tags: list of Tag
@@ -246,14 +246,17 @@
         :type FailureReason: str
         :param BillingInfo: 计费金额信息，eg：2.00元/小时 (for后付费)
 注意：此字段可能返回 null，表示取不到有效值。
         :type BillingInfo: str
         :param PodList: 运行中的Pod的名字
 注意：此字段可能返回 null，表示取不到有效值。
         :type PodList: list of str
+        :param ModelInferenceCodeInfo: 模型推理代码信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ModelInferenceCodeInfo: :class:`tencentcloud.tione.v20211111.models.CosPathInfo`
         """
         self.BatchTaskId = None
         self.BatchTaskName = None
         self.Uin = None
         self.SubUin = None
         self.Region = None
         self.ChargeType = None
@@ -279,14 +282,15 @@
         self.EndTime = None
         self.ChargeStatus = None
         self.LatestInstanceId = None
         self.Remark = None
         self.FailureReason = None
         self.BillingInfo = None
         self.PodList = None
+        self.ModelInferenceCodeInfo = None
 
 
     def _deserialize(self, params):
         self.BatchTaskId = params.get("BatchTaskId")
         self.BatchTaskName = params.get("BatchTaskName")
         self.Uin = params.get("Uin")
         self.SubUin = params.get("SubUin")
@@ -339,14 +343,17 @@
         self.EndTime = params.get("EndTime")
         self.ChargeStatus = params.get("ChargeStatus")
         self.LatestInstanceId = params.get("LatestInstanceId")
         self.Remark = params.get("Remark")
         self.FailureReason = params.get("FailureReason")
         self.BillingInfo = params.get("BillingInfo")
         self.PodList = params.get("PodList")
+        if params.get("ModelInferenceCodeInfo") is not None:
+            self.ModelInferenceCodeInfo = CosPathInfo()
+            self.ModelInferenceCodeInfo._deserialize(params.get("ModelInferenceCodeInfo"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -411,15 +418,15 @@
         :type ModelInfo: :class:`tencentcloud.tione.v20211111.models.ModelInfo`
         :param ImageInfo: 镜像信息
         :type ImageInfo: :class:`tencentcloud.tione.v20211111.models.ImageInfo`
         :param ChargeType: 计费模式
         :type ChargeType: str
         :param ChargeStatus: 计费状态，eg：BILLING计费中，ARREARS_STOP欠费停止，NOT_BILLING不在计费中
         :type ChargeStatus: str
-        :param ResourceGroupId: 预付费专用资源组
+        :param ResourceGroupId: 包年包月资源组ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResourceGroupId: str
         :param ResourceConfigInfo: 资源配置
         :type ResourceConfigInfo: :class:`tencentcloud.tione.v20211111.models.ResourceConfigInfo`
         :param Tags: 标签配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type Tags: list of Tag
@@ -437,20 +444,20 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type EndTime: str
         :param UpdateTime: 更新时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type UpdateTime: str
         :param Outputs: 输出
         :type Outputs: list of DataConfig
-        :param ResourceGroupName: 预付费专用资源组名称
+        :param ResourceGroupName: 包年包月资源组名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResourceGroupName: str
         :param FailureReason: 失败原因
         :type FailureReason: str
-        :param BillingInfo: 计费金额信息，eg：2.00元/小时 (for后付费)
+        :param BillingInfo: 计费金额信息，eg：2.00元/小时 (for 按量计费)
         :type BillingInfo: str
         """
         self.BatchTaskId = None
         self.BatchTaskName = None
         self.ModelInfo = None
         self.ImageInfo = None
         self.ChargeType = None
@@ -754,27 +761,27 @@
 
     """
 
     def __init__(self):
         r"""
         :param BatchTaskName: 跑批任务名称，不超过60个字符，仅支持中英文、数字、下划线"_"、短横"-"，只能以中英文、数字开头
         :type BatchTaskName: str
-        :param ChargeType: 计费模式，eg：PREPAID预付费，即包年包月；POSTPAID_BY_HOUR按小时后付费
+        :param ChargeType: 计费模式，eg：PREPAID 包年包月；POSTPAID_BY_HOUR 按量计费
         :type ChargeType: str
         :param ResourceConfigInfo: 资源配置
         :type ResourceConfigInfo: :class:`tencentcloud.tione.v20211111.models.ResourceConfigInfo`
         :param Outputs: 结果输出
         :type Outputs: list of DataConfig
         :param LogEnable: 是否上报日志
         :type LogEnable: bool
         :param JobType: 工作类型 1:单次 2:周期
         :type JobType: int
         :param CronInfo: 任务周期描述
         :type CronInfo: :class:`tencentcloud.tione.v20211111.models.CronInfo`
-        :param ResourceGroupId: 预付费专用资源组
+        :param ResourceGroupId: 包年包月资源组ID
         :type ResourceGroupId: str
         :param Tags: 标签配置
         :type Tags: list of Tag
         :param ModelInfo: 服务对应的模型信息，有模型文件时需要填写
         :type ModelInfo: :class:`tencentcloud.tione.v20211111.models.ModelInfo`
         :param ImageInfo: 自定义镜像信息
         :type ImageInfo: :class:`tencentcloud.tione.v20211111.models.ImageInfo`
@@ -2761,15 +2768,15 @@
         r"""
         :param Filters: 过滤器，eg：[{ "Name": "Id", "Values": ["train-23091792777383936"] }]
 
 取值范围：
 Name（名称）：task1
 Id（task ID）：train-23091792777383936
 Status（状态）：STARTING / RUNNING / STOPPING / STOPPED / FAILED / SUCCEED / SUBMIT_FAILED
-ChargeType（计费类型）：PREPAID（预付费）/ POSTPAID_BY_HOUR（后付费）
+ChargeType（计费类型）：PREPAID 包年包月 / POSTPAID_BY_HOUR 按量计费
 CHARGE_STATUS（计费状态）：NOT_BILLING（未开始计费）/ BILLING（计费中）/ ARREARS_STOP（欠费停止）
         :type Filters: list of Filter
         :param TagFilters: 标签过滤器，eg：[{ "TagKey": "TagKeyA", "TagValue": ["TagValueA"] }]
         :type TagFilters: list of TagFilter
         :param Offset: 偏移量，默认为0
         :type Offset: int
         :param Limit: 返回数量，默认为10，最大为50
```

### Comparing `tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.890/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.890/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.891/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.890
+Version: 3.0.891
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.890/setup.py` & `tencentcloud-sdk-python-tione-3.0.891/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.890/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tione-3.0.891/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.890/tencentcloud_sdk_python_tione.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.891/tencentcloud_sdk_python_tione.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.890
+Version: 3.0.891
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

