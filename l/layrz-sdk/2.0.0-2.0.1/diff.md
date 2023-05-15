# Comparing `tmp/layrz-sdk-2.0.0.tar.gz` & `tmp/layrz-sdk-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layrz-sdk-2.0.0.tar", last modified: Mon May 15 03:50:31 2023, max compression
+gzip compressed data, was "layrz-sdk-2.0.1.tar", last modified: Mon May 15 05:43:29 2023, max compression
```

## Comparing `layrz-sdk-2.0.0.tar` & `layrz-sdk-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,93 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:50:31.136110 layrz-sdk-2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-15 03:50:20.000000 layrz-sdk-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1218 2023-05-15 03:50:31.136110 layrz-sdk-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-05-15 03:50:20.000000 layrz-sdk-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:50:31.133107 layrz-sdk-2.0.0/layrz/
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-15 03:50:20.000000 layrz-sdk-2.0.0/layrz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:50:31.135109 layrz-sdk-2.0.0/layrz_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1218 2023-05-15 03:50:31.000000 layrz-sdk-2.0.0/layrz_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      208 2023-05-15 03:50:31.000000 layrz-sdk-2.0.0/layrz_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 03:50:31.000000 layrz-sdk-2.0.0/layrz_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-15 03:50:31.000000 layrz-sdk-2.0.0/layrz_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-15 03:50:31.000000 layrz-sdk-2.0.0/layrz_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 03:50:31.136110 layrz-sdk-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-05-15 03:50:20.000000 layrz-sdk-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.242751 layrz-sdk-2.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-05-15 05:43:29.241750 layrz-sdk-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.218748 layrz-sdk-2.0.1/layrz/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.219748 layrz-sdk-2.0.1/layrz/sdk/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.219748 layrz-sdk-2.0.1/layrz/sdk/entities/
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.221748 layrz-sdk-2.0.1/layrz/sdk/entities/broadcasts/
+-rw-rw-rw-   0 root         (0) root         (0)      204 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/broadcasts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/broadcasts/request.py
+-rw-rw-rw-   0 root         (0) root         (0)      723 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/broadcasts/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1660 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/broadcasts/result.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/broadcasts/service.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/broadcasts/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.223749 layrz-sdk-2.0.1/layrz/sdk/entities/cases/
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/cases/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/cases/case.py
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/cases/comment.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/cases/trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.229749 layrz-sdk-2.0.1/layrz/sdk/entities/charts/
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/alignment.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/bar.py
+-rw-rw-rw-   0 root         (0) root         (0)     5148 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/column.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/data_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      443 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     5431 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/line.py
+-rw-rw-rw-   0 root         (0) root         (0)     4788 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/map.py
+-rw-rw-rw-   0 root         (0) root         (0)     1028 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/number.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/pie.py
+-rw-rw-rw-   0 root         (0) root         (0)     3354 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/radar.py
+-rw-rw-rw-   0 root         (0) root         (0)     3114 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/radial_bar.py
+-rw-rw-rw-   0 root         (0) root         (0)     5242 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/scatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2057 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/serie.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/serie_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1693 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     4568 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/charts/timeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.230749 layrz-sdk-2.0.1/layrz/sdk/entities/checkpoints/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/checkpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/checkpoints/checkpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/checkpoints/geofence.py
+-rw-rw-rw-   0 root         (0) root         (0)     1728 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/checkpoints/waypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.231749 layrz-sdk-2.0.1/layrz/sdk/entities/events/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/events/event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.232750 layrz-sdk-2.0.1/layrz/sdk/entities/formatting/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/formatting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/formatting/text_align.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.234750 layrz-sdk-2.0.1/layrz/sdk/entities/general/
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/general/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/general/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/general/asset_operation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/general/custom_field.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/general/device.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/general/sensor.py
+-rw-rw-rw-   0 root         (0) root         (0)      694 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/general/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.234750 layrz-sdk-2.0.1/layrz/sdk/entities/repcom/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/repcom/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2653 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/repcom/transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.237750 layrz-sdk-2.0.1/layrz/sdk/entities/reports/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2396 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/reports/col.py
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/reports/format.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/reports/header.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/reports/page.py
+-rw-rw-rw-   0 root         (0) root         (0)     3882 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/reports/report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/reports/row.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.238750 layrz-sdk-2.0.1/layrz/sdk/entities/telemetry/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/telemetry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/telemetry/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/entities/telemetry/position.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.238750 layrz-sdk-2.0.1/layrz/sdk/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/helpers/color.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.239750 layrz-sdk-2.0.1/layrz/sdk/lcl/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/lcl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19560 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/lcl/core.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/layrz/sdk/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:43:29.241750 layrz-sdk-2.0.1/layrz_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-05-15 05:43:29.000000 layrz-sdk-2.0.1/layrz_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2609 2023-05-15 05:43:29.000000 layrz-sdk-2.0.1/layrz_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 05:43:29.000000 layrz-sdk-2.0.1/layrz_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-15 05:43:29.000000 layrz-sdk-2.0.1/layrz_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 05:43:29.000000 layrz-sdk-2.0.1/layrz_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-15 05:43:29.000000 layrz-sdk-2.0.1/layrz_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-15 05:43:29.000000 layrz-sdk-2.0.1/layrz_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 05:43:29.242751 layrz-sdk-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1137 2023-05-15 05:43:19.000000 layrz-sdk-2.0.1/setup.py
```

### Comparing `layrz-sdk-2.0.0/LICENSE` & `layrz-sdk-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.0.0/PKG-INFO` & `layrz-sdk-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-sdk
-Version: 2.0.0
+Version: 2.0.1
 Summary: Layrz SDK
 Home-page: https://gitlab.com/layrz-software/libraries/layrz-sdk
 Author: Layrz
 Author-email: software@layrz.com
 License: MIT
 Keywords: sdk goldenm lcl layrz compute language
 Classifier: Programming Language :: Python :: 3
```

### Comparing `layrz-sdk-2.0.0/README.md` & `layrz-sdk-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `layrz-sdk-2.0.0/layrz_sdk.egg-info/PKG-INFO` & `layrz-sdk-2.0.1/layrz_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-sdk
-Version: 2.0.0
+Version: 2.0.1
 Summary: Layrz SDK
 Home-page: https://gitlab.com/layrz-software/libraries/layrz-sdk
 Author: Layrz
 Author-email: software@layrz.com
 License: MIT
 Keywords: sdk goldenm lcl layrz compute language
 Classifier: Programming Language :: Python :: 3
```

### Comparing `layrz-sdk-2.0.0/setup.py` & `layrz-sdk-2.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,27 +13,29 @@
   """ Return long description """
   with open('README.md', 'r', encoding='utf-8') as fh:
     return fh.read()
 
 
 setuptools.setup(
   name='layrz-sdk',
-  version='2.0.0',
+  version='2.0.1',
   author='Layrz',
   author_email='software@layrz.com',
   url='https://gitlab.com/layrz-software/libraries/layrz-sdk',
   license='MIT',
   description='Layrz SDK',
   long_description=long_description(),
   long_description_content_type='text/markdown',
   keywords='sdk goldenm lcl layrz compute language',
   packages=setuptools.find_packages(),
+  namespace_packages=['layrz'],
+  zip_safe=False,
   classifiers=[
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
   ],
-  python_requires=">=3.8",
+  python_requires='>=3.8',
   install_requires=get_requirements(),
 )
```

