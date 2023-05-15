# Comparing `tmp/xgb2sql-0.114.tar.gz` & `tmp/xgb2sql-0.115.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgb2sql-0.114.tar", last modified: Mon May 15 16:30:17 2023, max compression
+gzip compressed data, was "xgb2sql-0.115.tar", last modified: Mon May 15 16:53:21 2023, max compression
```

## Comparing `xgb2sql-0.114.tar` & `xgb2sql-0.115.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-15 16:30:17.614424 xgb2sql-0.114/
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     2348 2023-03-13 17:57:29.000000 xgb2sql-0.114/CONTRIBUTING.md
--rw-r--r--   0 benjaminjiang   (501) staff       (20)    11357 2023-03-13 17:09:07.000000 xgb2sql-0.114/LICENSE
--rw-r--r--   0 benjaminjiang   (501) staff       (20)      111 2023-03-13 17:09:07.000000 xgb2sql-0.114/MANIFEST.in
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     8311 2023-05-15 16:30:17.613671 xgb2sql-0.114/PKG-INFO
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     7544 2023-05-12 18:56:46.000000 xgb2sql-0.114/README.md
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     1752 2023-05-15 16:23:09.000000 xgb2sql-0.114/settings.ini
--rw-r--r--   0 benjaminjiang   (501) staff       (20)       38 2023-05-15 16:30:17.614465 xgb2sql-0.114/setup.cfg
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     1911 2023-05-11 18:25:54.000000 xgb2sql-0.114/setup.py
-drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-15 16:30:17.612521 xgb2sql-0.114/xgb2sql/
--rw-r--r--   0 benjaminjiang   (501) staff       (20)       22 2023-03-13 18:30:03.000000 xgb2sql-0.114/xgb2sql/__init__.py
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     7422 2023-05-15 16:22:59.000000 xgb2sql-0.114/xgb2sql/core.py
-drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-15 16:30:17.613483 xgb2sql-0.114/xgb2sql.egg-info/
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     8311 2023-05-15 16:30:17.000000 xgb2sql-0.114/xgb2sql.egg-info/PKG-INFO
--rw-r--r--   0 benjaminjiang   (501) staff       (20)      257 2023-05-15 16:30:17.000000 xgb2sql-0.114/xgb2sql.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminjiang   (501) staff       (20)        1 2023-05-15 16:30:17.000000 xgb2sql-0.114/xgb2sql.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminjiang   (501) staff       (20)        1 2023-05-11 18:39:29.000000 xgb2sql-0.114/xgb2sql.egg-info/not-zip-safe
--rw-r--r--   0 benjaminjiang   (501) staff       (20)        8 2023-05-15 16:30:17.000000 xgb2sql-0.114/xgb2sql.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-15 16:53:21.019552 xgb2sql-0.115/
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     2348 2023-03-13 17:57:29.000000 xgb2sql-0.115/CONTRIBUTING.md
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)    11357 2023-03-13 17:09:07.000000 xgb2sql-0.115/LICENSE
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)      111 2023-03-13 17:09:07.000000 xgb2sql-0.115/MANIFEST.in
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     8311 2023-05-15 16:53:21.019324 xgb2sql-0.115/PKG-INFO
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     7544 2023-05-12 18:56:46.000000 xgb2sql-0.115/README.md
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     1752 2023-05-15 16:52:58.000000 xgb2sql-0.115/settings.ini
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)       38 2023-05-15 16:53:21.019613 xgb2sql-0.115/setup.cfg
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     1911 2023-05-11 18:25:54.000000 xgb2sql-0.115/setup.py
+drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-15 16:53:21.018050 xgb2sql-0.115/xgb2sql/
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)       22 2023-03-13 18:30:03.000000 xgb2sql-0.115/xgb2sql/__init__.py
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     7381 2023-05-15 16:52:44.000000 xgb2sql-0.115/xgb2sql/core.py
+drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-15 16:53:21.019127 xgb2sql-0.115/xgb2sql.egg-info/
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     8311 2023-05-15 16:53:21.000000 xgb2sql-0.115/xgb2sql.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)      257 2023-05-15 16:53:21.000000 xgb2sql-0.115/xgb2sql.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)        1 2023-05-15 16:53:21.000000 xgb2sql-0.115/xgb2sql.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)        1 2023-05-11 18:39:29.000000 xgb2sql-0.115/xgb2sql.egg-info/not-zip-safe
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)        8 2023-05-15 16:53:21.000000 xgb2sql-0.115/xgb2sql.egg-info/top_level.txt
```

### Comparing `xgb2sql-0.114/CONTRIBUTING.md` & `xgb2sql-0.115/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xgb2sql-0.114/LICENSE` & `xgb2sql-0.115/LICENSE`

 * *Files identical despite different names*

### Comparing `xgb2sql-0.114/PKG-INFO` & `xgb2sql-0.115/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgb2sql
-Version: 0.114
+Version: 0.115
 Summary: A simple library for converting the output of an XGB model to SQL.
 Home-page: https://github.com/Chryzanthemum/xgb2sql
 Author: Benjamin Jiang
 Author-email: benjamin.jiang@well.co
 License: Apache Software License 2.0
 Keywords: xgb2sql,xgb sql,xgboost sql,xgboost to sql,xgb to sql
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xgb2sql-0.114/README.md` & `xgb2sql-0.115/README.md`

 * *Files identical despite different names*

### Comparing `xgb2sql-0.114/settings.ini` & `xgb2sql-0.115/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = Chryzanthemum
 description = A simple library for converting the output of an XGB model to SQL. 
 keywords = xgb2sql, xgb sql, xgboost sql, xgboost to sql, xgb to sql
 author = Benjamin Jiang
 author_email = benjamin.jiang@well.co
 copyright = Well
 branch = master
-version = 0.114
+version = 0.115
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `xgb2sql-0.114/setup.py` & `xgb2sql-0.115/setup.py`

 * *Files identical despite different names*

### Comparing `xgb2sql-0.114/xgb2sql/core.py` & `xgb2sql-0.115/xgb2sql/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,14 @@
         when_list = []
         column = f"column_{counter}"
         columns.append(column)
         if len(leaves) == 1:
             column_list = f"{leaves.values()[0]} AS {column}"
         else:
             for base_leaf in leaves:
-                print(leaves, base_leaf)
                 leaf_query = (
                     "\t\t\tWHEN "
                     + _recurse_backwards(base_leaf)
                     + f"\n\t\tTHEN {leaves[base_leaf]}"
                 )
 
                 when_list.append(leaf_query)
```

### Comparing `xgb2sql-0.114/xgb2sql.egg-info/PKG-INFO` & `xgb2sql-0.115/xgb2sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgb2sql
-Version: 0.114
+Version: 0.115
 Summary: A simple library for converting the output of an XGB model to SQL.
 Home-page: https://github.com/Chryzanthemum/xgb2sql
 Author: Benjamin Jiang
 Author-email: benjamin.jiang@well.co
 License: Apache Software License 2.0
 Keywords: xgb2sql,xgb sql,xgboost sql,xgboost to sql,xgb to sql
 Classifier: Development Status :: 3 - Alpha
```

