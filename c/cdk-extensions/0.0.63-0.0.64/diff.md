# Comparing `tmp/cdk-extensions-0.0.63.tar.gz` & `tmp/cdk-extensions-0.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-extensions-0.0.63.tar", last modified: Mon May 15 14:47:56 2023, max compression
+gzip compressed data, was "cdk-extensions-0.0.64.tar", last modified: Mon May 15 19:14:01 2023, max compression
```

## Comparing `cdk-extensions-0.0.63.tar` & `cdk-extensions-0.0.64.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.510759 cdk-extensions-0.0.63/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.510759 cdk-extensions-0.0.63/src/cdk_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/_jsii/bin/init-aws.sh
--rw-r--r--   0 runner    (1001) docker     (123)  1594973 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/_jsii/cdk-extensions@0.0.63.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions/aps/
--rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/aps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions/asserts/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/asserts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions/athena/
--rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/athena/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)   702552 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.518759 cdk-extensions-0.0.63/src/cdk_extensions/ec2_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)   267981 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/ec2_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.518759 cdk-extensions-0.0.63/src/cdk_extensions/eks_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/eks_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.518759 cdk-extensions-0.0.63/src/cdk_extensions/glue/
--rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.518759 cdk-extensions-0.0.63/src/cdk_extensions/glue_tables/
--rw-r--r--   0 runner    (1001) docker     (123)   140852 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/glue_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.518759 cdk-extensions-0.0.63/src/cdk_extensions/k8s_aws/
--rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/k8s_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.518759 cdk-extensions-0.0.63/src/cdk_extensions/k8s_fargate/
--rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/k8s_fargate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.518759 cdk-extensions-0.0.63/src/cdk_extensions/kinesis_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/kinesis_firehose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/lambda_/
--rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/lambda_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/networkmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/ram/
--rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/ram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/ram_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/ram_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/rds/
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/rds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/route53/
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)   215302 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/s3_buckets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/sso/
--rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/sso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/stacks/
--rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-15 14:47:56.000000 cdk-extensions-0.0.63/src/cdk_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-15 14:47:56.000000 cdk-extensions-0.0.63/src/cdk_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:47:56.000000 cdk-extensions-0.0.63/src/cdk_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-15 14:47:56.000000 cdk-extensions-0.0.63/src/cdk_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 14:47:56.000000 cdk-extensions-0.0.63/src/cdk_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.912341 cdk-extensions-0.0.64/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.916341 cdk-extensions-0.0.64/src/cdk_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.916341 cdk-extensions-0.0.64/src/cdk_extensions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.916341 cdk-extensions-0.0.64/src/cdk_extensions/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/_jsii/bin/init-aws.sh
+-rw-r--r--   0 runner    (1001) docker     (123)  1595030 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/_jsii/cdk-extensions@0.0.64.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.916341 cdk-extensions-0.0.64/src/cdk_extensions/aps/
+-rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/aps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/asserts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/asserts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/athena/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)   702552 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/ec2_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)   267981 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/ec2_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/eks_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/eks_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/glue_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)   140852 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/glue_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/k8s_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/k8s_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/k8s_fargate/
+-rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/k8s_fargate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/kinesis_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/kinesis_firehose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/lambda_/
+-rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/lambda_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/networkmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/ram/
+-rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/ram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/ram_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/ram_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/rds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)   215302 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/s3_buckets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/sso/
+-rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/sso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/stacks/
+-rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.916341 cdk-extensions-0.0.64/src/cdk_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-15 19:14:01.000000 cdk-extensions-0.0.64/src/cdk_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-15 19:14:01.000000 cdk-extensions-0.0.64/src/cdk_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:14:01.000000 cdk-extensions-0.0.64/src/cdk_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-15 19:14:01.000000 cdk-extensions-0.0.64/src/cdk_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 19:14:01.000000 cdk-extensions-0.0.64/src/cdk_extensions.egg-info/top_level.txt
```

### Comparing `cdk-extensions-0.0.63/LICENSE` & `cdk-extensions-0.0.64/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/PKG-INFO` & `cdk-extensions-0.0.64/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.63
+Version: 0.0.64
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.63/README.md` & `cdk-extensions-0.0.64/README.md`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/setup.py` & `cdk-extensions-0.0.64/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-extensions",
-    "version": "0.0.63",
+    "version": "0.0.64",
     "description": "cdk-extensions",
     "license": "Apache-2.0",
     "url": "https://github.com/vibe-io/cdk-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Kevin Lucas<kevinluc08@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -43,15 +43,15 @@
         "cdk_extensions.route53",
         "cdk_extensions.s3_buckets",
         "cdk_extensions.sso",
         "cdk_extensions.stacks"
     ],
     "package_data": {
         "cdk_extensions._jsii": [
-            "cdk-extensions@0.0.63.jsii.tgz"
+            "cdk-extensions@0.0.64.jsii.tgz"
         ],
         "cdk_extensions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/aps/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/asserts/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/asserts/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/athena/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/core/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/ec2/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/ec2_patterns/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/ec2_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/eks_patterns/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/eks_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/glue/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/glue_tables/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/glue_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/k8s_aws/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/k8s_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/k8s_fargate/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/k8s_fargate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/kinesis_firehose/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/kinesis_firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/lambda_/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/networkmanager/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/ram/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/ram_resources/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/ram_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/rds/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/route53/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/s3_buckets/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/s3_buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/sso/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/sso/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions/stacks/__init__.py` & `cdk-extensions-0.0.64/src/cdk_extensions/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions.egg-info/PKG-INFO` & `cdk-extensions-0.0.64/src/cdk_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.63
+Version: 0.0.64
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.63/src/cdk_extensions.egg-info/SOURCES.txt` & `cdk-extensions-0.0.64/src/cdk_extensions.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdk_extensions/py.typed
 src/cdk_extensions.egg-info/PKG-INFO
 src/cdk_extensions.egg-info/SOURCES.txt
 src/cdk_extensions.egg-info/dependency_links.txt
 src/cdk_extensions.egg-info/requires.txt
 src/cdk_extensions.egg-info/top_level.txt
 src/cdk_extensions/_jsii/__init__.py
-src/cdk_extensions/_jsii/cdk-extensions@0.0.63.jsii.tgz
+src/cdk_extensions/_jsii/cdk-extensions@0.0.64.jsii.tgz
 src/cdk_extensions/_jsii/bin/init-aws.sh
 src/cdk_extensions/aps/__init__.py
 src/cdk_extensions/asserts/__init__.py
 src/cdk_extensions/athena/__init__.py
 src/cdk_extensions/core/__init__.py
 src/cdk_extensions/ec2/__init__.py
 src/cdk_extensions/ec2_patterns/__init__.py
```

