# Comparing `tmp/list-cli-0.1.1.tar.gz` & `tmp/list-cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list-cli-0.1.1.tar", last modified: Mon May 15 18:28:49 2023, max compression
+gzip compressed data, was "list-cli-0.1.2.tar", last modified: Mon May 15 18:51:20 2023, max compression
```

## Comparing `list-cli-0.1.1.tar` & `list-cli-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:28:49.233342 list-cli-0.1.1/
--rw-r--r--   0 jzaleski   (501) staff       (20)     1076 2023-05-15 02:28:40.000000 list-cli-0.1.1/LICENSE
--rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-15 18:28:49.233420 list-cli-0.1.1/PKG-INFO
--rw-r--r--   0 jzaleski   (501) staff       (20)     2569 2023-05-15 02:28:40.000000 list-cli-0.1.1/README.md
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:28:49.232501 list-cli-0.1.1/list_cli/
--rw-r--r--   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:28:18.000000 list-cli-0.1.1/list_cli/__init__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)     1490 2023-05-15 18:28:42.000000 list-cli-0.1.1/list_cli/__main__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)       22 2023-05-15 18:28:42.000000 list-cli-0.1.1/list_cli/__version__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)    10465 2023-05-15 18:28:18.000000 list-cli-0.1.1/list_cli/processors.py
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:28:49.233217 list-cli-0.1.1/list_cli.egg-info/
--rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-15 18:28:49.000000 list-cli-0.1.1/list_cli.egg-info/PKG-INFO
--rw-r--r--   0 jzaleski   (501) staff       (20)      288 2023-05-15 18:28:49.000000 list-cli-0.1.1/list_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)        1 2023-05-15 18:28:49.000000 list-cli-0.1.1/list_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)       52 2023-05-15 18:28:49.000000 list-cli-0.1.1/list_cli.egg-info/entry_points.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)        9 2023-05-15 18:28:49.000000 list-cli-0.1.1/list_cli.egg-info/top_level.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)       79 2023-05-15 18:28:49.233798 list-cli-0.1.1/setup.cfg
--rw-r--r--   0 jzaleski   (501) staff       (20)     1741 2023-05-15 18:28:18.000000 list-cli-0.1.1/setup.py
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:51:20.758345 list-cli-0.1.2/
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1076 2023-05-15 02:28:40.000000 list-cli-0.1.2/LICENSE
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-15 18:51:20.758444 list-cli-0.1.2/PKG-INFO
+-rw-r--r--   0 jzaleski   (501) staff       (20)     2569 2023-05-15 02:28:40.000000 list-cli-0.1.2/README.md
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:51:20.757376 list-cli-0.1.2/list_cli/
+-rw-r--r--   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:28:18.000000 list-cli-0.1.2/list_cli/__init__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1490 2023-05-15 18:28:42.000000 list-cli-0.1.2/list_cli/__main__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)       22 2023-05-15 18:50:54.000000 list-cli-0.1.2/list_cli/__version__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)    10642 2023-05-15 18:48:30.000000 list-cli-0.1.2/list_cli/processors.py
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:51:20.758191 list-cli-0.1.2/list_cli.egg-info/
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-15 18:51:20.000000 list-cli-0.1.2/list_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jzaleski   (501) staff       (20)      288 2023-05-15 18:51:20.000000 list-cli-0.1.2/list_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)        1 2023-05-15 18:51:20.000000 list-cli-0.1.2/list_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)       52 2023-05-15 18:51:20.000000 list-cli-0.1.2/list_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)        9 2023-05-15 18:51:20.000000 list-cli-0.1.2/list_cli.egg-info/top_level.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)       79 2023-05-15 18:51:20.758663 list-cli-0.1.2/setup.cfg
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1741 2023-05-15 18:28:18.000000 list-cli-0.1.2/setup.py
```

### Comparing `list-cli-0.1.1/LICENSE` & `list-cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.1/PKG-INFO` & `list-cli-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: List Management Application (CLI)
 Home-page: https://github.com/jzaleski/list-cli
 Author: Jonathan W. Zaleski
 Author-email: JonathanZaleski@gmail.com
 License: MIT
 Keywords: list,list-cli,tasktodo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `list-cli-0.1.1/README.md` & `list-cli-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.1/list_cli/__main__.py` & `list-cli-0.1.2/list_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.1/list_cli/processors.py` & `list-cli-0.1.2/list_cli/processors.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,20 @@
     ):
         self._database_file_paths = database_file_paths
         self._output_file_paths = output_file_paths
 
     def process(self, *args):
         had_error = False
         for index, database_file_path in enumerate(self._database_file_paths):
-            output_file_paths = self._output_file_paths
-            if index > 0 and output_file_paths:
-                print()
-            if not Processor(database_file_path, output_file_paths).process(*args):
+            processor = Processor(
+                database_file_path,
+                database_index=index,
+                output_file_path=self._output_file_paths
+            )
+            if not processor.process(*args):
                 had_error = True
         return not had_error
 
 
 class Processor():
     ADDED_BUCKET = 'a'
     ADD_OPERATIONS = {'a', 'add'}
@@ -54,18 +56,20 @@
         MOVED_BUCKET,
         REMOVED_BUCKET,
     }
 
     def __init__(
         self,
         database_file_path,
+        database_index=0,
         output_file_path=False
     ):
         self._database_file_path = database_file_path
         self._ensure_database_exists()
+        self._database_index = database_index
         self._output_file_path = output_file_path
 
     @property
     def _database(self):
         if not hasattr(self, '_database_'):
             self._database_ = self._get_database()
         return self._database_
@@ -210,25 +214,26 @@
                     continue
                 bucket = line_parts[6]
                 if bucket not in self.VALID_BUCKETS:
                     continue
                 message = line_parts[7]
                 if not message:
                     continue
-                datum = {
-                    'id': UUID(id_),
-                    'parent_id': UUID(parent_id),
-                    'created_by_user': created_by_user,
-                    'updated_by_user': updated_by_user,
-                    'created_timestamp': int(created_timestamp),
-                    'updated_timestamp': int(updated_timestamp),
-                    'bucket': bucket,
-                    'message': message,
-                }
-                database.append(datum)
+                database.append(
+                    {
+                        'id': UUID(id_),
+                        'parent_id': UUID(parent_id),
+                        'created_by_user': created_by_user,
+                        'updated_by_user': updated_by_user,
+                        'created_timestamp': int(created_timestamp),
+                        'updated_timestamp': int(updated_timestamp),
+                        'bucket': bucket,
+                        'message': message,
+                    }
+                )
         return database
 
     def _get_timestamp(self):
         return int(time())
 
     def _get_user(self):
         return getuser()
@@ -273,15 +278,15 @@
         return False
 
     def _render(self, bucket):
         bucket = self._get_bucket(bucket)
         if not bucket:
             return bucket != self.ADDED_BUCKET
         if self._output_file_path:
-            print(f'{self._database_file_path}:\n')
+            print(f'{linesep if self._database_index else ""}{self._database_file_path}:{linesep}')
         for datum_index, datum in enumerate(bucket):
             print('%3d. %s' % (datum_index + 1, datum['message']))
         return True
 
     def _touch(self, index=None):
         bucket = self._get_bucket(self.ADDED_BUCKET)
         if not bucket:
```

### Comparing `list-cli-0.1.1/list_cli.egg-info/PKG-INFO` & `list-cli-0.1.2/list_cli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: List Management Application (CLI)
 Home-page: https://github.com/jzaleski/list-cli
 Author: Jonathan W. Zaleski
 Author-email: JonathanZaleski@gmail.com
 License: MIT
 Keywords: list,list-cli,tasktodo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `list-cli-0.1.1/setup.py` & `list-cli-0.1.2/setup.py`

 * *Files identical despite different names*

