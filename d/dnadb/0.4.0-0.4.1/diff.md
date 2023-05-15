# Comparing `tmp/dnadb-0.4.0.tar.gz` & `tmp/dnadb-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.4.0.tar", last modified: Sun May 14 15:59:48 2023, max compression
+gzip compressed data, was "dnadb-0.4.1.tar", last modified: Mon May 15 01:08:45 2023, max compression
```

## Comparing `dnadb-0.4.0.tar` & `dnadb-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-14 15:59:48.755522 dnadb-0.4.0/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.4.0/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-14 15:59:48.755522 dnadb-0.4.0/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.4.0/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-14 15:58:37.000000 dnadb-0.4.0/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-14 15:59:48.755522 dnadb-0.4.0/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-14 15:59:48.751522 dnadb-0.4.0/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-14 15:59:48.755522 dnadb-0.4.0/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-14 15:58:48.000000 dnadb-0.4.0/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-14 15:59:48.755522 dnadb-0.4.0/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.4.0/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.4.0/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.4.0/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-14 15:59:48.755522 dnadb-0.4.0/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 15:33:28.000000 dnadb-0.4.0/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.4.0/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     2234 2023-05-10 12:52:14.000000 dnadb-0.4.0/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     4815 2023-05-11 20:35:23.000000 dnadb-0.4.0/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     5208 2023-05-11 01:32:34.000000 dnadb-0.4.0/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     5969 2023-05-11 01:44:43.000000 dnadb-0.4.0/src/dnadb/fastq.py
--rw-r--r--   0 dwl2x     (1000) users      (100)        0 2023-05-09 22:29:41.000000 dnadb-0.4.0/src/dnadb/otu.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    19344 2023-05-14 14:55:16.000000 dnadb-0.4.0/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.4.0/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-14 15:59:48.755522 dnadb-0.4.0/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-14 15:59:48.000000 dnadb-0.4.0/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      519 2023-05-14 15:59:48.000000 dnadb-0.4.0/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-14 15:59:48.000000 dnadb-0.4.0/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-14 15:59:48.000000 dnadb-0.4.0/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-14 15:59:48.000000 dnadb-0.4.0/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-15 01:08:45.388383 dnadb-0.4.1/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.4.1/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-15 01:08:45.388383 dnadb-0.4.1/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.4.1/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-15 01:07:43.000000 dnadb-0.4.1/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-15 01:08:45.388383 dnadb-0.4.1/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-15 01:08:45.388383 dnadb-0.4.1/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-15 01:08:45.388383 dnadb-0.4.1/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-15 01:07:47.000000 dnadb-0.4.1/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-15 01:08:45.388383 dnadb-0.4.1/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.4.1/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.4.1/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.4.1/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-15 01:08:45.388383 dnadb-0.4.1/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.4.1/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.4.1/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     2234 2023-05-10 12:52:14.000000 dnadb-0.4.1/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     4815 2023-05-11 20:35:23.000000 dnadb-0.4.1/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5208 2023-05-11 01:32:34.000000 dnadb-0.4.1/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5969 2023-05-11 01:44:43.000000 dnadb-0.4.1/src/dnadb/fastq.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)        0 2023-05-09 22:29:41.000000 dnadb-0.4.1/src/dnadb/otu.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    19190 2023-05-15 01:07:27.000000 dnadb-0.4.1/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.4.1/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-15 01:08:45.388383 dnadb-0.4.1/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-15 01:08:45.000000 dnadb-0.4.1/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      519 2023-05-15 01:08:45.000000 dnadb-0.4.1/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-15 01:08:45.000000 dnadb-0.4.1/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-15 01:08:45.000000 dnadb-0.4.1/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-15 01:08:45.000000 dnadb-0.4.1/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.4.0/LICENSE` & `dnadb-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.0/PKG-INFO` & `dnadb-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.4.0
+Version: 0.4.1
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.4.0/pyproject.toml` & `dnadb-0.4.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.4.0/src/dnadb/datasets/dataset.py` & `dnadb-0.4.1/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.0/src/dnadb/datasets/greengenes.py` & `dnadb-0.4.1/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.0/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.4.1/src/dnadb/datasets/silva/__init__.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.0/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.4.1/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.0/src/dnadb/db.py` & `dnadb-0.4.1/src/dnadb/db.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.0/src/dnadb/dna.py` & `dnadb-0.4.1/src/dnadb/dna.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.0/src/dnadb/fasta.py` & `dnadb-0.4.1/src/dnadb/fasta.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.0/src/dnadb/fastq.py` & `dnadb-0.4.1/src/dnadb/fastq.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.0/src/dnadb/taxonomy.py` & `dnadb-0.4.1/src/dnadb/taxonomy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 from dataclasses import dataclass, field, replace
-from functools import cached_property
 from itertools import chain
 import io
-import json
-from lmdbm import Lmdb
 import numpy as np
 import numpy.typing as npt
 from pathlib import Path
 import re
 from sortedcontainers import SortedDict
-from typing import Dict, Generator, Iterable, List, Optional, overload, Tuple, Union
+from typing import Dict, Generator, Iterable, List, Optional, Tuple, Union
 
 from .db import DbFactory, DbWrapper
 from .utils import open_file
 
 RANKS = ("Kingdom", "Phylum", "Class", "Order", "Family", "Genus", "Species")
 RANK_PREFIXES = ''.join(rank[0] for rank in RANKS).lower()
 
 # Utility Functions --------------------------------------------------------------------------------
 
 def split_taxonomy(taxonomy: str) -> Tuple[str, ...]:
     """
     Split taxonomy label into a tuple
     """
-    # print(f'Split: {tuple(re.findall(r"\w__([^;]+)", taxonomy))}')
     return tuple(re.findall(r"\w__([^;]+)", taxonomy))
 
 
 def join_taxonomy(taxonomy: Union[Tuple[str, ...], List[str]]) -> str:
     """
     Merge a taxonomy tuple into a string format
     """
@@ -337,43 +333,42 @@
         Add a taxonomy to the hierarchy.
 
         Args:
             taxonomy (str): The taxonomy label to add (e.g. "k__Bacteria; ...").
         """
         return self.add_taxons(split_taxonomy(taxonomy))
 
-    def add_taxons(self, taxonomy: Tuple[str, ...]):
+    def add_taxons(self, taxons: Tuple[str, ...]):
         """
         Add a taxonomy in the form of a taxon tuple to the hierarchy.
 
         Args:
             taxonomy (Tuple[str, ...]): The taxon tuple to add.
         """
-        if isinstance(taxonomy, str):
-            taxonomy = split_taxonomy(taxonomy)
+        taxons = taxons[:self.depth]
         parent: Optional[Taxon] = None
-        for rank, name in enumerate(taxonomy):
+        for rank, name in enumerate(taxons):
             if not self.has_taxon(name, rank):
                 self.__taxon_to_id_map = None
                 self.__id_to_taxon_map = None
                 self.taxons[rank].insert(Taxon(name, rank, parent))
             parent = self.taxons[rank][name]
 
-    def has_entry(self, taxonomy: TaxonomyEntry, strict: bool = False) -> bool:
+    def has_entry(self, entry: TaxonomyEntry, strict: bool = False) -> bool:
         """
         Check if the hierarchy has the given taxonomy.
 
         Args:
-            taxonomy (str): The taxonomy label to check (e.g. "k__Bacteria; ...").
+            entry (str): The taxonomy entry to check
             strict (bool, optional): Ensure every taxon exists. Defaults to False.
 
         Returns:
             bool: The hierarchy contains the taxonomy.
         """
-        return self.has_taxonomy(taxonomy.label, strict)
+        return self.has_taxonomy(entry.label, strict)
 
     def has_taxonomy(self, taxonomy: str, strict: bool = False) -> bool:
         """
         Check if the hierarchy has the given taxonomy.
 
         Args:
             taxonomy (TaxonomyEntry): The taxonomy to check.
@@ -402,30 +397,32 @@
 
     def has_taxons(self, taxons: Tuple[str, ...], strict: bool = False) -> bool:
         """
         Check if the hierarchy has a list of taxons.
 
         Note: When strict == False, a valid hierarchy is assumed.
         """
+        if len(taxons) > self.depth:
+            return False
         if not strict:
             return self.has_taxon(taxons[-1], len(taxons) - 1)
         return all(taxon.casefold() in self.taxons[rank] for rank, taxon in enumerate(taxons))
 
-    def reduce_entry(self, taxonomy: TaxonomyEntry, strict: bool = False) -> TaxonomyEntry:
+    def reduce_entry(self, entry: TaxonomyEntry, strict: bool = False) -> TaxonomyEntry:
         """
         Reduce the taxonomy to a valid known taxonomy label in the hierarchy.
 
         Args:
-            taxonomy (TaxonomyEntry): The taxonomy entry to reduce.
+            entry (TaxonomyEntry): The taxonomy entry to reduce.
             strict (bool, optional): Ensure every taxon exists. Defaults to False.
 
         Returns:
             TaxonomyEntry: A new TaxonomyEntry instance containing the reduced taxonomy label.
         """
-        return replace(taxonomy, label=self.reduce_taxonomy(taxonomy.label, strict))
+        return replace(entry, label=self.reduce_taxonomy(entry.label, strict))
 
     def reduce_taxonomy(self, taxonomy: str, strict: bool = False) -> str:
         """
         Reduce the taxonomy to a valid known taxonomy label in the hierarchy.
 
         Args:
             taxonomy (str): The taxonomy label to reduce (e.g. "k__Bacteria; ...").
@@ -443,14 +440,15 @@
         Args:
             taxons (Tuple[str, ...]): The taxonomy tuple to reduce.
             strict (bool, optional): Ensure every taxon exists. Defaults to False.
 
         Returns:
             Tuple[str, ...]: The reduced taxonomy tuple.
         """
+        taxons = taxons[:self.depth]
         if strict:
             for rank, taxon in enumerate(taxons):
                 if taxon not in self.taxons[rank]:
                     return taxons[:rank]
             return taxons
         for i in range(len(taxons) - 1, -1, -1):
             if taxons[i] in self.taxons[i]:
```

### Comparing `dnadb-0.4.0/src/dnadb/utils.py` & `dnadb-0.4.1/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.0/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.4.1/src/dnadb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.4.0
+Version: 0.4.1
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.4.0/src/dnadb.egg-info/SOURCES.txt` & `dnadb-0.4.1/src/dnadb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

