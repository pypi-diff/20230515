# Comparing `tmp/ToolBox4Test-1.0.2.tar.gz` & `tmp/ToolBox4Test-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ToolBox4Test-1.0.2.tar", last modified: Mon May 15 14:28:49 2023, max compression
+gzip compressed data, was "ToolBox4Test-1.0.3.tar", last modified: Mon May 15 14:54:11 2023, max compression
```

## Comparing `ToolBox4Test-1.0.2.tar` & `ToolBox4Test-1.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 14:28:49.267102 ToolBox4Test-1.0.2/
--rw-rw-rw-   0        0        0       90 2023-05-14 14:00:29.000000 ToolBox4Test-1.0.2/.gitignore
--rw-rw-rw-   0        0        0     1085 2023-05-14 12:44:22.000000 ToolBox4Test-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       43 2023-05-15 14:21:35.000000 ToolBox4Test-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1397 2023-05-15 14:28:49.267102 ToolBox4Test-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      891 2023-05-05 03:36:31.000000 ToolBox4Test-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 14:28:49.220238 ToolBox4Test-1.0.2/TestToolBox/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:28:49.220238 ToolBox4Test-1.0.2/TestToolBox/BaseUtility/
--rw-rw-rw-   0        0        0        0 2021-10-11 01:43:52.000000 ToolBox4Test-1.0.2/TestToolBox/BaseUtility/__init__.py
--rw-rw-rw-   0        0        0    32884 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.2/TestToolBox/BaseUtility/adbShell.py
--rw-rw-rw-   0        0        0     8958 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.2/TestToolBox/BaseUtility/dataDriver.py
--rw-rw-rw-   0        0        0    15470 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.2/TestToolBox/BaseUtility/iterToolkit.py
--rw-rw-rw-   0        0        0    22709 2023-05-14 11:57:25.000000 ToolBox4Test-1.0.2/TestToolBox/BaseUtility/toolkit.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:28:49.235894 ToolBox4Test-1.0.2/TestToolBox/CaseData/
--rw-rw-rw-   0        0        0      490 2023-05-05 03:35:53.000000 ToolBox4Test-1.0.2/TestToolBox/CaseData/__init__.py
--rw-rw-rw-   0        0        0    15310 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.2/TestToolBox/CaseData/generateXmind.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:28:49.251508 ToolBox4Test-1.0.2/TestToolBox/Common/
--rw-rw-rw-   0        0        0     1322 2023-05-14 12:22:11.000000 ToolBox4Test-1.0.2/TestToolBox/Common/Api_Template_Doc.yml
--rw-rw-rw-   0        0        0     4308 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.2/TestToolBox/Common/CMS_COMMON_ENUM.yml
--rw-rw-rw-   0        0        0     6107 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.2/TestToolBox/Common/CMS_Rules.yml
--rw-rw-rw-   0        0        0        0 2021-10-11 01:39:57.000000 ToolBox4Test-1.0.2/TestToolBox/Common/__init__.py
--rw-rw-rw-   0        0        0    11847 2023-05-15 14:25:10.000000 ToolBox4Test-1.0.2/TestToolBox/Common/initConfig.py
--rw-rw-rw-   0        0        0    17339 2023-05-14 11:57:25.000000 ToolBox4Test-1.0.2/TestToolBox/Common/initRequest.py
--rw-rw-rw-   0        0        0    11320 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.2/TestToolBox/Common/initRule.py
--rw-rw-rw-   0        0        0    15112 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.2/TestToolBox/Common/initUIEnv.py
--rw-rw-rw-   0        0        0      656 2023-05-14 13:12:05.000000 ToolBox4Test-1.0.2/TestToolBox/__init__.py
--rw-rw-rw-   0        0        0     3164 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.2/TestToolBox/invokeFuncTrack.py
--rwxrwxrwx   0        0        0       25 2023-05-05 03:35:53.000000 ToolBox4Test-1.0.2/TestToolBox/toolbox.bat
--rw-rw-rw-   0        0        0    25522 2023-05-14 11:21:50.000000 ToolBox4Test-1.0.2/TestToolBox/toolbox.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:28:49.267102 ToolBox4Test-1.0.2/ToolBox4Test.egg-info/
--rw-rw-rw-   0        0        0     1397 2023-05-15 14:28:49.000000 ToolBox4Test-1.0.2/ToolBox4Test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      914 2023-05-15 14:28:49.000000 ToolBox4Test-1.0.2/ToolBox4Test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 14:28:49.000000 ToolBox4Test-1.0.2/ToolBox4Test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-15 14:28:49.000000 ToolBox4Test-1.0.2/ToolBox4Test.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      193 2023-05-15 14:28:49.000000 ToolBox4Test-1.0.2/ToolBox4Test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-15 14:28:49.000000 ToolBox4Test-1.0.2/ToolBox4Test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      204 2023-05-14 12:59:26.000000 ToolBox4Test-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 14:28:49.267102 ToolBox4Test-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3648 2023-05-15 14:28:45.000000 ToolBox4Test-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:54:10.999469 ToolBox4Test-1.0.3/
+-rw-rw-rw-   0        0        0       90 2023-05-14 14:00:29.000000 ToolBox4Test-1.0.3/.gitignore
+-rw-rw-rw-   0        0        0     1085 2023-05-14 12:44:22.000000 ToolBox4Test-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-05-15 14:21:35.000000 ToolBox4Test-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1397 2023-05-15 14:54:10.998788 ToolBox4Test-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      891 2023-05-05 03:36:31.000000 ToolBox4Test-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 14:54:10.943222 ToolBox4Test-1.0.3/TestToolBox/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:54:10.956156 ToolBox4Test-1.0.3/TestToolBox/BaseUtility/
+-rw-rw-rw-   0        0        0        0 2021-10-11 01:43:52.000000 ToolBox4Test-1.0.3/TestToolBox/BaseUtility/__init__.py
+-rw-rw-rw-   0        0        0    32884 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/BaseUtility/adbShell.py
+-rw-rw-rw-   0        0        0     8958 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/BaseUtility/dataDriver.py
+-rw-rw-rw-   0        0        0    15470 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/BaseUtility/iterToolkit.py
+-rw-rw-rw-   0        0        0    22709 2023-05-14 11:57:25.000000 ToolBox4Test-1.0.3/TestToolBox/BaseUtility/toolkit.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:54:10.960572 ToolBox4Test-1.0.3/TestToolBox/CaseData/
+-rw-rw-rw-   0        0        0      490 2023-05-05 03:35:53.000000 ToolBox4Test-1.0.3/TestToolBox/CaseData/__init__.py
+-rw-rw-rw-   0        0        0    15310 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/CaseData/generateXmind.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:54:10.981314 ToolBox4Test-1.0.3/TestToolBox/Common/
+-rw-rw-rw-   0        0        0     1322 2023-05-14 12:22:11.000000 ToolBox4Test-1.0.3/TestToolBox/Common/Api_Template_Doc.yml
+-rw-rw-rw-   0        0        0     4308 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/Common/CMS_COMMON_ENUM.yml
+-rw-rw-rw-   0        0        0     6107 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/Common/CMS_Rules.yml
+-rw-rw-rw-   0        0        0        0 2021-10-11 01:39:57.000000 ToolBox4Test-1.0.3/TestToolBox/Common/__init__.py
+-rw-rw-rw-   0        0        0    11847 2023-05-15 14:25:10.000000 ToolBox4Test-1.0.3/TestToolBox/Common/initConfig.py
+-rw-rw-rw-   0        0        0    17339 2023-05-14 11:57:25.000000 ToolBox4Test-1.0.3/TestToolBox/Common/initRequest.py
+-rw-rw-rw-   0        0        0    11320 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/Common/initRule.py
+-rw-rw-rw-   0        0        0    15112 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/Common/initUIEnv.py
+-rw-rw-rw-   0        0        0      656 2023-05-14 13:12:05.000000 ToolBox4Test-1.0.3/TestToolBox/__init__.py
+-rw-rw-rw-   0        0        0     3164 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/invokeFuncTrack.py
+-rwxrwxrwx   0        0        0       25 2023-05-05 03:35:53.000000 ToolBox4Test-1.0.3/TestToolBox/toolbox.bat
+-rw-rw-rw-   0        0        0    25522 2023-05-14 11:21:50.000000 ToolBox4Test-1.0.3/TestToolBox/toolbox.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:54:10.996792 ToolBox4Test-1.0.3/ToolBox4Test.egg-info/
+-rw-rw-rw-   0        0        0     1397 2023-05-15 14:54:10.000000 ToolBox4Test-1.0.3/ToolBox4Test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2023-05-15 14:54:10.000000 ToolBox4Test-1.0.3/ToolBox4Test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 14:54:10.000000 ToolBox4Test-1.0.3/ToolBox4Test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-15 14:54:10.000000 ToolBox4Test-1.0.3/ToolBox4Test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      193 2023-05-15 14:54:10.000000 ToolBox4Test-1.0.3/ToolBox4Test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-15 14:54:10.000000 ToolBox4Test-1.0.3/ToolBox4Test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      223 2023-05-15 14:48:08.000000 ToolBox4Test-1.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 14:54:10.999469 ToolBox4Test-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3635 2023-05-15 14:48:08.000000 ToolBox4Test-1.0.3/setup.py
```

### Comparing `ToolBox4Test-1.0.2/LICENSE` & `ToolBox4Test-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/PKG-INFO` & `ToolBox4Test-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ToolBox4Test
-Version: 1.0.2
+Version: 1.0.3
 Summary: TestToolbox 测试工具箱
 Home-page: https://gitlab.com/Gavinwhy/TestToolBox
 Author: Gavin
 Author-email: guowenwhy@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ToolBox4Test-1.0.2/README.md` & `ToolBox4Test-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/BaseUtility/adbShell.py` & `ToolBox4Test-1.0.3/TestToolBox/BaseUtility/adbShell.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/BaseUtility/dataDriver.py` & `ToolBox4Test-1.0.3/TestToolBox/BaseUtility/dataDriver.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/BaseUtility/iterToolkit.py` & `ToolBox4Test-1.0.3/TestToolBox/BaseUtility/iterToolkit.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/BaseUtility/toolkit.py` & `ToolBox4Test-1.0.3/TestToolBox/BaseUtility/toolkit.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/CaseData/generateXmind.py` & `ToolBox4Test-1.0.3/TestToolBox/CaseData/generateXmind.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/Common/Api_Template_Doc.yml` & `ToolBox4Test-1.0.3/TestToolBox/Common/Api_Template_Doc.yml`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/Common/CMS_COMMON_ENUM.yml` & `ToolBox4Test-1.0.3/TestToolBox/Common/CMS_COMMON_ENUM.yml`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/Common/CMS_Rules.yml` & `ToolBox4Test-1.0.3/TestToolBox/Common/CMS_Rules.yml`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/Common/initConfig.py` & `ToolBox4Test-1.0.3/TestToolBox/Common/initConfig.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/Common/initRequest.py` & `ToolBox4Test-1.0.3/TestToolBox/Common/initRequest.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/Common/initRule.py` & `ToolBox4Test-1.0.3/TestToolBox/Common/initRule.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/Common/initUIEnv.py` & `ToolBox4Test-1.0.3/TestToolBox/Common/initUIEnv.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/__init__.py` & `ToolBox4Test-1.0.3/TestToolBox/__init__.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/invokeFuncTrack.py` & `ToolBox4Test-1.0.3/TestToolBox/invokeFuncTrack.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/TestToolBox/toolbox.py` & `ToolBox4Test-1.0.3/TestToolBox/toolbox.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/ToolBox4Test.egg-info/PKG-INFO` & `ToolBox4Test-1.0.3/ToolBox4Test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ToolBox4Test
-Version: 1.0.2
+Version: 1.0.3
 Summary: TestToolbox 测试工具箱
 Home-page: https://gitlab.com/Gavinwhy/TestToolBox
 Author: Gavin
 Author-email: guowenwhy@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ToolBox4Test-1.0.2/ToolBox4Test.egg-info/SOURCES.txt` & `ToolBox4Test-1.0.3/ToolBox4Test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.2/setup.py` & `ToolBox4Test-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ToolBox4Test",
-    version="1.0.2",
+    version="1.0.3",
     author="Gavin",
     author_email="guowenwhy@foxmail.com",
     description="TestToolbox 测试工具箱",
     long_description=long_description,
     long_description_content_type='text/markdown',
     
     # 项目主页
@@ -67,22 +67,21 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
     ],
     
     install_requires=[
-        'setuptools>=67.7.2',
-        'yaml>=0.2.5',
         'pyyaml>=6.0',
         'jsonpath>=0.82',
         'pycallgraph>=1.0.1',
         'pytest>=7.1.2',
         'selenium>=4.9.0',
         'faker>=13.3.2',
         'requests>=2.29.0',
         'xmind>=1.2.0',
         'loguru>=0.5.3',
         'pymysql>=1.0.2',
         'redis>=3.5.3',
+        'business-rules-enhanced>=1.2.2'
     ]
 )
```

