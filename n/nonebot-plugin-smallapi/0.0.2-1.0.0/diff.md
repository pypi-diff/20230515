# Comparing `tmp/nonebot_plugin_smallapi-0.0.2.tar.gz` & `tmp/nonebot_plugin_smallapi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_smallapi-0.0.2.tar", last modified: Mon May 15 01:32:58 2023, max compression
+gzip compressed data, was "nonebot_plugin_smallapi-1.0.0.tar", last modified: Mon May 15 01:47:33 2023, max compression
```

## Comparing `nonebot_plugin_smallapi-0.0.2.tar` & `nonebot_plugin_smallapi-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 01:32:58.138101 nonebot_plugin_smallapi-0.0.2/
--rwxr-xr-x   0 root         (0) root         (0)     1072 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      484 2023-05-15 01:32:58.138101 nonebot_plugin_smallapi-0.0.2/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     4851 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 01:32:58.135101 nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi/
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi/api_menu.py
--rw-r--r--   0 root         (0) root         (0)     2184 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi/api_pic.py
--rw-r--r--   0 root         (0) root         (0)     4418 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi/api_site.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi/api_text.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi/hander.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi/hander_site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 01:32:58.137102 nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      484 2023-05-15 01:32:57.000000 nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      481 2023-05-15 01:32:58.000000 nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 01:32:57.000000 nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-15 01:32:57.000000 nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)      918 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 01:32:58.138101 nonebot_plugin_smallapi-0.0.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1036 2023-05-15 01:32:16.000000 nonebot_plugin_smallapi-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 01:47:33.569897 nonebot_plugin_smallapi-1.0.0/
+-rwxr-xr-x   0 root         (0) root         (0)     1072 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      484 2023-05-15 01:47:33.569897 nonebot_plugin_smallapi-1.0.0/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     4851 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 01:47:33.567896 nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi/
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi/api_menu.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi/api_pic.py
+-rw-r--r--   0 root         (0) root         (0)     4418 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi/api_site.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi/api_text.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi/hander.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi/hander_site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 01:47:33.568897 nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      484 2023-05-15 01:47:33.000000 nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      481 2023-05-15 01:47:33.000000 nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 01:47:33.000000 nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-15 01:47:33.000000 nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)      918 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 01:47:33.569897 nonebot_plugin_smallapi-1.0.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1036 2023-05-15 01:46:03.000000 nonebot_plugin_smallapi-1.0.0/setup.py
```

### Comparing `nonebot_plugin_smallapi-0.0.2/LICENSE` & `nonebot_plugin_smallapi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-0.0.2/README.md` & `nonebot_plugin_smallapi-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi/api_menu.py` & `nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi/api_menu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi/api_pic.py` & `nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi/api_pic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi/api_site.py` & `nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi/api_site.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi/api_text.py` & `nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi/api_text.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi/hander.py` & `nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi/hander.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-0.0.2/nonebot_plugin_smallapi/hander_site.py` & `nonebot_plugin_smallapi-1.0.0/nonebot_plugin_smallapi/hander_site.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-0.0.2/pyproject.toml` & `nonebot_plugin_smallapi-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-0.0.2/setup.py` & `nonebot_plugin_smallapi-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools #导入setuptools打包工具
 
 install_requires=['jsonpath','nonebot2[aiohttp]','httpx'],
 
 setuptools.setup(
     name="nonebot_plugin_smallapi", # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.2",    #包版本号，便于维护版本
+    version="1.0.0",    #包版本号，便于维护版本
     author="Chaichaisi",    #作者，可以写自己的姓名
     author_email="chaichaisi@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="A small nonebot_plugin_smallapi plugin",#包的简述
     long_description="come in to read more",    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/chaichaisi/nonebot_plugin_smallapi",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

