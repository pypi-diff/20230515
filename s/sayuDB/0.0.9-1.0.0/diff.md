# Comparing `tmp/sayuDB-0.0.9.tar.gz` & `tmp/sayuDB-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayuDB-0.0.9.tar", last modified: Sun Apr 23 22:39:44 2023, max compression
+gzip compressed data, was "sayuDB-1.0.0.tar", last modified: Mon May 15 18:53:30 2023, max compression
```

## Comparing `sayuDB-0.0.9.tar` & `sayuDB-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 22:39:44.354617 sayuDB-0.0.9/
--rw-rw-rw-   0        0        0     1085 2023-04-23 05:32:47.000000 sayuDB-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     9981 2023-04-23 22:39:44.354617 sayuDB-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     9672 2023-04-23 22:35:49.000000 sayuDB-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 22:39:44.325718 sayuDB-0.0.9/sayuDB/
--rw-rw-rw-   0        0        0      635 2023-04-23 05:32:47.000000 sayuDB-0.0.9/sayuDB/__init__.py
--rw-rw-rw-   0        0        0     4799 2023-04-23 22:36:18.000000 sayuDB-0.0.9/sayuDB/__main__.py
--rw-rw-rw-   0        0        0    21632 2023-04-23 06:25:51.000000 sayuDB-0.0.9/sayuDB/processor.py
--rw-rw-rw-   0        0        0     2042 2023-04-23 05:32:47.000000 sayuDB-0.0.9/sayuDB/remote.py
--rw-rw-rw-   0        0        0     3252 2023-04-23 05:32:47.000000 sayuDB-0.0.9/sayuDB/server.py
-drwxrwxrwx   0        0        0        0 2023-04-23 22:39:44.353614 sayuDB-0.0.9/sayuDB.egg-info/
--rw-rw-rw-   0        0        0     9981 2023-04-23 22:39:44.000000 sayuDB-0.0.9/sayuDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-04-23 22:39:44.000000 sayuDB-0.0.9/sayuDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 22:39:44.000000 sayuDB-0.0.9/sayuDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-23 22:39:44.000000 sayuDB-0.0.9/sayuDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-23 22:39:44.000000 sayuDB-0.0.9/sayuDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 22:39:44.354617 sayuDB-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0    10184 2023-04-23 22:37:07.000000 sayuDB-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 18:53:30.112789 sayuDB-1.0.0/
+-rw-rw-rw-   0        0        0     1085 2023-04-23 05:32:47.000000 sayuDB-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     9981 2023-05-15 18:53:30.112789 sayuDB-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10068 2023-05-15 18:43:51.000000 sayuDB-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 18:53:30.079787 sayuDB-1.0.0/sayuDB/
+-rw-rw-rw-   0        0        0      635 2023-04-23 05:32:47.000000 sayuDB-1.0.0/sayuDB/__init__.py
+-rw-rw-rw-   0        0        0     4847 2023-05-15 18:50:36.000000 sayuDB-1.0.0/sayuDB/__main__.py
+-rw-rw-rw-   0        0        0    21637 2023-05-15 18:46:50.000000 sayuDB-1.0.0/sayuDB/processor.py
+-rw-rw-rw-   0        0        0     2042 2023-04-23 05:32:47.000000 sayuDB-1.0.0/sayuDB/remote.py
+-rw-rw-rw-   0        0        0     3252 2023-04-23 05:32:47.000000 sayuDB-1.0.0/sayuDB/server.py
+drwxrwxrwx   0        0        0        0 2023-05-15 18:53:30.111172 sayuDB-1.0.0/sayuDB.egg-info/
+-rw-rw-rw-   0        0        0     9981 2023-05-15 18:53:29.000000 sayuDB-1.0.0/sayuDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-05-15 18:53:29.000000 sayuDB-1.0.0/sayuDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 18:53:29.000000 sayuDB-1.0.0/sayuDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-15 18:53:29.000000 sayuDB-1.0.0/sayuDB.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-05-15 18:53:29.000000 sayuDB-1.0.0/sayuDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-15 18:53:29.000000 sayuDB-1.0.0/sayuDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 18:53:30.113792 sayuDB-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0    10344 2023-05-15 18:49:44.000000 sayuDB-1.0.0/setup.py
```

### Comparing `sayuDB-0.0.9/LICENSE` & `sayuDB-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sayuDB-0.0.9/PKG-INFO` & `sayuDB-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sayuDB
-Version: 0.0.9
+Version: 1.0.0
 Summary: Database management system based on python and JSON.
 Home-page: https://github.com/Arsybai/sayuDB
 Author: Arsybai
 Author-email: me@arsybai.com
 License: MIT
 Keywords: database
 Description-Content-Type: text/markdown
```

### Comparing `sayuDB-0.0.9/README.md` & `sayuDB-1.0.0/sayuDB.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: sayuDB
+Version: 1.0.0
+Summary: Database management system based on python and JSON.
+Home-page: https://github.com/Arsybai/sayuDB
+Author: Arsybai
+Author-email: me@arsybai.com
+License: MIT
+Keywords: database
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![banner](https://images.arsybai.app/images/pOMsOCbxLR.png)
 ---
 # Preface
 ### What is sayuDB
 sayuDB is an database management system based on python and JSON. Developed at Clee Ltd. This project actually for personal purpose only but for some reason I publish it.
 It supports a large part of the SQL standard feature
```

### Comparing `sayuDB-0.0.9/sayuDB/__init__.py` & `sayuDB-1.0.0/sayuDB/__init__.py`

 * *Files identical despite different names*

### Comparing `sayuDB-0.0.9/sayuDB/__main__.py` & `sayuDB-1.0.0/sayuDB/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except:
     print("Read the doc here : https://github.com/Arsybai/blob/main/README.md")
     print("""Invalid commad. get help by
 --h""")
     exit()
 
 if sys.argv[1] == "help" or sys.argv[1] == '--h':
-    print("sayuDB v0.0.9\nRead the doc here : https://github.com/Arsybai/blob/main/README.md")
+    print("sayuDB v1.0.0\nRead the doc here : https://github.com/Arsybai/blob/main/README.md")
     print("""
 [ USERS ]
 Show Users  \t\t: show users
 Create user \t\t: create user <username> <password>
 Remove user \t\t: remove user <username>
 
 [ DATABASE ]
@@ -92,14 +92,15 @@
     print(f"Granted all privileges of {sys.argv[4]} to {sys.argv[3]}")
 
 elif sys.argv[1] == 'activate' and sys.argv[2] == 'server':
     import os, platform
     if platform.system() == 'Windows':
         os.system(f'py {os.path.dirname(__file__)}/server.py {sys.argv[3]}')
     else:
+        os.system(f"screen -X -S sayuDB kill")
         os.system(f"screen -dmS sayuDB")
         os.system(f"screen -S sayuDB -X stuff 'python3 {os.path.dirname(__file__)}/server.py {sys.argv[3]}\n'")
     print("Server activated. access it within your IP")
 
 elif sys.argv[1] == 'deactivate' and sys.argv[2] == 'server':
     import os, platform
     if platform.system() == 'Windows':
```

### Comparing `sayuDB-0.0.9/sayuDB/processor.py` & `sayuDB-1.0.0/sayuDB/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -445,15 +445,15 @@
         if set_col not in db_[table]['column']:
             sys.exit("Column not found")        
         for i in db_[table]['datas']:
             if 'contain' in where:
                 if str(val_) in str(i[col_]):
                     i[set_col] = set_val
             else:
-                if i[col_] == val_:
+                if str(i[col_]) == val_:
                     i[set_col] = set_val
         self.save_table(table, db_)
         return "Column updated"
     
     def update_row_json(self, table:str, set_:object, where:str):
         """
         set_ = {
```

### Comparing `sayuDB-0.0.9/sayuDB/remote.py` & `sayuDB-1.0.0/sayuDB/remote.py`

 * *Files identical despite different names*

### Comparing `sayuDB-0.0.9/sayuDB/server.py` & `sayuDB-1.0.0/sayuDB/server.py`

 * *Files identical despite different names*

### Comparing `sayuDB-0.0.9/sayuDB.egg-info/PKG-INFO` & `sayuDB-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,34 @@
-Metadata-Version: 2.1
-Name: sayuDB
-Version: 0.0.9
-Summary: Database management system based on python and JSON.
-Home-page: https://github.com/Arsybai/sayuDB
-Author: Arsybai
-Author-email: me@arsybai.com
-License: MIT
-Keywords: database
-Description-Content-Type: text/markdown
-License-File: LICENSE
+import setuptools
 
-![banner](https://images.arsybai.app/images/pOMsOCbxLR.png)
+setuptools.setup(
+    name="sayuDB",
+    version="1.0.0",
+    author="Arsybai",
+    description="Database management system based on python and JSON.",
+    packages=["sayuDB"],
+    license="MIT",
+    author_email="me@arsybai.com",
+    url="https://github.com/Arsybai/sayuDB",
+    keywords=[
+        'database',
+    ],
+    install_requires=[
+    'requests',
+    'tabulate',
+    'flask'
+    ],
+    entry_points={
+        "console_scripts": [
+            "sayuDB = sayuDB.__main__:main",
+            "sayudb = sayuDB.__main__:main"
+        ]
+    },
+    long_description_content_type="text/markdown",
+    long_description="""![banner](https://images.arsybai.app/images/pOMsOCbxLR.png)
 ---
 # Preface
 ### What is sayuDB
 sayuDB is an database management system based on python and JSON. Developed at Clee Ltd. This project actually for personal purpose only but for some reason I publish it.
 It supports a large part of the SQL standard feature
 
 # Tutorial
@@ -299,7 +313,9 @@
 ```
 ### Clear table
 To clear table use this following function
 ```python
 db.clear_table(table="<table_name>")
 ```
 This will erase all rows data in the table.
+"""
+)
```

### Comparing `sayuDB-0.0.9/setup.py` & `sayuDB-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,34 @@
-import setuptools
-
-setuptools.setup(
-    name="sayuDB",
-    version="0.0.9",
-    author="Arsybai",
-    description="Database management system based on python and JSON.",
-    packages=["sayuDB"],
-    license="MIT",
-    author_email="me@arsybai.com",
-    url="https://github.com/Arsybai/sayuDB",
-    keywords=[
-        'database',
-    ],
-    install_requires=[
-    'requests',
-    'tabulate',
-    'flask'
-    ],
-    long_description_content_type="text/markdown",
-    long_description="""![banner](https://images.arsybai.app/images/pOMsOCbxLR.png)
+![banner](https://images.arsybai.app/images/pOMsOCbxLR.png)
 ---
 # Preface
 ### What is sayuDB
 sayuDB is an database management system based on python and JSON. Developed at Clee Ltd. This project actually for personal purpose only but for some reason I publish it.
 It supports a large part of the SQL standard feature
 
 # Tutorial
 ##### Table of contents
 
 - [Installation](#installation)
-- [Create or remove user](#Create_or_remove_user)
-- [Grant privileges to user](#Grant_privileges_to_user)
-- [Create and drop database](#Create_and_drop_database)
-- [Import and export database](#Import_and_export_database)
-- [Activate or deactivate server](#Activate_or_deactivate_server)
-- [Using the sayuDB](#Using_the_sayuDB)
-- [Create table](#Create_table)
-- [Drop table](#Drop_table)
-- [Show table](#Show_table)
+- [Create or remove user](#Create-or-remove-user)
+- [Grant privileges to user](#Grant-privileges-to-user)
+- [Create and drop database](#Create-and-drop-database)
+- [Import and export database](#Import-and-export-database)
+- [Activate or deactivate server](#Activate-or-deactivate-server)
+- [Using the sayuDB](#Using-the-sayuDB)
+- [Create table](#Create-table)
+- [Drop table](#Drop-table)
+- [Show table](#Show-table)
 - [Insert](#Insert)
 - [Select](#Select)
 - [Where](#Where)
 - [Update](#Update)
 - [Delete](#Delete)
-- [Alter table](#Alter_table)
-- [Clear table](#Clear_table)
+- [Alter table](#Alter-table)
+- [Clear table](#Clear-table)
 ---
 
 ### Installation
 ```shell
 > pip3 install sayuDB
 ```
 and if you want to show help menu just 
@@ -307,9 +287,13 @@
 ```
 ### Clear table
 To clear table use this following function
 ```python
 db.clear_table(table="<table_name>")
 ```
 This will erase all rows data in the table.
-"""
-)
+
+---
+# V0.0.9 Changelog
+- `ADD` [Now you can define "as_json" in class](https://github.com/Arsybai/sayuDB/commit/7ce2f54a1b94d8174b7d60c4f988a62cceedfd2b)
+- `ADD` [Delete row with row number or between row number](https://github.com/Arsybai/sayuDB/commit/734748513524ee4b9ac7ff14054a9153d7984825)
+- `UPDATE` [Update the documentation](https://github.com/Arsybai/sayuDB/blob/main/README.md)
```

