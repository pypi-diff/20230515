# Comparing `tmp/database-factory-1.0.5.tar.gz` & `tmp/database-factory-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/database-factory-1.0.5.tar", last modified: Fri Apr 14 13:58:01 2023, max compression
+gzip compressed data, was "dist/database-factory-1.0.6.tar", last modified: Mon May 15 05:12:40 2023, max compression
```

## Comparing `database-factory-1.0.5.tar` & `database-factory-1.0.6.tar`

### file list

```diff
@@ -1,42 +1,32 @@
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.730333 database-factory-1.0.5/
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.726333 database-factory-1.0.5/.circleci/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     1066 2023-04-14 13:57:53.000000 database-factory-1.0.5/.circleci/config.yml
--rw-rw-r--   0 ankit     (1001) ankit     (1001)    53248 2023-04-14 13:57:53.000000 database-factory-1.0.5/.coverage
--rw-rw-r--   0 ankit     (1001) ankit     (1001)      137 2021-03-16 10:53:13.000000 database-factory-1.0.5/.coveragerc
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       66 2023-04-14 13:57:53.000000 database-factory-1.0.5/.gitignore
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     1117 2021-03-16 10:53:13.000000 database-factory-1.0.5/LICENSE
--rw-rw-r--   0 ankit     (1001) ankit     (1001)      233 2021-03-16 12:44:42.000000 database-factory-1.0.5/MANIFEST.in
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     7677 2023-04-14 13:58:01.730333 database-factory-1.0.5/PKG-INFO
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     4979 2023-04-14 13:57:53.000000 database-factory-1.0.5/README.md
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     8582 2023-04-14 13:57:53.000000 database-factory-1.0.5/coverage.xml
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.726333 database-factory-1.0.5/database_factory/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       45 2023-04-14 13:58:01.000000 database-factory-1.0.5/database_factory/.version
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/__init__.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.726333 database-factory-1.0.5/database_factory/cloud/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/cloud/__init__.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.726333 database-factory-1.0.5/database_factory/cloud/aws/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/cloud/aws/__init__.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     3204 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/cloud/aws/auth.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     3888 2021-08-10 05:53:56.000000 database-factory-1.0.5/database_factory/cloud/aws/secrete_manager.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.730333 database-factory-1.0.5/database_factory/cloud/gcp/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/cloud/gcp/__init__.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     5800 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/cloud/gcp/auth.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     5435 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/cloud/gcp/resource_manager.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     3876 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/cloud/gcp/secrete_manager.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.730333 database-factory-1.0.5/database_factory/common/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/common/__init__.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     4217 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/common/common.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)    17304 2023-04-14 13:57:53.000000 database-factory-1.0.5/database_factory/manager.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     5435 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/operations.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.726333 database-factory-1.0.5/database_factory.egg-info/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     7677 2023-04-14 13:58:01.000000 database-factory-1.0.5/database_factory.egg-info/PKG-INFO
--rw-rw-r--   0 ankit     (1001) ankit     (1001)      878 2023-04-14 13:58:01.000000 database-factory-1.0.5/database_factory.egg-info/SOURCES.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        1 2023-04-14 13:58:01.000000 database-factory-1.0.5/database_factory.egg-info/dependency_links.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     1132 2023-04-14 13:58:01.000000 database-factory-1.0.5/database_factory.egg-info/requires.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       17 2023-04-14 13:58:01.000000 database-factory-1.0.5/database_factory.egg-info/top_level.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       67 2023-04-14 13:58:01.730333 database-factory-1.0.5/setup.cfg
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     7121 2023-04-14 13:57:53.000000 database-factory-1.0.5/setup.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.730333 database-factory-1.0.5/test/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2022-06-15 09:04:02.000000 database-factory-1.0.5/test/__init__.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     2719 2022-06-15 09:04:02.000000 database-factory-1.0.5/test/database_factory_test.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       18 2023-04-14 13:57:53.000000 database-factory-1.0.5/version.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-05-15 05:12:40.126346 database-factory-1.0.6/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     1117 2021-03-16 10:53:13.000000 database-factory-1.0.6/LICENSE
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)      233 2021-03-16 12:44:42.000000 database-factory-1.0.6/MANIFEST.in
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     8061 2023-05-15 05:12:40.126346 database-factory-1.0.6/PKG-INFO
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     5355 2023-05-15 05:12:34.000000 database-factory-1.0.6/README.md
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-05-15 05:12:40.122346 database-factory-1.0.6/database_factory/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)       45 2023-05-15 05:12:39.000000 database-factory-1.0.6/database_factory/.version
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/__init__.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-05-15 05:12:40.126346 database-factory-1.0.6/database_factory/cloud/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/cloud/__init__.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-05-15 05:12:40.126346 database-factory-1.0.6/database_factory/cloud/aws/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/cloud/aws/__init__.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     3204 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/cloud/aws/auth.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     3888 2021-08-10 05:53:56.000000 database-factory-1.0.6/database_factory/cloud/aws/secrete_manager.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-05-15 05:12:40.126346 database-factory-1.0.6/database_factory/cloud/gcp/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/cloud/gcp/__init__.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     5800 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/cloud/gcp/auth.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     5435 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/cloud/gcp/resource_manager.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     3876 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/cloud/gcp/secrete_manager.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-05-15 05:12:40.126346 database-factory-1.0.6/database_factory/common/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/common/__init__.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     4217 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/common/common.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)    17304 2023-04-14 13:57:53.000000 database-factory-1.0.6/database_factory/manager.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     5435 2021-03-16 10:53:13.000000 database-factory-1.0.6/database_factory/operations.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-05-15 05:12:40.126346 database-factory-1.0.6/database_factory.egg-info/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     8061 2023-05-15 05:12:40.000000 database-factory-1.0.6/database_factory.egg-info/PKG-INFO
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)      753 2023-05-15 05:12:40.000000 database-factory-1.0.6/database_factory.egg-info/SOURCES.txt
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        1 2023-05-15 05:12:40.000000 database-factory-1.0.6/database_factory.egg-info/dependency_links.txt
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     1139 2023-05-15 05:12:40.000000 database-factory-1.0.6/database_factory.egg-info/requires.txt
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)       17 2023-05-15 05:12:40.000000 database-factory-1.0.6/database_factory.egg-info/top_level.txt
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)       67 2023-05-15 05:12:40.126346 database-factory-1.0.6/setup.cfg
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     7026 2023-05-15 05:12:34.000000 database-factory-1.0.6/setup.py
```

### Comparing `database-factory-1.0.5/LICENSE` & `database-factory-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.5/PKG-INFO` & `database-factory-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-factory
-Version: 1.0.5
+Version: 1.0.6
 Summary: Database Factory;
 Home-page: https://github.com/shrivastava-v-ankit/database-factory
 Author: Ankit Shrivastava
 License: MIT
 Project-URL: Source, https://github.com/shrivastava-v-ankit/database-factory/
 Project-URL: Tracker, https://github.com/shrivastava-v-ankit/database-factory/issues
 Description: # database-factory
@@ -180,30 +180,41 @@
         pip install .
         ```
         
         ### Contributing
         
         1. Fork repo- https://github.com/shrivastava-v-ankit/database-factory.git
         2. Create your feature branch - `git checkout -b feature/name`
-        3. Add Python test (pytest) and covrage report for new/changed feature.
+        3. Install Python packages
+           * sqlalchemy==1.4.47
+           * pandas==1.5.3
+           * GitPython
+           * coverage==7.2.3
+           * exceptiongroup==1.1.1
+           * iniconfig==2.0.0
+           * pluggy==1.0.0
+           * pytest==7.3.0
+           * pytest-cov==4.0.0
+           * tomli==2.0.1
+        4. Run Python test (pytest)
+           * pytest -v --cov --cov-report html --cov-report xml --junitxml=test-results/database_factory_test/results.xml
+        5. Add Python test (pytest) and covrage report for new/changed feature.
         4. Commit your changes - `git commit -am "Added name"`
         5. Push to the branch - `git push origin feature/name`
         6. Create a new pull request
         
         
 Keywords: python,os independent,database,sqlalchemy,sqlite3,sqlite,postgres,mysql,maridb,snowflake,bigquery,secret manager
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
-Requires-Python: >=3.4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `database-factory-1.0.5/README.md` & `database-factory-1.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -171,12 +171,25 @@
 pip install .
 ```
 
 ### Contributing
 
 1. Fork repo- https://github.com/shrivastava-v-ankit/database-factory.git
 2. Create your feature branch - `git checkout -b feature/name`
-3. Add Python test (pytest) and covrage report for new/changed feature.
+3. Install Python packages
+   * sqlalchemy==1.4.47
+   * pandas==1.5.3
+   * GitPython
+   * coverage==7.2.3
+   * exceptiongroup==1.1.1
+   * iniconfig==2.0.0
+   * pluggy==1.0.0
+   * pytest==7.3.0
+   * pytest-cov==4.0.0
+   * tomli==2.0.1
+4. Run Python test (pytest)
+   * pytest -v --cov --cov-report html --cov-report xml --junitxml=test-results/database_factory_test/results.xml
+5. Add Python test (pytest) and covrage report for new/changed feature.
 4. Commit your changes - `git commit -am "Added name"`
 5. Push to the branch - `git push origin feature/name`
 6. Create a new pull request
```

### Comparing `database-factory-1.0.5/database_factory/cloud/aws/auth.py` & `database-factory-1.0.6/database_factory/cloud/aws/auth.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.5/database_factory/cloud/aws/secrete_manager.py` & `database-factory-1.0.6/database_factory/cloud/aws/secrete_manager.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.5/database_factory/cloud/gcp/auth.py` & `database-factory-1.0.6/database_factory/cloud/gcp/auth.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.5/database_factory/cloud/gcp/resource_manager.py` & `database-factory-1.0.6/database_factory/cloud/gcp/resource_manager.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.5/database_factory/cloud/gcp/secrete_manager.py` & `database-factory-1.0.6/database_factory/cloud/gcp/secrete_manager.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.5/database_factory/common/common.py` & `database-factory-1.0.6/database_factory/common/common.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.5/database_factory/manager.py` & `database-factory-1.0.6/database_factory/manager.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.5/database_factory/operations.py` & `database-factory-1.0.6/database_factory/operations.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.5/database_factory.egg-info/PKG-INFO` & `database-factory-1.0.6/database_factory.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-factory
-Version: 1.0.5
+Version: 1.0.6
 Summary: Database Factory;
 Home-page: https://github.com/shrivastava-v-ankit/database-factory
 Author: Ankit Shrivastava
 License: MIT
 Project-URL: Source, https://github.com/shrivastava-v-ankit/database-factory/
 Project-URL: Tracker, https://github.com/shrivastava-v-ankit/database-factory/issues
 Description: # database-factory
@@ -180,30 +180,41 @@
         pip install .
         ```
         
         ### Contributing
         
         1. Fork repo- https://github.com/shrivastava-v-ankit/database-factory.git
         2. Create your feature branch - `git checkout -b feature/name`
-        3. Add Python test (pytest) and covrage report for new/changed feature.
+        3. Install Python packages
+           * sqlalchemy==1.4.47
+           * pandas==1.5.3
+           * GitPython
+           * coverage==7.2.3
+           * exceptiongroup==1.1.1
+           * iniconfig==2.0.0
+           * pluggy==1.0.0
+           * pytest==7.3.0
+           * pytest-cov==4.0.0
+           * tomli==2.0.1
+        4. Run Python test (pytest)
+           * pytest -v --cov --cov-report html --cov-report xml --junitxml=test-results/database_factory_test/results.xml
+        5. Add Python test (pytest) and covrage report for new/changed feature.
         4. Commit your changes - `git commit -am "Added name"`
         5. Push to the branch - `git push origin feature/name`
         6. Create a new pull request
         
         
 Keywords: python,os independent,database,sqlalchemy,sqlite3,sqlite,postgres,mysql,maridb,snowflake,bigquery,secret manager
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
-Requires-Python: >=3.4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `database-factory-1.0.5/database_factory.egg-info/requires.txt` & `database-factory-1.0.6/database_factory.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 google-api-python-client==2.85.0
 google-cloud-secret-manager==2.16.1
 google-cloud-resource-manager==1.9.1
 pybigquery==0.10.2
 snowflake-connector-python==2.7.9
 snowflake-sqlalchemy==1.4.7
 pg8000==1.29.4
-pymysql
+pymysql==1.0.3
 asn1crypto==1.5.1
 botocore==1.29.113
 cachetools==5.3.0
 certifi==2022.12.7
 cffi==1.15.1
 charset-normalizer==2.0.12
 cryptography==36.0.2
@@ -32,15 +32,15 @@
 httplib2==0.22.0
 idna==3.4
 jmespath==1.0.1
 numpy==1.24.2
 oscrypto==1.3.0
 packaging==23.1
 proto-plus==1.22.2
-protobuf==4.22.3
+protobuf==3.20.3
 pyarrow==6.0.1
 pyasn1==0.4.8
 pyasn1-modules==0.2.8
 pycparser==2.21
 pycryptodomex==3.17
 pyjwt==2.6.0
 pymysql==1.0.3
```

### Comparing `database-factory-1.0.5/setup.py` & `database-factory-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 postgres = [
     # PostgreSQL interface library.
     "pg8000==1.29.4"
 ]
 
 mysql = [
     # Pure Python MySQL Driver
-    "pymysql"
+    "pymysql==1.0.3"
 ]
 
 dependencies = [
     "asn1crypto==1.5.1",
     "botocore==1.29.113",
     "cachetools==5.3.0",
     "certifi==2022.12.7",
@@ -103,15 +103,15 @@
     "httplib2==0.22.0",
     "idna==3.4",
     "jmespath==1.0.1",
     "numpy==1.24.2",
     "oscrypto==1.3.0",
     "packaging==23.1",
     "proto-plus==1.22.2",
-    "protobuf==4.22.3",
+    "protobuf==3.20.3",
     "pyarrow==6.0.1",
     "pyasn1==0.4.8",
     "pyasn1-modules==0.2.8",
     "pycparser==2.21",
     "pycryptodomex==3.17",
     "pyjwt==2.6.0",
     "pymysql==1.0.3",
@@ -202,32 +202,30 @@
         author="Ankit Shrivastava",
         url="https://github.com/shrivastava-v-ankit/database-factory",
         packages=find_packages(include=[__NAME__.replace("-", "_")]),
         include_package_data=True,
         setup_requires=setups,
         install_requires=requires,
         license="MIT",
-        python_requires=">=3.4",
+        python_requires=">=3.7, <4",
         platforms='any',
         project_urls={
             'Source': 'https://github.com/shrivastava-v-ankit/database-factory/',
             'Tracker': 'https://github.com/shrivastava-v-ankit/database-factory/issues',
         },
         classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Environment :: Web Environment',
             'Intended Audience :: Developers',
             'Natural Language :: English',
             'License :: OSI Approved :: MIT License',
             'Operating System :: OS Independent',
-            'Programming Language :: Python :: 3.4',
-            'Programming Language :: Python :: 3.5',
-            'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9',
             'Topic :: Software Development :: Libraries :: Python Modules',
             'Topic :: Software Development :: Version Control :: Git',
         ],
     )
 
 
 if __name__ == "__main__":
```

