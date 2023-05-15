# Comparing `tmp/t2c-0.0.5.tar.gz` & `tmp/t2c-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2c-0.0.5.tar", last modified: Mon May 15 17:01:24 2023, max compression
+gzip compressed data, was "t2c-0.0.6.tar", last modified: Mon May 15 17:12:00 2023, max compression
```

## Comparing `t2c-0.0.5.tar` & `t2c-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-15 17:01:24.248734 t2c-0.0.5/
--rw-r--r--   0 iguangyu   (502) staff       (20)    11356 2023-05-13 17:09:56.000000 t2c-0.0.5/LICENSE
--rw-r--r--   0 iguangyu   (502) staff       (20)     1257 2023-05-15 17:01:24.248562 t2c-0.0.5/PKG-INFO
--rw-r--r--   0 iguangyu   (502) staff       (20)      719 2023-05-15 17:00:47.000000 t2c-0.0.5/README.md
--rw-r--r--   0 iguangyu   (502) staff       (20)       38 2023-05-15 17:01:24.248775 t2c-0.0.5/setup.cfg
--rw-r--r--   0 iguangyu   (502) staff       (20)      918 2023-05-15 17:00:53.000000 t2c-0.0.5/setup.py
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-15 17:01:24.247324 t2c-0.0.5/t2c/
--rw-r--r--   0 iguangyu   (502) staff       (20)       86 2023-05-15 17:01:12.000000 t2c-0.0.5/t2c/__init__.py
--rw-r--r--   0 iguangyu   (502) staff       (20)     7505 2023-05-15 16:59:33.000000 t2c-0.0.5/t2c/text2cron.py
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-15 17:01:24.248343 t2c-0.0.5/t2c.egg-info/
--rw-r--r--   0 iguangyu   (502) staff       (20)     1257 2023-05-15 17:01:24.000000 t2c-0.0.5/t2c.egg-info/PKG-INFO
--rw-r--r--   0 iguangyu   (502) staff       (20)      193 2023-05-15 17:01:24.000000 t2c-0.0.5/t2c.egg-info/SOURCES.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)        1 2023-05-15 17:01:24.000000 t2c-0.0.5/t2c.egg-info/dependency_links.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)       15 2023-05-15 17:01:24.000000 t2c-0.0.5/t2c.egg-info/requires.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)        4 2023-05-15 17:01:24.000000 t2c-0.0.5/t2c.egg-info/top_level.txt
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-15 17:12:00.003732 t2c-0.0.6/
+-rw-r--r--   0 iguangyu   (502) staff       (20)    11356 2023-05-13 17:09:56.000000 t2c-0.0.6/LICENSE
+-rw-r--r--   0 iguangyu   (502) staff       (20)     1297 2023-05-15 17:12:00.003304 t2c-0.0.6/PKG-INFO
+-rw-r--r--   0 iguangyu   (502) staff       (20)      719 2023-05-15 17:00:47.000000 t2c-0.0.6/README.md
+-rw-r--r--   0 iguangyu   (502) staff       (20)       38 2023-05-15 17:12:00.003795 t2c-0.0.6/setup.cfg
+-rw-r--r--   0 iguangyu   (502) staff       (20)      969 2023-05-15 17:11:47.000000 t2c-0.0.6/setup.py
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-15 17:12:00.002260 t2c-0.0.6/t2c/
+-rw-r--r--   0 iguangyu   (502) staff       (20)       86 2023-05-15 17:11:33.000000 t2c-0.0.6/t2c/__init__.py
+-rw-r--r--   0 iguangyu   (502) staff       (20)     7505 2023-05-15 16:59:33.000000 t2c-0.0.6/t2c/text2cron.py
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-15 17:12:00.003114 t2c-0.0.6/t2c.egg-info/
+-rw-r--r--   0 iguangyu   (502) staff       (20)     1297 2023-05-15 17:11:59.000000 t2c-0.0.6/t2c.egg-info/PKG-INFO
+-rw-r--r--   0 iguangyu   (502) staff       (20)      193 2023-05-15 17:11:59.000000 t2c-0.0.6/t2c.egg-info/SOURCES.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)        1 2023-05-15 17:11:59.000000 t2c-0.0.6/t2c.egg-info/dependency_links.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)       15 2023-05-15 17:11:59.000000 t2c-0.0.6/t2c.egg-info/requires.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)        4 2023-05-15 17:11:59.000000 t2c-0.0.6/t2c.egg-info/top_level.txt
```

### Comparing `t2c-0.0.5/LICENSE` & `t2c-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `t2c-0.0.5/PKG-INFO` & `t2c-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: t2c
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python Library that converts human readable text to Cron Expression.
 Home-page: https://github.com/iguangyu/text2cron
 Author: iguangyu
 Author-email: oofheaven7@gmail.com
 License: MIT
 Keywords: text cron text langchain gpt npl
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## A Python Library that converts human readable text to Cron Expression
 ## 可以将人类语言转换为cron表达式的Python库
 
 ### Installation
 ``` bash
```

### Comparing `t2c-0.0.5/README.md` & `t2c-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `t2c-0.0.5/setup.py` & `t2c-0.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 # Get the long description from the relevant file
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='t2c',
-    version='0.0.5',
+    version='0.0.6',
     description='A Python Library that converts human readable text to Cron Expression.',
     long_description=long_description,
+    long_description_content_type="text/markdown",
     url='https://github.com/iguangyu/text2cron',
     author='iguangyu',
     author_email='oofheaven7@gmail.com',
     license='MIT',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

### Comparing `t2c-0.0.5/t2c/text2cron.py` & `t2c-0.0.6/t2c/text2cron.py`

 * *Files identical despite different names*

### Comparing `t2c-0.0.5/t2c.egg-info/PKG-INFO` & `t2c-0.0.6/t2c.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: t2c
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python Library that converts human readable text to Cron Expression.
 Home-page: https://github.com/iguangyu/text2cron
 Author: iguangyu
 Author-email: oofheaven7@gmail.com
 License: MIT
 Keywords: text cron text langchain gpt npl
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## A Python Library that converts human readable text to Cron Expression
 ## 可以将人类语言转换为cron表达式的Python库
 
 ### Installation
 ``` bash
```

