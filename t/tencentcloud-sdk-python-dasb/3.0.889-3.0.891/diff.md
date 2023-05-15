# Comparing `tmp/tencentcloud-sdk-python-dasb-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-dasb-3.0.891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.889.tar", last modified: Thu May 11 02:38:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.891.tar", last modified: Mon May 15 02:54:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dasb-3.0.889.tar` & `tencentcloud-sdk-python-dasb-3.0.891.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/tencentcloud/dasb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/tencentcloud/dasb/v20191018/
--rw-r--r--   0 root         (0) root         (0)     2500 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/tencentcloud/dasb/v20191018/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/tencentcloud/dasb/v20191018/__init__.py
--rw-r--r--   0 root         (0) root         (0)   157347 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/tencentcloud/dasb/v20191018/models.py
--rw-r--r--   0 root         (0) root         (0)    45577 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/tencentcloud/dasb/v20191018/dasb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/tencentcloud/dasb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/tencentcloud_sdk_python_dasb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 02:38:00.000000 tencentcloud-sdk-python-dasb-3.0.889/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/tencentcloud/dasb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/tencentcloud/dasb/v20191018/
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/tencentcloud/dasb/v20191018/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/tencentcloud/dasb/v20191018/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   157737 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/tencentcloud/dasb/v20191018/models.py
+-rw-r--r--   0 root         (0) root         (0)    45577 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/tencentcloud/dasb/v20191018/dasb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/tencentcloud/dasb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/tencentcloud_sdk_python_dasb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 02:54:24.000000 tencentcloud-sdk-python-dasb-3.0.891/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.889/README.rst` & `tencentcloud-sdk-python-dasb-3.0.891/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.889/tencentcloud/dasb/v20191018/errorcodes.py` & `tencentcloud-sdk-python-dasb-3.0.891/tencentcloud/dasb/v20191018/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.889/tencentcloud/dasb/v20191018/models.py` & `tencentcloud-sdk-python-dasb-3.0.891/tencentcloud/dasb/v20191018/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -661,14 +661,16 @@
         :type DeviceIdSet: list of int non-negative
         :param DeviceGroupIdSet: 关联的资产组ID
         :type DeviceGroupIdSet: list of int non-negative
         :param AccountSet: 关联的账号
         :type AccountSet: list of str
         :param CmdTemplateIdSet: 关联的高危命令模板ID
         :type CmdTemplateIdSet: list of int non-negative
+        :param ACTemplateIdSet: 关联高危DB模版ID
+        :type ACTemplateIdSet: list of str
         :param AllowDiskFileUp: 是否开启rdp磁盘映射文件上传
         :type AllowDiskFileUp: bool
         :param AllowDiskFileDown: 是否开启rdp磁盘映射文件下载
         :type AllowDiskFileDown: bool
         :param AllowShellFileUp: 是否开启rz sz文件上传
         :type AllowShellFileUp: bool
         :param AllowShellFileDown: 是否开启rz sz文件下载
@@ -697,14 +699,15 @@
         self.MaxFileDownSize = None
         self.UserIdSet = None
         self.UserGroupIdSet = None
         self.DeviceIdSet = None
         self.DeviceGroupIdSet = None
         self.AccountSet = None
         self.CmdTemplateIdSet = None
+        self.ACTemplateIdSet = None
         self.AllowDiskFileUp = None
         self.AllowDiskFileDown = None
         self.AllowShellFileUp = None
         self.AllowShellFileDown = None
         self.AllowFileDel = None
         self.ValidateFrom = None
         self.ValidateTo = None
@@ -725,14 +728,15 @@
         self.MaxFileDownSize = params.get("MaxFileDownSize")
         self.UserIdSet = params.get("UserIdSet")
         self.UserGroupIdSet = params.get("UserGroupIdSet")
         self.DeviceIdSet = params.get("DeviceIdSet")
         self.DeviceGroupIdSet = params.get("DeviceGroupIdSet")
         self.AccountSet = params.get("AccountSet")
         self.CmdTemplateIdSet = params.get("CmdTemplateIdSet")
+        self.ACTemplateIdSet = params.get("ACTemplateIdSet")
         self.AllowDiskFileUp = params.get("AllowDiskFileUp")
         self.AllowDiskFileDown = params.get("AllowDiskFileDown")
         self.AllowShellFileUp = params.get("AllowShellFileUp")
         self.AllowShellFileDown = params.get("AllowShellFileDown")
         self.AllowFileDel = params.get("AllowFileDel")
         self.ValidateFrom = params.get("ValidateFrom")
         self.ValidateTo = params.get("ValidateTo")
@@ -2977,14 +2981,16 @@
         :type DeviceIdSet: list of int non-negative
         :param DeviceGroupIdSet: 关联的资产组ID
         :type DeviceGroupIdSet: list of int non-negative
         :param AccountSet: 关联的账号
         :type AccountSet: list of str
         :param CmdTemplateIdSet: 关联的高危命令模板ID
         :type CmdTemplateIdSet: list of int non-negative
+        :param ACTemplateIdSet: 关联高危DB模版ID
+        :type ACTemplateIdSet: list of str
         :param AllowDiskFileUp: 是否开启 RDP 磁盘映射文件上传
         :type AllowDiskFileUp: bool
         :param AllowDiskFileDown: 是否开启 RDP 磁盘映射文件下载
         :type AllowDiskFileDown: bool
         :param AllowShellFileUp: 是否开启rz sz文件上传
         :type AllowShellFileUp: bool
         :param AllowShellFileDown: 是否开启rz sz文件下载
@@ -3014,14 +3020,15 @@
         self.MaxFileDownSize = None
         self.UserIdSet = None
         self.UserGroupIdSet = None
         self.DeviceIdSet = None
         self.DeviceGroupIdSet = None
         self.AccountSet = None
         self.CmdTemplateIdSet = None
+        self.ACTemplateIdSet = None
         self.AllowDiskFileUp = None
         self.AllowDiskFileDown = None
         self.AllowShellFileUp = None
         self.AllowShellFileDown = None
         self.AllowFileDel = None
         self.ValidateFrom = None
         self.ValidateTo = None
@@ -3043,14 +3050,15 @@
         self.MaxFileDownSize = params.get("MaxFileDownSize")
         self.UserIdSet = params.get("UserIdSet")
         self.UserGroupIdSet = params.get("UserGroupIdSet")
         self.DeviceIdSet = params.get("DeviceIdSet")
         self.DeviceGroupIdSet = params.get("DeviceGroupIdSet")
         self.AccountSet = params.get("AccountSet")
         self.CmdTemplateIdSet = params.get("CmdTemplateIdSet")
+        self.ACTemplateIdSet = params.get("ACTemplateIdSet")
         self.AllowDiskFileUp = params.get("AllowDiskFileUp")
         self.AllowDiskFileDown = params.get("AllowDiskFileDown")
         self.AllowShellFileUp = params.get("AllowShellFileUp")
         self.AllowShellFileDown = params.get("AllowShellFileDown")
         self.AllowFileDel = params.get("AllowFileDel")
         self.ValidateFrom = params.get("ValidateFrom")
         self.ValidateTo = params.get("ValidateTo")
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.889/tencentcloud/dasb/v20191018/dasb_client.py` & `tencentcloud-sdk-python-dasb-3.0.891/tencentcloud/dasb/v20191018/dasb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dasb-3.0.891/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dasb-3.0.889/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.891/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.891/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.889/setup.py` & `tencentcloud-sdk-python-dasb-3.0.891/setup.py`

 * *Files identical despite different names*

