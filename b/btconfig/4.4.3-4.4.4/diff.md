# Comparing `tmp/btconfig-4.4.3.tar.gz` & `tmp/btconfig-4.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btconfig-4.4.3.tar", last modified: Fri May 12 20:10:58 2023, max compression
+gzip compressed data, was "btconfig-4.4.4.tar", last modified: Mon May 15 01:07:02 2023, max compression
```

## Comparing `btconfig-4.4.3.tar` & `btconfig-4.4.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:10:58.743082 btconfig-4.4.3/
--rw-r--r--   0 etejeda    (501) staff       (20)     1311 2023-01-09 20:02:16.000000 btconfig-4.4.3/.gitignore
--rw-r--r--   0 etejeda    (501) staff       (20)      175 2023-01-09 20:02:16.000000 btconfig-4.4.3/AUTHORS.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     1097 2023-01-09 20:02:16.000000 btconfig-4.4.3/LICENSE
--rw-r--r--   0 etejeda    (501) staff       (20)      344 2023-01-09 20:02:16.000000 btconfig-4.4.3/MANIFEST.in
--rw-r--r--   0 etejeda    (501) staff       (20)     3796 2023-05-12 20:10:58.743402 btconfig-4.4.3/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     3132 2023-05-11 11:53:49.000000 btconfig-4.4.3/README.md
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:10:58.733956 btconfig-4.4.3/btconfig/
--rw-r--r--   0 etejeda    (501) staff       (20)     1267 2023-05-11 11:55:36.000000 btconfig-4.4.3/btconfig/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     3790 2023-05-11 11:53:07.000000 btconfig-4.4.3/btconfig/configloader.py
--rw-r--r--   0 etejeda    (501) staff       (20)     3217 2023-05-11 11:53:07.000000 btconfig-4.4.3/btconfig/configutils.py
--rw-r--r--   0 etejeda    (501) staff       (20)      813 2023-01-09 20:02:16.000000 btconfig-4.4.3/btconfig/logger.py
--rw-r--r--   0 etejeda    (501) staff       (20)     4576 2023-05-11 11:53:09.000000 btconfig-4.4.3/btconfig/superconf.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:10:58.737525 btconfig-4.4.3/btconfig.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)     3796 2023-05-12 20:10:58.000000 btconfig-4.4.3/btconfig.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      604 2023-05-12 20:10:58.000000 btconfig-4.4.3/btconfig.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-12 20:10:58.000000 btconfig-4.4.3/btconfig.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-12 20:10:58.000000 btconfig-4.4.3/btconfig.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)       78 2023-05-12 20:10:58.000000 btconfig-4.4.3/btconfig.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        9 2023-05-12 20:10:58.000000 btconfig-4.4.3/btconfig.egg-info/top_level.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:10:58.742524 btconfig-4.4.3/examples/
--rw-r--r--   0 etejeda    (501) staff       (20)     3045 2023-05-11 11:53:23.000000 btconfig-4.4.3/examples/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)      157 2023-05-11 11:53:25.000000 btconfig-4.4.3/examples/example1.py
--rw-r--r--   0 etejeda    (501) staff       (20)      170 2023-05-11 11:53:22.000000 btconfig-4.4.3/examples/example2.py
--rw-r--r--   0 etejeda    (501) staff       (20)      160 2023-05-11 11:53:23.000000 btconfig-4.4.3/examples/example3.py
--rw-r--r--   0 etejeda    (501) staff       (20)      189 2023-05-11 11:53:24.000000 btconfig-4.4.3/examples/example4.py
--rw-r--r--   0 etejeda    (501) staff       (20)       54 2023-01-09 20:02:16.000000 btconfig-4.4.3/examples/myconfig1.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      234 2023-01-09 20:02:16.000000 btconfig-4.4.3/examples/myconfig2.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      435 2023-01-09 20:02:16.000000 btconfig-4.4.3/examples/myconfig3.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      208 2023-01-09 20:02:16.000000 btconfig-4.4.3/examples/myconfig4.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-01-09 20:02:16.000000 btconfig-4.4.3/requirements.txt
--rw-r--r--   0 etejeda    (501) staff       (20)     1074 2023-05-12 20:10:58.744746 btconfig-4.4.3/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)       36 2023-01-09 20:02:16.000000 btconfig-4.4.3/setup.py
--rw-r--r--   0 etejeda    (501) staff       (20)      248 2023-05-11 11:54:41.000000 btconfig-4.4.3/test.py
--rw-r--r--   0 etejeda    (501) staff       (20)      315 2023-01-09 20:02:16.000000 btconfig-4.4.3/tox.ini
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 01:07:02.970992 btconfig-4.4.4/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1311 2023-01-09 20:02:16.000000 btconfig-4.4.4/.gitignore
+-rw-r--r--   0 etejeda    (501) staff       (20)      175 2023-01-09 20:02:16.000000 btconfig-4.4.4/AUTHORS.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     1097 2023-01-09 20:02:16.000000 btconfig-4.4.4/LICENSE
+-rw-r--r--   0 etejeda    (501) staff       (20)      344 2023-01-09 20:02:16.000000 btconfig-4.4.4/MANIFEST.in
+-rw-r--r--   0 etejeda    (501) staff       (20)     3796 2023-05-15 01:07:02.971218 btconfig-4.4.4/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     3132 2023-05-11 11:53:49.000000 btconfig-4.4.4/README.md
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 01:07:02.962983 btconfig-4.4.4/btconfig/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1267 2023-05-11 11:55:36.000000 btconfig-4.4.4/btconfig/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     3788 2023-05-14 18:16:20.000000 btconfig-4.4.4/btconfig/configloader.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     3217 2023-05-11 11:53:07.000000 btconfig-4.4.4/btconfig/configutils.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      813 2023-05-14 18:07:45.000000 btconfig-4.4.4/btconfig/logger.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     4576 2023-05-11 11:53:09.000000 btconfig-4.4.4/btconfig/superconf.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 01:07:02.965331 btconfig-4.4.4/btconfig.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3796 2023-05-15 01:07:02.000000 btconfig-4.4.4/btconfig.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)      604 2023-05-15 01:07:02.000000 btconfig-4.4.4/btconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-15 01:07:02.000000 btconfig-4.4.4/btconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-15 01:07:02.000000 btconfig-4.4.4/btconfig.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)       78 2023-05-15 01:07:02.000000 btconfig-4.4.4/btconfig.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        9 2023-05-15 01:07:02.000000 btconfig-4.4.4/btconfig.egg-info/top_level.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 01:07:02.970584 btconfig-4.4.4/examples/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3045 2023-05-11 11:53:23.000000 btconfig-4.4.4/examples/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)      157 2023-05-11 11:53:25.000000 btconfig-4.4.4/examples/example1.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      170 2023-05-11 11:53:22.000000 btconfig-4.4.4/examples/example2.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      160 2023-05-11 11:53:23.000000 btconfig-4.4.4/examples/example3.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      189 2023-05-11 11:53:24.000000 btconfig-4.4.4/examples/example4.py
+-rw-r--r--   0 etejeda    (501) staff       (20)       54 2023-01-09 20:02:16.000000 btconfig-4.4.4/examples/myconfig1.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      234 2023-01-09 20:02:16.000000 btconfig-4.4.4/examples/myconfig2.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      435 2023-01-09 20:02:16.000000 btconfig-4.4.4/examples/myconfig3.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      208 2023-01-09 20:02:16.000000 btconfig-4.4.4/examples/myconfig4.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-01-09 20:02:16.000000 btconfig-4.4.4/requirements.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)     1074 2023-05-15 01:07:02.972441 btconfig-4.4.4/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)       36 2023-01-09 20:02:16.000000 btconfig-4.4.4/setup.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      248 2023-05-11 11:54:41.000000 btconfig-4.4.4/test.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      315 2023-01-09 20:02:16.000000 btconfig-4.4.4/tox.ini
```

### Comparing `btconfig-4.4.3/.gitignore` & `btconfig-4.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.3/LICENSE` & `btconfig-4.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.3/PKG-INFO` & `btconfig-4.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btconfig
-Version: 4.4.3
+Version: 4.4.4
 Summary: Module for reading configuration files
 Home-page: https://github.com/berttejeda/bert.config
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btconfig-4.4.3/README.md` & `btconfig-4.4.4/README.md`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.3/btconfig/__init__.py` & `btconfig-4.4.4/btconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.3/btconfig/configloader.py` & `btconfig-4.4.4/btconfig/configloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,11 +98,11 @@
             if self.failfast:
                 self.logger.error(
                     "Aborting due to invalid or not found \
                     config(s) [%s]" % ','.join(config_file_uris)
                 )
                 sys.exit(1)
             else:
-                logger.warning('No settings could be derived, using defaults')
+                logger.debug('No settings could be derived, using defaults')
                 config_data = self.default_value
 
         return config_data
```

### Comparing `btconfig-4.4.3/btconfig/configutils.py` & `btconfig-4.4.4/btconfig/configutils.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.3/btconfig/logger.py` & `btconfig-4.4.4/btconfig/logger.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.3/btconfig/superconf.py` & `btconfig-4.4.4/btconfig/superconf.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.3/btconfig.egg-info/PKG-INFO` & `btconfig-4.4.4/btconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btconfig
-Version: 4.4.3
+Version: 4.4.4
 Summary: Module for reading configuration files
 Home-page: https://github.com/berttejeda/bert.config
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btconfig-4.4.3/btconfig.egg-info/SOURCES.txt` & `btconfig-4.4.4/btconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.3/examples/README.md` & `btconfig-4.4.4/examples/README.md`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.3/setup.cfg` & `btconfig-4.4.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = btconfig
 author = Engelbert Tejeda
 author_email = berttejeda@gmail.com
 description = Module for reading configuration files
-version = 4.4.3
+version = 4.4.4
 url = https://github.com/berttejeda/bert.config
 keywords = 
 	yaml
 	configuration
 	config
 	file
 	python
```

