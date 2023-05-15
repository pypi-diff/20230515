# Comparing `tmp/clear-skies-aws-1.2.5.tar.gz` & `tmp/clear-skies-aws-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear-skies-aws-1.2.5.tar", last modified: Tue May  2 17:00:59 2023, max compression
+gzip compressed data, was "clear-skies-aws-1.3.0.tar", last modified: Mon May 15 10:23:54 2023, max compression
```

## Comparing `clear-skies-aws-1.2.5.tar` & `clear-skies-aws-1.3.0.tar`

### file list

```diff
@@ -1,47 +1,53 @@
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-02 17:00:59.683677 clear-skies-aws-1.2.5/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1053 2022-01-16 00:26:29.000000 clear-skies-aws-1.2.5/LICENSE
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       25 2022-01-16 00:26:29.000000 clear-skies-aws-1.2.5/MANIFEST.in
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8371 2023-05-02 17:00:59.683677 clear-skies-aws-1.2.5/PKG-INFO
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     7780 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.5/README.md
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       79 2023-05-02 17:00:59.683677 clear-skies-aws-1.2.5/setup.cfg
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1375 2023-05-02 17:00:07.000000 clear-skies-aws-1.2.5/setup.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-02 17:00:59.671677 clear-skies-aws-1.2.5/src/
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-02 17:00:59.671677 clear-skies-aws-1.2.5/src/clear_skies_aws.egg-info/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8371 2023-05-02 17:00:59.000000 clear-skies-aws-1.2.5/src/clear_skies_aws.egg-info/PKG-INFO
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1604 2023-05-02 17:00:59.000000 clear-skies-aws-1.2.5/src/clear_skies_aws.egg-info/SOURCES.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        1 2023-05-02 17:00:59.000000 clear-skies-aws-1.2.5/src/clear_skies_aws.egg-info/dependency_links.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       36 2023-05-02 17:00:59.000000 clear-skies-aws-1.2.5/src/clear_skies_aws.egg-info/requires.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       15 2023-05-02 17:00:59.000000 clear-skies-aws-1.2.5/src/clear_skies_aws.egg-info/top_level.txt
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-02 17:00:59.671677 clear-skies-aws-1.2.5/src/clearskies_aws/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       42 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-02 17:00:59.675677 clear-skies-aws-1.2.5/src/clearskies_aws/backends/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       83 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.5/src/clearskies_aws/backends/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    27872 2023-05-02 16:59:54.000000 clear-skies-aws-1.2.5/src/clearskies_aws/backends/dynamo_db_backend.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2726 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.5/src/clearskies_aws/backends/sqs_backend.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-02 17:00:59.675677 clear-skies-aws-1.2.5/src/clearskies_aws/contexts/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      290 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.5/src/clearskies_aws/contexts/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      506 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.5/src/clearskies_aws/contexts/cli.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1002 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/contexts/lambda_api_gateway.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      952 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/contexts/lambda_elb.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1009 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/contexts/lambda_http_gateway.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1183 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/contexts/lambda_invocation.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1678 2023-04-04 23:13:02.000000 clear-skies-aws-1.2.5/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-02 17:00:59.675677 clear-skies-aws-1.2.5/src/clearskies_aws/di/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       56 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/di/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      775 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.5/src/clearskies_aws/di/standard_dependencies.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-02 17:00:59.679677 clear-skies-aws-1.2.5/src/clearskies_aws/input_outputs/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      233 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.5/src/clearskies_aws/input_outputs/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2932 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/input_outputs/lambda_api_gateway.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      662 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/input_outputs/lambda_elb.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      692 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/input_outputs/lambda_http_gateway.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      715 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/input_outputs/lambda_invocation.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2047 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.5/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-02 17:00:59.679677 clear-skies-aws-1.2.5/src/clearskies_aws/secrets/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      121 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/secrets/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-02 17:00:59.683677 clear-skies-aws-1.2.5/src/clearskies_aws/secrets/additional_configs/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1810 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/secrets/additional_configs/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1082 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3776 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6444 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.5/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1655 2023-04-14 14:57:45.000000 clear-skies-aws-1.2.5/src/clearskies_aws/secrets/parameter_store.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2898 2023-04-14 14:57:45.000000 clear-skies-aws-1.2.5/src/clearskies_aws/secrets/secrets_manager.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 10:23:54.204352 clear-skies-aws-1.3.0/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1053 2022-01-16 00:26:29.000000 clear-skies-aws-1.3.0/LICENSE
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       25 2022-01-16 00:26:29.000000 clear-skies-aws-1.3.0/MANIFEST.in
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8371 2023-05-15 10:23:54.204352 clear-skies-aws-1.3.0/PKG-INFO
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     7780 2023-03-26 15:10:17.000000 clear-skies-aws-1.3.0/README.md
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       79 2023-05-15 10:23:54.204352 clear-skies-aws-1.3.0/setup.cfg
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1375 2023-05-15 10:23:33.000000 clear-skies-aws-1.3.0/setup.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 10:23:54.192352 clear-skies-aws-1.3.0/src/
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 10:23:54.196352 clear-skies-aws-1.3.0/src/clear_skies_aws.egg-info/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8371 2023-05-15 10:23:54.000000 clear-skies-aws-1.3.0/src/clear_skies_aws.egg-info/PKG-INFO
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1787 2023-05-15 10:23:54.000000 clear-skies-aws-1.3.0/src/clear_skies_aws.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        1 2023-05-15 10:23:54.000000 clear-skies-aws-1.3.0/src/clear_skies_aws.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       36 2023-05-15 10:23:54.000000 clear-skies-aws-1.3.0/src/clear_skies_aws.egg-info/requires.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       15 2023-05-15 10:23:54.000000 clear-skies-aws-1.3.0/src/clear_skies_aws.egg-info/top_level.txt
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 10:23:54.196352 clear-skies-aws-1.3.0/src/clearskies_aws/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       51 2023-05-14 11:11:00.000000 clear-skies-aws-1.3.0/src/clearskies_aws/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 10:23:54.196352 clear-skies-aws-1.3.0/src/clearskies_aws/actions/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      885 2023-05-14 19:32:03.000000 clear-skies-aws-1.3.0/src/clearskies_aws/actions/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2023-05-14 11:10:30.000000 clear-skies-aws-1.3.0/src/clearskies_aws/actions/assume_role.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6728 2023-05-15 10:22:13.000000 clear-skies-aws-1.3.0/src/clearskies_aws/actions/ses.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2023-05-14 11:10:26.000000 clear-skies-aws-1.3.0/src/clearskies_aws/actions/sns.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2921 2023-05-15 10:23:42.000000 clear-skies-aws-1.3.0/src/clearskies_aws/actions/sqs.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 10:23:54.196352 clear-skies-aws-1.3.0/src/clearskies_aws/backends/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       83 2023-03-26 15:10:17.000000 clear-skies-aws-1.3.0/src/clearskies_aws/backends/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    27872 2023-05-02 16:59:54.000000 clear-skies-aws-1.3.0/src/clearskies_aws/backends/dynamo_db_backend.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2726 2023-03-26 15:10:17.000000 clear-skies-aws-1.3.0/src/clearskies_aws/backends/sqs_backend.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 10:23:54.200352 clear-skies-aws-1.3.0/src/clearskies_aws/contexts/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      290 2023-03-26 15:10:17.000000 clear-skies-aws-1.3.0/src/clearskies_aws/contexts/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      506 2023-03-26 15:10:17.000000 clear-skies-aws-1.3.0/src/clearskies_aws/contexts/cli.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1002 2023-03-26 13:26:58.000000 clear-skies-aws-1.3.0/src/clearskies_aws/contexts/lambda_api_gateway.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      952 2023-03-26 13:26:58.000000 clear-skies-aws-1.3.0/src/clearskies_aws/contexts/lambda_elb.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1009 2023-03-26 13:26:58.000000 clear-skies-aws-1.3.0/src/clearskies_aws/contexts/lambda_http_gateway.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1183 2023-03-26 13:26:58.000000 clear-skies-aws-1.3.0/src/clearskies_aws/contexts/lambda_invocation.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1678 2023-04-04 23:13:02.000000 clear-skies-aws-1.3.0/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 10:23:54.200352 clear-skies-aws-1.3.0/src/clearskies_aws/di/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       56 2023-03-26 13:26:58.000000 clear-skies-aws-1.3.0/src/clearskies_aws/di/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      775 2023-03-26 15:10:17.000000 clear-skies-aws-1.3.0/src/clearskies_aws/di/standard_dependencies.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 10:23:54.204352 clear-skies-aws-1.3.0/src/clearskies_aws/input_outputs/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      233 2023-03-26 15:10:17.000000 clear-skies-aws-1.3.0/src/clearskies_aws/input_outputs/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2932 2023-03-26 13:26:58.000000 clear-skies-aws-1.3.0/src/clearskies_aws/input_outputs/lambda_api_gateway.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      662 2023-03-26 13:26:58.000000 clear-skies-aws-1.3.0/src/clearskies_aws/input_outputs/lambda_elb.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      692 2023-03-26 13:26:58.000000 clear-skies-aws-1.3.0/src/clearskies_aws/input_outputs/lambda_http_gateway.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      715 2023-03-26 13:26:58.000000 clear-skies-aws-1.3.0/src/clearskies_aws/input_outputs/lambda_invocation.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2047 2023-03-26 15:10:17.000000 clear-skies-aws-1.3.0/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 10:23:54.204352 clear-skies-aws-1.3.0/src/clearskies_aws/secrets/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      121 2023-03-26 13:26:58.000000 clear-skies-aws-1.3.0/src/clearskies_aws/secrets/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 10:23:54.204352 clear-skies-aws-1.3.0/src/clearskies_aws/secrets/additional_configs/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1810 2023-03-26 13:26:58.000000 clear-skies-aws-1.3.0/src/clearskies_aws/secrets/additional_configs/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1082 2023-03-26 13:26:58.000000 clear-skies-aws-1.3.0/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3776 2023-03-26 13:26:58.000000 clear-skies-aws-1.3.0/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6444 2023-03-26 13:26:58.000000 clear-skies-aws-1.3.0/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1655 2023-04-14 14:57:45.000000 clear-skies-aws-1.3.0/src/clearskies_aws/secrets/parameter_store.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2898 2023-04-14 14:57:45.000000 clear-skies-aws-1.3.0/src/clearskies_aws/secrets/secrets_manager.py
```

### Comparing `clear-skies-aws-1.2.5/LICENSE` & `clear-skies-aws-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/PKG-INFO` & `clear-skies-aws-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-aws
-Version: 1.2.5
+Version: 1.3.0
 Summary: clearskies bindings for working in AWS
 Home-page: https://github.com/cmancone/clearskies-aws
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 License: MIT
 Keywords: setuptools development
 Classifier: Development Status :: 4 - Beta
```

### Comparing `clear-skies-aws-1.2.5/README.md` & `clear-skies-aws-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/setup.py` & `clear-skies-aws-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='clear-skies-aws',
-    version='1.2.5',
+    version='1.3.0',
     description='clearskies bindings for working in AWS',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cmancone/clearskies-aws',
     author='Conor Mancone',
     author_email='cmancone@gmail.com',
     license='MIT',
```

### Comparing `clear-skies-aws-1.2.5/src/clear_skies_aws.egg-info/PKG-INFO` & `clear-skies-aws-1.3.0/src/clear_skies_aws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-aws
-Version: 1.2.5
+Version: 1.3.0
 Summary: clearskies bindings for working in AWS
 Home-page: https://github.com/cmancone/clearskies-aws
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 License: MIT
 Keywords: setuptools development
 Classifier: Development Status :: 4 - Beta
```

### Comparing `clear-skies-aws-1.2.5/src/clear_skies_aws.egg-info/SOURCES.txt` & `clear-skies-aws-1.3.0/src/clear_skies_aws.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 setup.py
 src/clear_skies_aws.egg-info/PKG-INFO
 src/clear_skies_aws.egg-info/SOURCES.txt
 src/clear_skies_aws.egg-info/dependency_links.txt
 src/clear_skies_aws.egg-info/requires.txt
 src/clear_skies_aws.egg-info/top_level.txt
 src/clearskies_aws/__init__.py
+src/clearskies_aws/actions/__init__.py
+src/clearskies_aws/actions/assume_role.py
+src/clearskies_aws/actions/ses.py
+src/clearskies_aws/actions/sns.py
+src/clearskies_aws/actions/sqs.py
 src/clearskies_aws/backends/__init__.py
 src/clearskies_aws/backends/dynamo_db_backend.py
 src/clearskies_aws/backends/sqs_backend.py
 src/clearskies_aws/contexts/__init__.py
 src/clearskies_aws/contexts/cli.py
 src/clearskies_aws/contexts/lambda_api_gateway.py
 src/clearskies_aws/contexts/lambda_elb.py
```

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/backends/dynamo_db_backend.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/backends/dynamo_db_backend.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/backends/sqs_backend.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/backends/sqs_backend.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/contexts/lambda_api_gateway.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/contexts/lambda_api_gateway.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/contexts/lambda_elb.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/contexts/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/contexts/lambda_http_gateway.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/contexts/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/contexts/lambda_invocation.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/contexts/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/di/standard_dependencies.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/di/standard_dependencies.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/input_outputs/lambda_api_gateway.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/input_outputs/lambda_api_gateway.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/input_outputs/lambda_elb.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/input_outputs/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/input_outputs/lambda_http_gateway.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/input_outputs/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/input_outputs/lambda_invocation.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/input_outputs/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/input_outputs/lambda_sqs_standard.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/input_outputs/lambda_sqs_standard.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/secrets/additional_configs/__init__.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/secrets/additional_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/secrets/parameter_store.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/secrets/parameter_store.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.5/src/clearskies_aws/secrets/secrets_manager.py` & `clear-skies-aws-1.3.0/src/clearskies_aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

