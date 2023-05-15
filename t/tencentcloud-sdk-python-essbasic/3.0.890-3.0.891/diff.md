# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.890.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.890.tar", last modified: Fri May 12 02:10:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.891.tar", last modified: Mon May 15 03:27:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.890.tar` & `tencentcloud-sdk-python-essbasic-3.0.891.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    15673 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    50895 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   230011 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 02:10:54.000000 tencentcloud-sdk-python-essbasic-3.0.890/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:27:54.000000 tencentcloud-sdk-python-essbasic-3.0.891/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:27:54.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 03:27:54.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-15 03:27:54.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-15 03:27:54.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 03:27:54.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-15 03:27:53.000000 tencentcloud-sdk-python-essbasic-3.0.891/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:27:54.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 03:27:53.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:27:54.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:27:54.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    15673 2023-05-15 03:27:53.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    50895 2023-05-15 03:27:53.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 03:27:53.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   230345 2023-05-15 03:27:53.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 03:27:53.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:27:54.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-05-15 03:27:53.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-05-15 03:27:53.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 03:27:53.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-05-15 03:27:53.000000 tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-15 03:27:54.000000 tencentcloud-sdk-python-essbasic-3.0.891/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-05-15 03:27:53.000000 tencentcloud-sdk-python-essbasic-3.0.891/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 03:27:54.000000 tencentcloud-sdk-python-essbasic-3.0.891/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.890
+Version: 3.0.891
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.890/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.891/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,24 +193,27 @@
         :type IntelligentStatus: str
         :param FormFields: 填写控件内容
         :type FormFields: list of FormField
         :param NeedSignReview: 本企业(发起方企业)是否需要签署审批，true：开启本企业签署审批
         :type NeedSignReview: bool
         :param UserData: 用户流程自定义数据参数
         :type UserData: str
+        :param CcInfos: 抄送人信息
+        :type CcInfos: list of CcInfo
         """
         self.FlowName = None
         self.FlowType = None
         self.FlowDescription = None
         self.Deadline = None
         self.Unordered = None
         self.IntelligentStatus = None
         self.FormFields = None
         self.NeedSignReview = None
         self.UserData = None
+        self.CcInfos = None
 
 
     def _deserialize(self, params):
         self.FlowName = params.get("FlowName")
         self.FlowType = params.get("FlowType")
         self.FlowDescription = params.get("FlowDescription")
         self.Deadline = params.get("Deadline")
@@ -220,14 +223,20 @@
             self.FormFields = []
             for item in params.get("FormFields"):
                 obj = FormField()
                 obj._deserialize(item)
                 self.FormFields.append(obj)
         self.NeedSignReview = params.get("NeedSignReview")
         self.UserData = params.get("UserData")
+        if params.get("CcInfos") is not None:
+            self.CcInfos = []
+            for item in params.get("CcInfos"):
+                obj = CcInfo()
+                obj._deserialize(item)
+                self.CcInfos.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2316,18 +2325,18 @@
         :type ComponentId: str
         :param ComponentType: 如果是Component控件类型，则可选的字段为：
 TEXT - 普通文本控件，输入文本字符串；
 MULTI_LINE_TEXT - 多行文本控件，输入文本字符串；
 CHECK_BOX - 勾选框控件，若选中填写ComponentValue 填写 true或者 false 字符串；
 FILL_IMAGE - 图片控件，ComponentValue 填写图片的资源 ID；
 DYNAMIC_TABLE - 动态表格控件；
-ATTACHMENT - 附件控件,ComponentValue 填写福建图片的资源 ID列表，以逗号分割；
+ATTACHMENT - 附件控件,ComponentValue 填写附件图片的资源 ID列表，以逗号分割；
 SELECTOR - 选择器控件，ComponentValue填写选择的字符串内容；
 DATE - 日期控件；默认是格式化为xxxx年xx月xx日字符串；
-DISTRICT - 省市区行政区划控件，ComponentValue填写省市区行政区划字符串内容；
+DISTRICT - 省市区行政区控件，ComponentValue填写省市区行政区字符串内容；
 
 如果是SignComponent控件类型，则可选的字段为
 SIGN_SEAL - 签署印章控件；
 SIGN_DATE - 签署日期控件；
 SIGN_SIGNATURE - 用户签名控件；
 SIGN_PERSONAL_SEAL - 个人签署印章控件（使用文件发起暂不支持此类型）；
 SIGN_PAGING_SEAL - 骑缝章；若文件发起，需要对应填充ComponentPosY、ComponentWidth、ComponentHeight
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.890/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.891/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.890/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.891/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.890
+Version: 3.0.891
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.890/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.891/setup.py`

 * *Files identical despite different names*
