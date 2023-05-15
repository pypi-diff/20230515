# Comparing `tmp/satori_ci-1.2.4.tar.gz` & `tmp/satori_ci-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_ci-1.2.4.tar", last modified: Fri May 12 21:33:04 2023, max compression
+gzip compressed data, was "satori_ci-1.2.5.tar", last modified: Mon May 15 11:51:12 2023, max compression
```

## Comparing `satori_ci-1.2.4.tar` & `satori_ci-1.2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-03-28 19:49:33.588036 satori_ci-1.2.4/LICENSE
--rw-r--r--   0        0        0     4984 2023-03-28 19:49:33.588180 satori_ci-1.2.4/README.md
--rw-r--r--   0        0        0      646 2023-05-12 21:33:04.773533 satori_ci-1.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588599 satori_ci-1.2.4/src/satorici/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588697 satori_ci-1.2.4/src/satorici/classes/__init__.py
--rw-r--r--   0        0        0     4270 2023-05-12 21:32:46.495727 satori_ci-1.2.4/src/satorici/classes/api.py
--rw-r--r--   0        0        0     1770 2023-05-12 21:32:46.495905 satori_ci-1.2.4/src/satorici/classes/bundler.py
--rw-r--r--   0        0        0     2807 2023-05-12 21:32:46.496024 satori_ci-1.2.4/src/satorici/classes/playbooks.py
--rw-r--r--   0        0        0    21020 2023-05-12 21:32:46.496333 satori_ci-1.2.4/src/satorici/classes/satori.py
--rw-r--r--   0        0        0     9016 2023-05-12 21:32:46.496583 satori_ci-1.2.4/src/satorici/classes/utils.py
--rw-r--r--   0        0        0     1440 2023-05-12 21:32:46.496752 satori_ci-1.2.4/src/satorici/classes/validations.py
--rwxr-xr-x   0        0        0     6027 2023-05-12 21:32:46.496979 satori_ci-1.2.4/src/satorici/satori_module.py
--rw-r--r--   0        0        0    46006 1970-01-01 00:00:00.000000 satori_ci-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-28 19:49:33.588036 satori_ci-1.2.5/LICENSE
+-rw-r--r--   0        0        0     4984 2023-03-28 19:49:33.588180 satori_ci-1.2.5/README.md
+-rw-r--r--   0        0        0      646 2023-05-15 11:51:12.952517 satori_ci-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588599 satori_ci-1.2.5/src/satorici/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588697 satori_ci-1.2.5/src/satorici/classes/__init__.py
+-rw-r--r--   0        0        0     4066 2023-05-15 11:50:47.464226 satori_ci-1.2.5/src/satorici/classes/api.py
+-rw-r--r--   0        0        0     1770 2023-05-12 22:08:17.024021 satori_ci-1.2.5/src/satorici/classes/bundler.py
+-rw-r--r--   0        0        0     2807 2023-05-12 22:08:17.024155 satori_ci-1.2.5/src/satorici/classes/playbooks.py
+-rw-r--r--   0        0        0    20500 2023-05-15 11:50:47.464520 satori_ci-1.2.5/src/satorici/classes/satori.py
+-rw-r--r--   0        0        0     9855 2023-05-15 11:50:47.464751 satori_ci-1.2.5/src/satorici/classes/utils.py
+-rw-r--r--   0        0        0     1440 2023-05-12 22:08:17.024825 satori_ci-1.2.5/src/satorici/classes/validations.py
+-rwxr-xr-x   0        0        0     6027 2023-05-12 22:08:17.025008 satori_ci-1.2.5/src/satorici/satori_module.py
+-rw-r--r--   0        0        0    46006 1970-01-01 00:00:00.000000 satori_ci-1.2.5/PKG-INFO
```

### Comparing `satori_ci-1.2.4/LICENSE` & `satori_ci-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.4/README.md` & `satori_ci-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.4/pyproject.toml` & `satori_ci-1.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-ci"
-version = "1.2.4"
+version = "1.2.5"
 description = "Satori CI - Automated Software Testing Platform"
 authors = [
     { name = "Satori CI CLI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyyaml>=6.0",
```

### Comparing `satori_ci-1.2.4/src/satorici/classes/api.py` & `satori_ci-1.2.5/src/satorici/classes/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 import sys
 from requests import Response
-from requests.exceptions import ConnectionError, ReadTimeout, HTTPError
+from requests.exceptions import HTTPError
 from typing import Union, Any
 from argparse import Namespace
 
 from satorici.classes.utils import FAIL_COLOR, puts, autoformat, log, argument
 
 HOST = "https://api.satori-ci.com"
 
@@ -34,42 +34,38 @@
     ) -> Response:
         url = f"{self.server}/{endpoint}"
         try:
             resp = self.__session__.request(
                 method=method, url=url, timeout=self.timeout, **kwargs
             )
             log.debug(resp.headers)
-        except (ConnectionError, ReadTimeout, HTTPError) as e:
+        except HTTPError as e:
             if raise_error:
                 raise e
+            # Show reponse messages when server response is not 20x
+            res: Response = e.response
+            log.debug("Response headers:")
+            log.debug(res.headers)
             try:
-                res: Response = e.response  # can fail if is not a HTTPError
-            except Exception as e:
-                log.debug(e, stack_info=True)
-                puts(FAIL_COLOR, "Error")
+                status = res.json()
+            except Exception:
+                status = res.text
+            if self.debug:
+                autoformat(status, capitalize=True, color=FAIL_COLOR, jsonfmt=self.json)
             else:
-                log.debug("Response headers:")
-                log.debug(res.headers)
-                try:
-                    status = res.json()
-                except Exception:
-                    status = res.text
-                if self.debug:
-                    autoformat(
-                        status, capitalize=True, color=FAIL_COLOR, jsonfmt=self.json
-                    )
-                else:
-                    msg = "Error"
-                    if isinstance(status, dict) and "detail" in status:
-                        msg += f": {status['detail']}"
-                    puts(FAIL_COLOR, msg)
-            finally:
-                sys.exit(1)
-        else:
+                msg = "Error"
+                if isinstance(status, dict) and "detail" in status:
+                    msg += f": {status['detail']}"
+                puts(FAIL_COLOR, msg)
+        except Exception as e:
+            puts(FAIL_COLOR, "Error")
+            log.debug(e)
+        else:  # response is 20x
             return resp
+        sys.exit(1)
 
     def runs(self, run_type: str, secrets: str) -> Any:
         res = self.request("POST", f"runs/{run_type}", json={"secrets": secrets})
         return res.json()
 
     def repos(self, method: str, repo: str, action: str, **kwargs) -> Any:
         res = self.request(method, f"repos/{repo}/{action}", **kwargs)
```

### Comparing `satori_ci-1.2.4/src/satorici/classes/bundler.py` & `satori_ci-1.2.5/src/satorici/classes/bundler.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.4/src/satorici/classes/playbooks.py` & `satori_ci-1.2.5/src/satorici/classes/playbooks.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.4/src/satorici/classes/satori.py` & `satori_ci-1.2.5/src/satorici/classes/satori.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     FAIL_COLOR,
     KEYNAME_COLOR,
     SATORIURL_COLOR,
     VALUE_COLOR,
     UUID4_REGEX,
     autocolor,
     puts,
-    table_generator,
     argument,
     log,
+    autotable,
 )
 from satorici.classes.validations import get_parameters, validate_parameters
 from satorici.classes.playbooks import display_public_playbooks
 
 
 class Satori:
     """Have some class"""
@@ -119,33 +119,33 @@
         path = Path(args.path)
         params = set()
 
         if getattr(args, "data", False):
             try:
                 data = ast.literal_eval(args.data)
 
-                if not validate_parameters(args.data):
-                    raise
+                if not validate_parameters(data):
+                    raise ValueError("Malformed parameters")
 
                 params.update(data.keys())
-            except Exception:
-                puts(FAIL_COLOR, "Malformed parameters")
+            except Exception as e:
+                puts(FAIL_COLOR, str(e))
                 sys.exit(1)
 
         if path.is_dir():
             playbook = path / ".satori.yml"
         elif path.is_file():
             playbook = path
         else:
             puts(FAIL_COLOR, "Satori can not access to file/folder")
             sys.exit(1)
 
         with playbook.open() as f:
             variables = get_parameters(yaml.safe_load(f))
-            if variables != params:
+            if variables - params:
                 puts(FAIL_COLOR, f"Required parameters: {variables - params}")
                 sys.exit(1)
 
         if path.is_dir():
             exec_data = self.run_folder(args)
         else:  # is file
             exec_data = self.run_file(args)
@@ -375,19 +375,20 @@
             info = self.api.repos("GET", args.id, args.action, params=params)
         else:
             puts(FAIL_COLOR, "Unknown subcommand")
             sys.exit(1)
 
         if args.id != "" or args.action != "" or args.json:
             autoformat(info, jsonfmt=args.json, list_separator="-" * 48)
-        else:
-            print("Pending actions:")
-            autoformat(info["pending"])
+        else:  # Default command (satori-cli repo)
+            if len(info["pending"]) > 1:
+                print("Pending actions:")
+                autotable(info["pending"], "bold red")
             print("\nRepos:")
-            autoformat(info["list"], list_separator="-" * 48)
+            autotable(info["list"], "bold blue")
         if args.action == "run" and args.sync:
             if isinstance(info, list):
                 info = info[0]
             report = info.get("status", "")
             match = UUID4_REGEX.findall(report)
             if match:
                 self.run_sync({"type": "report", "id": match[0]})
@@ -430,20 +431,20 @@
         elif args.action in ("start", "stop"):
             info = self.api.monitors("PATCH", args.id, args.action)
         else:
             print("Unknown subcommand")
             sys.exit(1)
         if args.id != "" or args.action != "" or args.json:
             autoformat(info, jsonfmt=args.json, list_separator="*" * 48)
-        else:
+        else:  # Default command (satori-cli monitor)
             if len(info["pending"]) > 1:
                 print("Pending actions:")
-                autoformat(info["pending"])
+                autotable(info["pending"], "bold red")
             print("\nMonitors:")
-            autoformat(info["list"], list_separator="-" * 48, table=True)
+            autotable(info["list"], "bold blue")
 
     def output(self, args, params):
         """Returns commands output"""
         try:
             uuid.UUID(args.id)
         except ValueError:
             puts(FAIL_COLOR, f"{args.id} is not a valid report ID")
@@ -475,47 +476,32 @@
 
     def dashboard(self, args: Union[Namespace, argument]):
         """Get user dashboard"""
         info = self.api.dashboard()
         if args.json:
             autoformat(info, jsonfmt=True)
         else:
-            len_mon = len(info["Actions"]["Monitors"])
-            len_rep = len(info["Actions"]["Repos"])
+            len_mon = len(info["monitors"]["pending"])
+            len_rep = len(info["repos"]["pending"])
             if len_mon > 0 or len_rep > 0:
                 # print pending actions
                 if len_mon > 0:
                     print("Monitors(Actions required):")
-                    mon_items = []
-                    for m in info["Actions"]["Monitors"]:
-                        for key in m:
-                            mon_items.append([key, m[key]])
-                    table_generator(["Name", "Pending action"], mon_items, "bold green")
+                    autotable(info["monitors"]["pending"], "bold green")
                 if len_rep > 0:
                     print("Repos(Actions required):")
-                    rep_items = []
-                    for r in info["Actions"]["Repos"]:
-                        for key in r:
-                            rep_items.append([key, r[key]])
-                    table_generator(["Name", "Pending action"], rep_items, "bold green")
-            for title in info:
-                if title == "Actions":
-                    continue
-                if title == "Monitors":
-                    if len(info[title]) == 0:
-                        print("\nMonitors: no active monitors defined")
-                        continue
-                print(f"\n{title}:")
-                items = []
-                n = 0
-                for i in info[title]:
-                    n += 1
-                    for key in i:
-                        items.append([str(n), key, i[key]])
-                table_generator(["Nº", "Name", "Status"], items, "bold blue")
+                    autotable(info["repos"]["pending"], "bold green")
+            if len(info["monitors"]["list"]) == 0:
+                print("\nMonitors: no active monitors defined")
+            else:
+                print("Monitors:")
+                autotable(info["monitors"]["list"], "bold blue", True)
+            if len(info["repos"]["list"]) > 0:
+                print("Repos:")
+                autotable(info["repos"]["list"], "bold blue", True)
 
     def playbook(self, args: Union[Namespace, argument]):
         """Get playbooks"""
         if args.public:
             display_public_playbooks()
 
         if args.action == "":
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `satori_ci-1.2.4/src/satorici/classes/utils.py` & `satori_ci-1.2.5/src/satorici/classes/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -237,21 +237,33 @@
             return True
     else:  # Is JSON
         print()
         print_json(item, indent=ind)
         return True
 
 
-def table_generator(headers: list, items: list, header_style=None):
+def table_generator(headers: list[str], items: list[list], header_style=None):
+    """Print a rich table
+
+    Parameters
+    ----------
+    headers : list
+        A list of the headers names, ex: ["header1","header2"]
+    items : list
+        A list of rows with cells, ex: [["row1-1","row1-2"],["row2-1","row2-2"]]
+    header_style : _type_, optional
+        Rich Table header style, by default None
+    """
     table = Table(show_header=True, header_style=header_style)
     for header in headers:
         table.add_column(header)
     for item in items:
         cells = []
-        for i in item:
+        for raw_i in item:
+            i = str(raw_i)
             if PASS_REGEX.search(i):
                 styled = "[green]" + i
             elif FAIL_REGEX.search(i):
                 styled = "[red]" + i
             elif UNKNOWN_REGEX.search(i):
                 styled = "[yellow]" + i
             elif RUNNING_REGEX.search(i):
@@ -275,25 +287,40 @@
         self.sync = bool()
         self.timeout = int()
         self.playbook = str()
         self.page = int()
         self.public = bool()
 
 
-def autotable(items: list[dict], header_style=None) -> None:
-    headers = []
+def autotable(items: list[dict], header_style=None, numerate=False) -> None:
+    """Print a list of dictionaries like a table
+
+    Parameters
+    ----------
+    items : list[dict]
+        The list, ex: [{"id":1,"name":"one"},{"id":2,"name":"two"}]
+    header_style : _type_, optional
+        Rich Table header style, by default None
+    numerate : bool, optional
+        Add numeration, by default False
+    """
+    headers = ["N°"] if numerate else []
     # get headers
     for i in items:
         for h in i.keys():
             if h not in headers:
                 headers.append(h)
     rows = []
     # get rows
+    n = 0
     for item in items:
+        n += 1
         row = []
         for key in headers:
-            if key in item:
+            if key == "N°":
+                row.append(str(n))
+            elif key in item:
                 row.append(item[key])
             else:
                 row.append("")
         rows.append(row)
     table_generator(headers, rows, header_style)
```

### Comparing `satori_ci-1.2.4/src/satorici/classes/validations.py` & `satori_ci-1.2.5/src/satorici/classes/validations.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.4/src/satorici/satori_module.py` & `satori_ci-1.2.5/src/satorici/satori_module.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.4/PKG-INFO` & `satori_ci-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-ci
-Version: 1.2.4
+Version: 1.2.5
 Summary: Satori CI - Automated Software Testing Platform
 Author-Email: Satori CI CLI <info@satori-ci.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

