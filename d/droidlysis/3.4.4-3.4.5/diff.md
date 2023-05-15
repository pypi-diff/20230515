# Comparing `tmp/droidlysis-3.4.4.tar.gz` & `tmp/droidlysis-3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "droidlysis-3.4.4.tar", last modified: Mon May 15 13:37:01 2023, max compression
+gzip compressed data, was "droidlysis-3.4.5.tar", last modified: Mon May 15 16:01:30 2023, max compression
```

## Comparing `droidlysis-3.4.4.tar` & `droidlysis-3.4.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-05-15 13:37:01.027136 droidlysis-3.4.4/
--rw-r--r--   0 axelle    (1000) axelle    (1000)     1057 2019-06-03 07:49:35.000000 droidlysis-3.4.4/LICENSE
--rw-rw-r--   0 axelle    (1000) axelle    (1000)       45 2020-03-02 08:15:52.000000 droidlysis-3.4.4/MANIFEST.in
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     9375 2023-05-15 13:37:01.027136 droidlysis-3.4.4/PKG-INFO
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     8784 2023-05-15 13:36:04.000000 droidlysis-3.4.4/README.md
-drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-05-15 13:37:01.023136 droidlysis-3.4.4/conf/
--rw-rw-r--   0 axelle    (1000) axelle    (1000)        0 2020-03-02 08:09:36.000000 droidlysis-3.4.4/conf/__init__.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1768 2021-06-01 13:59:15.000000 droidlysis-3.4.4/conf/arm.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     3346 2021-02-18 13:02:54.000000 droidlysis-3.4.4/conf/exodustrack.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)      393 2023-05-02 09:09:40.000000 droidlysis-3.4.4/conf/general.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    60591 2023-03-10 11:17:45.000000 droidlysis-3.4.4/conf/kit.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1935 2020-06-22 07:33:42.000000 droidlysis-3.4.4/conf/manifest.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    14426 2022-06-20 13:30:17.000000 droidlysis-3.4.4/conf/smali.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1853 2021-02-18 13:02:54.000000 droidlysis-3.4.4/conf/sortconf.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     2396 2022-06-13 09:28:37.000000 droidlysis-3.4.4/conf/wide.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     4745 2023-05-02 09:09:40.000000 droidlysis-3.4.4/droidconfig.py
--rw-r--r--   0 axelle    (1000) axelle    (1000)     6075 2023-02-21 13:28:16.000000 droidlysis-3.4.4/droidcountry.py
--rwxrw-r--   0 axelle    (1000) axelle    (1000)      226 2022-01-27 12:02:01.000000 droidlysis-3.4.4/droidlysis
-drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-05-15 13:37:01.023136 droidlysis-3.4.4/droidlysis.egg-info/
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     9375 2023-05-15 13:37:01.000000 droidlysis-3.4.4/droidlysis.egg-info/PKG-INFO
--rw-rw-r--   0 axelle    (1000) axelle    (1000)      515 2023-05-15 13:37:01.000000 droidlysis-3.4.4/droidlysis.egg-info/SOURCES.txt
--rw-rw-r--   0 axelle    (1000) axelle    (1000)        1 2023-05-15 13:37:01.000000 droidlysis-3.4.4/droidlysis.egg-info/dependency_links.txt
--rw-rw-r--   0 axelle    (1000) axelle    (1000)       81 2023-05-15 13:37:01.000000 droidlysis-3.4.4/droidlysis.egg-info/requires.txt
--rw-rw-r--   0 axelle    (1000) axelle    (1000)      122 2023-05-15 13:37:01.000000 droidlysis-3.4.4/droidlysis.egg-info/top_level.txt
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     9564 2023-05-15 13:35:35.000000 droidlysis-3.4.4/droidlysis3.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     9832 2023-05-02 09:09:40.000000 droidlysis-3.4.4/droidproperties.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    13295 2023-03-10 13:39:17.000000 droidlysis-3.4.4/droidreport.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    52901 2023-05-15 13:25:37.000000 droidlysis-3.4.4/droidsample.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1191 2023-03-10 13:12:53.000000 droidlysis-3.4.4/droidsql.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     5140 2023-02-21 14:30:46.000000 droidlysis-3.4.4/droidurl.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    10903 2023-02-21 14:43:02.000000 droidlysis-3.4.4/droidutil.py
--rw-r--r--   0 axelle    (1000) axelle    (1000)     4907 2023-02-21 14:43:02.000000 droidlysis-3.4.4/droidziprar.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)       38 2023-05-15 13:37:01.027136 droidlysis-3.4.4/setup.cfg
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1335 2023-05-15 13:31:03.000000 droidlysis-3.4.4/setup.py
+drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-05-15 16:01:30.391940 droidlysis-3.4.5/
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1057 2021-08-19 09:28:51.000000 droidlysis-3.4.5/LICENSE
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)       45 2021-08-19 09:28:51.000000 droidlysis-3.4.5/MANIFEST.in
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     9760 2023-05-15 16:01:30.391940 droidlysis-3.4.5/PKG-INFO
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     9169 2023-05-15 15:59:40.000000 droidlysis-3.4.5/README.md
+drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-05-15 16:01:30.391940 droidlysis-3.4.5/conf/
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)        0 2021-08-19 09:28:51.000000 droidlysis-3.4.5/conf/__init__.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1768 2021-08-19 09:28:51.000000 droidlysis-3.4.5/conf/arm.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     3346 2021-08-19 09:28:51.000000 droidlysis-3.4.5/conf/exodustrack.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)      349 2023-05-15 15:35:24.000000 droidlysis-3.4.5/conf/general.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    60591 2023-03-10 15:08:56.000000 droidlysis-3.4.5/conf/kit.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1935 2021-08-19 09:28:51.000000 droidlysis-3.4.5/conf/manifest.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    14426 2022-06-28 05:53:13.000000 droidlysis-3.4.5/conf/smali.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1853 2021-08-19 09:28:51.000000 droidlysis-3.4.5/conf/sortconf.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     2396 2022-06-14 09:05:27.000000 droidlysis-3.4.5/conf/wide.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     5690 2023-05-15 15:46:42.000000 droidlysis-3.4.5/droidconfig.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     6075 2023-02-23 13:17:45.000000 droidlysis-3.4.5/droidcountry.py
+-rwxrwxr-x   0 axelle    (1000) axelle    (1000)      226 2023-02-23 13:17:45.000000 droidlysis-3.4.5/droidlysis
+drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-05-15 16:01:30.391940 droidlysis-3.4.5/droidlysis.egg-info/
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     9760 2023-05-15 16:01:30.000000 droidlysis-3.4.5/droidlysis.egg-info/PKG-INFO
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)      515 2023-05-15 16:01:30.000000 droidlysis-3.4.5/droidlysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)        1 2023-05-15 16:01:30.000000 droidlysis-3.4.5/droidlysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)       94 2023-05-15 16:01:30.000000 droidlysis-3.4.5/droidlysis.egg-info/requires.txt
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)      122 2023-05-15 16:01:30.000000 droidlysis-3.4.5/droidlysis.egg-info/top_level.txt
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     9508 2023-05-15 15:25:16.000000 droidlysis-3.4.5/droidlysis3.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     9831 2023-05-15 15:57:21.000000 droidlysis-3.4.5/droidproperties.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    13295 2023-02-23 13:17:45.000000 droidlysis-3.4.5/droidreport.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    52901 2023-05-15 14:59:10.000000 droidlysis-3.4.5/droidsample.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1191 2023-03-10 15:08:56.000000 droidlysis-3.4.5/droidsql.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     5140 2023-02-23 13:17:45.000000 droidlysis-3.4.5/droidurl.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    10903 2023-02-23 13:17:45.000000 droidlysis-3.4.5/droidutil.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     4907 2023-02-23 13:17:45.000000 droidlysis-3.4.5/droidziprar.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)       38 2023-05-15 16:01:30.391940 droidlysis-3.4.5/setup.cfg
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1359 2023-05-15 16:01:18.000000 droidlysis-3.4.5/setup.py
```

### Comparing `droidlysis-3.4.4/LICENSE` & `droidlysis-3.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/PKG-INFO` & `droidlysis-3.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: droidlysis
-Version: 3.4.4
+Version: 3.4.5
 Summary: DroidLysis: pre-analysis of suspicious Android samples
 Home-page: https://github.com/cryptax/droidlysis
 Author: @cryptax
 Author-email: aafortinet@gmail.com
 License: MIT
 Keywords: android malware reverse
 Classifier: Programming Language :: Python :: 3
@@ -19,81 +19,93 @@
 # DroidLysis
 
 DroidLysis is a **pre-analysis tool for Android apps**: it performs repetitive and boring tasks we'd typically do at the beginning of any reverse engineering. It disassembles the Android sample, organizes output in directories, and searches for suspicious spots in the code to look at.
 The output helps the reverse engineer speed up the first few steps of analysis.
 
 DroidLysis can be used over Android packages (apk), Dalvik executables (dex), Zip files (zip), Rar files (rar) or directories of files.
 
-<img src="https://img.shields.io/badge/PyPi%20-3.4.4-blue">
+<img src="https://img.shields.io/badge/PyPi%20-3.4.5-blue">
 
 ## Quick setup
 
 Can't wait to use DroidLysis? Then, use a Docker container:
 
 ```
-$ docker pull cryptax/droidlysis:2023.02
-$ docker run -it --rm -v /tmp/share:/share cryptax/droidlysis:2023.02  /bin/bash
+$ docker pull cryptax/droidlysis:2023.05
+$ docker run -it --rm -v /tmp/share:/share cryptax/droidlysis:2023.05  /bin/bash
 $ cd /opt/droidlysis
 $ python3 ./droidlysis3.py --help
 ```
 
 ## Installing DroidLysis
 
 1. Install required system packages
-2. Install Android disassembly tools
-3. Get DroidLysis from the Git repository (preferred) or from pip
-4. Configure `conf/general.conf`
-
-Install required system packages:
 
 ```
 sudo apt-get install default-jre git python3 python3-pip unzip wget libmagic-dev libxml2-dev libxslt-dev
 ```
 
-Install Android disassembly tools: [Apktool](https://ibotpeaches.github.io/Apktool/) , 
+
+2. Install Android disassembly tools
+
+[Apktool](https://ibotpeaches.github.io/Apktool/) , 
 [Baksmali](https://bitbucket.org/JesusFreke/smali/downloads), and optionally 
 [Dex2jar](https://github.com/pxb1988/dex2jar) and  
 [Procyon](https://bitbucket.org/mstrobel/procyon/wiki/Java%20Decompiler) (note that Procyon only works with Java 8, not Java 11).
 
 ```
 $ mkdir -p ~/softs
 $ cd ~/softs
 $ wget https://bitbucket.org/iBotPeaches/apktool/downloads/apktool_2.7.0.jar
 $ wget https://bitbucket.org/JesusFreke/smali/downloads/baksmali-2.5.2.jar
 $ wget https://github.com/pxb1988/dex2jar/releases/download/v2.2-SNAPSHOT-2021-10-31/dex-tools-2.2-SNAPSHOT-2021-10-31.zip
 $ unzip dex-tools-2.2-SNAPSHOT-2021-10-31.zip 
 $ rm -f dex-tools-2.2-SNAPSHOT-2021-10-31.zip 
 ```
 
+3. Get DroidLysis from the Git repository (preferred) or from pip
+
 Install from Git in a Python virtual environment:
 
 ```
 $ python3 -m venv venv
 $ source ./venv/bin/activate
 (venv) $ pip3 install git+https://github.com/cryptax/droidlysis
 ```
 
-Run it:
+Alternatively, you can install DroidLysis directly from PyPi (`pip3 install droidlysis`).
+
+4. Configure `conf/general.conf`. In particular make sure to change `/home/axelle` with your appropriate directories.
+
+```
+[tools]
+apktool = /home/axelle/softs/apktool_2.7.0.jar
+baksmali = /home/axelle/softs/baksmali-2.5.2.jar
+dex2jar = /home/axelle/softs/dex-tools-2.2-SNAPSHOT/d2j-dex2jar.sh
+procyon = /home/axelle/softs/procyon-decompiler-0.5.30.jar
+keytool = /usr/bin/keytool
+...
+```
+
+5. Run it:
 
 ```
-cd droidlysis
-./droidlysis --help
+python3 ./droidlysis3.py --help
 ```
 
-Alternatively, you can install DroidLysis directly from PyPi (`pip3 install droidlysis`).
 
 ## Configuration
 
-If you used the default install commands & directories as specified above, you won't need any configuration. 
-
 The configuration file is `./conf/general.conf` (you can switch to another file with the `--config` option).
 This is where you configure the location of various external tools (e.g. Apktool), the name of pattern files 
 (by default `./conf/smali.conf`, `./conf/wide.conf`, `./conf/arm.conf`, `./conf/kit.conf`) and the name of
 the database file (only used if you specify `--enable-sql`)
 
+Be sure to specify the correct paths for disassembly tools, or DroidLysis won't find them.
+
 
 ## Usage
 
 DroidLysis uses **Python 3**. To launch it and get options:
 
 ```
 droidlysis --help
@@ -172,33 +184,35 @@
 description=Sending SMS messages
 ```
 
 
 ## Importing Exodus Privacy Trackers
 
 Exodus Privacy maintains a list of various SDKs which are interesting to rule out in our analysis via `conf/kit.conf`.
-Add option `--import_exodus` to the droidlysis command line: this will parse existing trackers Exodus Privacy knows and which aren't yet in your `kit.conf`. Finally, it will **append** all new trackers to `kit.conf`.
+Add option `--import_exodus` to the droidlysis command line: this will parse existing trackers Exodus Privacy knows and which aren't yet in your `kit.conf`. Finally, it will **append** all new trackers to `~/.cache/droidlysis/kit.conf`.
 
 Afterwards, you may want to sort your `kit.conf` file:
 
 ```python
 import configparser
 import collections
+import os
 
 config = configparser.ConfigParser({}, collections.OrderedDict)
-config.read('./conf/kit.conf')
+config.read(os.path.expanduser('~/.cache/droidlysis/kit.conf'))
 # Order all sections alphabetically
 config._sections = collections.OrderedDict(sorted(config._sections.items(), key=lambda t: t[0] ))
 with open('sorted.conf','w') as f:
     config.write(f)
 ```    
 
 
 ## Updates
 
+- v3.4.5 - Creating a writable user kit.conf file
 - v3.4.4 - Bug fix #14
 - v3.4.3 - Using configuration files
 - v3.4.2 - Adding import of Exodus Privacy Trackers
 - v3.4.1 - Removed dependency to Androguard
 - v3.4.0 - Multidex support
 - v3.3.1 - Improving detection of Base64 strings
 - v3.3.0 - Dumping data to JSON
```

### Comparing `droidlysis-3.4.4/README.md` & `droidlysis-3.4.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,93 @@
 # DroidLysis
 
 DroidLysis is a **pre-analysis tool for Android apps**: it performs repetitive and boring tasks we'd typically do at the beginning of any reverse engineering. It disassembles the Android sample, organizes output in directories, and searches for suspicious spots in the code to look at.
 The output helps the reverse engineer speed up the first few steps of analysis.
 
 DroidLysis can be used over Android packages (apk), Dalvik executables (dex), Zip files (zip), Rar files (rar) or directories of files.
 
-<img src="https://img.shields.io/badge/PyPi%20-3.4.4-blue">
+<img src="https://img.shields.io/badge/PyPi%20-3.4.5-blue">
 
 ## Quick setup
 
 Can't wait to use DroidLysis? Then, use a Docker container:
 
 ```
-$ docker pull cryptax/droidlysis:2023.02
-$ docker run -it --rm -v /tmp/share:/share cryptax/droidlysis:2023.02  /bin/bash
+$ docker pull cryptax/droidlysis:2023.05
+$ docker run -it --rm -v /tmp/share:/share cryptax/droidlysis:2023.05  /bin/bash
 $ cd /opt/droidlysis
 $ python3 ./droidlysis3.py --help
 ```
 
 ## Installing DroidLysis
 
 1. Install required system packages
-2. Install Android disassembly tools
-3. Get DroidLysis from the Git repository (preferred) or from pip
-4. Configure `conf/general.conf`
-
-Install required system packages:
 
 ```
 sudo apt-get install default-jre git python3 python3-pip unzip wget libmagic-dev libxml2-dev libxslt-dev
 ```
 
-Install Android disassembly tools: [Apktool](https://ibotpeaches.github.io/Apktool/) , 
+
+2. Install Android disassembly tools
+
+[Apktool](https://ibotpeaches.github.io/Apktool/) , 
 [Baksmali](https://bitbucket.org/JesusFreke/smali/downloads), and optionally 
 [Dex2jar](https://github.com/pxb1988/dex2jar) and  
 [Procyon](https://bitbucket.org/mstrobel/procyon/wiki/Java%20Decompiler) (note that Procyon only works with Java 8, not Java 11).
 
 ```
 $ mkdir -p ~/softs
 $ cd ~/softs
 $ wget https://bitbucket.org/iBotPeaches/apktool/downloads/apktool_2.7.0.jar
 $ wget https://bitbucket.org/JesusFreke/smali/downloads/baksmali-2.5.2.jar
 $ wget https://github.com/pxb1988/dex2jar/releases/download/v2.2-SNAPSHOT-2021-10-31/dex-tools-2.2-SNAPSHOT-2021-10-31.zip
 $ unzip dex-tools-2.2-SNAPSHOT-2021-10-31.zip 
 $ rm -f dex-tools-2.2-SNAPSHOT-2021-10-31.zip 
 ```
 
+3. Get DroidLysis from the Git repository (preferred) or from pip
+
 Install from Git in a Python virtual environment:
 
 ```
 $ python3 -m venv venv
 $ source ./venv/bin/activate
 (venv) $ pip3 install git+https://github.com/cryptax/droidlysis
 ```
 
-Run it:
+Alternatively, you can install DroidLysis directly from PyPi (`pip3 install droidlysis`).
+
+4. Configure `conf/general.conf`. In particular make sure to change `/home/axelle` with your appropriate directories.
+
+```
+[tools]
+apktool = /home/axelle/softs/apktool_2.7.0.jar
+baksmali = /home/axelle/softs/baksmali-2.5.2.jar
+dex2jar = /home/axelle/softs/dex-tools-2.2-SNAPSHOT/d2j-dex2jar.sh
+procyon = /home/axelle/softs/procyon-decompiler-0.5.30.jar
+keytool = /usr/bin/keytool
+...
+```
+
+5. Run it:
 
 ```
-cd droidlysis
-./droidlysis --help
+python3 ./droidlysis3.py --help
 ```
 
-Alternatively, you can install DroidLysis directly from PyPi (`pip3 install droidlysis`).
 
 ## Configuration
 
-If you used the default install commands & directories as specified above, you won't need any configuration. 
-
 The configuration file is `./conf/general.conf` (you can switch to another file with the `--config` option).
 This is where you configure the location of various external tools (e.g. Apktool), the name of pattern files 
 (by default `./conf/smali.conf`, `./conf/wide.conf`, `./conf/arm.conf`, `./conf/kit.conf`) and the name of
 the database file (only used if you specify `--enable-sql`)
 
+Be sure to specify the correct paths for disassembly tools, or DroidLysis won't find them.
+
 
 ## Usage
 
 DroidLysis uses **Python 3**. To launch it and get options:
 
 ```
 droidlysis --help
@@ -154,33 +166,35 @@
 description=Sending SMS messages
 ```
 
 
 ## Importing Exodus Privacy Trackers
 
 Exodus Privacy maintains a list of various SDKs which are interesting to rule out in our analysis via `conf/kit.conf`.
-Add option `--import_exodus` to the droidlysis command line: this will parse existing trackers Exodus Privacy knows and which aren't yet in your `kit.conf`. Finally, it will **append** all new trackers to `kit.conf`.
+Add option `--import_exodus` to the droidlysis command line: this will parse existing trackers Exodus Privacy knows and which aren't yet in your `kit.conf`. Finally, it will **append** all new trackers to `~/.cache/droidlysis/kit.conf`.
 
 Afterwards, you may want to sort your `kit.conf` file:
 
 ```python
 import configparser
 import collections
+import os
 
 config = configparser.ConfigParser({}, collections.OrderedDict)
-config.read('./conf/kit.conf')
+config.read(os.path.expanduser('~/.cache/droidlysis/kit.conf'))
 # Order all sections alphabetically
 config._sections = collections.OrderedDict(sorted(config._sections.items(), key=lambda t: t[0] ))
 with open('sorted.conf','w') as f:
     config.write(f)
 ```    
 
 
 ## Updates
 
+- v3.4.5 - Creating a writable user kit.conf file
 - v3.4.4 - Bug fix #14
 - v3.4.3 - Using configuration files
 - v3.4.2 - Adding import of Exodus Privacy Trackers
 - v3.4.1 - Removed dependency to Androguard
 - v3.4.0 - Multidex support
 - v3.3.1 - Improving detection of Base64 strings
 - v3.3.0 - Dumping data to JSON
```

### Comparing `droidlysis-3.4.4/conf/arm.conf` & `droidlysis-3.4.5/conf/arm.conf`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/conf/exodustrack.py` & `droidlysis-3.4.5/conf/exodustrack.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/conf/kit.conf` & `droidlysis-3.4.5/conf/kit.conf`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/conf/manifest.conf` & `droidlysis-3.4.5/conf/manifest.conf`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/conf/smali.conf` & `droidlysis-3.4.5/conf/smali.conf`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/conf/sortconf.py` & `droidlysis-3.4.5/conf/sortconf.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/conf/wide.conf` & `droidlysis-3.4.5/conf/wide.conf`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/droidconfig.py` & `droidlysis-3.4.5/droidconfig.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,62 @@
 import os
 import configparser
 import logging
+import shutil
+from platformdirs import *
+
 
 logging.basicConfig(format='%(levelname)s:%(filename)s:%(message)s',
                     level=logging.INFO)
 
+
 # ------------------------- Reading *.conf configuration files -----------
 class generalconfig:
     def __init__(self, filename='./conf/general.conf', verbose=False):
         self.config = configparser.ConfigParser()
         self.config.read(filename)
-        
+
         # get config
-        self.APKTOOL_JAR = self.config['tools']['apktool']
-        self.BAKSMALI_JAR = self.config['tools']['baksmali']
-        self.DEX2JAR_CMD = self.config['tools']['dex2jar']
-        self.PROCYON_JAR = self.config['tools']['procyon']
-        self.KEYTOOL = self.config['tools']['keytool']
+        self.APKTOOL_JAR = os.path.expanduser(self.config['tools']['apktool'])
+        self.BAKSMALI_JAR = os.path.expanduser(self.config['tools']['baksmali'])
+        self.DEX2JAR_CMD = os.path.expanduser(self.config['tools']['dex2jar'])
+        self.PROCYON_JAR = os.path.expanduser(self.config['tools']['procyon'])
+        self.KEYTOOL = os.path.expanduser(self.config['tools']['keytool'])
         self.SMALI_CONFIGFILE = os.path.join(os.path.dirname(filename),
                                              self.config['general']['smali_config'])
-        self.WIDE_CONFIGFILE = os.path.join(os.path.dirname(filename), self.config['general']['wide_config'])
-        self.ARM_CONFIGFILE = os.path.join(os.path.dirname(filename), self.config['general']['arm_config'])
-        self.KIT_CONFIGFILE = os.path.join(os.path.dirname(filename), self.config['general']['kit_config'])
+        self.WIDE_CONFIGFILE = os.path.join(os.path.dirname(filename),
+                                            self.config['general']['wide_config'])
+        self.ARM_CONFIGFILE = os.path.join(os.path.dirname(filename),
+                                           self.config['general']['arm_config'])
+        self.DISTRIB_KIT_CONFIGFILE = os.path.join(os.path.dirname(filename),
+                                                   self.config['general']['kit_config'])
+
+        # duplicate kit configuration for edition
+        cache_dir = user_cache_dir('droidlysis', 'cryptax')
+        if not os.path.exists(cache_dir):
+            os.makedirs(cache_dir)
+        self.KIT_CONFIGFILE = os.path.join(cache_dir,
+                                           self.config['general']['kit_config'])
+        if not os.path.exists(self.KIT_CONFIGFILE):
+            logging.verbose(f'Copying {self.DISTRIB_KIT_CONFIGFILE}'
+                            'to {self.KIT_CONFIGFILE}')
+            shutil.copyfile(self.DISTRIB_KIT_CONFIGFILE, self.KIT_CONFIGFILE)
 
         self.SQLALCHEMY = f'sqlite:///{self.config["general"]["db_file"]}'
 
         # check files are accessible
         for f in [self.APKTOOL_JAR, self.BAKSMALI_JAR,
                   self.DEX2JAR_CMD, self.PROCYON_JAR,
                   self.SMALI_CONFIGFILE, self.WIDE_CONFIGFILE,
                   self.ARM_CONFIGFILE, self.KIT_CONFIGFILE]:
             if not os.access(f, os.R_OK):
-                logging.warning(f'Cannot access {f}')
+                logging.warning(f'Cannot access {f} - check your configuration file {filename}')
 
         if not os.access(self.KEYTOOL, os.X_OK):
-            logging.warning(f'Cannot access keytool at {self.KEYTOOL}')
+            logging.warning(f'Cannot access keytool at {self.KEYTOOL} - check your configuration file {filename}')
 
 
 class droidconfig:
     def __init__(self, filename, verbose=False):
         assert filename is not None, "Filename is invalid"
         assert os.access(filename, os.R_OK) is not False, "File {0} is not readable".format(filename)
```

### Comparing `droidlysis-3.4.4/droidcountry.py` & `droidlysis-3.4.5/droidcountry.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/droidlysis.egg-info/PKG-INFO` & `droidlysis-3.4.5/droidlysis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: droidlysis
-Version: 3.4.4
+Version: 3.4.5
 Summary: DroidLysis: pre-analysis of suspicious Android samples
 Home-page: https://github.com/cryptax/droidlysis
 Author: @cryptax
 Author-email: aafortinet@gmail.com
 License: MIT
 Keywords: android malware reverse
 Classifier: Programming Language :: Python :: 3
@@ -19,81 +19,93 @@
 # DroidLysis
 
 DroidLysis is a **pre-analysis tool for Android apps**: it performs repetitive and boring tasks we'd typically do at the beginning of any reverse engineering. It disassembles the Android sample, organizes output in directories, and searches for suspicious spots in the code to look at.
 The output helps the reverse engineer speed up the first few steps of analysis.
 
 DroidLysis can be used over Android packages (apk), Dalvik executables (dex), Zip files (zip), Rar files (rar) or directories of files.
 
-<img src="https://img.shields.io/badge/PyPi%20-3.4.4-blue">
+<img src="https://img.shields.io/badge/PyPi%20-3.4.5-blue">
 
 ## Quick setup
 
 Can't wait to use DroidLysis? Then, use a Docker container:
 
 ```
-$ docker pull cryptax/droidlysis:2023.02
-$ docker run -it --rm -v /tmp/share:/share cryptax/droidlysis:2023.02  /bin/bash
+$ docker pull cryptax/droidlysis:2023.05
+$ docker run -it --rm -v /tmp/share:/share cryptax/droidlysis:2023.05  /bin/bash
 $ cd /opt/droidlysis
 $ python3 ./droidlysis3.py --help
 ```
 
 ## Installing DroidLysis
 
 1. Install required system packages
-2. Install Android disassembly tools
-3. Get DroidLysis from the Git repository (preferred) or from pip
-4. Configure `conf/general.conf`
-
-Install required system packages:
 
 ```
 sudo apt-get install default-jre git python3 python3-pip unzip wget libmagic-dev libxml2-dev libxslt-dev
 ```
 
-Install Android disassembly tools: [Apktool](https://ibotpeaches.github.io/Apktool/) , 
+
+2. Install Android disassembly tools
+
+[Apktool](https://ibotpeaches.github.io/Apktool/) , 
 [Baksmali](https://bitbucket.org/JesusFreke/smali/downloads), and optionally 
 [Dex2jar](https://github.com/pxb1988/dex2jar) and  
 [Procyon](https://bitbucket.org/mstrobel/procyon/wiki/Java%20Decompiler) (note that Procyon only works with Java 8, not Java 11).
 
 ```
 $ mkdir -p ~/softs
 $ cd ~/softs
 $ wget https://bitbucket.org/iBotPeaches/apktool/downloads/apktool_2.7.0.jar
 $ wget https://bitbucket.org/JesusFreke/smali/downloads/baksmali-2.5.2.jar
 $ wget https://github.com/pxb1988/dex2jar/releases/download/v2.2-SNAPSHOT-2021-10-31/dex-tools-2.2-SNAPSHOT-2021-10-31.zip
 $ unzip dex-tools-2.2-SNAPSHOT-2021-10-31.zip 
 $ rm -f dex-tools-2.2-SNAPSHOT-2021-10-31.zip 
 ```
 
+3. Get DroidLysis from the Git repository (preferred) or from pip
+
 Install from Git in a Python virtual environment:
 
 ```
 $ python3 -m venv venv
 $ source ./venv/bin/activate
 (venv) $ pip3 install git+https://github.com/cryptax/droidlysis
 ```
 
-Run it:
+Alternatively, you can install DroidLysis directly from PyPi (`pip3 install droidlysis`).
+
+4. Configure `conf/general.conf`. In particular make sure to change `/home/axelle` with your appropriate directories.
+
+```
+[tools]
+apktool = /home/axelle/softs/apktool_2.7.0.jar
+baksmali = /home/axelle/softs/baksmali-2.5.2.jar
+dex2jar = /home/axelle/softs/dex-tools-2.2-SNAPSHOT/d2j-dex2jar.sh
+procyon = /home/axelle/softs/procyon-decompiler-0.5.30.jar
+keytool = /usr/bin/keytool
+...
+```
+
+5. Run it:
 
 ```
-cd droidlysis
-./droidlysis --help
+python3 ./droidlysis3.py --help
 ```
 
-Alternatively, you can install DroidLysis directly from PyPi (`pip3 install droidlysis`).
 
 ## Configuration
 
-If you used the default install commands & directories as specified above, you won't need any configuration. 
-
 The configuration file is `./conf/general.conf` (you can switch to another file with the `--config` option).
 This is where you configure the location of various external tools (e.g. Apktool), the name of pattern files 
 (by default `./conf/smali.conf`, `./conf/wide.conf`, `./conf/arm.conf`, `./conf/kit.conf`) and the name of
 the database file (only used if you specify `--enable-sql`)
 
+Be sure to specify the correct paths for disassembly tools, or DroidLysis won't find them.
+
 
 ## Usage
 
 DroidLysis uses **Python 3**. To launch it and get options:
 
 ```
 droidlysis --help
@@ -172,33 +184,35 @@
 description=Sending SMS messages
 ```
 
 
 ## Importing Exodus Privacy Trackers
 
 Exodus Privacy maintains a list of various SDKs which are interesting to rule out in our analysis via `conf/kit.conf`.
-Add option `--import_exodus` to the droidlysis command line: this will parse existing trackers Exodus Privacy knows and which aren't yet in your `kit.conf`. Finally, it will **append** all new trackers to `kit.conf`.
+Add option `--import_exodus` to the droidlysis command line: this will parse existing trackers Exodus Privacy knows and which aren't yet in your `kit.conf`. Finally, it will **append** all new trackers to `~/.cache/droidlysis/kit.conf`.
 
 Afterwards, you may want to sort your `kit.conf` file:
 
 ```python
 import configparser
 import collections
+import os
 
 config = configparser.ConfigParser({}, collections.OrderedDict)
-config.read('./conf/kit.conf')
+config.read(os.path.expanduser('~/.cache/droidlysis/kit.conf'))
 # Order all sections alphabetically
 config._sections = collections.OrderedDict(sorted(config._sections.items(), key=lambda t: t[0] ))
 with open('sorted.conf','w') as f:
     config.write(f)
 ```    
 
 
 ## Updates
 
+- v3.4.5 - Creating a writable user kit.conf file
 - v3.4.4 - Bug fix #14
 - v3.4.3 - Using configuration files
 - v3.4.2 - Adding import of Exodus Privacy Trackers
 - v3.4.1 - Removed dependency to Androguard
 - v3.4.0 - Multidex support
 - v3.3.1 - Improving detection of Base64 strings
 - v3.3.0 - Dumping data to JSON
```

### Comparing `droidlysis-3.4.4/droidlysis.egg-info/SOURCES.txt` & `droidlysis-3.4.5/droidlysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/droidlysis3.py` & `droidlysis-3.4.5/droidlysis3.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,30 +14,31 @@
 import logging
 from droidsql import DroidSql
 from droidconfig import generalconfig
 
 property_dump_file = 'details.md'
 report_file = 'report.md'
 json_file = 'report.json'
-__version__ = "3.4.4"
+__version__ = "3.4.5"
 
 logging.basicConfig(format='%(levelname)s:%(filename)s:%(message)s',
                     level=logging.INFO)
 
 
 def get_arguments():
     """Read arguments for the program and returns the ArgumentParser"""
     description = 'DroidLysis3 is a Python which processes Android samples. \n'
     'It prepares the sample for analysis, unzipping,'
     'disassembling, decompiling it.'
     'It parses for potentially suspicious features '
     '(e.g "sample roots the phone")'
     parser = argparse.ArgumentParser(description=description,
                                      prog='DroidLysis',
-                                     epilog='Version '+ __version__ + ' - Greetz from @cryptax')
+                                     epilog='Version ' + __version__
+                                     + ' - Greetz from @cryptax')
     parser.add_argument('-i', '--input',
                         help='input directories or files to process',
                         nargs='+', action='store', default='.')
     parser.add_argument('-o', '--output',
                         help='analysis of input files is written into '
                         'subdirectories of this directory',
                         action='store', default='.')
@@ -107,15 +108,15 @@
     if args.enable_sql:
         sql = DroidSql()
 
     for element in args.input:
         if os.path.isdir(element):
             listing = os.listdir(element)
             for file in listing:
-                process_file(config, 
+                process_file(config,
                              os.path.join(element, file),
                              outdir=args.output,
                              verbose=args.verbose,
                              clear=args.clearoutput,
                              enable_procyon=args.enable_procyon,
                              disable_report=args.disable_report,
                              no_kit_exception=args.no_kit_exception,
@@ -130,28 +131,27 @@
                     try:
                         os.rename(os.path.join(element, file),
                                   os.path.join(args.movein, file))
                     except OSError as e:
                         logging.debug("%s no longer present?: %s\n" % (file, str(e)))
 
         if os.path.isfile(element):
-            process_file(config, 
+            process_file(config,
                          os.path.join('.', element),
                          outdir=args.output,
                          verbose=args.verbose,
                          clear=args.clearoutput,
                          enable_procyon=args.enable_procyon,
                          disable_report=args.disable_report,
                          silent=args.silent,
                          no_kit_exception=args.no_kit_exception,
                          sql=sql,
                          disable_json=args.disable_json,
                          import_exodus=args.import_exodus
                          )
-            # dir name = os.path.join(args.output, '{filename}-*'.format(filename=element))
             if args.movein:
                 logging.debug("Moving %s to %s" %
                               (os.path.join('.', element),
                                os.path.join(args.movein, os.path.basename(element))))
                 os.rename(os.path.join('.', element), os.path.join(args.movein, os.path.basename(element)))
```

### Comparing `droidlysis-3.4.4/droidproperties.py` & `droidlysis-3.4.5/droidproperties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 """
 __author__ = "Axelle Apvrille"
-__status__ = "Alpha"
+__status__ = "Beta"
 __license__ = "MIT License"
 """
 
 import droidutil
 import droidconfig
 import droidcountry
 import droidsql
@@ -185,16 +185,16 @@
                     break
                 logging.debug(f'Adding Exodus Tracker: {name}')
                 config[name] = {}
                 config[name]['description'] = f'{tracker["name"]} (from ETIP Exodus Privacy list)'
                 config[name]['pattern'] = '|'.join(code_signature)
                 break
         logging.debug('Appending imported trackers '
-                      f'to {droidconfig.KIT_CONFIGFILE}')
-        with open(droidconfig.KIT_CONFIGFILE, 'a') as configfile:
+                      f'to {self.config.KIT_CONFIGFILE}')
+        with open(self.config.KIT_CONFIGFILE, 'a') as configfile:
             config.write(configfile)
 
     def write(self, sql):
         Session = sessionmaker(bind=sql.engine)
         session = Session()
         sample = droidsql.Sample(sha256=self.sha256,
                                  sanitized_basename=self.sanitized_basename,
```

### Comparing `droidlysis-3.4.4/droidreport.py` & `droidlysis-3.4.5/droidreport.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/droidsample.py` & `droidlysis-3.4.5/droidsample.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/droidsql.py` & `droidlysis-3.4.5/droidsql.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/droidurl.py` & `droidlysis-3.4.5/droidurl.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/droidutil.py` & `droidlysis-3.4.5/droidutil.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/droidziprar.py` & `droidlysis-3.4.5/droidziprar.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.4/setup.py` & `droidlysis-3.4.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     long_description_content_type="text/markdown",
     author='@cryptax',
     author_email='aafortinet@gmail.com',
     url='https://github.com/cryptax/droidlysis',
     license='MIT',
     keywords="android malware reverse",
     python_requires='>=3.0',
-    version='3.4.4',
+    version='3.4.5',
     packages=['conf'],
     py_modules=[
         'droidconfig',
         'droidcountry',
         'droidlysis3',
         'droidproperties',
         'droidreport',
@@ -39,11 +39,12 @@
     ],
     include_package_data=True,
     install_requires=[
         'configparser>=4.0.2',
         'python-magic==0.4.12',
         'requests',
         'SQLAlchemy>=1.1.1',
-        'rarfile>=3.0'
+        'rarfile>=3.0',
+        'platformdirs'
     ],
     scripts=[ 'droidlysis', 'droidlysis3.py' ]
 )
```

