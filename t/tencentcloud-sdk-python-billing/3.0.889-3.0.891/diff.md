# Comparing `tmp/tencentcloud-sdk-python-billing-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-billing-3.0.891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.889.tar", last modified: Thu May 11 02:22:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.891.tar", last modified: Mon May 15 02:31:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-billing-3.0.889.tar` & `tencentcloud-sdk-python-billing-3.0.891.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/tencentcloud/billing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/tencentcloud/billing/v20180709/
--rw-r--r--   0 root         (0) root         (0)     2904 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/tencentcloud/billing/v20180709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/tencentcloud/billing/v20180709/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148500 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/tencentcloud/billing/v20180709/models.py
--rw-r--r--   0 root         (0) root         (0)    19523 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/tencentcloud/billing/v20180709/billing_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/tencentcloud/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/tencentcloud_sdk_python_billing.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/tencentcloud_sdk_python_billing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 02:22:22.000000 tencentcloud-sdk-python-billing-3.0.889/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/tencentcloud/billing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/tencentcloud/billing/v20180709/
+-rw-r--r--   0 root         (0) root         (0)     2904 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/tencentcloud/billing/v20180709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/tencentcloud/billing/v20180709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   149520 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/tencentcloud/billing/v20180709/models.py
+-rw-r--r--   0 root         (0) root         (0)    20134 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/tencentcloud/billing/v20180709/billing_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/tencentcloud/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/tencentcloud_sdk_python_billing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/tencentcloud_sdk_python_billing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 02:31:51.000000 tencentcloud-sdk-python-billing-3.0.891/setup.cfg
```

### Comparing `tencentcloud-sdk-python-billing-3.0.889/README.rst` & `tencentcloud-sdk-python-billing-3.0.891/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-billing-3.0.891/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-billing-3.0.889/tencentcloud/billing/v20180709/errorcodes.py` & `tencentcloud-sdk-python-billing-3.0.891/tencentcloud/billing/v20180709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.889/tencentcloud/billing/v20180709/models.py` & `tencentcloud-sdk-python-billing-3.0.891/tencentcloud/billing/v20180709/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,15 @@
         :type UsedAmountUnit: str
         :param TimeSpan: 使用时长
         :type TimeSpan: str
         :param TimeUnitName: 时长单位
         :type TimeUnitName: str
         :param Cost: 组件原价
         :type Cost: str
-        :param Discount: 折扣率
+        :param Discount: 折扣率，本资源享受的折扣率（如果客户享受一口价/合同价则默认不展示，退费场景也默认不展示）
         :type Discount: str
         :param ReduceType: 优惠类型
         :type ReduceType: str
         :param RealCost: 优惠后总价
         :type RealCost: str
         :param VoucherPayAmount: 代金券支付金额
         :type VoucherPayAmount: str
@@ -284,36 +284,36 @@
         :type IncentivePayAmount: str
         :param ItemCode: 组件类型代码
 注意：此字段可能返回 null，表示取不到有效值。
         :type ItemCode: str
         :param ComponentCode: 组件名称代码
 注意：此字段可能返回 null，表示取不到有效值。
         :type ComponentCode: str
-        :param ContractPrice: 合同价
+        :param ContractPrice: 组件单价
 注意：此字段可能返回 null，表示取不到有效值。
         :type ContractPrice: str
         :param InstanceType: 资源包、预留实例、节省计划、竞价实例这四类特殊实例本身的扣费行为，此字段体现对应的实例类型。枚举值如下：
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceType: str
         :param RiTimeSpan: 预留实例抵扣的使用时长，时长单位与被抵扣的时长单位保持一致
 注意：此字段可能返回 null，表示取不到有效值。
         :type RiTimeSpan: str
-        :param OriginalCostWithRI: 按组件原价的口径换算的预留实例抵扣金额
+        :param OriginalCostWithRI: 预留实例抵扣组件原价，本产品或服务使用预留实例抵扣的组件原价金额
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginalCostWithRI: str
-        :param SPDeductionRate: 节省计划可用余额额度范围内，节省计划对于此组件打的折扣率
+        :param SPDeductionRate: 节省计划抵扣率，节省计划可用余额额度范围内，节省计划对于此组件打的折扣率
 注意：此字段可能返回 null，表示取不到有效值。
         :type SPDeductionRate: str
-        :param SPDeduction: 节省计划抵扣的SP包面值
+        :param SPDeduction: 节省计划抵扣金额，节省计划抵扣的SP包面值
 注意：此字段可能返回 null，表示取不到有效值。
         :type SPDeduction: str
-        :param OriginalCostWithSP: 按组件原价的口径换算的节省计划抵扣金额
+        :param OriginalCostWithSP: 节省计划抵扣组件原价，节省计划抵扣原价=节省计划包抵扣金额/节省计划抵扣率
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginalCostWithSP: str
-        :param BlendedDiscount: 综合了官网折扣、预留实例抵扣、节省计划抵扣的混合折扣率。若没有预留实例抵扣、节省计划抵扣,混合折扣率等于折扣率
+        :param BlendedDiscount: 混合折扣率，综合各类折扣抵扣信息后的最终折扣率，混合折扣率 = 优惠后总价 / 组件原价
 注意：此字段可能返回 null，表示取不到有效值。
         :type BlendedDiscount: str
         """
         self.ComponentCodeName = None
         self.ItemCodeName = None
         self.SinglePrice = None
         self.SpecifiedPrice = None
@@ -1710,25 +1710,25 @@
 class DescribeBillDetailRequest(AbstractModel):
     """DescribeBillDetail请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Offset: 偏移量
+        :param Offset: 分页偏移量，Offset=0表示第一页，如果Limit=100，则Offset=100表示第二页，Offset=200表示第三页，依次类推
         :type Offset: int
         :param Limit: 数量，最大值为100
         :type Limit: int
         :param PeriodType: 周期类型，byUsedTime按计费周期/byPayTime按扣费周期。需要与费用中心该月份账单的周期保持一致。您可前往[账单概览](https://console.cloud.tencent.com/expense/bill/overview)页面顶部查看确认您的账单统计周期类型。
         :type PeriodType: str
-        :param Month: 月份，格式为yyyy-mm，Month和BeginTime&EndTime必传一个，如果有传BeginTime&EndTime则Month字段无效。不能早于开通账单2.0的月份，最多可拉取24个月内的数据。
+        :param Month: 月份，格式为yyyy-mm，Month和BeginTime&EndTime必传一个，如果有传BeginTime&EndTime则Month字段无效。不能早于开通账单2.0的月份，最多可拉取18个月内的数据。
         :type Month: str
-        :param BeginTime: 周期开始时间，格式为Y-m-d H:i:s，Month和BeginTime&EndTime必传一个，如果有该字段则Month字段无效。BeginTime和EndTime必须一起传。不能早于开通账单2.0的月份，最多可拉取24个月内的数据。(不支持跨月查询)
+        :param BeginTime: 周期开始时间，格式为yyyy-mm-dd hh:ii:ss，Month和BeginTime&EndTime必传一个，如果有该字段则Month字段无效。BeginTime和EndTime必须一起传。不能早于开通账单2.0的月份，最多可拉取18个月内的数据。(不支持跨月查询)
         :type BeginTime: str
-        :param EndTime: 周期结束时间，格式为Y-m-d H:i:s，Month和BeginTime&EndTime必传一个，如果有该字段则Month字段无效。BeginTime和EndTime必须一起传。不能早于开通账单2.0的月份，最多可拉取24个月内的数据。（不支持跨月查询）
+        :param EndTime: 周期结束时间，格式为yyyy-mm-dd hh:ii:ss，Month和BeginTime&EndTime必传一个，如果有该字段则Month字段无效。BeginTime和EndTime必须一起传。不能早于开通账单2.0的月份，最多可拉取18个月内的数据。（不支持跨月查询）
         :type EndTime: str
         :param NeedRecordNum: 是否需要访问列表的总记录数，用于前端分页
 1-表示需要， 0-表示不需要
         :type NeedRecordNum: int
         :param ProductCode: 已废弃参数，未开放
         :type ProductCode: str
         :param PayMode: 付费模式 prePay/postPay
@@ -1764,28 +1764,31 @@
 包年包月转按量
         :type ActionType: str
         :param ProjectId: 项目ID:资源所属项目ID
         :type ProjectId: int
         :param BusinessCode: 产品名称代码
 备注：如需获取当月使用过的BusinessCode，请调用API：<a href="https://cloud.tencent.com/document/product/555/35761">获取产品汇总费用分布</a>
         :type BusinessCode: str
+        :param Context: 上一次请求返回的上下文信息，翻页查询Month>=2023-05的月份的数据可加快查询速度，数据量10万级别以上的用户建议使用，查询速度可提升2~10倍
+        :type Context: str
         """
         self.Offset = None
         self.Limit = None
         self.PeriodType = None
         self.Month = None
         self.BeginTime = None
         self.EndTime = None
         self.NeedRecordNum = None
         self.ProductCode = None
         self.PayMode = None
         self.ResourceId = None
         self.ActionType = None
         self.ProjectId = None
         self.BusinessCode = None
+        self.Context = None
 
 
     def _deserialize(self, params):
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
         self.PeriodType = params.get("PeriodType")
         self.Month = params.get("Month")
@@ -1794,14 +1797,15 @@
         self.NeedRecordNum = params.get("NeedRecordNum")
         self.ProductCode = params.get("ProductCode")
         self.PayMode = params.get("PayMode")
         self.ResourceId = params.get("ResourceId")
         self.ActionType = params.get("ActionType")
         self.ProjectId = params.get("ProjectId")
         self.BusinessCode = params.get("BusinessCode")
+        self.Context = params.get("Context")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1812,33 +1816,38 @@
 
     """
 
     def __init__(self):
         r"""
         :param DetailSet: 详情列表
         :type DetailSet: list of BillDetail
-        :param Total: 总记录数
+        :param Total: 总记录数，24小时缓存一次，可能比实际总记录数少
 注意：此字段可能返回 null，表示取不到有效值。
         :type Total: int
+        :param Context: 本次请求的上下文信息，可用于下一次请求的请求参数中，加快查询速度
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Context: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.DetailSet = None
         self.Total = None
+        self.Context = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         if params.get("DetailSet") is not None:
             self.DetailSet = []
             for item in params.get("DetailSet"):
                 obj = BillDetail()
                 obj._deserialize(item)
                 self.DetailSet.append(obj)
         self.Total = params.get("Total")
+        self.Context = params.get("Context")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeBillListRequest(AbstractModel):
     """DescribeBillList请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-billing-3.0.889/tencentcloud/billing/v20180709/billing_client.py` & `tencentcloud-sdk-python-billing-3.0.891/tencentcloud/billing/v20180709/billing_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,18 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeBillDetail(self, request):
-        """查询账单明细数据
+        """查询账单明细数据。
+        注意事项：
+        1.在请求接口时，由于网络不稳定或其它异常，可能会导致请求失败。如果您遇到这种情况，我们建议您在接口请求失败时，手动发起重试操作，这样可以更好地确保您的接口请求能够成功执行。
+        2.对于账单明细数据量级很大（例如每月账单明细量级超过20w）的客户，通过 API 调用账单数据效率较低，建议您开通账单数据存储功能，通过存储桶中获取账单文件进行分析。[账单存储至COS桶](https://cloud.tencent.com/document/product/555/61275)
 
         :param request: Request instance for DescribeBillDetail.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeBillDetailRequest`
         :rtype: :class:`tencentcloud.billing.v20180709.models.DescribeBillDetailResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-billing-3.0.889/tencentcloud_sdk_python_billing.egg-info/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.891/tencentcloud_sdk_python_billing.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.891/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.889/setup.py` & `tencentcloud-sdk-python-billing-3.0.891/setup.py`

 * *Files identical despite different names*

