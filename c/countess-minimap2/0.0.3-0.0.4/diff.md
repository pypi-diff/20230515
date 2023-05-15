# Comparing `tmp/countess-minimap2-0.0.3.tar.gz` & `tmp/countess-minimap2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-minimap2-0.0.3.tar", last modified: Mon May 15 00:40:33 2023, max compression
+gzip compressed data, was "countess-minimap2-0.0.4.tar", last modified: Mon May 15 00:58:18 2023, max compression
```

## Comparing `countess-minimap2-0.0.3.tar` & `countess-minimap2-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-15 00:40:33.649356 countess-minimap2-0.0.3/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2023-04-13 01:52:34.000000 countess-minimap2-0.0.3/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      384 2023-05-15 00:40:33.645356 countess-minimap2-0.0.3/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     1509 2023-05-14 23:58:05.000000 countess-minimap2-0.0.3/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-15 00:40:33.645356 countess-minimap2-0.0.3/countess_minimap2.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)      384 2023-05-15 00:40:33.000000 countess-minimap2-0.0.3/countess_minimap2.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      299 2023-05-15 00:40:33.000000 countess-minimap2-0.0.3/countess_minimap2.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-15 00:40:33.000000 countess-minimap2-0.0.3/countess_minimap2.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       63 2023-05-15 00:40:33.000000 countess-minimap2-0.0.3/countess_minimap2.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       68 2023-05-15 00:40:33.000000 countess-minimap2-0.0.3/countess_minimap2.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-15 00:40:33.000000 countess-minimap2-0.0.3/countess_minimap2.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     3897 2023-05-15 00:18:47.000000 countess-minimap2-0.0.3/countess_minimap2.py
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-15 00:40:33.649356 countess-minimap2-0.0.3/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)      917 2023-05-15 00:38:55.000000 countess-minimap2-0.0.3/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-15 00:58:18.304415 countess-minimap2-0.0.4/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2023-04-13 01:52:34.000000 countess-minimap2-0.0.4/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2082 2023-05-15 00:58:18.304415 countess-minimap2-0.0.4/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1509 2023-05-15 00:53:16.000000 countess-minimap2-0.0.4/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-15 00:58:18.304415 countess-minimap2-0.0.4/countess_minimap2.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2082 2023-05-15 00:58:18.000000 countess-minimap2-0.0.4/countess_minimap2.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      314 2023-05-15 00:58:18.000000 countess-minimap2-0.0.4/countess_minimap2.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-15 00:58:18.000000 countess-minimap2-0.0.4/countess_minimap2.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       63 2023-05-15 00:58:18.000000 countess-minimap2-0.0.4/countess_minimap2.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       68 2023-05-15 00:58:18.000000 countess-minimap2-0.0.4/countess_minimap2.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       18 2023-05-15 00:58:18.000000 countess-minimap2-0.0.4/countess_minimap2.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4113 2023-05-15 00:55:24.000000 countess-minimap2-0.0.4/countess_minimap2.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1086 2023-05-15 00:56:31.000000 countess-minimap2-0.0.4/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-15 00:58:18.304415 countess-minimap2-0.0.4/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-15 00:46:44.000000 countess-minimap2-0.0.4/setup.py
```

### Comparing `countess-minimap2-0.0.3/LICENSE.txt` & `countess-minimap2-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-minimap2-0.0.3/README.md` & `countess-minimap2-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS MiniMap2 Plugin v0.0.3
+# CountESS MiniMap2 Plugin v0.0.4
 
 This is a plugin to allow [MiniMap2](https://github.com/lh3/minimap2) 
 to be used from within [CountESS](https://github.com/CountESS-Project/CountESS/)
 
 This might be useful, but it also stands as a handy example of how to write
 a CountESS plugin which wraps an external Python library.
```

### Comparing `countess-minimap2-0.0.3/countess_minimap2.py` & `countess-minimap2-0.0.4/countess_minimap2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,35 @@
+""" CountESS Minimap2 Plugin"""
+
 import re
 
 import pandas as pd
 
-import mappy
+import mappy  # type: ignore
 
 from countess.core.logger import Logger
 from countess.core.parameters import (
     BooleanParam,
     ChoiceParam,
     ColumnOrIndexChoiceParam,
     IntegerParam,
     StringParam,
     FileParam,
 )
 from countess.core.plugins import PandasTransformPlugin
 
+VERSION = '0.0.4'
+
 CS_STRING_RE = r"(=[ACTGTN]+|:[0-9]+|(?:\*[ACGTN][ACGTN])+|\+[ACGTN]+|-[ACGTN]+)"
 MM2_PRESET_CHOICES = ["sr", "map-pb", "map-ont", "asm5", "asm10", "splice"]
 
 
 def cs_to_hgvs(cs_string, offset=1):
+    """Turn the Minimap2 "difference string" into a HGVS string"""
+
     hgvs_ops = []
     for op in re.findall(CS_STRING_RE, cs_string.upper()):
         if op[0] == ":":
             offset += int(op[1:])
         elif op[0] == "=":
             offset += len(op) - 1
         elif op[0] == "*":
@@ -42,40 +48,42 @@
     if len(hgvs_ops) == 0:
         return "g.{offset}="
     elif len(hgvs_ops) == 1:
         return "g." + hgvs_ops[0]
     else:
         return "g.[" + ";".join(hgvs_ops) + "]"
 
-
 class MiniMap2Plugin(PandasTransformPlugin):
     """Turns a DNA sequence into a HGVS variant code"""
 
     # XXX what is up with the CIGAR string not showing all variants?
 
     name = "MiniMap2 Plugin"
     description = """
         Finds variants using Minimap2.  Note that the CIGAR string doesn't always
         show all variants.
     """
-    version = "0.0.3"
+    version = VERSION
     link = "https://github.com/nickzoic/countess-minimap2#readme"
 
     FILE_TYPES = [("MMI", "*.mmi"), ("FASTA", "*.fa(sta)?")]
 
     parameters = {
         "column": ColumnOrIndexChoiceParam("Input Column", "sequence"),
         "prefix": StringParam("Output Column Prefix", "mm"),
         "ref": FileParam("Ref FA / Ref MMI", file_types = FILE_TYPES),
         "preset": ChoiceParam("Preset", "sr", choices=MM2_PRESET_CHOICES),
         "min_length": IntegerParam("Minimum Match Length", 0),
         "drop": BooleanParam("Drop Unmatched", False),
     }
 
     def run_df(self, df: pd.DataFrame, logger: Logger) -> pd.DataFrame:
+
+        assert isinstance(self.parameters['column'], ColumnOrIndexChoiceParam)
+
         prefix = self.parameters["prefix"].value
 
         aligner = mappy.Aligner(
             self.parameters["ref"].value, preset=self.parameters["preset"].value
         )
 
         if not aligner:
```

