# Comparing `tmp/json-grep-1.1.2.tar.gz` & `tmp/json-grep-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json-grep-1.1.2.tar", last modified: Thu Mar 11 07:39:31 2021, max compression
+gzip compressed data, was "json-grep-1.2.0.tar", last modified: Mon May 15 09:15:30 2023, max compression
```

## Comparing `json-grep-1.1.2.tar` & `json-grep-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2021-03-11 07:39:31.393426 json-grep-1.1.2/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)       24 2021-03-10 21:40:32.000000 json-grep-1.1.2/MANIFEST.in
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1980 2021-03-11 07:39:31.393426 json-grep-1.1.2/PKG-INFO
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1233 2021-03-10 21:53:01.000000 json-grep-1.1.2/README.md
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2021-03-11 07:39:31.393426 json-grep-1.1.2/json_grep.egg-info/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1980 2021-03-11 07:39:31.000000 json-grep-1.1.2/json_grep.egg-info/PKG-INFO
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      368 2021-03-11 07:39:31.000000 json-grep-1.1.2/json_grep.egg-info/SOURCES.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2021-03-11 07:39:31.000000 json-grep-1.1.2/json_grep.egg-info/dependency_links.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      107 2021-03-11 07:39:31.000000 json-grep-1.1.2/json_grep.egg-info/entry_points.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2021-03-10 21:46:42.000000 json-grep-1.1.2/json_grep.egg-info/not-zip-safe
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        9 2021-03-11 07:39:31.000000 json-grep-1.1.2/json_grep.egg-info/top_level.txt
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2021-03-11 07:39:31.393426 json-grep-1.1.2/jsongrep/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        5 2021-03-11 07:39:16.000000 json-grep-1.1.2/jsongrep/VERSION
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 18:47:36.000000 json-grep-1.1.2/jsongrep/__init__.py
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2021-03-11 07:39:31.393426 json-grep-1.1.2/jsongrep/libs/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 21:48:52.000000 json-grep-1.1.2/jsongrep/libs/__init__.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     3176 2021-03-10 21:42:48.000000 json-grep-1.1.2/jsongrep/libs/json_filter.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      332 2021-02-01 10:45:10.000000 json-grep-1.1.2/jsongrep/libs/setuptools.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     2251 2021-03-11 07:38:53.000000 json-grep-1.1.2/jsongrep/main.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)       38 2021-03-11 07:39:31.393426 json-grep-1.1.2/setup.cfg
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1142 2021-03-10 21:46:39.000000 json-grep-1.1.2/setup.py
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-05-15 09:15:30.804437 json-grep-1.2.0/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)       24 2021-03-10 21:40:32.000000 json-grep-1.2.0/MANIFEST.in
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1654 2023-05-15 09:15:30.804437 json-grep-1.2.0/PKG-INFO
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1233 2023-05-15 09:06:17.000000 json-grep-1.2.0/README.md
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-05-15 09:15:30.804437 json-grep-1.2.0/json_grep.egg-info/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1654 2023-05-15 09:15:30.000000 json-grep-1.2.0/json_grep.egg-info/PKG-INFO
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      368 2023-05-15 09:15:30.000000 json-grep-1.2.0/json_grep.egg-info/SOURCES.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-05-15 09:15:30.000000 json-grep-1.2.0/json_grep.egg-info/dependency_links.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      106 2023-05-15 09:15:30.000000 json-grep-1.2.0/json_grep.egg-info/entry_points.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-05-15 09:12:34.000000 json-grep-1.2.0/json_grep.egg-info/not-zip-safe
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        9 2023-05-15 09:15:30.000000 json-grep-1.2.0/json_grep.egg-info/top_level.txt
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-05-15 09:15:30.804437 json-grep-1.2.0/jsongrep/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        5 2023-05-15 09:05:59.000000 json-grep-1.2.0/jsongrep/VERSION
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 18:47:36.000000 json-grep-1.2.0/jsongrep/__init__.py
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-05-15 09:15:30.804437 json-grep-1.2.0/jsongrep/libs/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 21:48:52.000000 json-grep-1.2.0/jsongrep/libs/__init__.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     3343 2023-05-15 09:03:14.000000 json-grep-1.2.0/jsongrep/libs/json_filter.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      333 2021-08-06 07:59:08.000000 json-grep-1.2.0/jsongrep/libs/setuptools.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     2347 2023-05-15 09:09:12.000000 json-grep-1.2.0/jsongrep/main.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)       38 2023-05-15 09:15:30.804437 json-grep-1.2.0/setup.cfg
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1142 2021-03-10 21:46:39.000000 json-grep-1.2.0/setup.py
```

### Comparing `json-grep-1.1.2/PKG-INFO` & `json-grep-1.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,38 @@
-Metadata-Version: 2.1
-Name: json-grep
-Version: 1.1.2
-Summary: Filtering JSON dict keys from STDOUT
-Home-page: https://gitlab.com/alda78/json-grep
-Author: Ales Adamek
-Author-email: alda78@seznam.cz
-License: MIT
-Description: # json-grep
-        
-        ## Description
-        Simple tool for filtering JSON dict keys from STDOUT
-        
-        ## Usage
-        ```
-        json-grep --help
-        usage: json-grep [-h] [-m] [-v] [-i] filter_keys [filter_keys ...]
-        
-        JSON GREP is utility for filtering selected keys from json string piped from STDOUT
-        
-        positional arguments:
-          filter_keys           List of keys which you want to filter from json dict. You can also specify value of item which you want to pass only by operator = or ~. '~' means that value is in item on any string position. If key is in deeper level of tree structure
-                                use '.' separator to specify how deep is key in dict tree structure.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -m, --multiline-output
-                                Use multiline output for filtered result
-          -v, --values_only     Show only values without keys description
-          -i, --ignore-errors   Ignore errors caused by json decode
-        ```
-        
-        ## Installation
-        ```bash
-        wget https://gitlab.com/alda78/json-grep/-/archive/master/json-grep-master.tar && \
-        tar -xf json-grep-master.tar && \
-        cd json-grep-master/ && \
-        sudo python3 setup.py install && \
-        cd ../ &&  \
-        sudo rm -rf json-grep-master
-        ```
-        
-        or simply
-        ```bash
-        pip3 install json-grep
-        ```
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# json-grep
+
+## Description
+Simple tool for filtering JSON dict keys from STDOUT
+
+## Usage
+```
+json-grep --help
+usage: json-grep [-h] [-m] [-v] [-i] filter_keys [filter_keys ...]
+
+JSON GREP is utility for filtering selected keys from json string piped from STDOUT
+
+positional arguments:
+  filter_keys           List of keys which you want to filter from json dict. You can also specify value of item which you want to pass only by operator = or ~. '~' means that value is in item on any string position. If key is in deeper level of tree structure
+                        use '.' separator to specify how deep is key in dict tree structure.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -m, --multiline-output
+                        Use multiline output for filtered result
+  -v, --values_only     Show only values without keys description
+  -e, --show-errors     Ignore errors caused by json decode
+```
+
+## Installation
+```bash
+wget https://gitlab.com/alda78/json-grep/-/archive/master/json-grep-master.tar && \
+tar -xf json-grep-master.tar && \
+cd json-grep-master/ && \
+sudo python3 setup.py install && \
+cd ../ &&  \
+sudo rm -rf json-grep-master
+```
+
+or simply
+```bash
+pip3 install json-grep
+```
```

### Comparing `json-grep-1.1.2/README.md` & `json-grep-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: json-grep
+Version: 1.2.0
+Summary: Filtering JSON dict keys from STDOUT
+Home-page: https://gitlab.com/alda78/json-grep
+Author: Ales Adamek
+Author-email: alda78@seznam.cz
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # json-grep
 
 ## Description
 Simple tool for filtering JSON dict keys from STDOUT
 
 ## Usage
 ```
@@ -15,15 +29,15 @@
                         use '.' separator to specify how deep is key in dict tree structure.
 
 optional arguments:
   -h, --help            show this help message and exit
   -m, --multiline-output
                         Use multiline output for filtered result
   -v, --values_only     Show only values without keys description
-  -i, --ignore-errors   Ignore errors caused by json decode
+  -e, --show-errors     Ignore errors caused by json decode
 ```
 
 ## Installation
 ```bash
 wget https://gitlab.com/alda78/json-grep/-/archive/master/json-grep-master.tar && \
 tar -xf json-grep-master.tar && \
 cd json-grep-master/ && \
@@ -31,8 +45,8 @@
 cd ../ &&  \
 sudo rm -rf json-grep-master
 ```
 
 or simply
 ```bash
 pip3 install json-grep
-```
+```
```

### Comparing `json-grep-1.1.2/json_grep.egg-info/PKG-INFO` & `json-grep-1.2.0/json_grep.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 Metadata-Version: 2.1
 Name: json-grep
-Version: 1.1.2
+Version: 1.2.0
 Summary: Filtering JSON dict keys from STDOUT
 Home-page: https://gitlab.com/alda78/json-grep
 Author: Ales Adamek
 Author-email: alda78@seznam.cz
 License: MIT
-Description: # json-grep
-        
-        ## Description
-        Simple tool for filtering JSON dict keys from STDOUT
-        
-        ## Usage
-        ```
-        json-grep --help
-        usage: json-grep [-h] [-m] [-v] [-i] filter_keys [filter_keys ...]
-        
-        JSON GREP is utility for filtering selected keys from json string piped from STDOUT
-        
-        positional arguments:
-          filter_keys           List of keys which you want to filter from json dict. You can also specify value of item which you want to pass only by operator = or ~. '~' means that value is in item on any string position. If key is in deeper level of tree structure
-                                use '.' separator to specify how deep is key in dict tree structure.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -m, --multiline-output
-                                Use multiline output for filtered result
-          -v, --values_only     Show only values without keys description
-          -i, --ignore-errors   Ignore errors caused by json decode
-        ```
-        
-        ## Installation
-        ```bash
-        wget https://gitlab.com/alda78/json-grep/-/archive/master/json-grep-master.tar && \
-        tar -xf json-grep-master.tar && \
-        cd json-grep-master/ && \
-        sudo python3 setup.py install && \
-        cd ../ &&  \
-        sudo rm -rf json-grep-master
-        ```
-        
-        or simply
-        ```bash
-        pip3 install json-grep
-        ```
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+# json-grep
+
+## Description
+Simple tool for filtering JSON dict keys from STDOUT
+
+## Usage
+```
+json-grep --help
+usage: json-grep [-h] [-m] [-v] [-i] filter_keys [filter_keys ...]
+
+JSON GREP is utility for filtering selected keys from json string piped from STDOUT
+
+positional arguments:
+  filter_keys           List of keys which you want to filter from json dict. You can also specify value of item which you want to pass only by operator = or ~. '~' means that value is in item on any string position. If key is in deeper level of tree structure
+                        use '.' separator to specify how deep is key in dict tree structure.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -m, --multiline-output
+                        Use multiline output for filtered result
+  -v, --values_only     Show only values without keys description
+  -e, --show-errors     Ignore errors caused by json decode
+```
+
+## Installation
+```bash
+wget https://gitlab.com/alda78/json-grep/-/archive/master/json-grep-master.tar && \
+tar -xf json-grep-master.tar && \
+cd json-grep-master/ && \
+sudo python3 setup.py install && \
+cd ../ &&  \
+sudo rm -rf json-grep-master
+```
+
+or simply
+```bash
+pip3 install json-grep
+```
```

### Comparing `json-grep-1.1.2/jsongrep/libs/json_filter.py` & `json-grep-1.2.0/jsongrep/libs/json_filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,84 @@
-import collections
 import json
 import re
 
 
 class JsonFilterException(Exception):
     pass
 
 
 class JsonFilter:
 
     PARSED_KEY_CACHE = {}
 
     @classmethod
-    def parse_key(cls, key: str)->tuple:
+    def parse_key(cls, key: str) -> (str, str, str):
         if key in cls.PARSED_KEY_CACHE:
             return cls.PARSED_KEY_CACHE[key]
 
-        rkey: str = None
-        rvalue: str = None
+        rkey: str
+        rvalue: str
         operator: str = None
         re_sign = re.search("([=~])", key)
         if re_sign:
             operator = re_sign.group()
         parsed_key: list = str(key).split(operator)
         rkey = parsed_key[0].strip()
         rvalue = parsed_key[1].strip() if len(parsed_key) > 1 else None
         cls.PARSED_KEY_CACHE[key] = (rkey, rvalue, operator)
         return rkey, rvalue, operator
 
     @classmethod
-    def filter_keys_and_values(cls, line: str, keys: dict, is_value_operator_used: bool=False) -> dict:
+    def filter_keys_and_values(cls, line: str, keys: dict, is_value_operator_used: bool = False) -> dict:
         ret = {}
         is_value_matched = False
         try:
             json_data_tree = json.loads(line)
             json_data_flat = cls.flatten_dict(json_data_tree)
             if not isinstance(json_data_flat, dict):
                 raise JsonFilterException("JSON data is not dict on line: {}".format(line))
             for ikey in keys:
                 key, value, operator = cls.parse_key(ikey)
-                if key in json_data_flat:
-                    if not value:
-                        ret[key] = json_data_flat[key]
-                    elif operator == "=" and str(value) == str(json_data_flat[key]):
-                        ret[key] = json_data_flat[key]
-                        is_value_matched = True
-                    elif operator == "~" and str(value) in str(json_data_flat[key]):
-                        ret[key] = json_data_flat[key]
-                        is_value_matched = True
-                    else:
-                        return None
+                flat_key: str
+                key_matches = [flat_key for flat_key in json_data_flat.keys() if flat_key == key or (key[-1] == "*" and flat_key.startswith(key[:-1]))]
+                for key in key_matches:
+                    if key in json_data_flat:
+                        if not value:
+                            ret[key] = json_data_flat[key]
+                        elif operator == "=" and str(value) == str(json_data_flat[key]):
+                            ret[key] = json_data_flat[key]
+                            is_value_matched = True
+                        elif operator == "~" and str(value) in str(json_data_flat[key]):
+                            ret[key] = json_data_flat[key]
+                            is_value_matched = True
+                        else:
+                            return None
         except Exception as ex:
             raise JsonFilterException("Error decoding JSON from line: {} caused by: {}".format(line, ex))
         if is_value_operator_used and not is_value_matched:
             return None
         return ret
 
     @classmethod
-    def flatten_dict(cls, input_dict: dict, parent_key: str='')->dict:
+    def flatten_dict(cls, input_dict: dict, parent_key: str = "") -> dict:
         items = []
         for k, v in input_dict.items():
             new_key = "{}.{}".format(parent_key, k) if parent_key else "{}".format(k)
-            if isinstance(v, collections.MutableMapping):
+            if isinstance(v, dict):
                 items.extend(cls.flatten_dict(v, new_key).items())
-            elif isinstance(v, collections.MutableSequence):
+            elif isinstance(v, list):
                 new_v = dict(enumerate(v))
                 items.extend(cls.flatten_dict(new_v, new_key).items())
             else:
                 items.append((new_key, v))
         return dict(items)
 
     @staticmethod
     def format_result(data: dict, multiline_output: bool = False, values_only: bool = False) -> str:
         ret = ""
         for key, value in data.items():
             br_line = "\n" if multiline_output else " "
             if values_only:
-                ret = "{}\33[33m{}\33[0m{}".format(ret, value, br_line)
+                ret = f"{ret}\33[33m{value}\33[0m{br_line}"
             else:
-                ret = "{}\"\33[32m{}\33[0m\": \"\33[36m{}\33[0m\"{}".format(ret, key, value, br_line)
-        return "{}{}".format(ret, "\n")
+                ret = f"{ret}\"\33[32m{key}\33[0m\": \"\33[36m{value}\33[0m\"{br_line}"
+        return f"{ret}\n"
```

### Comparing `json-grep-1.1.2/setup.py` & `json-grep-1.2.0/setup.py`

 * *Files identical despite different names*

