# Comparing `tmp/cdk-extensions-0.0.64.tar.gz` & `tmp/cdk-extensions-0.0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-extensions-0.0.64.tar", last modified: Mon May 15 19:14:01 2023, max compression
+gzip compressed data, was "cdk-extensions-0.0.65.tar", last modified: Mon May 15 20:47:34 2023, max compression
```

## Comparing `cdk-extensions-0.0.64.tar` & `cdk-extensions-0.0.65.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.912341 cdk-extensions-0.0.64/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.916341 cdk-extensions-0.0.64/src/cdk_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.916341 cdk-extensions-0.0.64/src/cdk_extensions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.916341 cdk-extensions-0.0.64/src/cdk_extensions/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/_jsii/bin/init-aws.sh
--rw-r--r--   0 runner    (1001) docker     (123)  1595030 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/_jsii/cdk-extensions@0.0.64.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.916341 cdk-extensions-0.0.64/src/cdk_extensions/aps/
--rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/aps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/asserts/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/asserts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/athena/
--rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/athena/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)   702552 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/ec2_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)   267981 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/ec2_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/eks_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/eks_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/glue/
--rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/glue_tables/
--rw-r--r--   0 runner    (1001) docker     (123)   140852 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/glue_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.920341 cdk-extensions-0.0.64/src/cdk_extensions/k8s_aws/
--rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/k8s_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/k8s_fargate/
--rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/k8s_fargate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/kinesis_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/kinesis_firehose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/lambda_/
--rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/lambda_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/networkmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/ram/
--rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/ram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/ram_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/ram_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/rds/
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/rds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/route53/
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)   215302 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/s3_buckets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/sso/
--rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/sso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.924341 cdk-extensions-0.0.64/src/cdk_extensions/stacks/
--rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-05-15 19:13:50.000000 cdk-extensions-0.0.64/src/cdk_extensions/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:14:01.916341 cdk-extensions-0.0.64/src/cdk_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-15 19:14:01.000000 cdk-extensions-0.0.64/src/cdk_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-15 19:14:01.000000 cdk-extensions-0.0.64/src/cdk_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:14:01.000000 cdk-extensions-0.0.64/src/cdk_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-15 19:14:01.000000 cdk-extensions-0.0.64/src/cdk_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 19:14:01.000000 cdk-extensions-0.0.64/src/cdk_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.921141 cdk-extensions-0.0.65/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-15 20:47:34.921141 cdk-extensions-0.0.65/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:47:34.921141 cdk-extensions-0.0.65/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.909141 cdk-extensions-0.0.65/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.913141 cdk-extensions-0.0.65/src/cdk_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.913141 cdk-extensions-0.0.65/src/cdk_extensions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.913141 cdk-extensions-0.0.65/src/cdk_extensions/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/_jsii/bin/init-aws.sh
+-rw-r--r--   0 runner    (1001) docker     (123)  1596255 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/_jsii/cdk-extensions@0.0.65.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.913141 cdk-extensions-0.0.65/src/cdk_extensions/aps/
+-rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/aps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.917141 cdk-extensions-0.0.65/src/cdk_extensions/asserts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/asserts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.917141 cdk-extensions-0.0.65/src/cdk_extensions/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/athena/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.917141 cdk-extensions-0.0.65/src/cdk_extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.917141 cdk-extensions-0.0.65/src/cdk_extensions/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)   702552 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.917141 cdk-extensions-0.0.65/src/cdk_extensions/ec2_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)   278802 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/ec2_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.917141 cdk-extensions-0.0.65/src/cdk_extensions/eks_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/eks_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.917141 cdk-extensions-0.0.65/src/cdk_extensions/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.917141 cdk-extensions-0.0.65/src/cdk_extensions/glue_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)   140852 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/glue_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.917141 cdk-extensions-0.0.65/src/cdk_extensions/k8s_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/k8s_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.917141 cdk-extensions-0.0.65/src/cdk_extensions/k8s_fargate/
+-rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/k8s_fargate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.921141 cdk-extensions-0.0.65/src/cdk_extensions/kinesis_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/kinesis_firehose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.921141 cdk-extensions-0.0.65/src/cdk_extensions/lambda_/
+-rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/lambda_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.921141 cdk-extensions-0.0.65/src/cdk_extensions/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/networkmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.921141 cdk-extensions-0.0.65/src/cdk_extensions/ram/
+-rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/ram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.921141 cdk-extensions-0.0.65/src/cdk_extensions/ram_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/ram_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.921141 cdk-extensions-0.0.65/src/cdk_extensions/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/rds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.921141 cdk-extensions-0.0.65/src/cdk_extensions/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.921141 cdk-extensions-0.0.65/src/cdk_extensions/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)   215302 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/s3_buckets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.921141 cdk-extensions-0.0.65/src/cdk_extensions/sso/
+-rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/sso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.921141 cdk-extensions-0.0.65/src/cdk_extensions/stacks/
+-rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-05-15 20:47:23.000000 cdk-extensions-0.0.65/src/cdk_extensions/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:34.913141 cdk-extensions-0.0.65/src/cdk_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-15 20:47:34.000000 cdk-extensions-0.0.65/src/cdk_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-15 20:47:34.000000 cdk-extensions-0.0.65/src/cdk_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:47:34.000000 cdk-extensions-0.0.65/src/cdk_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-15 20:47:34.000000 cdk-extensions-0.0.65/src/cdk_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 20:47:34.000000 cdk-extensions-0.0.65/src/cdk_extensions.egg-info/top_level.txt
```

### Comparing `cdk-extensions-0.0.64/LICENSE` & `cdk-extensions-0.0.65/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/PKG-INFO` & `cdk-extensions-0.0.65/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.64
+Version: 0.0.65
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.64/README.md` & `cdk-extensions-0.0.65/README.md`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/setup.py` & `cdk-extensions-0.0.65/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-extensions",
-    "version": "0.0.64",
+    "version": "0.0.65",
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
-            "cdk-extensions@0.0.64.jsii.tgz"
+            "cdk-extensions@0.0.65.jsii.tgz"
         ],
         "cdk_extensions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/aps/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/asserts/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/asserts/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/athena/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/core/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/ec2/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/ec2_patterns/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/ec2_patterns/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1475,14 +1475,85 @@
             environment_from_arn=environment_from_arn,
             physical_name=physical_name,
             region=region,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
+    @jsii.member(jsii_name="addIsolatedClientVpnEndpoint")
+    def add_isolated_client_vpn_endpoint(
+        self,
+        id: builtins.str,
+        *,
+        server_certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
+        authorize_all_users_to_vpc_cidr: typing.Optional[builtins.bool] = None,
+        client_certificate: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
+        client_connection_handler: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IClientVpnConnectionHandler] = None,
+        client_login_banner: typing.Optional[builtins.str] = None,
+        description: typing.Optional[builtins.str] = None,
+        dns_servers: typing.Optional[typing.Sequence[builtins.str]] = None,
+        logging: typing.Optional[builtins.bool] = None,
+        log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
+        log_stream: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogStream] = None,
+        max_azs: typing.Optional[jsii.Number] = None,
+        port: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.VpnPort] = None,
+        self_service_portal: typing.Optional[builtins.bool] = None,
+        split_tunnel: typing.Optional[builtins.bool] = None,
+        subnet_cidr: typing.Optional[_IIpv4CidrAssignment_b412e3a5] = None,
+        transport_protocol: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.TransportProtocol] = None,
+        user_based_authentication: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ClientVpnUserBasedAuthentication] = None,
+        vpn_cidr: typing.Optional[_IIpv4CidrAssignment_b412e3a5] = None,
+    ) -> "NetworkIsolatedClientVpnEndpoint":
+        '''
+        :param id: -
+        :param server_certificate: 
+        :param authorize_all_users_to_vpc_cidr: 
+        :param client_certificate: 
+        :param client_connection_handler: 
+        :param client_login_banner: 
+        :param description: 
+        :param dns_servers: 
+        :param logging: 
+        :param log_group: 
+        :param log_stream: 
+        :param max_azs: 
+        :param port: 
+        :param self_service_portal: 
+        :param split_tunnel: 
+        :param subnet_cidr: 
+        :param transport_protocol: 
+        :param user_based_authentication: 
+        :param vpn_cidr: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__6c49ca1a51873108507dce275532ebffebdbd243a871747933a28ae18720a36d)
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        options = AddIsolatedClientVpnEndpointOptions(
+            server_certificate=server_certificate,
+            authorize_all_users_to_vpc_cidr=authorize_all_users_to_vpc_cidr,
+            client_certificate=client_certificate,
+            client_connection_handler=client_connection_handler,
+            client_login_banner=client_login_banner,
+            description=description,
+            dns_servers=dns_servers,
+            logging=logging,
+            log_group=log_group,
+            log_stream=log_stream,
+            max_azs=max_azs,
+            port=port,
+            self_service_portal=self_service_portal,
+            split_tunnel=split_tunnel,
+            subnet_cidr=subnet_cidr,
+            transport_protocol=transport_protocol,
+            user_based_authentication=user_based_authentication,
+            vpn_cidr=vpn_cidr,
+        )
+
+        return typing.cast("NetworkIsolatedClientVpnEndpoint", jsii.invoke(self, "addIsolatedClientVpnEndpoint", [id, options]))
+
     @jsii.member(jsii_name="addSpoke")
     def add_spoke(
         self,
         scope: _constructs_77d1e7e8.IConstruct,
         id: builtins.str,
         *,
         availability_zones: typing.Optional[typing.Sequence[builtins.str]] = None,
@@ -2304,14 +2375,85 @@
             environment_from_arn=environment_from_arn,
             physical_name=physical_name,
             region=region,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
+    @jsii.member(jsii_name="addIsolatedClientVpnEndpoint")
+    def add_isolated_client_vpn_endpoint(
+        self,
+        id: builtins.str,
+        *,
+        server_certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
+        authorize_all_users_to_vpc_cidr: typing.Optional[builtins.bool] = None,
+        client_certificate: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
+        client_connection_handler: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IClientVpnConnectionHandler] = None,
+        client_login_banner: typing.Optional[builtins.str] = None,
+        description: typing.Optional[builtins.str] = None,
+        dns_servers: typing.Optional[typing.Sequence[builtins.str]] = None,
+        logging: typing.Optional[builtins.bool] = None,
+        log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
+        log_stream: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogStream] = None,
+        max_azs: typing.Optional[jsii.Number] = None,
+        port: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.VpnPort] = None,
+        self_service_portal: typing.Optional[builtins.bool] = None,
+        split_tunnel: typing.Optional[builtins.bool] = None,
+        subnet_cidr: typing.Optional[_IIpv4CidrAssignment_b412e3a5] = None,
+        transport_protocol: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.TransportProtocol] = None,
+        user_based_authentication: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ClientVpnUserBasedAuthentication] = None,
+        vpn_cidr: typing.Optional[_IIpv4CidrAssignment_b412e3a5] = None,
+    ) -> "NetworkIsolatedClientVpnEndpoint":
+        '''
+        :param id: -
+        :param server_certificate: 
+        :param authorize_all_users_to_vpc_cidr: 
+        :param client_certificate: 
+        :param client_connection_handler: 
+        :param client_login_banner: 
+        :param description: 
+        :param dns_servers: 
+        :param logging: 
+        :param log_group: 
+        :param log_stream: 
+        :param max_azs: 
+        :param port: 
+        :param self_service_portal: 
+        :param split_tunnel: 
+        :param subnet_cidr: 
+        :param transport_protocol: 
+        :param user_based_authentication: 
+        :param vpn_cidr: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__6b76c9a1e301e4dda738f73bbb659640ffa1096698102a7f1973cf19efc0449b)
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        options = AddIsolatedClientVpnEndpointOptions(
+            server_certificate=server_certificate,
+            authorize_all_users_to_vpc_cidr=authorize_all_users_to_vpc_cidr,
+            client_certificate=client_certificate,
+            client_connection_handler=client_connection_handler,
+            client_login_banner=client_login_banner,
+            description=description,
+            dns_servers=dns_servers,
+            logging=logging,
+            log_group=log_group,
+            log_stream=log_stream,
+            max_azs=max_azs,
+            port=port,
+            self_service_portal=self_service_portal,
+            split_tunnel=split_tunnel,
+            subnet_cidr=subnet_cidr,
+            transport_protocol=transport_protocol,
+            user_based_authentication=user_based_authentication,
+            vpn_cidr=vpn_cidr,
+        )
+
+        return typing.cast("NetworkIsolatedClientVpnEndpoint", jsii.invoke(self, "addIsolatedClientVpnEndpoint", [id, options]))
+
     @builtins.property
     @jsii.member(jsii_name="transitGateway")
     def transit_gateway(self) -> _ITransitGateway_25936657:
         return typing.cast(_ITransitGateway_25936657, jsii.get(self, "transitGateway"))
 
     @builtins.property
     @jsii.member(jsii_name="transitGatewayAttachment")
@@ -3742,14 +3884,27 @@
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         options = AddMultiSubnetRouteOptions(
             cidr=cidr, description=description, scope=scope
         )
 
         return typing.cast(typing.Any, jsii.invoke(self, "addMultiSubnetRoute", [id, options]))
 
+    @jsii.member(jsii_name="registerTransitGateway")
+    def register_transit_gateway(
+        self,
+        transit_gateway: _ITransitGateway_25936657,
+    ) -> None:
+        '''
+        :param transit_gateway: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a636729a85f9b24e667b45fba5e6a71cfcc20ba93b2dac0fc735157a06072ebf)
+            check_type(argname="argument transit_gateway", value=transit_gateway, expected_type=type_hints["transit_gateway"])
+        return typing.cast(None, jsii.invoke(self, "registerTransitGateway", [transit_gateway]))
+
     @jsii.python.classproperty
     @jsii.member(jsii_name="DEFAULT_VPN_CIDR")
     def DEFAULT_VPN_CIDR(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "DEFAULT_VPN_CIDR"))
 
     @builtins.property
     @jsii.member(jsii_name="clientVpnEndpoint")
@@ -4750,14 +4905,39 @@
     environment_from_arn: typing.Optional[builtins.str] = None,
     physical_name: typing.Optional[builtins.str] = None,
     region: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__6c49ca1a51873108507dce275532ebffebdbd243a871747933a28ae18720a36d(
+    id: builtins.str,
+    *,
+    server_certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
+    authorize_all_users_to_vpc_cidr: typing.Optional[builtins.bool] = None,
+    client_certificate: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
+    client_connection_handler: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IClientVpnConnectionHandler] = None,
+    client_login_banner: typing.Optional[builtins.str] = None,
+    description: typing.Optional[builtins.str] = None,
+    dns_servers: typing.Optional[typing.Sequence[builtins.str]] = None,
+    logging: typing.Optional[builtins.bool] = None,
+    log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
+    log_stream: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogStream] = None,
+    max_azs: typing.Optional[jsii.Number] = None,
+    port: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.VpnPort] = None,
+    self_service_portal: typing.Optional[builtins.bool] = None,
+    split_tunnel: typing.Optional[builtins.bool] = None,
+    subnet_cidr: typing.Optional[_IIpv4CidrAssignment_b412e3a5] = None,
+    transport_protocol: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.TransportProtocol] = None,
+    user_based_authentication: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ClientVpnUserBasedAuthentication] = None,
+    vpn_cidr: typing.Optional[_IIpv4CidrAssignment_b412e3a5] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__b427eb756711b9be0d1724b92283f7b8b658149d02d0860ddfaae4ca009451a6(
     scope: _constructs_77d1e7e8.IConstruct,
     id: builtins.str,
     *,
     availability_zones: typing.Optional[typing.Sequence[builtins.str]] = None,
     cidr: typing.Optional[_IIpv4CidrAssignment_b412e3a5] = None,
     default_instance_tenancy: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.DefaultInstanceTenancy] = None,
@@ -4859,14 +5039,39 @@
     environment_from_arn: typing.Optional[builtins.str] = None,
     physical_name: typing.Optional[builtins.str] = None,
     region: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__6b76c9a1e301e4dda738f73bbb659640ffa1096698102a7f1973cf19efc0449b(
+    id: builtins.str,
+    *,
+    server_certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
+    authorize_all_users_to_vpc_cidr: typing.Optional[builtins.bool] = None,
+    client_certificate: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
+    client_connection_handler: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IClientVpnConnectionHandler] = None,
+    client_login_banner: typing.Optional[builtins.str] = None,
+    description: typing.Optional[builtins.str] = None,
+    dns_servers: typing.Optional[typing.Sequence[builtins.str]] = None,
+    logging: typing.Optional[builtins.bool] = None,
+    log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
+    log_stream: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogStream] = None,
+    max_azs: typing.Optional[jsii.Number] = None,
+    port: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.VpnPort] = None,
+    self_service_portal: typing.Optional[builtins.bool] = None,
+    split_tunnel: typing.Optional[builtins.bool] = None,
+    subnet_cidr: typing.Optional[_IIpv4CidrAssignment_b412e3a5] = None,
+    transport_protocol: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.TransportProtocol] = None,
+    user_based_authentication: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ClientVpnUserBasedAuthentication] = None,
+    vpn_cidr: typing.Optional[_IIpv4CidrAssignment_b412e3a5] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__0f20b71c01dce683a9711971685bfd423a84bb51b3ae70144ed170d14b6b7721(
     *,
     account: typing.Optional[builtins.str] = None,
     environment_from_arn: typing.Optional[builtins.str] = None,
     physical_name: typing.Optional[builtins.str] = None,
     region: typing.Optional[builtins.str] = None,
     hub: FourTierNetworkHub,
@@ -5168,14 +5373,20 @@
     cidr: builtins.str,
     description: typing.Optional[builtins.str] = None,
     scope: typing.Optional[_constructs_77d1e7e8.IConstruct] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__a636729a85f9b24e667b45fba5e6a71cfcc20ba93b2dac0fc735157a06072ebf(
+    transit_gateway: _ITransitGateway_25936657,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__3802025d1d451c01388cfc739e97c163e6f87b2af20266ee60e0b8b5f0be1607(
     *,
     account: typing.Optional[builtins.str] = None,
     environment_from_arn: typing.Optional[builtins.str] = None,
     physical_name: typing.Optional[builtins.str] = None,
     region: typing.Optional[builtins.str] = None,
     server_certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
```

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/eks_patterns/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/eks_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/glue/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/glue_tables/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/glue_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/k8s_aws/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/k8s_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/k8s_fargate/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/k8s_fargate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/kinesis_firehose/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/kinesis_firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/lambda_/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/networkmanager/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/ram/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/ram_resources/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/ram_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/rds/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/route53/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/s3_buckets/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/s3_buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/sso/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/sso/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions/stacks/__init__.py` & `cdk-extensions-0.0.65/src/cdk_extensions/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions.egg-info/PKG-INFO` & `cdk-extensions-0.0.65/src/cdk_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.64
+Version: 0.0.65
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.64/src/cdk_extensions.egg-info/SOURCES.txt` & `cdk-extensions-0.0.65/src/cdk_extensions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdk_extensions/py.typed
 src/cdk_extensions.egg-info/PKG-INFO
 src/cdk_extensions.egg-info/SOURCES.txt
 src/cdk_extensions.egg-info/dependency_links.txt
 src/cdk_extensions.egg-info/requires.txt
 src/cdk_extensions.egg-info/top_level.txt
 src/cdk_extensions/_jsii/__init__.py
-src/cdk_extensions/_jsii/cdk-extensions@0.0.64.jsii.tgz
+src/cdk_extensions/_jsii/cdk-extensions@0.0.65.jsii.tgz
 src/cdk_extensions/_jsii/bin/init-aws.sh
 src/cdk_extensions/aps/__init__.py
 src/cdk_extensions/asserts/__init__.py
 src/cdk_extensions/athena/__init__.py
 src/cdk_extensions/core/__init__.py
 src/cdk_extensions/ec2/__init__.py
 src/cdk_extensions/ec2_patterns/__init__.py
```

