# Comparing `tmp/sbomdiff-0.4.2-py2.py3-none-any.whl.zip` & `tmp/sbomdiff-0.5.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13521 bytes, number of entries: 12
+Zip file size: 14236 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-02 07:31 sbomdiff/__init__.py
--rw-r--r--  2.0 unx     6174 b- defN 23-Apr-10 17:04 sbomdiff/cli.py
+-rw-r--r--  2.0 unx     8734 b- defN 23-May-15 21:10 sbomdiff/cli.py
 -rw-r--r--  2.0 unx     4470 b- defN 23-Mar-28 20:15 sbomdiff/cyclonedx_parser.py
 -rw-r--r--  2.0 unx     1298 b- defN 22-Oct-20 16:02 sbomdiff/output.py
 -rw-r--r--  2.0 unx     7841 b- defN 23-Apr-13 20:22 sbomdiff/spdx_parser.py
--rw-r--r--  2.0 unx      100 b- defN 23-Apr-10 18:30 sbomdiff/version.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 15:13 sbomdiff-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     6336 b- defN 23-Apr-14 15:13 sbomdiff-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 15:13 sbomdiff-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Apr-14 15:13 sbomdiff-0.4.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-14 15:13 sbomdiff-0.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      949 b- defN 23-Apr-14 15:13 sbomdiff-0.4.2.dist-info/RECORD
-12 files, 38691 bytes uncompressed, 11931 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx      100 b- defN 23-May-15 21:02 sbomdiff/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-15 21:18 sbomdiff-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7573 b- defN 23-May-15 21:18 sbomdiff-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-15 21:18 sbomdiff-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-May-15 21:18 sbomdiff-0.5.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-May-15 21:18 sbomdiff-0.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      949 b- defN 23-May-15 21:18 sbomdiff-0.5.0.dist-info/RECORD
+12 files, 42488 bytes uncompressed, 12646 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: sbomdiff/spdx_parser.py
 Comment: 
 
 Filename: sbomdiff/version.py
 Comment: 
 
-Filename: sbomdiff-0.4.2.dist-info/LICENSE
+Filename: sbomdiff-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: sbomdiff-0.4.2.dist-info/METADATA
+Filename: sbomdiff-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: sbomdiff-0.4.2.dist-info/WHEEL
+Filename: sbomdiff-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: sbomdiff-0.4.2.dist-info/entry_points.txt
+Filename: sbomdiff-0.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbomdiff-0.4.2.dist-info/top_level.txt
+Filename: sbomdiff-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sbomdiff-0.4.2.dist-info/RECORD
+Filename: sbomdiff-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbomdiff/cli.py

```diff
@@ -1,18 +1,19 @@
-# Copyright (C) 2022 Anthony Harrison
+# Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
 import argparse
 import pathlib
 import sys
 import textwrap
 from collections import ChainMap
 
+from lib4sbom.output import SBOMOutput
+
 from sbomdiff.cyclonedx_parser import CycloneDXParser
-from sbomdiff.output import SBOMOutput
 from sbomdiff.spdx_parser import SPDXParser
 from sbomdiff.version import VERSION
 
 # CLI processing
 
 
 def main(argv=None):
@@ -51,24 +52,33 @@
     output_group.add_argument(
         "-o",
         "--output-file",
         action="store",
         default="",
         help="output filename (default: output to stdout)",
     )
+    output_group.add_argument(
+        "-f",
+        "--format",
+        action="store",
+        default="text",
+        choices=["text", "json", "yaml"],
+        help="specify format of output file (default: text)",
+    )
     parser.add_argument("-V", "--version", action="version", version=VERSION)
 
     parser.add_argument("FILE1", help="first SBOM file")
     parser.add_argument("FILE2", help="second SBOM file")
 
     defaults = {
         "output_file": "",
         "sbom": "auto",
         "exclude_license": False,
         "debug": False,
+        "format": "text",
     }
     raw_args = parser.parse_args(argv[1:])
     args = {key: value for key, value in vars(raw_args).items() if value}
     args = ChainMap(args, defaults)
 
     # Validate CLI parameters
     if args["FILE1"] != args["FILE2"]:
@@ -110,74 +120,129 @@
         if len(packages2) == 0:
             file2_type = "CYCLONEDX"
             packages2 = cyclonedx.parse(args["FILE2"])
 
     if args["debug"]:
         print("SBOM type", args["sbom"])
         print("Output file", args["output_file"])
+        print("Format", args["format"])
         print("SBOM File1", args["FILE1"])
         print("SBOM File1 - type", file1_type)
         print("SBOM File1 - packages", len(packages1))
         print("SBOM File2", args["FILE2"])
         print("SBOM File2 - type", file2_type)
         print("SBOM File2 - packages", len(packages2))
         print("Exclude Licences", args["exclude_license"])
 
     # Keep count of differences
     version_changes = 0
     new_packages = 0
     removed_packages = 0
     license_changes = 0
 
-    sbom_out = SBOMOutput(args["output_file"])
+    sbom_out = SBOMOutput(args["output_file"], args["format"])
+
+    if args["format"] != "text":
+        diff_doc = []
 
     for package in packages1:
+        package_info = dict()
         if package in packages2:
             # Compare values for common package
             version1, license1 = packages1[package]
             version2, license2 = packages2[package]
+            package_info["package"] = package
+            diff_record = False
             if version1 != version2:
                 if len(version1) == 0:
                     version1 = "UNKNOWN"
                 if len(version2) == 0:
                     version2 = "UNKNOWN"
-                sbom_out.send_output(
-                    f"[VERSION] {package}: "
-                    f"Version changed from {version1} to {version2}"
-                )
+                if args["format"] == "text":
+                    sbom_out.send_output(
+                        f"[VERSION] {package}: "
+                        f"Version changed from {version1} to {version2}"
+                    )
+                package_info["status"] = "change"
+                version_info = dict()
+                version_info["from"] = version1
+                version_info["to"] = version2
+                package_info["version"] = version_info
                 version_changes += 1
+                diff_record = True
             if not args["exclude_license"] and license1 != license2:
-                sbom_out.send_output(
-                    f"[LICENSE] {package}: "
-                    f"License changed from {license1} to {license2}"
-                )
+                if args["format"] == "text":
+                    sbom_out.send_output(
+                        f"[LICENSE] {package}: "
+                        f"License changed from {license1} to {license2}"
+                    )
+                package_info["status"] = "change"
+                license_info = dict()
+                license_info["from"] = license1
+                license_info["to"] = license2
+                package_info["license"] = license_info
                 license_changes += 1
+                diff_record = True
         else:
             # Package must have been removed
             version1, license1 = packages1[package]
             if len(version1) == 0:
                 version1 = "UNKNOWN"
-            sbom_out.send_output(f"[REMOVED] {package}: (Version {version1})")
+            if args["format"] == "text":
+                sbom_out.send_output(f"[REMOVED] {package}: (Version {version1})")
+            package_info["status"] = "remove"
+            version_info = dict()
+            version_info["from"] = version1
+            package_info["version"] = version_info
             removed_packages += 1
+            diff_record = True
+        if args["format"] != "text" and diff_record:
+            diff_doc.append(package_info)
     # Check for any new packages
     for package in packages2:
         if package not in packages1:
             version2, license2 = packages2[package]
             if len(version2) == 0:
                 version2 = "UNKNOWN"
-            sbom_out.send_output(f"[ADDED  ] {package}: (Version {version2})")
+            if args["format"] == "text":
+                sbom_out.send_output(f"[ADDED  ] {package}: (Version {version2})")
+            else:
+                package_info = dict()
+                package_info["package"] = package
+                package_info["status"] = "add"
+                version_info = dict()
+                version_info["from"] = version2
+                package_info["version"] = version_info
+                diff_doc.append(package_info)
             new_packages += 1
-    sbom_out.send_output("\nSummary\n-------")
-    sbom_out.send_output(f"Version changes:  {version_changes}")
-    if not args["exclude_license"]:
-        sbom_out.send_output(f"License changes:  {license_changes}")
-    sbom_out.send_output(f"Removed packages: {removed_packages}")
-    sbom_out.send_output(f"New packages:     {new_packages}")
-
-    sbom_out.close_output()
+    if args["format"] == "text":
+        sbom_out.send_output("\nSummary\n-------")
+        sbom_out.send_output(f"Version changes:  {version_changes}")
+        if not args["exclude_license"]:
+            sbom_out.send_output(f"License changes:  {license_changes}")
+        sbom_out.send_output(f"Removed packages: {removed_packages}")
+        sbom_out.send_output(f"New packages:     {new_packages}")
+
+    if args["format"] != "text":
+        json_doc = {}
+        tool = dict()
+        tool["name"] = "sbomdiff"
+        tool["version"] = VERSION
+        json_doc["tool"] = tool
+        json_doc["file_1"] = args["FILE1"]
+        json_doc["file_2"] = args["FILE2"]
+        json_doc["differences"] = diff_doc
+        summary = dict()
+        summary["version_changes"] = version_changes
+        summary["new_packages"] = new_packages
+        summary["removed_packages"] = removed_packages
+        if not args["exclude_license"]:
+            summary["license_changes"] = license_changes
+        json_doc["summary"] = summary
+        sbom_out.generate_output(json_doc)
 
     # Return code indicates if any differences have been detected
     if (version_changes or license_changes or removed_packages or new_packages) != 0:
         return 1
 
     return 0
```

## sbomdiff/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2022 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.4.2"
+VERSION: str = "0.5.0"
```

## Comparing `sbomdiff-0.4.2.dist-info/LICENSE` & `sbomdiff-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbomdiff-0.4.2.dist-info/METADATA` & `sbomdiff-0.5.0.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbomdiff
-Version: 0.4.2
+Version: 0.5.0
 Summary: Software Bill of Material (SBOM) difference tool
 Home-page: https://github.com/anthonyharrison/sbomdiff
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: Apache-2.0
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: defusedxml
 Requires-Dist: pyyaml (>=5.4)
+Requires-Dist: lib4sbom (>=0.3.1)
 
 # SBOMDiff
 
 SBOMDiff is a tool to compare two Software Bill of Materials (SBOM) files and
 reports the differences. It supports SBOMs created in both
 [SPDX](https://www.spdx.org) and [CycloneDX](https://www.cyclonedx.org) formats.
 
@@ -53,36 +54,37 @@
 if you are using different versions of python. `virtualenv` is a tool for setting up virtual python environments which
 allows you to have all the dependencies for the tool set up in a single environment, or have different environments set
 up for testing using different versions of Python.
 
 ## Usage
 
 ```
-usage: sbomdiff [-h] [--sbom {auto,spdx,cyclonedx}] [--exclude-license] [-d] [-o OUTPUT_FILE] [-V] FILE1 FILE2
+usage: sbomdiff [-h] [--sbom {auto,spdx,cyclonedx}] [--exclude-license] [-d] [-o OUTPUT_FILE] [-f {text,json,yaml}] [-V] FILE1 FILE2
 
 SBOMDiff compares two Software Bill of Materials and reports the differences.
 
 positional arguments:
   FILE1                 first SBOM file
   FILE2                 second SBOM file
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
 
 Input:
   --sbom {auto,spdx,cyclonedx}
                         specify type of sbom to compare (default: auto)
   --exclude-license     suppress reporting differences in the license of components
 
 Output:
   -d, --debug           show debug information
   -o OUTPUT_FILE, --output-file OUTPUT_FILE
                         output filename (default: output to stdout)
-
+  -f {text,json,yaml}, --format {text,json,yaml}
+                        specify format of output file (default: text)
 ```
 						
 ## Operation
 
 The `--sbom` option is used to specify the format of the SBOM files. The default is for the type and format of the SBOM to be
 automatically detected based on the extension of the file name.
 
@@ -140,14 +142,74 @@
 -------
 Version changes:  2
 License changes:  2
 Removed packages: 1
 New packages:     0
 ```
 
+The following is an example of an output file in JSON format:
+
+```json
+{
+  "tool": {
+    "name": "sbomdiff",
+    "version": "0.4.2"
+  },
+  "file_1": "file1.json",
+  "file_2": "file2.spdx",
+  "differences": [
+    {
+      "package": "glibc",
+      "status": "change",
+      "license": {
+        "from": "GPL-2.0-only",
+        "to": "(LGPL-2.0-only OR LicenseRef-3)"
+      }
+    },
+    {
+      "package": "saxon",
+      "status": "change",
+      "license": {
+        "from": "Apache-2.0",
+        "to": "MPL-1.0"
+      }
+    },
+    {
+      "package": "rich",
+      "status": "change",
+      "version": {
+        "from": "11.0.0",
+        "to": "12.5.1"
+      },
+    },
+    {
+      "package": "colorama",
+      "status": "remove",
+      "version": {
+        "from": "0.4.4"
+      },
+    },   
+    {
+      "package": "pygments",
+      "status": "change",
+      "version": {
+        "from": "11.0.0",
+        "to": "12.5.1"
+      },
+    }
+  ],
+  "summary": {
+    "version_changes": "2",
+    "new_packages": "0"
+    "removed_packages": "1",
+    "license_changes": "2",
+  }
+}
+```
+
 ## License
 
 Licensed under the Apache 2.0 License.
 
 ## Limitations
 
 This tool is meant to support software development and security audit functions. However the usefulness of the tool is dependent on the SBOM data
```

## Comparing `sbomdiff-0.4.2.dist-info/RECORD` & `sbomdiff-0.5.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 sbomdiff/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sbomdiff/cli.py,sha256=-WhHmTKi9zj2HihBxc-poiMA3WsYVaKhFpZM91ljqO8,6174
+sbomdiff/cli.py,sha256=Nq9kZ0qLGn0txXBSIxCo23A-Tb5loq2N_la_lFoaHtY,8734
 sbomdiff/cyclonedx_parser.py,sha256=lBp9SvYnVNxqlznYajTQWVIcTB-rn6bCTs5Ji9bFm0g,4470
 sbomdiff/output.py,sha256=G9tbsqlbCapnTyPgo6ROnSXVoVM2c4Hp1QfhvvvcQcQ,1298
 sbomdiff/spdx_parser.py,sha256=Wtpjg8PhL_6BS7l5GQvNlMMfMo0_Z59vMl13FBP0F5s,7841
-sbomdiff/version.py,sha256=of7zNevWtgkB2MkHViOqddYl3CG4lSvYLWFUoceBUlo,100
-sbomdiff-0.4.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbomdiff-0.4.2.dist-info/METADATA,sha256=lh1_3yLl3bXRtLUb_j2seKWW3Jv9XSzNkKF-JNdjCRM,6336
-sbomdiff-0.4.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-sbomdiff-0.4.2.dist-info/entry_points.txt,sha256=fcONsvnGhylyVE47AbBD9yrXj47ScGZbVyJ7jGRcx9o,47
-sbomdiff-0.4.2.dist-info/top_level.txt,sha256=vt1EhODe3hHuS5SesbQue8uX-pOojrBfdtCwYdbEUgg,9
-sbomdiff-0.4.2.dist-info/RECORD,,
+sbomdiff/version.py,sha256=Jpb0I-mkqELebity9eHVTcRu5I4Sjc_mXpT39iSYqWU,100
+sbomdiff-0.5.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbomdiff-0.5.0.dist-info/METADATA,sha256=agnhvvlLD04dXvlbTnyg2u6K-z4BG4DwymRJB7SqLpA,7573
+sbomdiff-0.5.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+sbomdiff-0.5.0.dist-info/entry_points.txt,sha256=fcONsvnGhylyVE47AbBD9yrXj47ScGZbVyJ7jGRcx9o,47
+sbomdiff-0.5.0.dist-info/top_level.txt,sha256=vt1EhODe3hHuS5SesbQue8uX-pOojrBfdtCwYdbEUgg,9
+sbomdiff-0.5.0.dist-info/RECORD,,
```

