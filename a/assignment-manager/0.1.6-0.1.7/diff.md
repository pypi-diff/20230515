# Comparing `tmp/assignment-manager-0.1.6.tar.gz` & `tmp/assignment-manager-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assignment-manager-0.1.6.tar", last modified: Tue May  9 06:25:04 2023, max compression
+gzip compressed data, was "assignment-manager-0.1.7.tar", last modified: Mon May 15 13:05:08 2023, max compression
```

## Comparing `assignment-manager-0.1.6.tar` & `assignment-manager-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-05-09 06:25:04.318008 assignment-manager-0.1.6/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     1074 2023-04-23 16:17:44.000000 assignment-manager-0.1.6/LICENSE
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-05-09 06:25:04.318008 assignment-manager-0.1.6/PKG-INFO
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       21 2023-04-23 16:24:52.000000 assignment-manager-0.1.6/README.md
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      129 2023-04-26 20:40:07.000000 assignment-manager-0.1.6/pyproject.toml
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       74 2023-05-09 06:25:04.318008 assignment-manager-0.1.6/setup.cfg
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     2136 2023-05-09 06:24:46.000000 assignment-manager-0.1.6/setup.py
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-05-09 06:25:04.314008 assignment-manager-0.1.6/src/
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-05-09 06:25:04.314008 assignment-manager-0.1.6/src/assignment_manager/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)        0 2023-04-23 16:35:05.000000 assignment-manager-0.1.6/src/assignment_manager/__init__.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     5193 2023-05-09 06:24:19.000000 assignment-manager-0.1.6/src/assignment_manager/assignments.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     1817 2023-04-28 15:55:50.000000 assignment-manager-0.1.6/src/assignment_manager/data.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     2461 2023-04-28 09:11:02.000000 assignment-manager-0.1.6/src/assignment_manager/io.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     1013 2023-04-28 09:09:32.000000 assignment-manager-0.1.6/src/assignment_manager/main.py
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-05-09 06:25:04.318008 assignment-manager-0.1.6/src/assignment_manager.egg-info/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-05-09 06:25:04.000000 assignment-manager-0.1.6/src/assignment_manager.egg-info/PKG-INFO
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      493 2023-05-09 06:25:04.000000 assignment-manager-0.1.6/src/assignment_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)        1 2023-05-09 06:25:04.000000 assignment-manager-0.1.6/src/assignment_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      106 2023-05-09 06:25:04.000000 assignment-manager-0.1.6/src/assignment_manager.egg-info/entry_points.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       20 2023-05-09 06:25:04.000000 assignment-manager-0.1.6/src/assignment_manager.egg-info/requires.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       19 2023-05-09 06:25:04.000000 assignment-manager-0.1.6/src/assignment_manager.egg-info/top_level.txt
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-05-15 13:05:08.300391 assignment-manager-0.1.7/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     1074 2023-04-23 16:17:44.000000 assignment-manager-0.1.7/LICENSE
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     4383 2023-05-15 13:05:08.300391 assignment-manager-0.1.7/PKG-INFO
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     3546 2023-05-15 12:27:11.000000 assignment-manager-0.1.7/README.md
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      129 2023-04-26 20:40:07.000000 assignment-manager-0.1.7/pyproject.toml
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       74 2023-05-15 13:05:08.300391 assignment-manager-0.1.7/setup.cfg
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     2136 2023-05-15 13:04:44.000000 assignment-manager-0.1.7/setup.py
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-05-15 13:05:08.300391 assignment-manager-0.1.7/src/
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-05-15 13:05:08.300391 assignment-manager-0.1.7/src/assignment_manager/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)        0 2023-04-23 16:35:05.000000 assignment-manager-0.1.7/src/assignment_manager/__init__.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     5500 2023-05-15 12:50:16.000000 assignment-manager-0.1.7/src/assignment_manager/assignments.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     1868 2023-05-15 12:48:46.000000 assignment-manager-0.1.7/src/assignment_manager/data.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     2498 2023-05-15 12:39:18.000000 assignment-manager-0.1.7/src/assignment_manager/io.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      971 2023-05-15 12:48:02.000000 assignment-manager-0.1.7/src/assignment_manager/main.py
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-05-15 13:05:08.300391 assignment-manager-0.1.7/src/assignment_manager.egg-info/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     4383 2023-05-15 13:05:08.000000 assignment-manager-0.1.7/src/assignment_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      493 2023-05-15 13:05:08.000000 assignment-manager-0.1.7/src/assignment_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)        1 2023-05-15 13:05:08.000000 assignment-manager-0.1.7/src/assignment_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      106 2023-05-15 13:05:08.000000 assignment-manager-0.1.7/src/assignment_manager.egg-info/entry_points.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       20 2023-05-15 13:05:08.000000 assignment-manager-0.1.7/src/assignment_manager.egg-info/requires.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       19 2023-05-15 13:05:08.000000 assignment-manager-0.1.7/src/assignment_manager.egg-info/top_level.txt
```

### Comparing `assignment-manager-0.1.6/LICENSE` & `assignment-manager-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `assignment-manager-0.1.6/setup.py` & `assignment-manager-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="assignment-manager",
-    version="0.1.6",
+    version="0.1.7",
     description=("Manage reoccuring assignments and tasks."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PraxTube/assignment-manager",
     author="Prax",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `assignment-manager-0.1.6/src/assignment_manager/assignments.py` & `assignment-manager-0.1.7/src/assignment_manager/assignments.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,18 @@
     for i, d in enumerate(assignment_data):
         if (datetime.strptime(d[1], "%d.%m.%Y") - current_date).days >= -1:
             return i
     return len(assignment_data) - 1
 
 
 def sort_data(row_data, sort_index, ascending=True):
-    if sort_index < 0 or sort_index >= len(row_data):
+    if len(row_data) == 0:
+        raise ValueError("The row data musn't be empty!", row_data)
+
+    if sort_index < 0 or sort_index >= len(row_data[0]):
         raise ValueError(
             "The given index must be in range of the row_data",
             sort_index,
             row_data,
         )
 
     row_data.sort(key=lambda x: x[sort_index], reverse=not ascending)
@@ -52,14 +55,21 @@
     return table_rows
 
 
 def show_all_assignments(sort):
     table_headers = ["Name", "Start", "Deadline", "Progress", "Days"]
     table_rows = get_table_rows()
 
+    if len(table_rows) == 0:
+        io.print_msg(
+            "\nYou have not added any assignments so far. "
+            "You can do that by running [bold]assman add[/bold]."
+        )
+        return
+
     if sort:
         sort_index = table_headers.index(
             io.list_prompt(table_headers, "Which to sort by?")
         )
         ascending = io.binary_prompt("Sort ascending?")
     else:
         sort_index = 4
@@ -112,15 +122,15 @@
 
     if data_file_empty():
         data = {}
     else:
         data = load_data()
 
     if params[0] in data:
-        raise ValueError("Name already exists!", name, data.keys())
+        raise ValueError("Name already exists!", params[0], data.keys())
 
     progress = generate_dates(params[1], params[2], params[3], params[4])
     data[params[0]] = progress
     write_data(data)
 
 
 def update_assignment():
```

### Comparing `assignment-manager-0.1.6/src/assignment_manager/data.py` & `assignment-manager-0.1.7/src/assignment_manager/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,15 +65,18 @@
 def get_backup_data_file_path():
     return join(get_backup_dir(), "data.json")
 
 
 def load_data():
     if data_file_empty():
         raise EOFError(
-            "The data file is empty. You should first add assignments before accessing them.",
+            (
+                "The data file is empty. "
+                "You should first add assignments before accessing them."
+            ),
             get_data_file_path(),
         )
     with open(get_data_file_path(), "r") as f:
         data = json.load(f)
     return data
```

### Comparing `assignment-manager-0.1.6/src/assignment_manager/io.py` & `assignment-manager-0.1.7/src/assignment_manager/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 
     table = RichTable(*table_headers)
     for row in table_rows:
         table.add_row(*row)
     print(table)
 
 
+def print_msg(msg):
+    print(msg)
+
+
 def confirmation_prompt(msg=""):
     if msg != "":
         print(msg)
 
     if binary_prompt("Are you sure you want to continue?"):
         return True
     print("[bold]Aborting...[/bold]")
```

### Comparing `assignment-manager-0.1.6/src/assignment_manager/main.py` & `assignment-manager-0.1.7/src/assignment_manager/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from datetime import datetime, timedelta
-
 import typer
 
 from assignment_manager import assignments
 
 
 app = typer.Typer()
 backup_app = typer.Typer()
```

