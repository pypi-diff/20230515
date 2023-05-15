# Comparing `tmp/asa-tools-0.1.2.tar.gz` & `tmp/asa-tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asa-tools-0.1.2.tar", last modified: Sat May 13 11:25:35 2023, max compression
+gzip compressed data, was "asa-tools-0.1.3.tar", last modified: Mon May 15 10:46:47 2023, max compression
```

## Comparing `asa-tools-0.1.2.tar` & `asa-tools-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 11:25:35.410844 asa-tools-0.1.2/
--rw-rw-rw-   0        0        0      393 2023-05-13 11:25:35.408850 asa-tools-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-13 11:25:35.404860 asa-tools-0.1.2/asa_tools.egg-info/
--rw-rw-rw-   0        0        0      393 2023-05-13 11:25:35.000000 asa-tools-0.1.2/asa_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-05-13 11:25:35.000000 asa-tools-0.1.2/asa_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 11:25:35.000000 asa-tools-0.1.2/asa_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-13 11:25:35.000000 asa-tools-0.1.2/asa_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-13 11:25:35.000000 asa-tools-0.1.2/asa_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-13 11:25:35.000000 asa-tools-0.1.2/asa_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 11:25:35.410844 asa-tools-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      649 2023-05-13 11:25:31.000000 asa-tools-0.1.2/setup.py
--rw-rw-rw-   0        0        0     2575 2023-05-13 11:23:03.000000 asa-tools-0.1.2/turn2release.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:46:47.916396 asa-tools-0.1.3/
+-rw-rw-rw-   0        0        0      393 2023-05-15 10:46:47.912407 asa-tools-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-15 10:46:47.906423 asa-tools-0.1.3/asa_tools.egg-info/
+-rw-rw-rw-   0        0        0      393 2023-05-15 10:46:47.000000 asa-tools-0.1.3/asa_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-05-15 10:46:47.000000 asa-tools-0.1.3/asa_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 10:46:47.000000 asa-tools-0.1.3/asa_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-15 10:46:47.000000 asa-tools-0.1.3/asa_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-15 10:46:47.000000 asa-tools-0.1.3/asa_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-15 10:46:47.000000 asa-tools-0.1.3/asa_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 10:46:47.916396 asa-tools-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-05-15 10:46:26.000000 asa-tools-0.1.3/setup.py
+-rw-rw-rw-   0        0        0     3421 2023-05-15 02:13:56.000000 asa-tools-0.1.3/turn2release.py
```

### Comparing `asa-tools-0.1.2/setup.py` & `asa-tools-0.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from setuptools import setup
 
 setup(
     name='asa-tools',
-    version='0.1.2',
+    version='0.1.3',
     py_modules=['turn2release'],
     install_requires=[
         'Click',
-        'openpyxl'
+        'openpyxl',
+        'requests',
+        'tqdm'
     ],
     entry_points='''
         [console_scripts]
         asa=turn2release:cli
     ''',
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `asa-tools-0.1.2/turn2release.py` & `asa-tools-0.1.3/turn2release.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import click
 import shutil
+import configparser
 from pathlib import Path
 import re
 from out_dutys import out_duty
 import os
 from copyallmp4 import cmp4, createTurnTxt, turnToMp4
+from spyderBili import bifirstResolve
 
 asa_home = os.environ.get('ASA_HOME')
-
+# config = configparser.ConfigParser()
+config = configparser.RawConfigParser()
+config.read('conf.ini')
+sess = config.get('spiderbi','SESSDATA')
 
 @click.group()
 def cli():
     """
     待完成：
         - 下载进度条，可传递视频传入的格式avi、mp4等
         - 抖音下载并有进度条
         - git管理，更新就自动发布pypi
+        - b站多视频下载，需要判断是否有p参数 如 https://www.bilibili.com/video/BV1ha4y1H7sx?p=59 是多个视频
+            https://www.bilibili.com/video/BV11S4y1a7X9/  是单个视频
     """
     pass
 
 
 @click.command()
 @click.argument('source')
 def ra(source):
@@ -85,14 +92,26 @@
 def ttm4(e):
     """
     合并mp4视频，转为h264编码mp4或海信电视可播放的mp4
     equipment ： --e
     """
     turnToMp4(e)
 
+@click.command()
+@click.argument('url')
+@click.option("-t", "--dtype", "dtype",default=0,help="定义下载的类型，0为不下载番剧，其它值为下载。如 asa bira https://www.bilibili.com/video/BV1ha4y1H7sx?p=9 -t 1")
+def bira(url,dtype):
+    """
+    解析下载b站视频
+    需要新建conf.ini并配置
+    [spiderbi]
+    SESSDATA = "XXXX"
+    """
+    bifirstResolve(url,sess,dtype)
 
 cli.add_command(ra)
 cli.add_command(cf)
 cli.add_command(od)
 cli.add_command(cp4)
 cli.add_command(ctt)
 cli.add_command(ttm4)
+cli.add_command(bira)
```

