# Comparing `tmp/droidlysis-3.4.3.tar.gz` & `tmp/droidlysis-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "droidlysis-3.4.3.tar", last modified: Fri Mar 10 16:07:11 2023, max compression
+gzip compressed data, was "droidlysis-3.4.4.tar", last modified: Mon May 15 13:37:01 2023, max compression
```

## Comparing `droidlysis-3.4.3.tar` & `droidlysis-3.4.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-03-10 16:07:11.428538 droidlysis-3.4.3/
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1057 2021-08-19 09:28:51.000000 droidlysis-3.4.3/LICENSE
--rw-rw-r--   0 axelle    (1000) axelle    (1000)       45 2021-08-19 09:28:51.000000 droidlysis-3.4.3/MANIFEST.in
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     9352 2023-03-10 16:07:11.428538 droidlysis-3.4.3/PKG-INFO
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     8761 2023-03-10 16:04:01.000000 droidlysis-3.4.3/README.md
-drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-03-10 16:07:11.428538 droidlysis-3.4.3/conf/
--rw-rw-r--   0 axelle    (1000) axelle    (1000)        0 2021-08-19 09:28:51.000000 droidlysis-3.4.3/conf/__init__.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1768 2021-08-19 09:28:51.000000 droidlysis-3.4.3/conf/arm.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     3346 2021-08-19 09:28:51.000000 droidlysis-3.4.3/conf/exodustrack.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)      393 2023-03-10 15:55:25.000000 droidlysis-3.4.3/conf/general.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    60591 2023-03-10 15:08:56.000000 droidlysis-3.4.3/conf/kit.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1935 2021-08-19 09:28:51.000000 droidlysis-3.4.3/conf/manifest.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    14426 2022-06-28 05:53:13.000000 droidlysis-3.4.3/conf/smali.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1853 2021-08-19 09:28:51.000000 droidlysis-3.4.3/conf/sortconf.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     2396 2022-06-14 09:05:27.000000 droidlysis-3.4.3/conf/wide.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     4745 2023-03-10 15:56:01.000000 droidlysis-3.4.3/droidconfig.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     6075 2023-02-23 13:17:45.000000 droidlysis-3.4.3/droidcountry.py
--rwxrwxr-x   0 axelle    (1000) axelle    (1000)      226 2023-02-23 13:17:45.000000 droidlysis-3.4.3/droidlysis
-drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-03-10 16:07:11.428538 droidlysis-3.4.3/droidlysis.egg-info/
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     9352 2023-03-10 16:07:11.000000 droidlysis-3.4.3/droidlysis.egg-info/PKG-INFO
--rw-rw-r--   0 axelle    (1000) axelle    (1000)      515 2023-03-10 16:07:11.000000 droidlysis-3.4.3/droidlysis.egg-info/SOURCES.txt
--rw-rw-r--   0 axelle    (1000) axelle    (1000)        1 2023-03-10 16:07:11.000000 droidlysis-3.4.3/droidlysis.egg-info/dependency_links.txt
--rw-rw-r--   0 axelle    (1000) axelle    (1000)       81 2023-03-10 16:07:11.000000 droidlysis-3.4.3/droidlysis.egg-info/requires.txt
--rw-rw-r--   0 axelle    (1000) axelle    (1000)      122 2023-03-10 16:07:11.000000 droidlysis-3.4.3/droidlysis.egg-info/top_level.txt
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     9564 2023-03-10 15:58:50.000000 droidlysis-3.4.3/droidlysis3.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     9832 2023-03-10 15:44:18.000000 droidlysis-3.4.3/droidproperties.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    13295 2023-02-23 13:17:45.000000 droidlysis-3.4.3/droidreport.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    52909 2023-03-10 15:56:42.000000 droidlysis-3.4.3/droidsample.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1191 2023-03-10 15:08:56.000000 droidlysis-3.4.3/droidsql.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     5140 2023-02-23 13:17:45.000000 droidlysis-3.4.3/droidurl.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    10903 2023-02-23 13:17:45.000000 droidlysis-3.4.3/droidutil.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     4907 2023-02-23 13:17:45.000000 droidlysis-3.4.3/droidziprar.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)       38 2023-03-10 16:07:11.428538 droidlysis-3.4.3/setup.cfg
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1335 2023-03-10 15:59:01.000000 droidlysis-3.4.3/setup.py
+drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-05-15 13:37:01.027136 droidlysis-3.4.4/
+-rw-r--r--   0 axelle    (1000) axelle    (1000)     1057 2019-06-03 07:49:35.000000 droidlysis-3.4.4/LICENSE
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)       45 2020-03-02 08:15:52.000000 droidlysis-3.4.4/MANIFEST.in
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     9375 2023-05-15 13:37:01.027136 droidlysis-3.4.4/PKG-INFO
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     8784 2023-05-15 13:36:04.000000 droidlysis-3.4.4/README.md
+drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-05-15 13:37:01.023136 droidlysis-3.4.4/conf/
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)        0 2020-03-02 08:09:36.000000 droidlysis-3.4.4/conf/__init__.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1768 2021-06-01 13:59:15.000000 droidlysis-3.4.4/conf/arm.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     3346 2021-02-18 13:02:54.000000 droidlysis-3.4.4/conf/exodustrack.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)      393 2023-05-02 09:09:40.000000 droidlysis-3.4.4/conf/general.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    60591 2023-03-10 11:17:45.000000 droidlysis-3.4.4/conf/kit.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1935 2020-06-22 07:33:42.000000 droidlysis-3.4.4/conf/manifest.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    14426 2022-06-20 13:30:17.000000 droidlysis-3.4.4/conf/smali.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1853 2021-02-18 13:02:54.000000 droidlysis-3.4.4/conf/sortconf.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     2396 2022-06-13 09:28:37.000000 droidlysis-3.4.4/conf/wide.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     4745 2023-05-02 09:09:40.000000 droidlysis-3.4.4/droidconfig.py
+-rw-r--r--   0 axelle    (1000) axelle    (1000)     6075 2023-02-21 13:28:16.000000 droidlysis-3.4.4/droidcountry.py
+-rwxrw-r--   0 axelle    (1000) axelle    (1000)      226 2022-01-27 12:02:01.000000 droidlysis-3.4.4/droidlysis
+drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-05-15 13:37:01.023136 droidlysis-3.4.4/droidlysis.egg-info/
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     9375 2023-05-15 13:37:01.000000 droidlysis-3.4.4/droidlysis.egg-info/PKG-INFO
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)      515 2023-05-15 13:37:01.000000 droidlysis-3.4.4/droidlysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)        1 2023-05-15 13:37:01.000000 droidlysis-3.4.4/droidlysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)       81 2023-05-15 13:37:01.000000 droidlysis-3.4.4/droidlysis.egg-info/requires.txt
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)      122 2023-05-15 13:37:01.000000 droidlysis-3.4.4/droidlysis.egg-info/top_level.txt
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     9564 2023-05-15 13:35:35.000000 droidlysis-3.4.4/droidlysis3.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     9832 2023-05-02 09:09:40.000000 droidlysis-3.4.4/droidproperties.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    13295 2023-03-10 13:39:17.000000 droidlysis-3.4.4/droidreport.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    52901 2023-05-15 13:25:37.000000 droidlysis-3.4.4/droidsample.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1191 2023-03-10 13:12:53.000000 droidlysis-3.4.4/droidsql.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     5140 2023-02-21 14:30:46.000000 droidlysis-3.4.4/droidurl.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    10903 2023-02-21 14:43:02.000000 droidlysis-3.4.4/droidutil.py
+-rw-r--r--   0 axelle    (1000) axelle    (1000)     4907 2023-02-21 14:43:02.000000 droidlysis-3.4.4/droidziprar.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)       38 2023-05-15 13:37:01.027136 droidlysis-3.4.4/setup.cfg
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1335 2023-05-15 13:31:03.000000 droidlysis-3.4.4/setup.py
```

### Comparing `droidlysis-3.4.3/LICENSE` & `droidlysis-3.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/PKG-INFO` & `droidlysis-3.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: droidlysis
-Version: 3.4.3
+Version: 3.4.4
 Summary: DroidLysis: pre-analysis of suspicious Android samples
 Home-page: https://github.com/cryptax/droidlysis
 Author: @cryptax
 Author-email: aafortinet@gmail.com
 License: MIT
 Keywords: android malware reverse
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 # DroidLysis
 
 DroidLysis is a **pre-analysis tool for Android apps**: it performs repetitive and boring tasks we'd typically do at the beginning of any reverse engineering. It disassembles the Android sample, organizes output in directories, and searches for suspicious spots in the code to look at.
 The output helps the reverse engineer speed up the first few steps of analysis.
 
 DroidLysis can be used over Android packages (apk), Dalvik executables (dex), Zip files (zip), Rar files (rar) or directories of files.
 
-<img src="https://img.shields.io/badge/PyPi%20-3.4.1-blue">
+<img src="https://img.shields.io/badge/PyPi%20-3.4.4-blue">
 
 ## Quick setup
 
 Can't wait to use DroidLysis? Then, use a Docker container:
 
 ```
 $ docker pull cryptax/droidlysis:2023.02
@@ -191,14 +191,15 @@
 with open('sorted.conf','w') as f:
     config.write(f)
 ```    
 
 
 ## Updates
 
+- v3.4.4 - Bug fix #14
 - v3.4.3 - Using configuration files
 - v3.4.2 - Adding import of Exodus Privacy Trackers
 - v3.4.1 - Removed dependency to Androguard
 - v3.4.0 - Multidex support
 - v3.3.1 - Improving detection of Base64 strings
 - v3.3.0 - Dumping data to JSON
 - v3.2.1 - IP address detection
```

### Comparing `droidlysis-3.4.3/README.md` & `droidlysis-3.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # DroidLysis
 
 DroidLysis is a **pre-analysis tool for Android apps**: it performs repetitive and boring tasks we'd typically do at the beginning of any reverse engineering. It disassembles the Android sample, organizes output in directories, and searches for suspicious spots in the code to look at.
 The output helps the reverse engineer speed up the first few steps of analysis.
 
 DroidLysis can be used over Android packages (apk), Dalvik executables (dex), Zip files (zip), Rar files (rar) or directories of files.
 
-<img src="https://img.shields.io/badge/PyPi%20-3.4.1-blue">
+<img src="https://img.shields.io/badge/PyPi%20-3.4.4-blue">
 
 ## Quick setup
 
 Can't wait to use DroidLysis? Then, use a Docker container:
 
 ```
 $ docker pull cryptax/droidlysis:2023.02
@@ -173,14 +173,15 @@
 with open('sorted.conf','w') as f:
     config.write(f)
 ```    
 
 
 ## Updates
 
+- v3.4.4 - Bug fix #14
 - v3.4.3 - Using configuration files
 - v3.4.2 - Adding import of Exodus Privacy Trackers
 - v3.4.1 - Removed dependency to Androguard
 - v3.4.0 - Multidex support
 - v3.3.1 - Improving detection of Base64 strings
 - v3.3.0 - Dumping data to JSON
 - v3.2.1 - IP address detection
```

### Comparing `droidlysis-3.4.3/conf/arm.conf` & `droidlysis-3.4.4/conf/arm.conf`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/conf/exodustrack.py` & `droidlysis-3.4.4/conf/exodustrack.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/conf/kit.conf` & `droidlysis-3.4.4/conf/kit.conf`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/conf/manifest.conf` & `droidlysis-3.4.4/conf/manifest.conf`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/conf/smali.conf` & `droidlysis-3.4.4/conf/smali.conf`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/conf/sortconf.py` & `droidlysis-3.4.4/conf/sortconf.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/conf/wide.conf` & `droidlysis-3.4.4/conf/wide.conf`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/droidconfig.py` & `droidlysis-3.4.4/droidconfig.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/droidcountry.py` & `droidlysis-3.4.4/droidcountry.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/droidlysis.egg-info/PKG-INFO` & `droidlysis-3.4.4/droidlysis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: droidlysis
-Version: 3.4.3
+Version: 3.4.4
 Summary: DroidLysis: pre-analysis of suspicious Android samples
 Home-page: https://github.com/cryptax/droidlysis
 Author: @cryptax
 Author-email: aafortinet@gmail.com
 License: MIT
 Keywords: android malware reverse
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 # DroidLysis
 
 DroidLysis is a **pre-analysis tool for Android apps**: it performs repetitive and boring tasks we'd typically do at the beginning of any reverse engineering. It disassembles the Android sample, organizes output in directories, and searches for suspicious spots in the code to look at.
 The output helps the reverse engineer speed up the first few steps of analysis.
 
 DroidLysis can be used over Android packages (apk), Dalvik executables (dex), Zip files (zip), Rar files (rar) or directories of files.
 
-<img src="https://img.shields.io/badge/PyPi%20-3.4.1-blue">
+<img src="https://img.shields.io/badge/PyPi%20-3.4.4-blue">
 
 ## Quick setup
 
 Can't wait to use DroidLysis? Then, use a Docker container:
 
 ```
 $ docker pull cryptax/droidlysis:2023.02
@@ -191,14 +191,15 @@
 with open('sorted.conf','w') as f:
     config.write(f)
 ```    
 
 
 ## Updates
 
+- v3.4.4 - Bug fix #14
 - v3.4.3 - Using configuration files
 - v3.4.2 - Adding import of Exodus Privacy Trackers
 - v3.4.1 - Removed dependency to Androguard
 - v3.4.0 - Multidex support
 - v3.3.1 - Improving detection of Base64 strings
 - v3.3.0 - Dumping data to JSON
 - v3.2.1 - IP address detection
```

### Comparing `droidlysis-3.4.3/droidlysis.egg-info/SOURCES.txt` & `droidlysis-3.4.4/droidlysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/droidlysis3.py` & `droidlysis-3.4.4/droidlysis3.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import logging
 from droidsql import DroidSql
 from droidconfig import generalconfig
 
 property_dump_file = 'details.md'
 report_file = 'report.md'
 json_file = 'report.json'
-__version__ = "3.4.3"
+__version__ = "3.4.4"
 
 logging.basicConfig(format='%(levelname)s:%(filename)s:%(message)s',
                     level=logging.INFO)
 
 
 def get_arguments():
     """Read arguments for the program and returns the ArgumentParser"""
```

### Comparing `droidlysis-3.4.3/droidproperties.py` & `droidlysis-3.4.4/droidproperties.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/droidreport.py` & `droidlysis-3.4.4/droidreport.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/droidsample.py` & `droidlysis-3.4.4/droidsample.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,16 +328,16 @@
                         if self.verbose:
                             logging.debug("Dex2jar on " + d)
                             try:
                                 subprocess.call([self.config.DEX2JAR_CMD, "--force", d, "-o", jar_file],
                                                 stdout=self.process_output, stderr=self.process_output)
                             except:
                                 logging.warning("[-] Dex2jar failed on {}".format(d))
-                        else:
-                            logging.warning("Dex2jar software is not executable, skipping (file: {0})".format(self.config.DEX2JAR_CMD))
+                    else:
+                        logging.warning("Dex2jar software is not executable, skipping (file: {0})".format(self.config.DEX2JAR_CMD))
                     
                     if os.access(jar_file, os.R_OK):
                         if self.enable_procyon and os.access(self.config.PROCYON_JAR, os.R_OK):
                             logging.debug("Procyon decompiler on " + jar_file)
                             subprocess.call(["java", "-jar", self.config.PROCYON_JAR,
                                             jar_file, "-o", os.path.join(self.outdir, 'procyon')],
                                             stdout=self.process_output, stderr=self.process_output)
```

### Comparing `droidlysis-3.4.3/droidsql.py` & `droidlysis-3.4.4/droidsql.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/droidurl.py` & `droidlysis-3.4.4/droidurl.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/droidutil.py` & `droidlysis-3.4.4/droidutil.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/droidziprar.py` & `droidlysis-3.4.4/droidziprar.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.3/setup.py` & `droidlysis-3.4.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     long_description_content_type="text/markdown",
     author='@cryptax',
     author_email='aafortinet@gmail.com',
     url='https://github.com/cryptax/droidlysis',
     license='MIT',
     keywords="android malware reverse",
     python_requires='>=3.0',
-    version='3.4.3',
+    version='3.4.4',
     packages=['conf'],
     py_modules=[
         'droidconfig',
         'droidcountry',
         'droidlysis3',
         'droidproperties',
         'droidreport',
```

