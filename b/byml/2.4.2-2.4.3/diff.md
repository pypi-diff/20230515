# Comparing `tmp/byml-2.4.2-py3-none-any.whl.zip` & `tmp/byml-2.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 16351 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      113 b- defN 19-Jun-23 10:34 byml/__init__.py
--rw-r--r--  2.0 unx      498 b- defN 20-Aug-11 15:48 byml/_version.py
+-rw-r--r--  2.0 unx      498 b- defN 23-May-15 11:22 byml/_version.py
 -rw-r--r--  2.0 unx    18041 b- defN 20-Mar-21 13:40 byml/byml.py
 -rw-r--r--  2.0 unx     1522 b- defN 20-Aug-11 15:45 byml/byml_to_yml.py
 -rw-r--r--  2.0 unx     1379 b- defN 20-Mar-21 13:16 byml/yaml_util.py
--rw-r--r--  2.0 unx     1605 b- defN 20-Aug-11 15:45 byml/yml_to_byml.py
--rw-r--r--  2.0 unx    17879 b- defN 20-Aug-11 15:48 byml-2.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3030 b- defN 20-Aug-11 15:48 byml-2.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 20-Aug-11 15:48 byml-2.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       91 b- defN 20-Aug-11 15:48 byml-2.4.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 20-Aug-11 15:48 byml-2.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      903 b- defN 20-Aug-11 15:48 byml-2.4.2.dist-info/RECORD
-12 files, 45158 bytes uncompressed, 14857 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx     1615 b- defN 23-May-15 11:20 byml/yml_to_byml.py
+-rw-r--r--  2.0 unx    17879 b- defN 23-May-15 11:22 byml-2.4.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3015 b- defN 23-May-15 11:22 byml-2.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 11:22 byml-2.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       90 b- defN 23-May-15 11:22 byml-2.4.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-May-15 11:22 byml-2.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      903 b- defN 23-May-15 11:22 byml-2.4.3.dist-info/RECORD
+12 files, 45152 bytes uncompressed, 14857 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: byml/yaml_util.py
 Comment: 
 
 Filename: byml/yml_to_byml.py
 Comment: 
 
-Filename: byml-2.4.2.dist-info/LICENSE
+Filename: byml-2.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: byml-2.4.2.dist-info/METADATA
+Filename: byml-2.4.3.dist-info/METADATA
 Comment: 
 
-Filename: byml-2.4.2.dist-info/WHEEL
+Filename: byml-2.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: byml-2.4.2.dist-info/entry_points.txt
+Filename: byml-2.4.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: byml-2.4.2.dist-info/top_level.txt
+Filename: byml-2.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: byml-2.4.2.dist-info/RECORD
+Filename: byml-2.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## byml/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2020-08-11T17:46:05+0200",
+ "date": "2023-05-15T12:18:44+0100",
  "dirty": false,
  "error": null,
- "full-revisionid": "cb06181913f978ea527dd156926ddb75a5929beb",
- "version": "v2.4.2"
+ "full-revisionid": "17770f9d34f09a3d8f9e982120537c4d287c2e43",
+ "version": "v2.4.3"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## byml/yml_to_byml.py

```diff
@@ -9,15 +9,15 @@
 import oead
 from . import yaml_util
 
 def main() -> None:
     parser = argparse.ArgumentParser(description='Converts a YAML file to BYML.')
     parser.add_argument('yml', help='Path to a YAML file', nargs='?', default='-')
     parser.add_argument('byml', help='Path to destination BYAML file', nargs='?', default='-')
-    parser.add_argument('-V', '--version', default=2, help='BYML version (1, 2, 3)')
+    parser.add_argument('-V', '--version', type=int, default=2, help='BYML version (1, 2, 3)')
     parser.add_argument('-b', '--be', action='store_true', help='Use big endian. Defaults to false.')
     args = parser.parse_args()
 
     loader = yaml.CSafeLoader
     yaml_util.add_constructors(loader)
 
     file = sys.stdin if args.yml == '-' else open(args.yml, 'r', encoding='utf-8')
```

## Comparing `byml-2.4.2.dist-info/LICENSE` & `byml-2.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `byml-2.4.2.dist-info/METADATA` & `byml-2.4.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: byml
-Version: 2.4.2
+Version: 2.4.3
 Summary: A simple Nintendo BYML or BYAML v2/v3 parser and writer
 Home-page: https://github.com/leoetlino/byml-v2
 Author: leoetlino
 Author-email: leo@leolam.fr
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: PyYAML (~=5.1)
 Requires-Dist: oead (~=1.1)
 Requires-Dist: sortedcontainers (~=2.0)
 
 ## Simple bymlv2 parser + writer + converters
 
 Features:
@@ -85,9 +84,7 @@
 writer = byml.Writer(document, be=big_endian_mode, version=byml_version)
 writer.write(writable_seekable_stream)
 ```
 
 ### License
 
 This software is licensed under the terms of the GNU General Public License, version 2 or later.
-
-
```

