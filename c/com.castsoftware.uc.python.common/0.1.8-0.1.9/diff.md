# Comparing `tmp/com.castsoftware.uc.python.common-0.1.8.tar.gz` & `tmp/com.castsoftware.uc.python.common-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.python.common-0.1.8.tar", last modified: Tue Feb 21 23:08:51 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.python.common-0.1.9.tar", last modified: Fri Feb 24 19:00:21 2023, max compression
```

## Comparing `com.castsoftware.uc.python.common-0.1.8.tar` & `com.castsoftware.uc.python.common-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-21 23:08:51.052223 com.castsoftware.uc.python.common-0.1.8/
--rw-rw-rw-   0        0        0    35823 2021-04-05 17:40:19.000000 com.castsoftware.uc.python.common-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      712 2023-02-21 23:08:51.049221 com.castsoftware.uc.python.common-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      103 2021-06-01 15:37:40.000000 com.castsoftware.uc.python.common-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-21 23:08:50.983625 com.castsoftware.uc.python.common-0.1.8/cast_common/
--rw-rw-rw-   0        0        0        0 2021-06-01 14:42:59.000000 com.castsoftware.uc.python.common-0.1.8/cast_common/__init__.py
--rw-rw-rw-   0        0        0     2036 2022-12-28 17:18:00.000000 com.castsoftware.uc.python.common-0.1.8/cast_common/abstractClass.py
--rw-rw-rw-   0        0        0    11962 2023-01-25 20:42:45.000000 com.castsoftware.uc.python.common-0.1.8/cast_common/aipRestCall.py
--rw-rw-rw-   0        0        0     5199 2023-01-25 21:07:43.000000 com.castsoftware.uc.python.common-0.1.8/cast_common/hlRestCall.py
--rw-rw-rw-   0        0        0     1681 2023-01-25 15:27:20.000000 com.castsoftware.uc.python.common-0.1.8/cast_common/logger.py
--rw-rw-rw-   0        0        0     4421 2023-01-25 21:09:02.000000 com.castsoftware.uc.python.common-0.1.8/cast_common/restAPI.py
--rw-rw-rw-   0        0        0     7175 2023-02-17 22:27:29.000000 com.castsoftware.uc.python.common-0.1.8/cast_common/util.py
-drwxrwxrwx   0        0        0        0 2023-02-21 23:08:51.044613 com.castsoftware.uc.python.common-0.1.8/com.castsoftware.uc.python.common.egg-info/
--rw-rw-rw-   0        0        0      712 2023-02-21 23:08:50.000000 com.castsoftware.uc.python.common-0.1.8/com.castsoftware.uc.python.common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-02-21 23:08:50.000000 com.castsoftware.uc.python.common-0.1.8/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-21 23:08:50.000000 com.castsoftware.uc.python.common-0.1.8/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-02-21 23:08:50.000000 com.castsoftware.uc.python.common-0.1.8/com.castsoftware.uc.python.common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      618 2023-02-21 23:08:22.000000 com.castsoftware.uc.python.common-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-21 23:08:51.053223 com.castsoftware.uc.python.common-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-02-24 19:00:21.430959 com.castsoftware.uc.python.common-0.1.9/
+-rw-rw-rw-   0        0        0    35823 2021-04-05 17:40:19.000000 com.castsoftware.uc.python.common-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      712 2023-02-24 19:00:21.427959 com.castsoftware.uc.python.common-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2021-06-01 15:37:40.000000 com.castsoftware.uc.python.common-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-24 19:00:21.390949 com.castsoftware.uc.python.common-0.1.9/cast_common/
+-rw-rw-rw-   0        0        0        0 2021-06-01 14:42:59.000000 com.castsoftware.uc.python.common-0.1.9/cast_common/__init__.py
+-rw-rw-rw-   0        0        0     2036 2022-12-28 17:18:00.000000 com.castsoftware.uc.python.common-0.1.9/cast_common/abstractClass.py
+-rw-rw-rw-   0        0        0    11962 2023-01-25 20:42:45.000000 com.castsoftware.uc.python.common-0.1.9/cast_common/aipRestCall.py
+-rw-rw-rw-   0        0        0     5199 2023-01-25 21:07:43.000000 com.castsoftware.uc.python.common-0.1.9/cast_common/hlRestCall.py
+-rw-rw-rw-   0        0        0     1681 2023-01-25 15:27:20.000000 com.castsoftware.uc.python.common-0.1.9/cast_common/logger.py
+-rw-rw-rw-   0        0        0     4421 2023-01-25 21:09:02.000000 com.castsoftware.uc.python.common-0.1.9/cast_common/restAPI.py
+-rw-rw-rw-   0        0        0     7243 2023-02-24 18:59:02.000000 com.castsoftware.uc.python.common-0.1.9/cast_common/util.py
+drwxrwxrwx   0        0        0        0 2023-02-24 19:00:21.422959 com.castsoftware.uc.python.common-0.1.9/com.castsoftware.uc.python.common.egg-info/
+-rw-rw-rw-   0        0        0      712 2023-02-24 19:00:21.000000 com.castsoftware.uc.python.common-0.1.9/com.castsoftware.uc.python.common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-02-24 19:00:21.000000 com.castsoftware.uc.python.common-0.1.9/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-24 19:00:21.000000 com.castsoftware.uc.python.common-0.1.9/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-02-24 19:00:21.000000 com.castsoftware.uc.python.common-0.1.9/com.castsoftware.uc.python.common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      618 2023-02-24 19:00:03.000000 com.castsoftware.uc.python.common-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-02-24 19:00:21.431962 com.castsoftware.uc.python.common-0.1.9/setup.cfg
```

### Comparing `com.castsoftware.uc.python.common-0.1.8/LICENSE` & `com.castsoftware.uc.python.common-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-0.1.8/PKG-INFO` & `com.castsoftware.uc.python.common-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 0.1.8
+Version: 0.1.9
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.python.common-0.1.8/cast_common/abstractClass.py` & `com.castsoftware.uc.python.common-0.1.9/cast_common/abstractClass.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-0.1.8/cast_common/aipRestCall.py` & `com.castsoftware.uc.python.common-0.1.9/cast_common/aipRestCall.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-0.1.8/cast_common/hlRestCall.py` & `com.castsoftware.uc.python.common-0.1.9/cast_common/hlRestCall.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-0.1.8/cast_common/logger.py` & `com.castsoftware.uc.python.common-0.1.9/cast_common/logger.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-0.1.8/cast_common/restAPI.py` & `com.castsoftware.uc.python.common-0.1.9/cast_common/restAPI.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-0.1.8/cast_common/util.py` & `com.castsoftware.uc.python.common-0.1.9/cast_common/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,17 +140,20 @@
     ret = []
     while process.poll() is None:
         line = process.stdout.readline()
         line = line.lstrip("b'").rstrip('\n')
         if output == True and len(line.strip(' ')) > 0:
             print(line)
         ret.append(line)
-    stdout, stderr = process.communicate()
+    try:
+        stdout, stderr = process.communicate()
+    except: 
+        return process.returncode,ret
     return process.returncode,ret
-    
+     
 def format_table(writer, data, sheet_name,width=None):
     
     data.to_excel(writer, index=False, sheet_name=sheet_name, startrow=1,header=False)
 
     workbook = writer.book
     worksheet = writer.sheets[sheet_name]
     rows = len(data)+1
```

### Comparing `com.castsoftware.uc.python.common-0.1.8/com.castsoftware.uc.python.common.egg-info/PKG-INFO` & `com.castsoftware.uc.python.common-0.1.9/com.castsoftware.uc.python.common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 0.1.8
+Version: 0.1.9
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.python.common-0.1.8/pyproject.toml` & `com.castsoftware.uc.python.common-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name='com.castsoftware.uc.python.common'
 description="A set of common classes and methods for use with python projects"
 
-version='0.1.8' #prod version
+version='0.1.9' #prod version
 #version='0.1.8' #test version
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
```

