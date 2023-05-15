# Comparing `tmp/serviceboot-2.1.4.tar.gz` & `tmp/serviceboot-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/serviceboot-2.1.4.tar", last modified: Fri May 12 01:55:21 2023, max compression
+gzip compressed data, was "dist/serviceboot-2.1.5.tar", last modified: Mon May 15 02:25:35 2023, max compression
```

## Comparing `serviceboot-2.1.4.tar` & `serviceboot-2.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-12 01:55:21.000000 serviceboot-2.1.4/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-12 01:55:21.000000 serviceboot-2.1.4/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1526 2023-05-09 04:02:39.000000 serviceboot-2.1.4/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2764 2023-04-04 03:17:10.000000 serviceboot-2.1.4/serviceboot/build_docker.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     4167 2023-04-03 13:17:50.000000 serviceboot-2.1.4/serviceboot/build_zip.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1376 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/command.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     4143 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/compile_python.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      417 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/config_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3010 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/consul_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3171 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/oauth_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2790 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/onboarding.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      178 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/request_info.py
--rw-rw-r--   0 hls       (1000) hls       (1000)    23524 2023-05-12 01:54:19.000000 serviceboot-2.1.4/serviceboot/serviceboot.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1144 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/token_service.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      556 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       83 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       93 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       12 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-12 01:55:21.000000 serviceboot-2.1.4/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2438 2023-05-12 01:55:19.000000 serviceboot-2.1.4/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-15 02:25:35.000000 serviceboot-2.1.5/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-15 02:25:35.000000 serviceboot-2.1.5/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1526 2023-05-09 04:02:39.000000 serviceboot-2.1.5/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3283 2023-05-15 02:24:29.000000 serviceboot-2.1.5/serviceboot/build_docker.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     4542 2023-05-15 02:24:29.000000 serviceboot-2.1.5/serviceboot/build_zip.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1376 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/command.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     4143 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/compile_python.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      417 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/config_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3010 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/consul_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3171 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/oauth_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2790 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/onboarding.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      178 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/request_info.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)    23524 2023-05-12 02:13:11.000000 serviceboot-2.1.5/serviceboot/serviceboot.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1144 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/token_service.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      556 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       83 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       93 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       12 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-15 02:25:35.000000 serviceboot-2.1.5/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2438 2023-05-15 02:25:29.000000 serviceboot-2.1.5/setup.py
```

### Comparing `serviceboot-2.1.4/PKG-INFO` & `serviceboot-2.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serviceboot
-Version: 2.1.4
+Version: 2.1.5
 Summary: ServiceBoot云原生微服务引擎
 Home-page: https://openi.pcl.ac.cn/cubepy/serviceboot
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # ServiceBoot云原生微服务引擎
```

### Comparing `serviceboot-2.1.4/README.md` & `serviceboot-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.4/serviceboot/build_docker.py` & `serviceboot-2.1.5/serviceboot/build_docker.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,24 +41,35 @@
     if platform.system() == 'Windows':
         os.system('rd /s /q temp')
         os.system('mkdir temp')
         os.system('xcopy /q application.yml temp')
         os.system('xcopy /q requirements.txt temp')
         os.system('xcopy /q pip-install-reqs.sh temp')
         os.system('xcopy /q Dockerfile temp')
+        os.system('xcopy /q README.md temp')
         os.system('mkdir temp\\app')
         os.system('xcopy /y /q /s /e app temp\\app')
+        if os.path.exists('docs'):
+            os.system('mkdir temp\\docs')
+            os.system('xcopy /y /q /s /e docs\\ temp\\docs\\')
+        if os.path.exists('demo_data'):
+            os.system('mkdir temp\\demo_data')
+            os.system('xcopy /y /q /s /e demo_data\\ temp\\demo_data\\')
     else:
         os.system('rm -rf temp')
         os.system('mkdir temp')
         os.system('cp ./application.yml ./temp')
         os.system('cp ./requirements.txt ./temp')
         os.system('cp ./pip-install-reqs.sh ./temp')
         os.system('cp ./Dockerfile ./temp')
         os.system('cp -rf ./app ./temp/')
+        if os.path.exists('docs'):
+            os.system('cp -rf ./docs ./temp/')
+        if os.path.exists('demo_data'):
+            os.system('cp -rf ./demo_data ./temp/')
 
     if build_web:
         if os.path.exists('./webapp/src'):
             cwd = os.getcwd()
             os.chdir(os.path.join(cwd, 'webapp'))
             if not os.path.exists('./node_modules'):
                 os.system('npm install')
```

### Comparing `serviceboot-2.1.4/serviceboot/build_zip.py` & `serviceboot-2.1.5/serviceboot/build_zip.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,30 +66,36 @@
         os.system('copy requirements.txt out\\{}\\'.format(name))
         os.system('copy pip-install-reqs.sh out\\{}\\'.format(name))
         if os.path.exists('Dockerfile'):
             os.system('copy Dockerfile out\\{}\\'.format(name))
         if os.path.exists('README.md'):
             os.system('copy README.md out\\{}\\'.format(name))
         if os.path.exists('docs'):
-            os.system('xcopy /y /q /s /e docs\\ out\\docs\\')
+            os.system('mkdir out\\{}\\docs'.format(name))
+            os.system('xcopy /y /q /s /e docs\\ out\\{}\\docs\\'.format(name))
+        if os.path.exists('demo_data'):
+            os.system('mkdir out\\{}\\demo_data'.format(name))
+            os.system('xcopy /y /q /s /e demo_data\\ out\\{}\\demo_data\\'.format(name))
         os.system('mkdir out\\{}\\app'.format(name))
         os.system('xcopy /y /q /s /e app\\ out\\{}\\app\\'.format(name))
     else:
         os.system('rm -rf ./out')
         os.system('mkdir out')
         os.system('mkdir out/{}'.format(name))
         os.system('cp ./application.yml ./out/{}/'.format(name))
         os.system('cp ./requirements.txt ./out/{}/'.format(name))
         os.system('cp ./pip-install-reqs.sh ./out/{}/'.format(name))
         if os.path.exists('Dockerfile'):
             os.system('cp ./Dockerfile ./out/{}/'.format(name))
         if os.path.exists('README.md'):
             os.system('cp ./README.md ./out/{}/'.format(name))
         if os.path.exists('docs'):
-            os.system('cp -r ./docs ./out/{}/'.format(name))
+            os.system('cp -rf ./docs ./out/{}/'.format(name))
+        if os.path.exists('demo_data'):
+            os.system('cp -rf ./demo_data ./out/{}/'.format(name))
         os.system('cp -rf ./app ./out/{}/'.format(name))
 
     if build_web:
         if os.path.exists('./webapp/src'):
             cwd = os.getcwd()
             os.chdir(os.path.join(cwd, 'webapp'))
             if not os.path.exists('./node_modules'):
```

### Comparing `serviceboot-2.1.4/serviceboot/command.py` & `serviceboot-2.1.5/serviceboot/command.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.4/serviceboot/compile_python.py` & `serviceboot-2.1.5/serviceboot/compile_python.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.4/serviceboot/consul_client.py` & `serviceboot-2.1.5/serviceboot/consul_client.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.4/serviceboot/oauth_client.py` & `serviceboot-2.1.5/serviceboot/oauth_client.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.4/serviceboot/onboarding.py` & `serviceboot-2.1.5/serviceboot/onboarding.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.4/serviceboot/serviceboot.py` & `serviceboot-2.1.5/serviceboot/serviceboot.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.4/serviceboot/token_service.py` & `serviceboot-2.1.5/serviceboot/token_service.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.4/serviceboot.egg-info/PKG-INFO` & `serviceboot-2.1.5/serviceboot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serviceboot
-Version: 2.1.4
+Version: 2.1.5
 Summary: ServiceBoot云原生微服务引擎
 Home-page: https://openi.pcl.ac.cn/cubepy/serviceboot
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # ServiceBoot云原生微服务引擎
```

### Comparing `serviceboot-2.1.4/serviceboot.egg-info/SOURCES.txt` & `serviceboot-2.1.5/serviceboot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.4/setup.py` & `serviceboot-2.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='serviceboot',
-    version='2.1.4',
+    version='2.1.5',
     author='cubeai',
     author_email='cubeai@163.com',
     description='ServiceBoot云原生微服务引擎',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```

