# Comparing `tmp/pyclickhouse3-0.9.32.tar.gz` & `tmp/pyclickhouse3-0.9.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclickhouse3-0.9.32.tar", last modified: Mon May 15 07:49:44 2023, max compression
+gzip compressed data, was "pyclickhouse3-0.9.33.tar", last modified: Mon May 15 07:57:19 2023, max compression
```

## Comparing `pyclickhouse3-0.9.32.tar` & `pyclickhouse3-0.9.33.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 07:49:44.490765 pyclickhouse3-0.9.32/
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    11357 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.32/LICENSE
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)      463 2023-05-15 07:49:44.490765 pyclickhouse3-0.9.32/PKG-INFO
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     1779 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.32/README.md
-drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 07:49:44.490765 pyclickhouse3-0.9.32/pyclickhouse/
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     8887 2022-05-20 10:07:52.000000 pyclickhouse3-0.9.32/pyclickhouse/Connection.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    25465 2023-01-23 16:34:27.000000 pyclickhouse3-0.9.32/pyclickhouse/Cursor.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     3702 2021-09-29 15:05:05.000000 pyclickhouse3-0.9.32/pyclickhouse/FilterableCache.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)       61 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.32/pyclickhouse/__init__.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    23715 2023-05-15 07:48:35.000000 pyclickhouse3-0.9.32/pyclickhouse/formatter.py
-drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 07:49:44.490765 pyclickhouse3-0.9.32/pyclickhouse3.egg-info/
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)      463 2023-05-15 07:49:44.000000 pyclickhouse3-0.9.32/pyclickhouse3.egg-info/PKG-INFO
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)      485 2023-05-15 07:49:44.000000 pyclickhouse3-0.9.32/pyclickhouse3.egg-info/SOURCES.txt
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)        1 2023-05-15 07:49:44.000000 pyclickhouse3-0.9.32/pyclickhouse3.egg-info/dependency_links.txt
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)        1 2021-02-10 13:40:28.000000 pyclickhouse3-0.9.32/pyclickhouse3.egg-info/not-zip-safe
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)       25 2023-05-15 07:49:44.000000 pyclickhouse3-0.9.32/pyclickhouse3.egg-info/requires.txt
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)       13 2023-05-15 07:49:44.000000 pyclickhouse3-0.9.32/pyclickhouse3.egg-info/top_level.txt
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)      103 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.32/pyproject.toml
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)       79 2023-05-15 07:49:44.490765 pyclickhouse3-0.9.32/setup.cfg
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)      683 2023-05-15 07:49:32.000000 pyclickhouse3-0.9.32/setup.py
-drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 07:49:44.490765 pyclickhouse3-0.9.32/test/
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     1560 2023-01-23 10:37:59.000000 pyclickhouse3-0.9.32/test/test_compatibility.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     2613 2023-01-23 14:27:59.000000 pyclickhouse3-0.9.32/test/test_map.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    10330 2023-01-26 12:08:31.000000 pyclickhouse3-0.9.32/test/test_new.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     4759 2023-01-23 10:49:05.000000 pyclickhouse3-0.9.32/test/test_simple.py
+drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 07:57:19.784933 pyclickhouse3-0.9.33/
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    11357 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.33/LICENSE
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)      463 2023-05-15 07:57:19.784933 pyclickhouse3-0.9.33/PKG-INFO
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     1779 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.33/README.md
+drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 07:57:19.784933 pyclickhouse3-0.9.33/pyclickhouse/
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     8887 2022-05-20 10:07:52.000000 pyclickhouse3-0.9.33/pyclickhouse/Connection.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    25465 2023-01-23 16:34:27.000000 pyclickhouse3-0.9.33/pyclickhouse/Cursor.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     3702 2021-09-29 15:05:05.000000 pyclickhouse3-0.9.33/pyclickhouse/FilterableCache.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)       61 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.33/pyclickhouse/__init__.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    23715 2023-05-15 07:48:35.000000 pyclickhouse3-0.9.33/pyclickhouse/formatter.py
+drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 07:57:19.784933 pyclickhouse3-0.9.33/pyclickhouse3.egg-info/
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)      463 2023-05-15 07:57:19.000000 pyclickhouse3-0.9.33/pyclickhouse3.egg-info/PKG-INFO
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)      485 2023-05-15 07:57:19.000000 pyclickhouse3-0.9.33/pyclickhouse3.egg-info/SOURCES.txt
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)        1 2023-05-15 07:57:19.000000 pyclickhouse3-0.9.33/pyclickhouse3.egg-info/dependency_links.txt
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)        1 2021-02-10 13:40:28.000000 pyclickhouse3-0.9.33/pyclickhouse3.egg-info/not-zip-safe
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)       25 2023-05-15 07:57:19.000000 pyclickhouse3-0.9.33/pyclickhouse3.egg-info/requires.txt
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)       13 2023-05-15 07:57:19.000000 pyclickhouse3-0.9.33/pyclickhouse3.egg-info/top_level.txt
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)      103 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.33/pyproject.toml
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)       79 2023-05-15 07:57:19.784933 pyclickhouse3-0.9.33/setup.cfg
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)      683 2023-05-15 07:56:17.000000 pyclickhouse3-0.9.33/setup.py
+drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 07:57:19.784933 pyclickhouse3-0.9.33/test/
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     1560 2023-01-23 10:37:59.000000 pyclickhouse3-0.9.33/test/test_compatibility.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     2613 2023-01-23 14:27:59.000000 pyclickhouse3-0.9.33/test/test_map.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    10330 2023-01-26 12:08:31.000000 pyclickhouse3-0.9.33/test/test_new.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     4759 2023-01-23 10:49:05.000000 pyclickhouse3-0.9.33/test/test_simple.py
```

### Comparing `pyclickhouse3-0.9.32/LICENSE` & `pyclickhouse3-0.9.33/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.32/README.md` & `pyclickhouse3-0.9.33/README.md`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.32/pyclickhouse/Connection.py` & `pyclickhouse3-0.9.33/pyclickhouse/Connection.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.32/pyclickhouse/Cursor.py` & `pyclickhouse3-0.9.33/pyclickhouse/Cursor.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.32/pyclickhouse/FilterableCache.py` & `pyclickhouse3-0.9.33/pyclickhouse/FilterableCache.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.32/pyclickhouse/formatter.py` & `pyclickhouse3-0.9.33/pyclickhouse/formatter.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.32/setup.py` & `pyclickhouse3-0.9.33/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 REQUIRED=['requests', 'six', 'ujson', 'numpy']
 
 setup(name='pyclickhouse3',
-      version='0.9.32',
+      version='0.9.33',
       description='Clickhouse Python driver with an API roughly resembling Python DB API 2.0 specification.',
       url='https://github.com/mfridental/PyClickhouse',
-      download_url='https://github.com/mfridental/PyClickhouse/archive/0.9.32.tar.gz',
+      download_url='https://github.com/mfridental/PyClickhouse/archive/0.9.33.tar.gz',
       keywords=['Clickhouse', 'Database', 'Driver'],
       classifiers=[],
       author='Maxim Fridental (Maintainer)',
       author_email='maxim@fridental.de',
       license='Apache2',
       packages=['pyclickhouse'],
       install_requires=REQUIRED,
```

### Comparing `pyclickhouse3-0.9.32/test/test_compatibility.py` & `pyclickhouse3-0.9.33/test/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.32/test/test_map.py` & `pyclickhouse3-0.9.33/test/test_map.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.32/test/test_new.py` & `pyclickhouse3-0.9.33/test/test_new.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.32/test/test_simple.py` & `pyclickhouse3-0.9.33/test/test_simple.py`

 * *Files identical despite different names*

