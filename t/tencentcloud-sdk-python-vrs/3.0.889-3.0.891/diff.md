# Comparing `tmp/tencentcloud-sdk-python-vrs-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-vrs-3.0.891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vrs-3.0.889.tar", last modified: Thu May 11 03:28:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vrs-3.0.891.tar", last modified: Mon May 15 04:56:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vrs-3.0.889.tar` & `tencentcloud-sdk-python-vrs-3.0.891.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/tencentcloud/vrs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/tencentcloud/vrs/v20200824/
--rw-r--r--   0 root         (0) root         (0)     5710 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/tencentcloud/vrs/v20200824/vrs_client.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/tencentcloud/vrs/v20200824/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/tencentcloud/vrs/v20200824/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15482 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/tencentcloud/vrs/v20200824/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/tencentcloud/vrs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/tencentcloud_sdk_python_vrs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/tencentcloud_sdk_python_vrs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/tencentcloud_sdk_python_vrs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/tencentcloud_sdk_python_vrs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:28:52.000000 tencentcloud-sdk-python-vrs-3.0.889/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/tencentcloud/vrs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/tencentcloud/vrs/v20200824/
+-rw-r--r--   0 root         (0) root         (0)     5710 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/tencentcloud/vrs/v20200824/vrs_client.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/tencentcloud/vrs/v20200824/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/tencentcloud/vrs/v20200824/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15471 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/tencentcloud/vrs/v20200824/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/tencentcloud/vrs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/tencentcloud_sdk_python_vrs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/tencentcloud_sdk_python_vrs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/tencentcloud_sdk_python_vrs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/tencentcloud_sdk_python_vrs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 04:56:01.000000 tencentcloud-sdk-python-vrs-3.0.891/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.889/README.rst` & `tencentcloud-sdk-python-vrs-3.0.891/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.889/tencentcloud/vrs/v20200824/vrs_client.py` & `tencentcloud-sdk-python-vrs-3.0.891/tencentcloud/vrs/v20200824/vrs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.889/tencentcloud/vrs/v20200824/errorcodes.py` & `tencentcloud-sdk-python-vrs-3.0.891/tencentcloud/vrs/v20200824/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.889/tencentcloud/vrs/v20200824/models.py` & `tencentcloud-sdk-python-vrs-3.0.891/tencentcloud/vrs/v20200824/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,25 +27,25 @@
         r"""
         :param SessionId: 唯一请求 ID
         :type SessionId: str
         :param VoiceName: 音色名称
         :type VoiceName: str
         :param SampleRate: 音频采样率：
 
-16000：16k（默认）
+16000：16k
         :type SampleRate: int
         :param VoiceGender: 音色性别:
 
 1-male
 
 2-female
         :type VoiceGender: int
         :param VoiceLanguage: 语言类型：
 
-1-中文（默认）
+1-中文
         :type VoiceLanguage: int
         :param Codec: 音频格式，音频类型(wav,mp3,aac,m4a)
         :type Codec: str
         :param AudioIdList: 音频ID集合
         :type AudioIdList: list of str
         :param CallbackUrl: 回调 URL，用户自行搭建的用于接收结果的服务URL。如果用户使用轮询方式获取识别结果，则无需提交该参数。
 回调采用POST请求方式，Content-Type为application/x-www-form-urlencoded，回调数据格式如下:callback_body=checksum=&data={"TaskId":"xxxxxxxxxxxxxx","Status":2,"StatusStr":"success","VoiceType":xxxxx,"ErrorMsg":""}
@@ -224,15 +224,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param TextId: 标注文本信息 ID
         :type TextId: str
-        :param AudioData: 语音数据 要使用base64编码(采用python语言时注意读取文件应该为string而不是byte，以byte格式读取后要decode()。编码后的数据不可带有回车换行符)。
+        :param AudioData: 语音数据 要使用base64编码(采用python语言时注意读取文件时需要转成base64字符串编码，例如：str(base64.b64encode(open("input.aac", mode="rb").read()), encoding='utf-8') )。
         :type AudioData: str
         :param Codec: 音频格式，音频类型(wav,mp3,aac,m4a)
         :type Codec: str
         :param TypeId: 1:环境检测 2:音质检测
         :type TypeId: int
         :param SampleRate: 音频采样率：
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vrs-3.0.891/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vrs-3.0.889/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vrs-3.0.891/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vrs
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Vrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-vrs-3.0.891/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vrs
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Vrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.889/setup.py` & `tencentcloud-sdk-python-vrs-3.0.891/setup.py`

 * *Files identical despite different names*

