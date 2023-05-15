# Comparing `tmp/cdk-extensions-0.0.62.tar.gz` & `tmp/cdk-extensions-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-extensions-0.0.62.tar", last modified: Fri May 12 21:02:10 2023, max compression
+gzip compressed data, was "cdk-extensions-0.0.63.tar", last modified: Mon May 15 14:47:56 2023, max compression
```

## Comparing `cdk-extensions-0.0.62.tar` & `cdk-extensions-0.0.63.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.423453 cdk-extensions-0.0.62/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-12 21:02:10.423453 cdk-extensions-0.0.62/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 21:02:10.423453 cdk-extensions-0.0.62/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.411453 cdk-extensions-0.0.62/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.415453 cdk-extensions-0.0.62/src/cdk_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.415453 cdk-extensions-0.0.62/src/cdk_extensions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.415453 cdk-extensions-0.0.62/src/cdk_extensions/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/_jsii/bin/init-aws.sh
--rw-r--r--   0 runner    (1001) docker     (123)  1594047 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/_jsii/cdk-extensions@0.0.62.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.415453 cdk-extensions-0.0.62/src/cdk_extensions/aps/
--rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/aps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.415453 cdk-extensions-0.0.62/src/cdk_extensions/asserts/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/asserts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.415453 cdk-extensions-0.0.62/src/cdk_extensions/athena/
--rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/athena/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.415453 cdk-extensions-0.0.62/src/cdk_extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.419453 cdk-extensions-0.0.62/src/cdk_extensions/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)   702552 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.419453 cdk-extensions-0.0.62/src/cdk_extensions/ec2_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)   261565 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/ec2_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.419453 cdk-extensions-0.0.62/src/cdk_extensions/eks_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/eks_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.419453 cdk-extensions-0.0.62/src/cdk_extensions/glue/
--rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.419453 cdk-extensions-0.0.62/src/cdk_extensions/glue_tables/
--rw-r--r--   0 runner    (1001) docker     (123)   140852 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/glue_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.419453 cdk-extensions-0.0.62/src/cdk_extensions/k8s_aws/
--rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/k8s_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.419453 cdk-extensions-0.0.62/src/cdk_extensions/k8s_fargate/
--rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/k8s_fargate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.419453 cdk-extensions-0.0.62/src/cdk_extensions/kinesis_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/kinesis_firehose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.419453 cdk-extensions-0.0.62/src/cdk_extensions/lambda_/
--rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/lambda_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.419453 cdk-extensions-0.0.62/src/cdk_extensions/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/networkmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.419453 cdk-extensions-0.0.62/src/cdk_extensions/ram/
--rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/ram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.419453 cdk-extensions-0.0.62/src/cdk_extensions/ram_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/ram_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.419453 cdk-extensions-0.0.62/src/cdk_extensions/rds/
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/rds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.423453 cdk-extensions-0.0.62/src/cdk_extensions/route53/
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.423453 cdk-extensions-0.0.62/src/cdk_extensions/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)   215302 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/s3_buckets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.423453 cdk-extensions-0.0.62/src/cdk_extensions/sso/
--rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/sso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.423453 cdk-extensions-0.0.62/src/cdk_extensions/stacks/
--rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-05-12 21:01:58.000000 cdk-extensions-0.0.62/src/cdk_extensions/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:02:10.415453 cdk-extensions-0.0.62/src/cdk_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-12 21:02:10.000000 cdk-extensions-0.0.62/src/cdk_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-12 21:02:10.000000 cdk-extensions-0.0.62/src/cdk_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:02:10.000000 cdk-extensions-0.0.62/src/cdk_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-12 21:02:10.000000 cdk-extensions-0.0.62/src/cdk_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-12 21:02:10.000000 cdk-extensions-0.0.62/src/cdk_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.510759 cdk-extensions-0.0.63/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.510759 cdk-extensions-0.0.63/src/cdk_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/_jsii/bin/init-aws.sh
+-rw-r--r--   0 runner    (1001) docker     (123)  1594973 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/_jsii/cdk-extensions@0.0.63.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions/aps/
+-rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/aps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions/asserts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/asserts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/athena/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)   702552 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.518759 cdk-extensions-0.0.63/src/cdk_extensions/ec2_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)   267981 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/ec2_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.518759 cdk-extensions-0.0.63/src/cdk_extensions/eks_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/eks_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.518759 cdk-extensions-0.0.63/src/cdk_extensions/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.518759 cdk-extensions-0.0.63/src/cdk_extensions/glue_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)   140852 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/glue_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.518759 cdk-extensions-0.0.63/src/cdk_extensions/k8s_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/k8s_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.518759 cdk-extensions-0.0.63/src/cdk_extensions/k8s_fargate/
+-rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/k8s_fargate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.518759 cdk-extensions-0.0.63/src/cdk_extensions/kinesis_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/kinesis_firehose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/lambda_/
+-rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/lambda_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/networkmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/ram/
+-rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/ram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/ram_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/ram_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/rds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)   215302 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/s3_buckets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/sso/
+-rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/sso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.522759 cdk-extensions-0.0.63/src/cdk_extensions/stacks/
+-rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-05-15 14:47:43.000000 cdk-extensions-0.0.63/src/cdk_extensions/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:47:56.514759 cdk-extensions-0.0.63/src/cdk_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-15 14:47:56.000000 cdk-extensions-0.0.63/src/cdk_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-15 14:47:56.000000 cdk-extensions-0.0.63/src/cdk_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:47:56.000000 cdk-extensions-0.0.63/src/cdk_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-15 14:47:56.000000 cdk-extensions-0.0.63/src/cdk_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 14:47:56.000000 cdk-extensions-0.0.63/src/cdk_extensions.egg-info/top_level.txt
```

### Comparing `cdk-extensions-0.0.62/LICENSE` & `cdk-extensions-0.0.63/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/PKG-INFO` & `cdk-extensions-0.0.63/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.62
+Version: 0.0.63
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.62/README.md` & `cdk-extensions-0.0.63/README.md`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/setup.py` & `cdk-extensions-0.0.63/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-extensions",
-    "version": "0.0.62",
+    "version": "0.0.63",
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
-            "cdk-extensions@0.0.62.jsii.tgz"
+            "cdk-extensions@0.0.63.jsii.tgz"
         ],
         "cdk_extensions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/aps/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/asserts/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/asserts/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/athena/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/core/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/ec2/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/ec2_patterns/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/ec2_patterns/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,99 @@
 from ..ram import (
     ISharedPrincipal as _ISharedPrincipal_9cde791b,
     ResourceShare as _ResourceShare_f0180713,
 )
 
 
 @jsii.data_type(
+    jsii_type="cdk-extensions.ec2_patterns.AddAuthorizationRuleOptions",
+    jsii_struct_bases=[_aws_cdk_aws_ec2_ceddda9d.ClientVpnAuthorizationRuleOptions],
+    name_mapping={
+        "cidr": "cidr",
+        "description": "description",
+        "group_id": "groupId",
+        "scope": "scope",
+    },
+)
+class AddAuthorizationRuleOptions(
+    _aws_cdk_aws_ec2_ceddda9d.ClientVpnAuthorizationRuleOptions,
+):
+    def __init__(
+        self,
+        *,
+        cidr: builtins.str,
+        description: typing.Optional[builtins.str] = None,
+        group_id: typing.Optional[builtins.str] = None,
+        scope: typing.Optional[_constructs_77d1e7e8.IConstruct] = None,
+    ) -> None:
+        '''
+        :param cidr: The IPv4 address range, in CIDR notation, of the network for which access is being authorized.
+        :param description: A brief description of the authorization rule. Default: - no description
+        :param group_id: The ID of the group to grant access to, for example, the Active Directory group or identity provider (IdP) group. Default: - authorize all groups
+        :param scope: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__e37c3a43b0a9a57358c4cc8d1a2409a5aa73ff324c6705b24acdd272253addab)
+            check_type(argname="argument cidr", value=cidr, expected_type=type_hints["cidr"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "cidr": cidr,
+        }
+        if description is not None:
+            self._values["description"] = description
+        if group_id is not None:
+            self._values["group_id"] = group_id
+        if scope is not None:
+            self._values["scope"] = scope
+
+    @builtins.property
+    def cidr(self) -> builtins.str:
+        '''The IPv4 address range, in CIDR notation, of the network for which access is being authorized.'''
+        result = self._values.get("cidr")
+        assert result is not None, "Required property 'cidr' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def description(self) -> typing.Optional[builtins.str]:
+        '''A brief description of the authorization rule.
+
+        :default: - no description
+        '''
+        result = self._values.get("description")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def group_id(self) -> typing.Optional[builtins.str]:
+        '''The ID of the group to grant access to, for example, the Active Directory group or identity provider (IdP) group.
+
+        :default: - authorize all groups
+        '''
+        result = self._values.get("group_id")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def scope(self) -> typing.Optional[_constructs_77d1e7e8.IConstruct]:
+        result = self._values.get("scope")
+        return typing.cast(typing.Optional[_constructs_77d1e7e8.IConstruct], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "AddAuthorizationRuleOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
     jsii_type="cdk-extensions.ec2_patterns.AddCidrBlockOptions",
     jsii_struct_bases=[],
     name_mapping={"cidr_assignment": "cidrAssignment"},
 )
 class AddCidrBlockOptions:
     def __init__(self, *, cidr_assignment: _ICidrAssignment_01d14e24) -> None:
         '''
@@ -3507,15 +3592,15 @@
 
     def __repr__(self) -> str:
         return "NetworkControllerProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-@jsii.implements(_aws_cdk_aws_ec2_ceddda9d.IConnectable)
+@jsii.implements(_aws_cdk_aws_ec2_ceddda9d.IClientVpnEndpoint, _aws_cdk_aws_ec2_ceddda9d.IConnectable)
 class NetworkIsolatedClientVpnEndpoint(
     _aws_cdk_ceddda9d.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-extensions.ec2_patterns.NetworkIsolatedClientVpnEndpoint",
 ):
     def __init__(
         self,
@@ -3607,14 +3692,40 @@
             environment_from_arn=environment_from_arn,
             physical_name=physical_name,
             region=region,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
+    @jsii.member(jsii_name="addAuthorizationRule")
+    def add_authorization_rule(
+        self,
+        id: builtins.str,
+        *,
+        scope: typing.Optional[_constructs_77d1e7e8.IConstruct] = None,
+        cidr: builtins.str,
+        description: typing.Optional[builtins.str] = None,
+        group_id: typing.Optional[builtins.str] = None,
+    ) -> _aws_cdk_aws_ec2_ceddda9d.ClientVpnAuthorizationRule:
+        '''
+        :param id: -
+        :param scope: 
+        :param cidr: The IPv4 address range, in CIDR notation, of the network for which access is being authorized.
+        :param description: A brief description of the authorization rule. Default: - no description
+        :param group_id: The ID of the group to grant access to, for example, the Active Directory group or identity provider (IdP) group. Default: - authorize all groups
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__4e08d9588792454fb78aa3d88587dc399e7a624958bef57ca7a0a2aeb69171b1)
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        options = AddAuthorizationRuleOptions(
+            scope=scope, cidr=cidr, description=description, group_id=group_id
+        )
+
+        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.ClientVpnAuthorizationRule, jsii.invoke(self, "addAuthorizationRule", [id, options]))
+
     @jsii.member(jsii_name="addMultiSubnetRoute")
     def add_multi_subnet_route(
         self,
         id: builtins.str,
         *,
         cidr: builtins.str,
         description: typing.Optional[builtins.str] = None,
@@ -3648,14 +3759,20 @@
     @builtins.property
     @jsii.member(jsii_name="connections")
     def connections(self) -> _aws_cdk_aws_ec2_ceddda9d.Connections:
         '''The network connections associated with this resource.'''
         return typing.cast(_aws_cdk_aws_ec2_ceddda9d.Connections, jsii.get(self, "connections"))
 
     @builtins.property
+    @jsii.member(jsii_name="endpointId")
+    def endpoint_id(self) -> builtins.str:
+        '''The endpoint ID.'''
+        return typing.cast(builtins.str, jsii.get(self, "endpointId"))
+
+    @builtins.property
     @jsii.member(jsii_name="maxAzs")
     def max_azs(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "maxAzs"))
 
     @builtins.property
     @jsii.member(jsii_name="serverCertificate")
     def server_certificate(
@@ -3665,14 +3782,20 @@
 
     @builtins.property
     @jsii.member(jsii_name="subnets")
     def subnets(self) -> typing.List[_aws_cdk_aws_ec2_ceddda9d.ISubnet]:
         return typing.cast(typing.List[_aws_cdk_aws_ec2_ceddda9d.ISubnet], jsii.get(self, "subnets"))
 
     @builtins.property
+    @jsii.member(jsii_name="targetNetworksAssociated")
+    def target_networks_associated(self) -> _constructs_77d1e7e8.IDependable:
+        '''Dependable that can be depended upon to force target networks associations.'''
+        return typing.cast(_constructs_77d1e7e8.IDependable, jsii.get(self, "targetNetworksAssociated"))
+
+    @builtins.property
     @jsii.member(jsii_name="vpc")
     def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
         return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, jsii.get(self, "vpc"))
 
     @builtins.property
     @jsii.member(jsii_name="vpcCidrBlock")
     def vpc_cidr_block(self) -> _VpcCidrBlock_a9d3de4b:
@@ -4364,14 +4487,15 @@
     def __repr__(self) -> str:
         return "AddHubOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
+    "AddAuthorizationRuleOptions",
     "AddCidrBlockOptions",
     "AddClientVpnEndpointOptions",
     "AddHubOptions",
     "AddIsolatedClientVpnEndpointOptions",
     "AddMultiSubnetRouteOptions",
     "AddNetworkOptions",
     "AddPoolOptions",
@@ -4397,14 +4521,24 @@
     "NetworkIsolatedClientVpnEndpointProps",
     "TransitGatewayHubConfiguration",
     "TransitGatewaySpokeConfiguration",
 ]
 
 publication.publish()
 
+def _typecheckingstub__e37c3a43b0a9a57358c4cc8d1a2409a5aa73ff324c6705b24acdd272253addab(
+    *,
+    cidr: builtins.str,
+    description: typing.Optional[builtins.str] = None,
+    group_id: typing.Optional[builtins.str] = None,
+    scope: typing.Optional[_constructs_77d1e7e8.IConstruct] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__cba621fedbedacb26cb265a41cf239ca46b66a4c0109678bbc3f426bda09caaa(
     *,
     cidr_assignment: _ICidrAssignment_01d14e24,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -5013,14 +5147,25 @@
     environment_from_arn: typing.Optional[builtins.str] = None,
     physical_name: typing.Optional[builtins.str] = None,
     region: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__4e08d9588792454fb78aa3d88587dc399e7a624958bef57ca7a0a2aeb69171b1(
+    id: builtins.str,
+    *,
+    scope: typing.Optional[_constructs_77d1e7e8.IConstruct] = None,
+    cidr: builtins.str,
+    description: typing.Optional[builtins.str] = None,
+    group_id: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__474ff1f3d7805ad25fb8ef0d62e9d0b5e3c0c8fa7c0d5a895288ab6abd22e207(
     id: builtins.str,
     *,
     cidr: builtins.str,
     description: typing.Optional[builtins.str] = None,
     scope: typing.Optional[_constructs_77d1e7e8.IConstruct] = None,
 ) -> None:
```

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/eks_patterns/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/eks_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/glue/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/glue_tables/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/glue_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/k8s_aws/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/k8s_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/k8s_fargate/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/k8s_fargate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/kinesis_firehose/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/kinesis_firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/lambda_/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/networkmanager/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/ram/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/ram_resources/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/ram_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/rds/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/route53/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/s3_buckets/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/s3_buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/sso/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/sso/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions/stacks/__init__.py` & `cdk-extensions-0.0.63/src/cdk_extensions/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions.egg-info/PKG-INFO` & `cdk-extensions-0.0.63/src/cdk_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.62
+Version: 0.0.63
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.62/src/cdk_extensions.egg-info/SOURCES.txt` & `cdk-extensions-0.0.63/src/cdk_extensions.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdk_extensions/py.typed
 src/cdk_extensions.egg-info/PKG-INFO
 src/cdk_extensions.egg-info/SOURCES.txt
 src/cdk_extensions.egg-info/dependency_links.txt
 src/cdk_extensions.egg-info/requires.txt
 src/cdk_extensions.egg-info/top_level.txt
 src/cdk_extensions/_jsii/__init__.py
-src/cdk_extensions/_jsii/cdk-extensions@0.0.62.jsii.tgz
+src/cdk_extensions/_jsii/cdk-extensions@0.0.63.jsii.tgz
 src/cdk_extensions/_jsii/bin/init-aws.sh
 src/cdk_extensions/aps/__init__.py
 src/cdk_extensions/asserts/__init__.py
 src/cdk_extensions/athena/__init__.py
 src/cdk_extensions/core/__init__.py
 src/cdk_extensions/ec2/__init__.py
 src/cdk_extensions/ec2_patterns/__init__.py
```

