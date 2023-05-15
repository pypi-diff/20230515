# Comparing `tmp/trex-model-1.0.2.tar.gz` & `tmp/trex-model-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-model-1.0.2.tar", last modified: Mon May 15 02:07:42 2023, max compression
+gzip compressed data, was "trex-model-1.0.3.tar", last modified: Mon May 15 06:05:38 2023, max compression
```

## Comparing `trex-model-1.0.2.tar` & `trex-model-1.0.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.475790 trex-model-1.0.2/
--rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.0.2/LICENSE
--rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.0.2/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-05-15 02:07:42.476014 trex-model-1.0.2/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.0.2/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-05-15 02:07:42.476994 trex-model-1.0.2/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      922 2023-05-15 02:07:17.000000 trex-model-1.0.2/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.442059 trex-model-1.0.2/trex_model.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-05-15 02:07:42.000000 trex-model-1.0.2/trex_model.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1847 2023-05-15 02:07:42.000000 trex-model-1.0.2/trex_model.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-05-15 02:07:42.000000 trex-model-1.0.2/trex_model.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       95 2023-05-15 02:07:42.000000 trex-model-1.0.2/trex_model.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       16 2023-05-15 02:07:42.000000 trex-model-1.0.2/trex_model.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.443521 trex-model-1.0.2/trexmodel/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.0.2/trexmodel/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1122 2021-09-03 09:11:14.000000 trex-model-1.0.2/trexmodel/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.446853 trex-model-1.0.2/trexmodel/models/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.0.2/trexmodel/models/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.471429 trex-model-1.0.2/trexmodel/models/datastore/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.0.2/trexmodel/models/datastore/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-1.0.2/trexmodel/models/datastore/admin_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3223 2023-04-11 07:48:46.000000 trex-model-1.0.2/trexmodel/models/datastore/analytic_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-1.0.2/trexmodel/models/datastore/coporate_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13539 2023-03-15 08:15:01.000000 trex-model-1.0.2/trexmodel/models/datastore/customer_model_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    48341 2023-05-12 06:20:00.000000 trex-model-1.0.2/trexmodel/models/datastore/customer_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1712 2020-10-26 01:02:17.000000 trex-model-1.0.2/trexmodel/models/datastore/fb_subsriber_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-1.0.2/trexmodel/models/datastore/inventory_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5974 2023-05-15 01:59:38.000000 trex-model-1.0.2/trexmodel/models/datastore/loyalty_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3663 2023-05-12 08:12:47.000000 trex-model-1.0.2/trexmodel/models/datastore/lucky_draw_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11281 2023-04-05 03:48:05.000000 trex-model-1.0.2/trexmodel/models/datastore/membership_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    57199 2023-04-25 06:49:40.000000 trex-model-1.0.2/trexmodel/models/datastore/merchant_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.0.2/trexmodel/models/datastore/model_decorators.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17711 2023-02-10 02:53:30.000000 trex-model-1.0.2/trexmodel/models/datastore/ndb_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    32251 2023-05-15 02:04:46.000000 trex-model-1.0.2/trexmodel/models/datastore/pos_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    20750 2023-04-10 08:59:10.000000 trex-model-1.0.2/trexmodel/models/datastore/prepaid_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    38941 2023-02-28 05:40:30.000000 trex-model-1.0.2/trexmodel/models/datastore/product_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    47521 2023-03-15 14:31:35.000000 trex-model-1.0.2/trexmodel/models/datastore/program_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    36350 2023-04-13 13:46:37.000000 trex-model-1.0.2/trexmodel/models/datastore/redeem_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    31165 2023-04-10 09:19:08.000000 trex-model-1.0.2/trexmodel/models/datastore/reward_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.0.2/trexmodel/models/datastore/spending_base_program_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6610 2021-03-30 06:42:06.000000 trex-model-1.0.2/trexmodel/models/datastore/system_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-1.0.2/trexmodel/models/datastore/task_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-1.0.2/trexmodel/models/datastore/test_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    36809 2023-04-24 09:59:51.000000 trex-model-1.0.2/trexmodel/models/datastore/transaction_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15228 2022-09-23 07:10:51.000000 trex-model-1.0.2/trexmodel/models/datastore/user_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17441 2022-12-29 13:44:05.000000 trex-model-1.0.2/trexmodel/models/datastore/voucher_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6452 2023-03-19 11:12:11.000000 trex-model-1.0.2/trexmodel/models/merchant_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.0.2/trexmodel/models/model_decorator.py
--rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.0.2/trexmodel/models/prepaid_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.0.2/trexmodel/pos_conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16572 2023-04-07 03:52:51.000000 trex-model-1.0.2/trexmodel/program_conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.473093 trex-model-1.0.2/trexmodel/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.2/trexmodel/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.473780 trex-model-1.0.2/trexmodel/utils/gcloud/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.2/trexmodel/utils/gcloud/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.0.2/trexmodel/utils/gcloud/datastore_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:07:42.474926 trex-model-1.0.2/trexmodel/utils/model/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.2/trexmodel/utils/model/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-1.0.2/trexmodel/utils/model/model_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:05:38.220173 trex-model-1.0.3/
+-rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.0.3/LICENSE
+-rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.0.3/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-05-15 06:05:38.220382 trex-model-1.0.3/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.0.3/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-05-15 06:05:38.221271 trex-model-1.0.3/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      922 2023-05-15 06:05:30.000000 trex-model-1.0.3/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:05:38.182376 trex-model-1.0.3/trex_model.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-05-15 06:05:37.000000 trex-model-1.0.3/trex_model.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1847 2023-05-15 06:05:37.000000 trex-model-1.0.3/trex_model.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-05-15 06:05:37.000000 trex-model-1.0.3/trex_model.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       95 2023-05-15 06:05:37.000000 trex-model-1.0.3/trex_model.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       16 2023-05-15 06:05:37.000000 trex-model-1.0.3/trex_model.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:05:38.185574 trex-model-1.0.3/trexmodel/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.0.3/trexmodel/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1122 2021-09-03 09:11:14.000000 trex-model-1.0.3/trexmodel/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:05:38.189370 trex-model-1.0.3/trexmodel/models/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.0.3/trexmodel/models/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:05:38.216505 trex-model-1.0.3/trexmodel/models/datastore/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.0.3/trexmodel/models/datastore/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-1.0.3/trexmodel/models/datastore/admin_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3223 2023-04-11 07:48:46.000000 trex-model-1.0.3/trexmodel/models/datastore/analytic_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-1.0.3/trexmodel/models/datastore/coporate_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13539 2023-03-15 08:15:01.000000 trex-model-1.0.3/trexmodel/models/datastore/customer_model_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    48341 2023-05-12 06:20:00.000000 trex-model-1.0.3/trexmodel/models/datastore/customer_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1712 2020-10-26 01:02:17.000000 trex-model-1.0.3/trexmodel/models/datastore/fb_subsriber_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-1.0.3/trexmodel/models/datastore/inventory_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5974 2023-05-15 01:59:38.000000 trex-model-1.0.3/trexmodel/models/datastore/loyalty_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3663 2023-05-12 08:12:47.000000 trex-model-1.0.3/trexmodel/models/datastore/lucky_draw_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11281 2023-04-05 03:48:05.000000 trex-model-1.0.3/trexmodel/models/datastore/membership_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    57379 2023-05-15 02:58:36.000000 trex-model-1.0.3/trexmodel/models/datastore/merchant_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.0.3/trexmodel/models/datastore/model_decorators.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17711 2023-02-10 02:53:30.000000 trex-model-1.0.3/trexmodel/models/datastore/ndb_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    32251 2023-05-15 02:04:46.000000 trex-model-1.0.3/trexmodel/models/datastore/pos_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    20750 2023-04-10 08:59:10.000000 trex-model-1.0.3/trexmodel/models/datastore/prepaid_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    38941 2023-02-28 05:40:30.000000 trex-model-1.0.3/trexmodel/models/datastore/product_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    47521 2023-03-15 14:31:35.000000 trex-model-1.0.3/trexmodel/models/datastore/program_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    36350 2023-04-13 13:46:37.000000 trex-model-1.0.3/trexmodel/models/datastore/redeem_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    31165 2023-04-10 09:19:08.000000 trex-model-1.0.3/trexmodel/models/datastore/reward_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.0.3/trexmodel/models/datastore/spending_base_program_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6610 2021-03-30 06:42:06.000000 trex-model-1.0.3/trexmodel/models/datastore/system_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-1.0.3/trexmodel/models/datastore/task_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-1.0.3/trexmodel/models/datastore/test_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    36809 2023-04-24 09:59:51.000000 trex-model-1.0.3/trexmodel/models/datastore/transaction_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15228 2022-09-23 07:10:51.000000 trex-model-1.0.3/trexmodel/models/datastore/user_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17441 2022-12-29 13:44:05.000000 trex-model-1.0.3/trexmodel/models/datastore/voucher_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6452 2023-03-19 11:12:11.000000 trex-model-1.0.3/trexmodel/models/merchant_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.0.3/trexmodel/models/model_decorator.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.0.3/trexmodel/models/prepaid_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.0.3/trexmodel/pos_conf.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16572 2023-04-07 03:52:51.000000 trex-model-1.0.3/trexmodel/program_conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:05:38.217468 trex-model-1.0.3/trexmodel/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.3/trexmodel/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:05:38.218362 trex-model-1.0.3/trexmodel/utils/gcloud/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.3/trexmodel/utils/gcloud/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.0.3/trexmodel/utils/gcloud/datastore_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:05:38.219449 trex-model-1.0.3/trexmodel/utils/model/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.3/trexmodel/utils/model/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-1.0.3/trexmodel/utils/model/model_util.py
```

### Comparing `trex-model-1.0.2/LICENSE` & `trex-model-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/setup.py` & `trex-model-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      name='trex-model',  
-     version='1.0.2',
+     version='1.0.3',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex database module package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-model",
      packages=setuptools.find_packages(),
```

### Comparing `trex-model-1.0.2/trex_model.egg-info/SOURCES.txt` & `trex-model-1.0.3/trex_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/conf.py` & `trex-model-1.0.3/trexmodel/conf.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/admin_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/admin_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/analytic_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/analytic_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/coporate_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/coporate_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/customer_model_helpers.py` & `trex-model-1.0.3/trexmodel/models/datastore/customer_model_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/customer_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/customer_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/fb_subsriber_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/fb_subsriber_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/inventory_model.py` & `trex-model-1.0.3/trexmodel/models/datastore/inventory_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/loyalty_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/loyalty_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/lucky_draw_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/lucky_draw_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/membership_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/membership_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/merchant_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/merchant_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     stat_figure_update_interval_in_minutes  = conf.MERCHANT_STAT_FIGURE_UPDATE_INTERVAL_IN_MINUTES
     stat_figure_update_datetime_format      = '%d-%m-%Y %H:%M:%S'
     
     dict_properties = ['company_name', 'brand_name', 'contact_name', 'business_reg_no', 'mobile_phone', 'office_phone', 'fax_phone', 'email', 'account_code', 'country',
                        'registered_datetime', 'modified_datetime', 'plan_start_date', 'plan_end_date', 'currency_code', 
                        'published_program_configuration', 'published_voucher_configuration', 'membership_configuration', 
                        'tier_membership_configuration', 'prepaid_configuration', 'product_modifier_configuration',
-                       'dashboard_stat_figure', 'program_settings', 'is_tier_membership_configured',
+                       'dashboard_stat_figure', 'program_settings', 'is_tier_membership_configured', 'website',
                        ]
     
     
     def to_login_dict(self):
         return {
                 'account_code'      : self.account_code,
                 'plan_end_date'     : self.plan_end_date,
@@ -130,24 +130,26 @@
                 'days_of_repeat_purchase_measurement'   : 7,
                 'membership_renew_advance_day'          : 7,
                 'membership_renew_late_day'             : 30,
                 }   
     
     
     @staticmethod
-    def update_details(merchant_acct, company_name=None, brand_name=None, business_reg_no=None, contact_name=None, email=None, mobile_phone=None, office_phone=None, currency_code=None, country=None):
+    def update_details(merchant_acct, company_name=None, brand_name=None, business_reg_no=None, contact_name=None, 
+                       email=None, mobile_phone=None, office_phone=None, currency_code=None, country=None, website=None):
         merchant_acct.company_name      = company_name
         merchant_acct.brand_name        = brand_name
         merchant_acct.business_reg_no   = business_reg_no
         merchant_acct.contact_name      = contact_name
         merchant_acct.email             = email
         merchant_acct.mobile_phone      = mobile_phone
         merchant_acct.office_phone      = office_phone
         merchant_acct.currency_code     = currency_code
         merchant_acct.country           = country
+        merchant_acct.website           = website
         merchant_acct.put()
     
     @staticmethod
     def format_account_code(account_code):
         if is_not_empty(account_code):
             if len(account_code) == 16:
                 account_code = '-'.join(split_by_length(account_code,4))
@@ -647,15 +649,15 @@
                 else:
                     return dashboard_stat_figure.get('stat_details')
         
         return None
     
     @staticmethod
     def create(company_name=None, brand_name=None, contact_name=None, email=None, mobile_phone=None, office_phone=None, plan_start_date=None, plan_end_date=None, 
-               account_code=None, currency_code=None, country=None):
+               account_code=None, currency_code=None, country=None, website=None):
         
         if account_code is None:
             account_code    = "%s-%s-%s-%s" % (random_number(4),random_number(4),random_number(4),random_number(4))
             
         merchant_acct   = MerchantAcct(
                                        company_name     = company_name,
                                        brand_name       = brand_name,     
@@ -663,14 +665,15 @@
                                        email            = email,
                                        mobile_phone     = mobile_phone,
                                        office_phone     = office_phone,
                                        plan_start_date  = plan_start_date, 
                                        plan_end_date    = plan_end_date,
                                        currency_code    = currency_code,
                                        country          = country,    
+                                       website          = website,
                                        api_key          = random_string(24),
                                        program_settings = MerchantAcct.default_program_settings(),
                                        )
         
         logging.debug('account_code=%s', account_code)
         
         merchant_acct.account_code = account_code
```

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/model_decorators.py` & `trex-model-1.0.3/trexmodel/models/datastore/model_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/ndb_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/ndb_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/pos_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/pos_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/prepaid_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/prepaid_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/product_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/product_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/program_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/program_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/redeem_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/redeem_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/reward_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/reward_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/spending_base_program_model.py` & `trex-model-1.0.3/trexmodel/models/datastore/spending_base_program_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/system_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/system_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/task_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/task_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/test_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/test_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/transaction_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/transaction_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/user_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/user_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/datastore/voucher_models.py` & `trex-model-1.0.3/trexmodel/models/datastore/voucher_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/models/merchant_helpers.py` & `trex-model-1.0.3/trexmodel/models/merchant_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/program_conf.py` & `trex-model-1.0.3/trexmodel/program_conf.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.2/trexmodel/utils/model/model_util.py` & `trex-model-1.0.3/trexmodel/utils/model/model_util.py`

 * *Files identical despite different names*

