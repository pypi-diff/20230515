# Comparing `tmp/satori_ci-1.2.5.tar.gz` & `tmp/satori_ci-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_ci-1.2.5.tar", last modified: Mon May 15 11:51:12 2023, max compression
+gzip compressed data, was "satori_ci-1.2.6.tar", last modified: Mon May 15 15:53:53 2023, max compression
```

## Comparing `satori_ci-1.2.5.tar` & `satori_ci-1.2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-03-28 19:49:33.588036 satori_ci-1.2.5/LICENSE
--rw-r--r--   0        0        0     4984 2023-03-28 19:49:33.588180 satori_ci-1.2.5/README.md
--rw-r--r--   0        0        0      646 2023-05-15 11:51:12.952517 satori_ci-1.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588599 satori_ci-1.2.5/src/satorici/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588697 satori_ci-1.2.5/src/satorici/classes/__init__.py
--rw-r--r--   0        0        0     4066 2023-05-15 11:50:47.464226 satori_ci-1.2.5/src/satorici/classes/api.py
--rw-r--r--   0        0        0     1770 2023-05-12 22:08:17.024021 satori_ci-1.2.5/src/satorici/classes/bundler.py
--rw-r--r--   0        0        0     2807 2023-05-12 22:08:17.024155 satori_ci-1.2.5/src/satorici/classes/playbooks.py
--rw-r--r--   0        0        0    20500 2023-05-15 11:50:47.464520 satori_ci-1.2.5/src/satorici/classes/satori.py
--rw-r--r--   0        0        0     9855 2023-05-15 11:50:47.464751 satori_ci-1.2.5/src/satorici/classes/utils.py
--rw-r--r--   0        0        0     1440 2023-05-12 22:08:17.024825 satori_ci-1.2.5/src/satorici/classes/validations.py
--rwxr-xr-x   0        0        0     6027 2023-05-12 22:08:17.025008 satori_ci-1.2.5/src/satorici/satori_module.py
--rw-r--r--   0        0        0    46006 1970-01-01 00:00:00.000000 satori_ci-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-28 19:49:33.588036 satori_ci-1.2.6/LICENSE
+-rw-r--r--   0        0        0     4984 2023-05-15 15:49:56.139568 satori_ci-1.2.6/README.md
+-rw-r--r--   0        0        0      646 2023-05-15 15:53:53.559390 satori_ci-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588599 satori_ci-1.2.6/src/satorici/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588697 satori_ci-1.2.6/src/satorici/classes/__init__.py
+-rw-r--r--   0        0        0     4066 2023-05-15 12:33:16.870027 satori_ci-1.2.6/src/satorici/classes/api.py
+-rw-r--r--   0        0        0     1770 2023-05-15 12:33:16.870199 satori_ci-1.2.6/src/satorici/classes/bundler.py
+-rw-r--r--   0        0        0     2807 2023-05-15 12:33:16.870273 satori_ci-1.2.6/src/satorici/classes/playbooks.py
+-rw-r--r--   0        0        0    20500 2023-05-15 12:33:16.870475 satori_ci-1.2.6/src/satorici/classes/satori.py
+-rw-r--r--   0        0        0    10143 2023-05-15 15:49:56.139735 satori_ci-1.2.6/src/satorici/classes/utils.py
+-rw-r--r--   0        0        0     1440 2023-05-15 12:33:16.870721 satori_ci-1.2.6/src/satorici/classes/validations.py
+-rwxr-xr-x   0        0        0     6027 2023-05-15 12:33:16.870846 satori_ci-1.2.6/src/satorici/satori_module.py
+-rw-r--r--   0        0        0    46006 1970-01-01 00:00:00.000000 satori_ci-1.2.6/PKG-INFO
```

### Comparing `satori_ci-1.2.5/LICENSE` & `satori_ci-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.5/README.md` & `satori_ci-1.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -156,25 +156,25 @@
 ```
 
 # Playbooks:
 
 You can see a list of public playbooks when at https://github.com/satorici/playbooks/
 
 ```sh
-$ satori-cli playbooks
+$ satori-cli playbook
 Private playbooks:
 Public Playbooks:
 ```
 
 ## Public playbooks:
 
 They can be imported by playbooks that you have in your CI or on assets being Monitored.
 
 ```sh
-$ satori-cli playbooks public
+$ satori-cli playbook --public
 URI                          | Name                                            
 satori://code/trufflehog.yml | Trufflehog will search for secrets in your code 
 ...
 ```
 
 ## Private Playbooks:
```

### Comparing `satori_ci-1.2.5/pyproject.toml` & `satori_ci-1.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-ci"
-version = "1.2.5"
+version = "1.2.6"
 description = "Satori CI - Automated Software Testing Platform"
 authors = [
     { name = "Satori CI CLI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyyaml>=6.0",
```

### Comparing `satori_ci-1.2.5/src/satorici/classes/api.py` & `satori_ci-1.2.6/src/satorici/classes/api.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.5/src/satorici/classes/bundler.py` & `satori_ci-1.2.6/src/satorici/classes/bundler.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.5/src/satorici/classes/playbooks.py` & `satori_ci-1.2.6/src/satorici/classes/playbooks.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.5/src/satorici/classes/satori.py` & `satori_ci-1.2.6/src/satorici/classes/satori.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.5/src/satorici/classes/utils.py` & `satori_ci-1.2.6/src/satorici/classes/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from rich.logging import RichHandler
 import logging
 from rich import print_json
 from rich.console import Console
 from rich.syntax import Syntax
 from rich.table import Table
 import random
+from attr import dataclass
 
 __decorations = "▢•○░"
 __random_colors = ["green", "blue", "red"]
 # IDs
 UUID4_REGEX = re.compile(
     r"[0-9a-f]{8}-[0-9a-f]{4}-4[0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}",
     re.I,
@@ -271,56 +272,71 @@
             else:
                 styled = i
             cells.append(styled)
         table.add_row(*cells)
     console.log(table)
 
 
+@dataclass
 class argument:
-    def __init__(self) -> None:
-        self.id = str()
-        self.action = str()
-        self.profile = str()
-        self.debug = bool()
-        self.json = bool()
-        self.path = str()
-        self.data = Any
-        self.sync = bool()
-        self.timeout = int()
-        self.playbook = str()
-        self.page = int()
-        self.public = bool()
+    id: str
+    action: str
+    profile: str
+    debug: bool
+    json: bool
+    path: str
+    data: Any
+    sync: bool
+    timeout: int
+    playbook: str
+    page: int
+    public: bool
 
 
 def autotable(items: list[dict], header_style=None, numerate=False) -> None:
     """Print a list of dictionaries like a table
 
     Parameters
     ----------
     items : list[dict]
         The list, ex: [{"id":1,"name":"one"},{"id":2,"name":"two"}]
     header_style : _type_, optional
         Rich Table header style, by default None
     numerate : bool, optional
         Add numeration, by default False
     """
-    headers = ["N°"] if numerate else []
-    # get headers
+    h = get_headers(items)
+    headers = ["N°", *h] if numerate else h
+    rows = get_rows(items, headers)
+    table_generator(capitalize_list(headers), rows, header_style)
+
+
+def get_headers(items: list[dict]) -> list[str]:
+    headers = []
     for i in items:
         for h in i.keys():
+            h = str(h)
             if h not in headers:
                 headers.append(h)
+    return headers
+
+
+def get_rows(items: list[dict], headers: list[str]) -> list[list]:
     rows = []
-    # get rows
     n = 0
     for item in items:
         n += 1
         row = []
         for key in headers:
-            if key == "N°":
+            if key == "N°":  # add numeration
                 row.append(str(n))
             elif key in item:
                 row.append(item[key])
             else:
                 row.append("")
         rows.append(row)
-    table_generator(headers, rows, header_style)
+    return rows
+
+
+def capitalize_list(items: list[str]) -> list[str]:
+    new_list = map(lambda x: x.capitalize() if len(x) > 2 else x.upper(), items)
+    return list(new_list)
```

### Comparing `satori_ci-1.2.5/src/satorici/classes/validations.py` & `satori_ci-1.2.6/src/satorici/classes/validations.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.5/src/satorici/satori_module.py` & `satori_ci-1.2.6/src/satorici/satori_module.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.5/PKG-INFO` & `satori_ci-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-ci
-Version: 1.2.5
+Version: 1.2.6
 Summary: Satori CI - Automated Software Testing Platform
 Author-Email: Satori CI CLI <info@satori-ci.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -846,25 +846,25 @@
 ```
 
 # Playbooks:
 
 You can see a list of public playbooks when at https://github.com/satorici/playbooks/
 
 ```sh
-$ satori-cli playbooks
+$ satori-cli playbook
 Private playbooks:
 Public Playbooks:
 ```
 
 ## Public playbooks:
 
 They can be imported by playbooks that you have in your CI or on assets being Monitored.
 
 ```sh
-$ satori-cli playbooks public
+$ satori-cli playbook --public
 URI                          | Name                                            
 satori://code/trufflehog.yml | Trufflehog will search for secrets in your code 
 ...
 ```
 
 ## Private Playbooks:
```

