# Comparing `tmp/aws_cron_expression_validator-1.0.9.tar.gz` & `tmp/aws_cron_expression_validator-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/aws_cron_expression_validator/aws_cron_expression_validator/dist/.tmp-n72164f3/aws_cron_expression_validator-", last modified: Tue Mar  7 07:36:38 2023, max compression
+gzip compressed data, was "/home/runner/work/aws_cron_expression_validator/aws_cron_expression_validator/dist/.tmp-_ohzvamu/aws_cron_expression_validator-", last modified: Sun May 14 23:42:02 2023, max compression
```

## Comparing `aws_cron_expression_validator-1.0.9.tar` & `aws_cron_expression_validator-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:36:38.000000 aws_cron_expression_validator-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-07 07:36:16.000000 aws_cron_expression_validator-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-03-07 07:36:38.000000 aws_cron_expression_validator-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-03-07 07:36:16.000000 aws_cron_expression_validator-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-07 07:36:16.000000 aws_cron_expression_validator-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 07:36:38.000000 aws_cron_expression_validator-1.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:36:38.000000 aws_cron_expression_validator-1.0.9/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:36:16.000000 aws_cron_expression_validator-1.0.9/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:36:38.000000 aws_cron_expression_validator-1.0.9/src/aws_cron_expression_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 07:36:16.000000 aws_cron_expression_validator-1.0.9/src/aws_cron_expression_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-03-07 07:36:16.000000 aws_cron_expression_validator-1.0.9/src/aws_cron_expression_validator/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:36:38.000000 aws_cron_expression_validator-1.0.9/src/aws_cron_expression_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-03-07 07:36:38.000000 aws_cron_expression_validator-1.0.9/src/aws_cron_expression_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-07 07:36:38.000000 aws_cron_expression_validator-1.0.9/src/aws_cron_expression_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 07:36:38.000000 aws_cron_expression_validator-1.0.9/src/aws_cron_expression_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-07 07:36:38.000000 aws_cron_expression_validator-1.0.9/src/aws_cron_expression_validator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-14 23:41:41.000000 aws_cron_expression_validator-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-14 23:41:41.000000 aws_cron_expression_validator-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-14 23:41:41.000000 aws_cron_expression_validator-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:41.000000 aws_cron_expression_validator-1.1.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:41.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-14 23:41:41.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 23:42:02.000000 aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator.egg-info/top_level.txt
```

### Comparing `aws_cron_expression_validator-1.0.9/LICENSE` & `aws_cron_expression_validator-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_cron_expression_validator-1.0.9/PKG-INFO` & `aws_cron_expression_validator-1.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: aws_cron_expression_validator
-Version: 1.0.9
-Summary: ValidatesAWS EventBridge cron expressions, which are similar to, but not compatible with Unix style cron expressions
-Author-email: Graham Coster <bitjugglers@gmail.com>
-Project-URL: Homepage, https://github.com/grumBit/aws_cron_expression_validator.git
-Project-URL: Bug Tracker, https://github.com/grumBit/aws_cron_expression_validator/issues
-Project-URL: Source, https://github.com/grumBit/aws_cron_expression_validator
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![PyPI](https://img.shields.io/pypi/v/aws_cron_expression_validator)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aws_cron_expression_validator)
 ![GitHub all releases](https://img.shields.io/github/downloads/grumbit/aws_cron_expression_validator/total)
 [![GitHub license](https://img.shields.io/github/license/grumbit/aws_cron_expression_validator)](https://github.com/grumbit/aws_cron_expression_validator/blob/master/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/aws_cron_expression_validator)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/aws_cron_expression_validator)
 ![PyPI - Status](https://img.shields.io/pypi/status/aws_cron_expression_validator)
```

### Comparing `aws_cron_expression_validator-1.0.9/README.md` & `aws_cron_expression_validator-1.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: aws_cron_expression_validator
+Version: 1.1.2
+Summary: ValidatesAWS EventBridge cron expressions, which are similar to, but not compatible with Unix style cron expressions
+Author-email: Graham Coster <bitjugglers@gmail.com>
+Project-URL: Homepage, https://github.com/grumBit/aws_cron_expression_validator.git
+Project-URL: Bug Tracker, https://github.com/grumBit/aws_cron_expression_validator/issues
+Project-URL: Source, https://github.com/grumBit/aws_cron_expression_validator
+Project-URL: Security Policy, https://github.com/grumbit/aws_cron_expression_validator/blob/master/.github/SECURITY.md
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![PyPI](https://img.shields.io/pypi/v/aws_cron_expression_validator)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aws_cron_expression_validator)
 ![GitHub all releases](https://img.shields.io/github/downloads/grumbit/aws_cron_expression_validator/total)
 [![GitHub license](https://img.shields.io/github/license/grumbit/aws_cron_expression_validator)](https://github.com/grumbit/aws_cron_expression_validator/blob/master/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/aws_cron_expression_validator)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/aws_cron_expression_validator)
 ![PyPI - Status](https://img.shields.io/pypi/status/aws_cron_expression_validator)
```

### Comparing `aws_cron_expression_validator-1.0.9/pyproject.toml` & `aws_cron_expression_validator-1.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aws_cron_expression_validator"
-version = "1.0.9"
+version = "1.1.2"
 authors = [
   { name="Graham Coster", email="bitjugglers@gmail.com" },
 ]
 description = "ValidatesAWS EventBridge cron expressions, which are similar to, but not compatible with Unix style cron expressions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,14 +18,15 @@
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/grumBit/aws_cron_expression_validator.git"
 "Bug Tracker" = "https://github.com/grumBit/aws_cron_expression_validator/issues"
 "Source" = "https://github.com/grumBit/aws_cron_expression_validator"
+"Security Policy" = "https://github.com/grumbit/aws_cron_expression_validator/blob/master/.github/SECURITY.md"
 
 [tool.pytest.ini_options]
 addopts = "--cov-report html --cov-report term-missing --cov-fail-under 95"
 
 [tool.coverage.run]
 source = ["src"]
```

### Comparing `aws_cron_expression_validator-1.0.9/src/aws_cron_expression_validator/validator.py` & `aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,18 @@
     @classmethod
     def list_regex(cls, values: str) -> str:
         range_ = cls.range_regex(values)
         return rf"({range_}(\,{range_})*)"  # One or more ranges separated by a comma
 
     @classmethod
     def slash_regex(cls, values: str) -> str:
-        return rf"((\*|{values})\/[0-9]*[1-9][0-9]*)"
-        # Slash can be preceded by * or a valid value and must be followed by an natural number as the increment.
+        range_ = cls.range_regex(values)
+        return rf"((\*|{range_}|{values})\/[0-9]*[1-9][0-9]*)"
+        # Slash can be preceded by *, range, or a valid value and must be followed by an natural
+        # number as the increment.
 
     @classmethod
     def common_regex(cls, values: str) -> str:
         return rf"({cls.list_regex(values)}|\*|{cls.slash_regex(values)})"  # values , - * /
 
     @classmethod
     def minute_regex(cls) -> str:
```

### Comparing `aws_cron_expression_validator-1.0.9/src/aws_cron_expression_validator.egg-info/PKG-INFO` & `aws_cron_expression_validator-1.1.2/src/aws_cron_expression_validator.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: aws-cron-expression-validator
-Version: 1.0.9
+Version: 1.1.2
 Summary: ValidatesAWS EventBridge cron expressions, which are similar to, but not compatible with Unix style cron expressions
 Author-email: Graham Coster <bitjugglers@gmail.com>
 Project-URL: Homepage, https://github.com/grumBit/aws_cron_expression_validator.git
 Project-URL: Bug Tracker, https://github.com/grumBit/aws_cron_expression_validator/issues
 Project-URL: Source, https://github.com/grumBit/aws_cron_expression_validator
+Project-URL: Security Policy, https://github.com/grumbit/aws_cron_expression_validator/blob/master/.github/SECURITY.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

