# Comparing `tmp/xgb2sql-0.113.tar.gz` & `tmp/xgb2sql-0.114.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgb2sql-0.113.tar", last modified: Fri May 12 18:49:42 2023, max compression
+gzip compressed data, was "xgb2sql-0.114.tar", last modified: Mon May 15 16:30:17 2023, max compression
```

## Comparing `xgb2sql-0.113.tar` & `xgb2sql-0.114.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-12 18:49:42.613446 xgb2sql-0.113/
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     2348 2023-03-13 17:57:29.000000 xgb2sql-0.113/CONTRIBUTING.md
--rw-r--r--   0 benjaminjiang   (501) staff       (20)    11357 2023-03-13 17:09:07.000000 xgb2sql-0.113/LICENSE
--rw-r--r--   0 benjaminjiang   (501) staff       (20)      111 2023-03-13 17:09:07.000000 xgb2sql-0.113/MANIFEST.in
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     8281 2023-05-12 18:49:42.613127 xgb2sql-0.113/PKG-INFO
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     7514 2023-05-11 17:03:06.000000 xgb2sql-0.113/README.md
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     1752 2023-05-12 16:24:23.000000 xgb2sql-0.113/settings.ini
--rw-r--r--   0 benjaminjiang   (501) staff       (20)       38 2023-05-12 18:49:42.613903 xgb2sql-0.113/setup.cfg
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     1911 2023-05-11 18:25:54.000000 xgb2sql-0.113/setup.py
-drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-12 18:49:42.607272 xgb2sql-0.113/xgb2sql/
--rw-r--r--   0 benjaminjiang   (501) staff       (20)       22 2023-03-13 18:30:03.000000 xgb2sql-0.113/xgb2sql/__init__.py
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     7281 2023-05-12 18:35:10.000000 xgb2sql-0.113/xgb2sql/core.py
-drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-12 18:49:42.609314 xgb2sql-0.113/xgb2sql.egg-info/
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     8281 2023-05-12 18:49:42.000000 xgb2sql-0.113/xgb2sql.egg-info/PKG-INFO
--rw-r--r--   0 benjaminjiang   (501) staff       (20)      257 2023-05-12 18:49:42.000000 xgb2sql-0.113/xgb2sql.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminjiang   (501) staff       (20)        1 2023-05-12 18:49:42.000000 xgb2sql-0.113/xgb2sql.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminjiang   (501) staff       (20)        1 2023-05-11 18:39:29.000000 xgb2sql-0.113/xgb2sql.egg-info/not-zip-safe
--rw-r--r--   0 benjaminjiang   (501) staff       (20)        8 2023-05-12 18:49:42.000000 xgb2sql-0.113/xgb2sql.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-15 16:30:17.614424 xgb2sql-0.114/
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     2348 2023-03-13 17:57:29.000000 xgb2sql-0.114/CONTRIBUTING.md
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)    11357 2023-03-13 17:09:07.000000 xgb2sql-0.114/LICENSE
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)      111 2023-03-13 17:09:07.000000 xgb2sql-0.114/MANIFEST.in
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     8311 2023-05-15 16:30:17.613671 xgb2sql-0.114/PKG-INFO
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     7544 2023-05-12 18:56:46.000000 xgb2sql-0.114/README.md
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     1752 2023-05-15 16:23:09.000000 xgb2sql-0.114/settings.ini
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)       38 2023-05-15 16:30:17.614465 xgb2sql-0.114/setup.cfg
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     1911 2023-05-11 18:25:54.000000 xgb2sql-0.114/setup.py
+drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-15 16:30:17.612521 xgb2sql-0.114/xgb2sql/
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)       22 2023-03-13 18:30:03.000000 xgb2sql-0.114/xgb2sql/__init__.py
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     7422 2023-05-15 16:22:59.000000 xgb2sql-0.114/xgb2sql/core.py
+drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-15 16:30:17.613483 xgb2sql-0.114/xgb2sql.egg-info/
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     8311 2023-05-15 16:30:17.000000 xgb2sql-0.114/xgb2sql.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)      257 2023-05-15 16:30:17.000000 xgb2sql-0.114/xgb2sql.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)        1 2023-05-15 16:30:17.000000 xgb2sql-0.114/xgb2sql.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)        1 2023-05-11 18:39:29.000000 xgb2sql-0.114/xgb2sql.egg-info/not-zip-safe
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)        8 2023-05-15 16:30:17.000000 xgb2sql-0.114/xgb2sql.egg-info/top_level.txt
```

### Comparing `xgb2sql-0.113/CONTRIBUTING.md` & `xgb2sql-0.114/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xgb2sql-0.113/LICENSE` & `xgb2sql-0.114/LICENSE`

 * *Files identical despite different names*

### Comparing `xgb2sql-0.113/PKG-INFO` & `xgb2sql-0.114/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgb2sql
-Version: 0.113
+Version: 0.114
 Summary: A simple library for converting the output of an XGB model to SQL.
 Home-page: https://github.com/Chryzanthemum/xgb2sql
 Author: Benjamin Jiang
 Author-email: benjamin.jiang@well.co
 License: Apache Software License 2.0
 Keywords: xgb2sql,xgb sql,xgboost sql,xgboost to sql,xgb to sql
 Classifier: Development Status :: 3 - Alpha
@@ -43,14 +43,15 @@
 ## How to use
 
 So easy even I could do it!
 <div class="codecell" markdown="1">
 <div class="input_area" markdown="1">
 
 ```python
+from xgb2sql import core
 import xgboost as xgb
 from sklearn.datasets import load_breast_cancer
 from sklearn.model_selection import train_test_split
 
 X, y = load_breast_cancer(return_X_y=True)
 
 X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=0)
@@ -73,15 +74,15 @@
 </div>
 
 </div>
 <div class="codecell" markdown="1">
 <div class="input_area" markdown="1">
 
 ```python
-tree = xgb2sql(woo.get_booster(), 'breast_cancer')
+tree = core.xgb2sql(woo.get_booster(), 'breast_cancer')
 print(tree)
 ```
 
 </div>
 <div class="output_area" markdown="1">
 
     WITH booster_output AS (
```

### Comparing `xgb2sql-0.113/README.md` & `xgb2sql-0.114/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 ## How to use
 
 So easy even I could do it!
 <div class="codecell" markdown="1">
 <div class="input_area" markdown="1">
 
 ```python
+from xgb2sql import core
 import xgboost as xgb
 from sklearn.datasets import load_breast_cancer
 from sklearn.model_selection import train_test_split
 
 X, y = load_breast_cancer(return_X_y=True)
 
 X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=0)
@@ -53,15 +54,15 @@
 </div>
 
 </div>
 <div class="codecell" markdown="1">
 <div class="input_area" markdown="1">
 
 ```python
-tree = xgb2sql(woo.get_booster(), 'breast_cancer')
+tree = core.xgb2sql(woo.get_booster(), 'breast_cancer')
 print(tree)
 ```
 
 </div>
 <div class="output_area" markdown="1">
 
     WITH booster_output AS (
```

### Comparing `xgb2sql-0.113/settings.ini` & `xgb2sql-0.114/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = Chryzanthemum
 description = A simple library for converting the output of an XGB model to SQL. 
 keywords = xgb2sql, xgb sql, xgboost sql, xgboost to sql, xgb to sql
 author = Benjamin Jiang
 author_email = benjamin.jiang@well.co
 copyright = Well
 branch = master
-version = 0.113
+version = 0.114
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `xgb2sql-0.113/setup.py` & `xgb2sql-0.114/setup.py`

 * *Files identical despite different names*

### Comparing `xgb2sql-0.113/xgb2sql/core.py` & `xgb2sql-0.114/xgb2sql/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                     query_list.insert(0, text)
                     _recurse(next_node)
                 elif node["if_greater_than"] == prev_node:
                     text = f"({node['split_column']} >= {node['split_number']})"
                     query_list.insert(0, text)
                     _recurse(next_node)
             except:
-                query_list.insert(0, "TRUE = TRUE")
+                pass
 
         _recurse(first_node)
 
         s = "\n\t\t\tAND "
 
         return s.join(query_list)
 
@@ -193,29 +193,33 @@
     index_string = ",\n".join(index_list)
 
     leaf_list = []
     columns = []
     counter = 0
     for i in range(0, len(tree_json)):
         leaves, splits = _extract_values(tree_json[i], "leaf")
-        column_list = []
+        when_list = []
+        column = f"column_{counter}"
+        columns.append(column)
+        if len(leaves) == 1:
+            column_list = f"{leaves.values()[0]} AS {column}"
+        else:
+            for base_leaf in leaves:
+                print(leaves, base_leaf)
+                leaf_query = (
+                    "\t\t\tWHEN "
+                    + _recurse_backwards(base_leaf)
+                    + f"\n\t\tTHEN {leaves[base_leaf]}"
+                )
 
-        for base_leaf in leaves:
-            leaf_query = (
-                "\t\t\tWHEN "
-                + _recurse_backwards(base_leaf)
-                + f"\n\t\tTHEN {leaves[base_leaf]}"
-            )
+                when_list.append(leaf_query)
 
-            column_list.append(leaf_query)
 
-        column = f"column_{counter}"
-        column_list = "\t\tCASE\n" + ("\n").join(column_list) + f"\n\t\tEND AS {column}"
+            column_list = "\t\tCASE\n" + ("\n").join(when_list) + f"\n\t\tEND AS {column}"
 
-        columns.append(column)
         leaf_list.append(column_list)
         counter += 1
 
     if sql_type == "bigquery":
         output = _bq_eval(index_list)
     else:
         output = _psql_eval(index_list, leaf_list)
```

### Comparing `xgb2sql-0.113/xgb2sql.egg-info/PKG-INFO` & `xgb2sql-0.114/xgb2sql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgb2sql
-Version: 0.113
+Version: 0.114
 Summary: A simple library for converting the output of an XGB model to SQL.
 Home-page: https://github.com/Chryzanthemum/xgb2sql
 Author: Benjamin Jiang
 Author-email: benjamin.jiang@well.co
 License: Apache Software License 2.0
 Keywords: xgb2sql,xgb sql,xgboost sql,xgboost to sql,xgb to sql
 Classifier: Development Status :: 3 - Alpha
@@ -43,14 +43,15 @@
 ## How to use
 
 So easy even I could do it!
 <div class="codecell" markdown="1">
 <div class="input_area" markdown="1">
 
 ```python
+from xgb2sql import core
 import xgboost as xgb
 from sklearn.datasets import load_breast_cancer
 from sklearn.model_selection import train_test_split
 
 X, y = load_breast_cancer(return_X_y=True)
 
 X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=0)
@@ -73,15 +74,15 @@
 </div>
 
 </div>
 <div class="codecell" markdown="1">
 <div class="input_area" markdown="1">
 
 ```python
-tree = xgb2sql(woo.get_booster(), 'breast_cancer')
+tree = core.xgb2sql(woo.get_booster(), 'breast_cancer')
 print(tree)
 ```
 
 </div>
 <div class="output_area" markdown="1">
 
     WITH booster_output AS (
```

