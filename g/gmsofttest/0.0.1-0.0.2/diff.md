# Comparing `tmp/gmsofttest-0.0.1.tar.gz` & `tmp/gmsofttest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gmsofttest-0.0.1.tar", last modified: Mon May 15 12:20:04 2023, max compression
+gzip compressed data, was "dist\gmsofttest-0.0.2.tar", last modified: Mon May 15 12:35:04 2023, max compression
```

## Comparing `gmsofttest-0.0.1.tar` & `gmsofttest-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 12:20:04.000000 gmsofttest-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-02-11 08:11:24.000000 gmsofttest-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      847 2023-05-15 12:20:04.000000 gmsofttest-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-04-13 06:39:22.000000 gmsofttest-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 12:20:04.000000 gmsofttest-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      801 2023-05-15 12:17:48.000000 gmsofttest-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 12:20:04.000000 gmsofttest-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-15 12:20:04.000000 gmsofttest-0.0.1/src/gmexcelhandler/
--rw-rw-rw-   0        0        0      124 2023-02-13 01:53:02.000000 gmsofttest-0.0.1/src/gmexcelhandler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 12:20:04.000000 gmsofttest-0.0.1/src/gmfakerdata/
--rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.1/src/gmfakerdata/__init__.py
--rw-rw-rw-   0        0        0    89848 2023-04-22 07:37:37.000000 gmsofttest-0.0.1/src/gmfakerdata/china_address.py
--rw-rw-rw-   0        0        0     4261 2023-04-22 13:37:51.000000 gmsofttest-0.0.1/src/gmfakerdata/getidcard.py
--rw-rw-rw-   0        0        0     2071 2023-03-11 05:43:46.000000 gmsofttest-0.0.1/src/gmfakerdata/getrandomdata.py
--rw-rw-rw-   0        0        0     4490 2023-04-22 10:02:28.000000 gmsofttest-0.0.1/src/gmfakerdata/sucreditcode.py
-drwxrwxrwx   0        0        0        0 2023-05-15 12:20:04.000000 gmsofttest-0.0.1/src/gmmysql/
--rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.1/src/gmmysql/__init__.py
--rw-rw-rw-   0        0        0    12335 2023-03-08 06:26:47.000000 gmsofttest-0.0.1/src/gmmysql/mysqlexe.py
-drwxrwxrwx   0        0        0        0 2023-05-15 12:20:04.000000 gmsofttest-0.0.1/src/gmmysql/utils/
--rw-rw-rw-   0        0        0      125 2023-02-13 02:10:07.000000 gmsofttest-0.0.1/src/gmmysql/utils/__init__.py
--rw-rw-rw-   0        0        0     2214 2022-12-06 12:17:47.000000 gmsofttest-0.0.1/src/gmmysql/utils/yamlhandler.py
-drwxrwxrwx   0        0        0        0 2023-05-15 12:20:04.000000 gmsofttest-0.0.1/src/gmsofttest.egg-info/
--rw-rw-rw-   0        0        0      847 2023-05-15 12:20:04.000000 gmsofttest-0.0.1/src/gmsofttest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-05-15 12:20:04.000000 gmsofttest-0.0.1/src/gmsofttest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 12:20:04.000000 gmsofttest-0.0.1/src/gmsofttest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-15 12:20:04.000000 gmsofttest-0.0.1/src/gmsofttest.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 12:20:04.000000 gmsofttest-0.0.1/src/gmverifyhandler/
--rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.1/src/gmverifyhandler/__init__.py
--rw-rw-rw-   0        0        0      205 2023-02-11 08:09:19.000000 gmsofttest-0.0.1/src/gmverifyhandler/bye.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:35:04.000000 gmsofttest-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-11 08:11:24.000000 gmsofttest-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      655 2023-05-15 12:35:04.000000 gmsofttest-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-05-15 12:34:58.000000 gmsofttest-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-15 12:35:04.000000 gmsofttest-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      801 2023-05-15 12:34:43.000000 gmsofttest-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:35:04.000000 gmsofttest-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-15 12:35:04.000000 gmsofttest-0.0.2/src/gmexcelhandler/
+-rw-rw-rw-   0        0        0      124 2023-02-13 01:53:02.000000 gmsofttest-0.0.2/src/gmexcelhandler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:35:04.000000 gmsofttest-0.0.2/src/gmfakerdata/
+-rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.2/src/gmfakerdata/__init__.py
+-rw-rw-rw-   0        0        0    89848 2023-04-22 07:37:37.000000 gmsofttest-0.0.2/src/gmfakerdata/china_address.py
+-rw-rw-rw-   0        0        0     4261 2023-04-22 13:37:51.000000 gmsofttest-0.0.2/src/gmfakerdata/getidcard.py
+-rw-rw-rw-   0        0        0     2071 2023-03-11 05:43:46.000000 gmsofttest-0.0.2/src/gmfakerdata/getrandomdata.py
+-rw-rw-rw-   0        0        0     4490 2023-04-22 10:02:28.000000 gmsofttest-0.0.2/src/gmfakerdata/sucreditcode.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:35:04.000000 gmsofttest-0.0.2/src/gmmysql/
+-rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.2/src/gmmysql/__init__.py
+-rw-rw-rw-   0        0        0    12335 2023-03-08 06:26:47.000000 gmsofttest-0.0.2/src/gmmysql/mysqlexe.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:35:04.000000 gmsofttest-0.0.2/src/gmmysql/utils/
+-rw-rw-rw-   0        0        0      125 2023-02-13 02:10:07.000000 gmsofttest-0.0.2/src/gmmysql/utils/__init__.py
+-rw-rw-rw-   0        0        0     2214 2022-12-06 12:17:47.000000 gmsofttest-0.0.2/src/gmmysql/utils/yamlhandler.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:35:04.000000 gmsofttest-0.0.2/src/gmsofttest.egg-info/
+-rw-rw-rw-   0        0        0      655 2023-05-15 12:35:04.000000 gmsofttest-0.0.2/src/gmsofttest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-05-15 12:35:04.000000 gmsofttest-0.0.2/src/gmsofttest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 12:35:04.000000 gmsofttest-0.0.2/src/gmsofttest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-15 12:35:04.000000 gmsofttest-0.0.2/src/gmsofttest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 12:35:04.000000 gmsofttest-0.0.2/src/gmverifyhandler/
+-rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.2/src/gmverifyhandler/__init__.py
+-rw-rw-rw-   0        0        0      205 2023-02-11 08:09:19.000000 gmsofttest-0.0.2/src/gmverifyhandler/bye.py
```

### Comparing `gmsofttest-0.0.1/LICENSE` & `gmsofttest-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.1/PKG-INFO` & `gmsofttest-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmsofttest
-Version: 0.0.1
+Version: 0.0.2
 Summary: 大家软件内部测试技术线支撑工具
 Home-page: https://www.gec123.com
 Author: ronaldsu
 Author-email: uph4rmt@dingtalk.com
 Project-URL: Bug Tracker, https://www.gpwbeta.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,18 +15,12 @@
 
 # Gmtestplugin
 
     大家软件Python插件定制私有库开发项目
 
 ## change logs
 
-v0.0.4 优化组件
-
-v0.0.3 新增组件
-gmfakerdata组件：模拟生成测试数据
-gmmysql:数据库连接生成工具，可直接调用show,test1,test2数据库
-
 v0.0.2 
-  更新mydemo-package 实验项目
+  try something
 
 v0.0.1 
   mydemo-package 实验项目
```

### Comparing `gmsofttest-0.0.1/setup.py` & `gmsofttest-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gmsofttest",
-    version="0.0.1",
+    version="0.0.2",
     author="ronaldsu",
     author_email="uph4rmt@dingtalk.com",
     description="大家软件内部测试技术线支撑工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.gec123.com",
     project_urls={
```

### Comparing `gmsofttest-0.0.1/src/gmfakerdata/china_address.py` & `gmsofttest-0.0.2/src/gmfakerdata/china_address.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.1/src/gmfakerdata/getidcard.py` & `gmsofttest-0.0.2/src/gmfakerdata/getidcard.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.1/src/gmfakerdata/getrandomdata.py` & `gmsofttest-0.0.2/src/gmfakerdata/getrandomdata.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.1/src/gmfakerdata/sucreditcode.py` & `gmsofttest-0.0.2/src/gmfakerdata/sucreditcode.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.1/src/gmmysql/mysqlexe.py` & `gmsofttest-0.0.2/src/gmmysql/mysqlexe.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.1/src/gmmysql/utils/yamlhandler.py` & `gmsofttest-0.0.2/src/gmmysql/utils/yamlhandler.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.1/src/gmsofttest.egg-info/PKG-INFO` & `gmsofttest-0.0.2/src/gmsofttest.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmsofttest
-Version: 0.0.1
+Version: 0.0.2
 Summary: 大家软件内部测试技术线支撑工具
 Home-page: https://www.gec123.com
 Author: ronaldsu
 Author-email: uph4rmt@dingtalk.com
 Project-URL: Bug Tracker, https://www.gpwbeta.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,18 +15,12 @@
 
 # Gmtestplugin
 
     大家软件Python插件定制私有库开发项目
 
 ## change logs
 
-v0.0.4 优化组件
-
-v0.0.3 新增组件
-gmfakerdata组件：模拟生成测试数据
-gmmysql:数据库连接生成工具，可直接调用show,test1,test2数据库
-
 v0.0.2 
-  更新mydemo-package 实验项目
+  try something
 
 v0.0.1 
   mydemo-package 实验项目
```

### Comparing `gmsofttest-0.0.1/src/gmsofttest.egg-info/SOURCES.txt` & `gmsofttest-0.0.2/src/gmsofttest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

