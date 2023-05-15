# Comparing `tmp/trex-model-1.0.1.tar.gz` & `tmp/trex-model-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-model-1.0.1.tar", last modified: Fri Apr 28 10:31:17 2023, max compression
+gzip compressed data, was "trex-model-1.0.2.tar", last modified: Mon May 15 02:07:42 2023, max compression
```

## Comparing `trex-model-1.0.1.tar` & `trex-model-1.0.2.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.177978 trex-model-1.0.1/
--rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.0.1/LICENSE
--rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.0.1/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-04-28 10:31:17.178389 trex-model-1.0.1/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.0.1/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-04-28 10:31:17.179287 trex-model-1.0.1/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      922 2023-04-28 10:15:33.000000 trex-model-1.0.1/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.137434 trex-model-1.0.1/trex_model.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-04-28 10:31:16.000000 trex-model-1.0.1/trex_model.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1799 2023-04-28 10:31:16.000000 trex-model-1.0.1/trex_model.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-04-28 10:31:16.000000 trex-model-1.0.1/trex_model.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       95 2023-04-28 10:31:16.000000 trex-model-1.0.1/trex_model.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       16 2023-04-28 10:31:16.000000 trex-model-1.0.1/trex_model.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.140045 trex-model-1.0.1/trexmodel/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.0.1/trexmodel/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1122 2021-09-03 09:11:14.000000 trex-model-1.0.1/trexmodel/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.143298 trex-model-1.0.1/trexmodel/models/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.0.1/trexmodel/models/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.173728 trex-model-1.0.1/trexmodel/models/datastore/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.0.1/trexmodel/models/datastore/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-1.0.1/trexmodel/models/datastore/admin_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3223 2023-04-11 07:48:46.000000 trex-model-1.0.1/trexmodel/models/datastore/analytic_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-1.0.1/trexmodel/models/datastore/coporate_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13539 2023-03-15 08:15:01.000000 trex-model-1.0.1/trexmodel/models/datastore/customer_model_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    47628 2023-04-13 05:33:49.000000 trex-model-1.0.1/trexmodel/models/datastore/customer_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1712 2020-10-26 01:02:17.000000 trex-model-1.0.1/trexmodel/models/datastore/fb_subsriber_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-1.0.1/trexmodel/models/datastore/inventory_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5816 2023-03-02 14:42:44.000000 trex-model-1.0.1/trexmodel/models/datastore/loyalty_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11281 2023-04-05 03:48:05.000000 trex-model-1.0.1/trexmodel/models/datastore/membership_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    57199 2023-04-25 06:49:40.000000 trex-model-1.0.1/trexmodel/models/datastore/merchant_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.0.1/trexmodel/models/datastore/model_decorators.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17711 2023-02-10 02:53:30.000000 trex-model-1.0.1/trexmodel/models/datastore/ndb_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    32092 2023-01-04 03:56:36.000000 trex-model-1.0.1/trexmodel/models/datastore/pos_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    20750 2023-04-10 08:59:10.000000 trex-model-1.0.1/trexmodel/models/datastore/prepaid_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    38941 2023-02-28 05:40:30.000000 trex-model-1.0.1/trexmodel/models/datastore/product_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    47521 2023-03-15 14:31:35.000000 trex-model-1.0.1/trexmodel/models/datastore/program_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    36350 2023-04-13 13:46:37.000000 trex-model-1.0.1/trexmodel/models/datastore/redeem_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    31165 2023-04-10 09:19:08.000000 trex-model-1.0.1/trexmodel/models/datastore/reward_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.0.1/trexmodel/models/datastore/spending_base_program_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6610 2021-03-30 06:42:06.000000 trex-model-1.0.1/trexmodel/models/datastore/system_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-1.0.1/trexmodel/models/datastore/task_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-1.0.1/trexmodel/models/datastore/test_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    36809 2023-04-24 09:59:51.000000 trex-model-1.0.1/trexmodel/models/datastore/transaction_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15228 2022-09-23 07:10:51.000000 trex-model-1.0.1/trexmodel/models/datastore/user_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17441 2022-12-29 13:44:05.000000 trex-model-1.0.1/trexmodel/models/datastore/voucher_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6452 2023-03-19 11:12:11.000000 trex-model-1.0.1/trexmodel/models/merchant_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.0.1/trexmodel/models/model_decorator.py
--rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.0.1/trexmodel/models/prepaid_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.0.1/trexmodel/pos_conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16572 2023-04-07 03:52:51.000000 trex-model-1.0.1/trexmodel/program_conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.175242 trex-model-1.0.1/trexmodel/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.1/trexmodel/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.175877 trex-model-1.0.1/trexmodel/utils/gcloud/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.1/trexmodel/utils/gcloud/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.0.1/trexmodel/utils/gcloud/datastore_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.177110 trex-model-1.0.1/trexmodel/utils/model/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.1/trexmodel/utils/model/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-1.0.1/trexmodel/utils/model/model_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.475790 trex-model-1.0.2/
+-rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.0.2/LICENSE
+-rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.0.2/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-05-15 02:07:42.476014 trex-model-1.0.2/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.0.2/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-05-15 02:07:42.476994 trex-model-1.0.2/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      922 2023-05-15 02:07:17.000000 trex-model-1.0.2/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.442059 trex-model-1.0.2/trex_model.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-05-15 02:07:42.000000 trex-model-1.0.2/trex_model.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1847 2023-05-15 02:07:42.000000 trex-model-1.0.2/trex_model.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-05-15 02:07:42.000000 trex-model-1.0.2/trex_model.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       95 2023-05-15 02:07:42.000000 trex-model-1.0.2/trex_model.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       16 2023-05-15 02:07:42.000000 trex-model-1.0.2/trex_model.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.443521 trex-model-1.0.2/trexmodel/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.0.2/trexmodel/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1122 2021-09-03 09:11:14.000000 trex-model-1.0.2/trexmodel/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.446853 trex-model-1.0.2/trexmodel/models/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.0.2/trexmodel/models/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.471429 trex-model-1.0.2/trexmodel/models/datastore/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.0.2/trexmodel/models/datastore/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-1.0.2/trexmodel/models/datastore/admin_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3223 2023-04-11 07:48:46.000000 trex-model-1.0.2/trexmodel/models/datastore/analytic_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-1.0.2/trexmodel/models/datastore/coporate_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13539 2023-03-15 08:15:01.000000 trex-model-1.0.2/trexmodel/models/datastore/customer_model_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    48341 2023-05-12 06:20:00.000000 trex-model-1.0.2/trexmodel/models/datastore/customer_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1712 2020-10-26 01:02:17.000000 trex-model-1.0.2/trexmodel/models/datastore/fb_subsriber_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-1.0.2/trexmodel/models/datastore/inventory_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5974 2023-05-15 01:59:38.000000 trex-model-1.0.2/trexmodel/models/datastore/loyalty_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3663 2023-05-12 08:12:47.000000 trex-model-1.0.2/trexmodel/models/datastore/lucky_draw_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11281 2023-04-05 03:48:05.000000 trex-model-1.0.2/trexmodel/models/datastore/membership_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    57199 2023-04-25 06:49:40.000000 trex-model-1.0.2/trexmodel/models/datastore/merchant_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.0.2/trexmodel/models/datastore/model_decorators.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17711 2023-02-10 02:53:30.000000 trex-model-1.0.2/trexmodel/models/datastore/ndb_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    32251 2023-05-15 02:04:46.000000 trex-model-1.0.2/trexmodel/models/datastore/pos_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    20750 2023-04-10 08:59:10.000000 trex-model-1.0.2/trexmodel/models/datastore/prepaid_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    38941 2023-02-28 05:40:30.000000 trex-model-1.0.2/trexmodel/models/datastore/product_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    47521 2023-03-15 14:31:35.000000 trex-model-1.0.2/trexmodel/models/datastore/program_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    36350 2023-04-13 13:46:37.000000 trex-model-1.0.2/trexmodel/models/datastore/redeem_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    31165 2023-04-10 09:19:08.000000 trex-model-1.0.2/trexmodel/models/datastore/reward_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.0.2/trexmodel/models/datastore/spending_base_program_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6610 2021-03-30 06:42:06.000000 trex-model-1.0.2/trexmodel/models/datastore/system_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-1.0.2/trexmodel/models/datastore/task_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-1.0.2/trexmodel/models/datastore/test_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    36809 2023-04-24 09:59:51.000000 trex-model-1.0.2/trexmodel/models/datastore/transaction_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15228 2022-09-23 07:10:51.000000 trex-model-1.0.2/trexmodel/models/datastore/user_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17441 2022-12-29 13:44:05.000000 trex-model-1.0.2/trexmodel/models/datastore/voucher_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6452 2023-03-19 11:12:11.000000 trex-model-1.0.2/trexmodel/models/merchant_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.0.2/trexmodel/models/model_decorator.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.0.2/trexmodel/models/prepaid_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.0.2/trexmodel/pos_conf.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16572 2023-04-07 03:52:51.000000 trex-model-1.0.2/trexmodel/program_conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.473093 trex-model-1.0.2/trexmodel/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.2/trexmodel/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.473780 trex-model-1.0.2/trexmodel/utils/gcloud/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.2/trexmodel/utils/gcloud/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.0.2/trexmodel/utils/gcloud/datastore_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.474926 trex-model-1.0.2/trexmodel/utils/model/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.2/trexmodel/utils/model/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-1.0.2/trexmodel/utils/model/model_util.py
```

### Comparing `trex-model-1.0.1/LICENSE` & `trex-model-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/setup.py` & `trex-model-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      name='trex-model',  
-     version='1.0.1',
+     version='1.0.2',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex database module package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-model",
      packages=setuptools.find_packages(),
```

### Comparing `trex-model-1.0.1/trex_model.egg-info/SOURCES.txt` & `trex-model-1.0.2/trex_model.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 trexmodel/models/datastore/analytic_models.py
 trexmodel/models/datastore/coporate_models.py
 trexmodel/models/datastore/customer_model_helpers.py
 trexmodel/models/datastore/customer_models.py
 trexmodel/models/datastore/fb_subsriber_models.py
 trexmodel/models/datastore/inventory_model.py
 trexmodel/models/datastore/loyalty_models.py
+trexmodel/models/datastore/lucky_draw_models.py
 trexmodel/models/datastore/membership_models.py
 trexmodel/models/datastore/merchant_models.py
 trexmodel/models/datastore/model_decorators.py
 trexmodel/models/datastore/ndb_models.py
 trexmodel/models/datastore/pos_models.py
 trexmodel/models/datastore/prepaid_models.py
 trexmodel/models/datastore/product_models.py
```

### Comparing `trex-model-1.0.1/trexmodel/conf.py` & `trex-model-1.0.2/trexmodel/conf.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/admin_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/admin_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/analytic_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/analytic_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/coporate_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/coporate_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/customer_model_helpers.py` & `trex-model-1.0.2/trexmodel/models/datastore/customer_model_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/customer_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/customer_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,20 +164,27 @@
         return cls.query(ndb.AND(cls.reference_code==reference_code, cls.merchant_acct==merchant_acct.create_ndb_key())).get()
     
     @classmethod
     def get_by_merchant_reference_code(cls, merchant_reference_code, merchant_acct):
         return cls.query(ndb.AND(cls.merchant_reference_code==merchant_reference_code, cls.merchant_acct==merchant_acct.create_ndb_key())).get()
     
     @classmethod
-    def get_by_email(cls, email):
-        return cls.query(cls.email==email).get()
+    def get_by_email(cls, email, merchant_acct=None):
+        if merchant_acct:
+            return cls.query(ndb.AND(cls.email==email, cls.merchant_acct==merchant_acct.create_ndb_key())).get()
+        else:
+            return cls.query(cls.email==email).get()
     
     @classmethod
-    def get_by_mobile_phone(cls, mobile_phone):
-        return cls.query(cls.mobile_phone==mobile_phone).get()
+    def get_by_mobile_phone(cls, mobile_phone, merchant_acct=None):
+        
+        if merchant_acct:
+            return cls.query(ndb.AND(cls.mobile_phone==mobile_phone, cls.merchant_acct==merchant_acct.create_ndb_key())).get()
+        else:
+            return cls.query(cls.mobile_phone==mobile_phone).get()
     
     @classmethod
     def create(cls, outlet=None, name=None, email=None, mobile_phone=None, merchant_reference_code=None, gender=None, birth_date=None,
                password=None):
         
         created_user = User.create(name=name, email=email, mobile_phone=mobile_phone, gender=gender, birth_date=birth_date, 
                            password=password)
@@ -276,14 +283,20 @@
         return cls.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
     
     @classmethod
     def list_by_user_account(cls, user_acct):
         return cls.query(ancestor=user_acct.create_ndb_key()).fetch(limit=conf.MAX_FETCH_RECORD)
     
     @classmethod
+    def list_paginated_by_user_account(cls, user_acct, limit=conf.MAX_FETCH_RECORD, start_cursor=None):
+        query = cls.query(ancestor=user_acct.create_ndb_key())
+        
+        return cls.list_all_with_condition_query(query, limit=limit, start_cursor=start_cursor, return_with_cursor=True, keys_only=False)
+    
+    @classmethod
     def count_merchant_customer(cls, merchant_acct):
         if merchant_acct:
             query = cls.query(ndb.AND(cls.merchant_acct==merchant_acct.create_ndb_key()))
         else:
             query = cls.query()
         
         return cls.count_with_condition_query(query)
```

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/fb_subsriber_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/fb_subsriber_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/inventory_model.py` & `trex-model-1.0.2/trexmodel/models/datastore/inventory_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/loyalty_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/loyalty_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,23 @@
     device_name             = ndb.StringProperty(required=True)
     activation_code         = ndb.StringProperty(required=True)
     device_id               = ndb.StringProperty(required=False)
     activated               = ndb.BooleanProperty(required=True, default=False)
     assigned_outlet         = ndb.KeyProperty(name="assigned_outlet", kind=Outlet)
     created_datetime        = ndb.DateTimeProperty(required=True, auto_now_add=True)
     activated_datetime      = ndb.DateTimeProperty(required=False)
+    testing                 = ndb.BooleanProperty(required=False, default=False)
     
     dict_properties = ['device_name', 'activation_code', 'device_id', 'activated', 'assigned_outlet_key', 'activated_datetime', 'created_datetime']
     
     @property
+    def is_test_setting(self):
+        return self.testing
+    
+    @property
     def assigned_outlet_key(self):
         return self.assigned_outlet.urlsafe().decode('utf-8')
     
     @property
     def assigned_outlet_entity(self):
         return Outlet.fetch(self.assigned_outlet_key)
     
@@ -114,15 +119,15 @@
                         LoyaltyDeviceSetting.assigned_outlet==assigned_outlet.create_ndb_key()
                         ),ancestor=merchant_acct.create_ndb_key())
         
         return LoyaltyDeviceSetting.count_with_condition_query(query)
         
     def activate(self, device_id):
         self.device_id          = device_id
-        #self.activated          = True
+        self.activated          = True
         self.activated_datetime = datetime.utcnow()
         self.put()
         
         
     @staticmethod
     def remove_by_activation_code(activation_code):
         checking_device_setting = LoyaltyDeviceSetting.get_by_activation_code(activation_code)
```

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/membership_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/membership_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/merchant_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/merchant_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/model_decorators.py` & `trex-model-1.0.2/trexmodel/models/datastore/model_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/ndb_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/ndb_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/pos_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/pos_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,18 +23,23 @@
     activation_code         = ndb.StringProperty(required=True)
     device_id               = ndb.StringProperty(required=False)
     activated               = ndb.BooleanProperty(required=True, default=False)
     assigned_outlet         = ndb.KeyProperty(name="assigned_outlet", kind=Outlet)
     #assigned_catalogue      = ndb.KeyProperty(name="assigned_outlet", kind=ProductCatalogue)
     created_datetime        = ndb.DateTimeProperty(required=True, auto_now_add=True)
     activated_datetime      = ndb.DateTimeProperty(required=False)
+    testing                 = ndb.BooleanProperty(required=False, default=False)
     
     dict_properties = ['device_name', 'activation_code', 'device_id', 'activated', 'assigned_outlet_key', 'activated_datetime', 'created_datetime']
     
     @property
+    def is_test_setting(self):
+        return self.testing
+    
+    @property
     def assigned_outlet_key(self):
         return self.assigned_outlet.urlsafe().decode('utf-8')
     
     @property
     def assigned_outlet_entity(self):
         return Outlet.fetch(self.assigned_outlet_key)
```

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/prepaid_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/prepaid_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/product_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/product_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/program_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/program_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/redeem_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/redeem_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/reward_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/reward_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/spending_base_program_model.py` & `trex-model-1.0.2/trexmodel/models/datastore/spending_base_program_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/system_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/system_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/task_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/task_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/test_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/test_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/transaction_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/transaction_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/user_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/user_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/datastore/voucher_models.py` & `trex-model-1.0.2/trexmodel/models/datastore/voucher_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/models/merchant_helpers.py` & `trex-model-1.0.2/trexmodel/models/merchant_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/program_conf.py` & `trex-model-1.0.2/trexmodel/program_conf.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.1/trexmodel/utils/model/model_util.py` & `trex-model-1.0.2/trexmodel/utils/model/model_util.py`

 * *Files identical despite different names*

