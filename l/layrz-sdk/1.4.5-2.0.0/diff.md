# Comparing `tmp/layrz-sdk-1.4.5.tar.gz` & `tmp/layrz-sdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layrz-sdk-1.4.5.tar", last modified: Fri Mar 24 22:51:10 2023, max compression
+gzip compressed data, was "layrz-sdk-2.0.0.tar", last modified: Mon May 15 03:50:31 2023, max compression
```

## Comparing `layrz-sdk-1.4.5.tar` & `layrz-sdk-2.0.0.tar`

### file list

```diff
@@ -1,93 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.255110 layrz-sdk-1.4.5/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1074 2023-03-24 22:51:10.254110 layrz-sdk-1.4.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.235109 layrz-sdk-1.4.5/layrz_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-03-24 22:51:10.000000 layrz-sdk-1.4.5/layrz_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2495 2023-03-24 22:51:10.000000 layrz-sdk-1.4.5/layrz_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 22:51:10.000000 layrz-sdk-1.4.5/layrz_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-24 22:51:10.000000 layrz-sdk-1.4.5/layrz_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-24 22:51:10.000000 layrz-sdk-1.4.5/layrz_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.235109 layrz-sdk-1.4.5/layrzsdk/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.236109 layrz-sdk-1.4.5/layrzsdk/entities/
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.237109 layrz-sdk-1.4.5/layrzsdk/entities/broadcasts/
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/broadcasts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/broadcasts/request.py
--rw-rw-rw-   0 root         (0) root         (0)      723 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/broadcasts/response.py
--rw-rw-rw-   0 root         (0) root         (0)     1660 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/broadcasts/result.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/broadcasts/service.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/broadcasts/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.238109 layrz-sdk-1.4.5/layrzsdk/entities/cases/
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/cases/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/cases/case.py
--rw-rw-rw-   0 root         (0) root         (0)     1216 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/cases/comment.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/cases/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.244109 layrz-sdk-1.4.5/layrzsdk/entities/charts/
--rw-rw-rw-   0 root         (0) root         (0)      747 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/alignment.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/bar.py
--rw-rw-rw-   0 root         (0) root         (0)     5147 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/column.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/data_type.py
--rw-rw-rw-   0 root         (0) root         (0)      443 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/html.py
--rw-rw-rw-   0 root         (0) root         (0)     5430 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/line.py
--rw-rw-rw-   0 root         (0) root         (0)     4788 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/map.py
--rw-rw-rw-   0 root         (0) root         (0)     1028 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/number.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/pie.py
--rw-rw-rw-   0 root         (0) root         (0)     3354 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/radar.py
--rw-rw-rw-   0 root         (0) root         (0)     3114 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/radial_bar.py
--rw-rw-rw-   0 root         (0) root         (0)     5242 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/scatter.py
--rw-rw-rw-   0 root         (0) root         (0)     2057 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/serie.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/serie_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1693 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/table.py
--rw-rw-rw-   0 root         (0) root         (0)     4568 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/charts/timeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.245110 layrz-sdk-1.4.5/layrzsdk/entities/checkpoints/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/checkpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1388 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/checkpoints/checkpoint.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/checkpoints/geofence.py
--rw-rw-rw-   0 root         (0) root         (0)     1728 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/checkpoints/waypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.246110 layrz-sdk-1.4.5/layrzsdk/entities/events/
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/events/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.246110 layrz-sdk-1.4.5/layrzsdk/entities/formatting/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/formatting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/formatting/text_align.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.249110 layrz-sdk-1.4.5/layrzsdk/entities/general/
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/general/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/general/asset.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/general/asset_operation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      795 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/general/custom_field.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/general/device.py
--rw-rw-rw-   0 root         (0) root         (0)      874 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/general/sensor.py
--rw-rw-rw-   0 root         (0) root         (0)      694 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/general/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.249110 layrz-sdk-1.4.5/layrzsdk/entities/repcom/
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/repcom/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2653 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/repcom/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.251110 layrz-sdk-1.4.5/layrzsdk/entities/reports/
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2396 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/reports/col.py
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/reports/format.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/reports/header.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/reports/page.py
--rw-rw-rw-   0 root         (0) root         (0)     3882 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/reports/report.py
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/reports/row.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.252110 layrz-sdk-1.4.5/layrzsdk/entities/telemetry/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/telemetry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1208 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/telemetry/message.py
--rw-rw-rw-   0 root         (0) root         (0)     1636 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/entities/telemetry/position.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.252110 layrz-sdk-1.4.5/layrzsdk/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1049 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/helpers/color.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.253110 layrz-sdk-1.4.5/layrzsdk/lcl/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/lcl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/layrzsdk/lcl/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.253110 layrz-sdk-1.4.5/lcl/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/lcl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 22:51:10.254110 layrz-sdk-1.4.5/lcl/core/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/lcl/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19561 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/lcl/core/language.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-24 22:51:10.255110 layrz-sdk-1.4.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      711 2023-03-24 22:51:01.000000 layrz-sdk-1.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:50:31.136110 layrz-sdk-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-15 03:50:20.000000 layrz-sdk-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-05-15 03:50:31.136110 layrz-sdk-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-05-15 03:50:20.000000 layrz-sdk-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:50:31.133107 layrz-sdk-2.0.0/layrz/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-15 03:50:20.000000 layrz-sdk-2.0.0/layrz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:50:31.135109 layrz-sdk-2.0.0/layrz_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-05-15 03:50:31.000000 layrz-sdk-2.0.0/layrz_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      208 2023-05-15 03:50:31.000000 layrz-sdk-2.0.0/layrz_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 03:50:31.000000 layrz-sdk-2.0.0/layrz_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-15 03:50:31.000000 layrz-sdk-2.0.0/layrz_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-15 03:50:31.000000 layrz-sdk-2.0.0/layrz_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 03:50:31.136110 layrz-sdk-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-05-15 03:50:20.000000 layrz-sdk-2.0.0/setup.py
```

### Comparing `layrz-sdk-1.4.5/LICENSE` & `layrz-sdk-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `layrz-sdk-1.4.5/README.md` & `layrz-sdk-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `layrz-sdk-1.4.5/setup.py` & `layrz-sdk-2.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,39 @@
+""" Setup file for layrz-sdk. """
 import setuptools
 
 
-def read(filename):
-  import os
-  return open(os.path.join(os.path.dirname(__file__), filename)).read()
+def get_requirements():
+  with open('requirements.txt', 'rb') as f:
+    lines = f.read().decode('utf-8').splitlines()
+
+  return [line for line in lines if not line.startswith('--')]
+
+
+def long_description():
+  """ Return long description """
+  with open('README.md', 'r', encoding='utf-8') as fh:
+    return fh.read()
 
 
 setuptools.setup(
-  name="layrz-sdk",
-  version="1.4.5",
-  author="Layrz",
-  author_email="software@layrz.com",
+  name='layrz-sdk',
+  version='2.0.0',
+  author='Layrz',
+  author_email='software@layrz.com',
   url='https://gitlab.com/layrz-software/libraries/layrz-sdk',
   license='MIT',
-  description="Layrz SDK",
-  long_description=read('README.md'),
+  description='Layrz SDK',
+  long_description=long_description(),
+  long_description_content_type='text/markdown',
   keywords='sdk goldenm lcl layrz compute language',
   packages=setuptools.find_packages(),
   classifiers=[
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
   ],
-  install_requires=['requests', 'pytz', 'xlsxwriter'],
-  python_requires='>=3.8',
+  python_requires=">=3.8",
+  install_requires=get_requirements(),
 )
```

