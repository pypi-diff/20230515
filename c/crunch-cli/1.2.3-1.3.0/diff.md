# Comparing `tmp/crunch-cli-1.2.3.tar.gz` & `tmp/crunch-cli-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-1.2.3.tar", last modified: Fri May 12 16:45:32 2023, max compression
+gzip compressed data, was "crunch-cli-1.3.0.tar", last modified: Mon May 15 11:21:11 2023, max compression
```

## Comparing `crunch-cli-1.2.3.tar` & `crunch-cli-1.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:45:32.764836 crunch-cli-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-12 16:45:32.764836 crunch-cli-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:45:32.756836 crunch-cli-1.2.3/crunch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:45:32.756836 crunch-cli-1.2.3/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:45:32.760836 crunch-cli-1.2.3/crunch/demo-project/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/demo-project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/demo-project/files.json
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/demo-project/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/demo-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:45:32.764836 crunch-cli-1.2.3/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-12 16:45:32.000000 crunch-cli-1.2.3/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-12 16:45:32.000000 crunch-cli-1.2.3/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:45:32.000000 crunch-cli-1.2.3/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 16:45:32.000000 crunch-cli-1.2.3/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:45:32.000000 crunch-cli-1.2.3/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 16:45:32.000000 crunch-cli-1.2.3/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 16:45:32.000000 crunch-cli-1.2.3/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 16:45:32.764836 crunch-cli-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-12 16:45:27.000000 crunch-cli-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:21:11.632765 crunch-cli-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-15 11:21:11.632765 crunch-cli-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:21:11.628765 crunch-cli-1.3.0/crunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:21:11.628765 crunch-cli-1.3.0/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:21:11.628765 crunch-cli-1.3.0/crunch/demo-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/demo-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/demo-project/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/demo-project/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/demo-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:21:11.632765 crunch-cli-1.3.0/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-15 11:21:11.000000 crunch-cli-1.3.0/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-15 11:21:11.000000 crunch-cli-1.3.0/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:21:11.000000 crunch-cli-1.3.0/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 11:21:11.000000 crunch-cli-1.3.0/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:21:11.000000 crunch-cli-1.3.0/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-15 11:21:11.000000 crunch-cli-1.3.0/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 11:21:11.000000 crunch-cli-1.3.0/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 11:21:11.632765 crunch-cli-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-15 11:21:06.000000 crunch-cli-1.3.0/setup.py
```

### Comparing `crunch-cli-1.2.3/crunch/command/convert.py` & `crunch-cli-1.3.0/crunch/command/convert.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.3/crunch/command/download.py` & `crunch-cli-1.3.0/crunch/command/download.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import typing
 import datetime
+import dataclasses
 
 import click
 import requests
 import tqdm
 
 from .. import constants, utils
 
@@ -25,119 +26,122 @@
     if url.endswith(".csv"):
         return "csv"
 
     print(f"unknown file extension: {url}")
     raise click.Abort()
 
 
+@dataclasses.dataclass
+class DataFile:
+
+    url: str
+    path: str
+    size: int
+    signed: bool
+
+
 def get_data_urls(
     session: utils.CustomSession,
     data_directory: str,
     push_token: str,
 ) -> typing.Tuple[typing.Dict[str, str], str, str, str]:
     current_crunch = session.get("/v1/crunches/@current").json()
     data_release = session.get(f"/v1/crunches/{current_crunch['number']}/data-release", params={
         "pushToken": push_token
     }).json()
 
     embargo = data_release["embargo"]
     moon_column_name = data_release["moonColumnName"]
-    urls = data_release["dataUrls"]
+    data_files = data_release["dataFiles"]
 
-    x_train_url = urls["xTrain"]
-    x_train_path = os.path.join(
-        data_directory,
-        f"X_train.{get_extension(x_train_url)}"
-    )
+    def get_file(key: str, file_name: str) -> DataFile:
+        data_file = data_files[key]
 
-    y_train_url = urls["yTrain"]
-    y_train_path = os.path.join(
-        data_directory,
-        f"y_train.{get_extension(y_train_url)}"
-    )
+        url = data_file["url"]
+        path = os.path.join(
+            data_directory,
+            f"{file_name}.{get_extension(url)}"
+        )
 
-    x_test_url = urls["xTest"]
-    x_test_path = os.path.join(
-        data_directory,
-        f"X_test.{get_extension(x_test_url)}"
-    )
+        size = data_file["size"]
+        signed = data_file["signed"]
 
-    data_urls = {
-        x_train_path: x_train_url,
-        y_train_path: y_train_url,
-        x_test_path: x_test_url,
-    }
+        return DataFile(url, path, size, signed)
+
+    x_train = get_file("xTrain", "X_train")
+    y_train = get_file("yTrain", "y_train")
+    x_test = get_file("xTest", "X_test")
 
     return (
         embargo,
         moon_column_name,
-        data_urls,
-        x_train_path,
-        y_train_path,
-        x_test_path
+        x_train,
+        y_train,
+        x_test
     )
 
 
-def _download(url: str, path: str, force: bool):
-    print(f"download {path} from {cut_url(url)}")
+def _download(data_file: DataFile, force: bool):
+    print(f"download {data_file.path} from {cut_url(data_file.url)}")
+
+    exists = os.path.exists(data_file.path)
+    if not force and exists:
+        stat = os.stat(data_file.path)
+        if stat.st_size == data_file.size:
+            print(f"already exists: file length match")
+            return
+
+    if not data_file.signed:
+        print(f"signature missing: cannot download file without being authenticated")
+        raise click.Abort()
 
-    with requests.get(url, stream=True) as response:
+    with requests.get(data_file.url, stream=True) as response:
         response.raise_for_status()
 
         file_length = response.headers.get("Content-Length", None)
         file_length = int(file_length) if not None else None
 
-        exists = os.path.exists(path)
-        if not force and exists:
-            if file_length is None:
-                print(f"already exists: skip since unknown size")
-                return
-
-            stat = os.stat(path)
-            if stat.st_size == file_length:
-                print(f"already exists: file length match")
-                return
-
-        with open(path, 'wb') as fd, tqdm.tqdm(total=file_length, unit='iB', unit_scale=True, leave=False) as progress:
+        with open(data_file.path, 'wb') as fd, tqdm.tqdm(total=file_length, unit='iB', unit_scale=True, leave=False) as progress:
             for chunk in response.iter_content(chunk_size=8192):
                 progress.update(len(chunk))
                 fd.write(chunk)
 
 
 def download(
     session: utils.CustomSession,
     force=False,
 ):
-    push_token = utils.read_token()
+    push_token = utils.read_token(raise_if_missing=False)
 
     os.makedirs(constants.DOT_DATA_DIRECTORY, exist_ok=True)
 
     (
         embargo,
         moon_column_name,
-        data_urls,
-        x_train_path,
-        y_train_path,
-        x_test_path
+        x_train,
+        y_train,
+        x_test
     ) = get_data_urls(session, constants.DOT_DATA_DIRECTORY, push_token)
 
-    for path, url in data_urls.items():
-        _download(url, path, force)
+    _download(x_train, force)
+    _download(y_train, force)
+    _download(x_test, force)
 
     return (
         embargo,
         moon_column_name,
-        x_train_path,
-        y_train_path,
-        x_test_path
+        x_train.path,
+        y_train.path,
+        x_test.path
     )
 
+
 def download_no_data_available():
     today = datetime.date.today()
-    
+
     print("\n---")
 
     # competition lunch
     if today <= datetime.date(2023, 5, 16):
         print("The data will be released on May 16th, 2023, 05.00 PM CET")
     else:
         print("No data is available yet")
```

### Comparing `crunch-cli-1.2.3/crunch/command/push.py` & `crunch-cli-1.3.0/crunch/command/push.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.3/crunch/command/setup.py` & `crunch-cli-1.3.0/crunch/command/setup.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.3/crunch/command/test.py` & `crunch-cli-1.3.0/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.3/crunch/constants.py` & `crunch-cli-1.3.0/crunch/constants.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.3/crunch/demo-project/.gitignore` & `crunch-cli-1.3.0/crunch/demo-project/.gitignore`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.3/crunch/demo-project/main.py` & `crunch-cli-1.3.0/crunch/demo-project/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.3/crunch/ensure.py` & `crunch-cli-1.3.0/crunch/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.3/crunch/inline.py` & `crunch-cli-1.3.0/crunch/inline.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.3/crunch/main.py` & `crunch-cli-1.3.0/crunch/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.3/crunch/tester.py` & `crunch-cli-1.3.0/crunch/tester.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.3/crunch/utils.py` & `crunch-cli-1.3.0/crunch/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,30 +87,34 @@
 
         os.chdir("../")
         if current == os.getcwd():
             print("no project found")
             raise click.Abort()
 
 
-def _read_crunchdao_file(name: str):
+def _read_crunchdao_file(name: str, raise_if_missing: bool):
     path = os.path.join(constants.DOT_CRUNCHDAO_DIRECTORY, name)
+
     if not os.path.exists(path):
-        print(f"{path}: not found, are you in a project directory?")
-        raise click.Abort()
+        if raise_if_missing:
+            print(f"{path}: not found, are you in a project directory?")
+            raise click.Abort()
+        
+        return None
 
     with open(path) as fd:
         return fd.read()
 
 
 def read_project_name():
-    return _read_crunchdao_file(constants.PROJECT_FILE)
+    return _read_crunchdao_file(constants.PROJECT_FILE, True)
 
 
-def read_token():
-    return _read_crunchdao_file(constants.TOKEN_FILE)
+def read_token(raise_if_missing=False):
+    return _read_crunchdao_file(constants.TOKEN_FILE, raise_if_missing)
 
 
 def read(path: str, dataframe=True) -> typing.Union[pandas.DataFrame, typing.Any]:
     if dataframe:
         if path.endswith(".parquet"):
             return pandas.read_parquet(path)
         return pandas.read_csv(path)
```

### Comparing `crunch-cli-1.2.3/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-1.3.0/crunch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.3/setup.py` & `crunch-cli-1.3.0/setup.py`

 * *Files identical despite different names*

