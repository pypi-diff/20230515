# Comparing `tmp/tencentcloud-sdk-python-postgres-3.0.890.tar.gz` & `tmp/tencentcloud-sdk-python-postgres-3.0.891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.890.tar", last modified: Fri May 12 03:12:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.891.tar", last modified: Mon May 15 04:00:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-postgres-3.0.890.tar` & `tencentcloud-sdk-python-postgres-3.0.891.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:12:10.000000 tencentcloud-sdk-python-postgres-3.0.890/
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-12 03:12:09.000000 tencentcloud-sdk-python-postgres-3.0.890/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:12:10.000000 tencentcloud-sdk-python-postgres-3.0.890/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:12:10.000000 tencentcloud-sdk-python-postgres-3.0.890/tencentcloud/postgres/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:12:10.000000 tencentcloud-sdk-python-postgres-3.0.890/tencentcloud/postgres/v20170312/
--rw-r--r--   0 root         (0) root         (0)    84591 2023-05-12 03:12:09.000000 tencentcloud-sdk-python-postgres-3.0.890/tencentcloud/postgres/v20170312/postgres_client.py
--rw-r--r--   0 root         (0) root         (0)    20657 2023-05-12 03:12:09.000000 tencentcloud-sdk-python-postgres-3.0.890/tencentcloud/postgres/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:12:09.000000 tencentcloud-sdk-python-postgres-3.0.890/tencentcloud/postgres/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   277276 2023-05-12 03:12:09.000000 tencentcloud-sdk-python-postgres-3.0.890/tencentcloud/postgres/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:12:09.000000 tencentcloud-sdk-python-postgres-3.0.890/tencentcloud/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-12 03:12:09.000000 tencentcloud-sdk-python-postgres-3.0.890/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-12 03:12:10.000000 tencentcloud-sdk-python-postgres-3.0.890/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-05-12 03:12:09.000000 tencentcloud-sdk-python-postgres-3.0.890/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 03:12:10.000000 tencentcloud-sdk-python-postgres-3.0.890/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:12:10.000000 tencentcloud-sdk-python-postgres-3.0.890/tencentcloud_sdk_python_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 03:12:10.000000 tencentcloud-sdk-python-postgres-3.0.890/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-05-12 03:12:10.000000 tencentcloud-sdk-python-postgres-3.0.890/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-12 03:12:10.000000 tencentcloud-sdk-python-postgres-3.0.890/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 03:12:10.000000 tencentcloud-sdk-python-postgres-3.0.890/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/tencentcloud/postgres/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/tencentcloud/postgres/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    84591 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/tencentcloud/postgres/v20170312/postgres_client.py
+-rw-r--r--   0 root         (0) root         (0)    20657 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/tencentcloud/postgres/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/tencentcloud/postgres/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   277276 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/tencentcloud/postgres/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/tencentcloud/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/tencentcloud_sdk_python_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 04:00:24.000000 tencentcloud-sdk-python-postgres-3.0.891/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.890/README.rst` & `tencentcloud-sdk-python-postgres-3.0.891/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.890/tencentcloud/postgres/v20170312/postgres_client.py` & `tencentcloud-sdk-python-postgres-3.0.891/tencentcloud/postgres/v20170312/postgres_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.890/tencentcloud/postgres/v20170312/errorcodes.py` & `tencentcloud-sdk-python-postgres-3.0.891/tencentcloud/postgres/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.890/tencentcloud/postgres/v20170312/models.py` & `tencentcloud-sdk-python-postgres-3.0.891/tencentcloud/postgres/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.890/tencentcloud/__init__.py` & `tencentcloud-sdk-python-postgres-3.0.891/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-postgres-3.0.890/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.891/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.890
+Version: 3.0.891
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.890/setup.py` & `tencentcloud-sdk-python-postgres-3.0.891/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.890/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.891/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.890
+Version: 3.0.891
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```
