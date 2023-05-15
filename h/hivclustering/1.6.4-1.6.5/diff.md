# Comparing `tmp/hivclustering-1.6.4.tar.gz` & `tmp/hivclustering-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivclustering-1.6.4.tar", last modified: Mon May 15 19:24:20 2023, max compression
+gzip compressed data, was "hivclustering-1.6.5.tar", last modified: Mon May 15 19:26:24 2023, max compression
```

## Comparing `hivclustering-1.6.4.tar` & `hivclustering-1.6.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:24:20.904826 hivclustering-1.6.4/
--rw-r--r--   0 sweaver    (554) veg        (576)      225 2023-05-15 19:24:20.903826 hivclustering-1.6.4/PKG-INFO
--rw-r--r--   0 sweaver    (554) veg        (576)     8869 2020-07-20 19:37:54.000000 hivclustering-1.6.4/README.md
-drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:24:20.896826 hivclustering-1.6.4/hivclustering/
--rw-r--r--   0 sweaver    (554) veg        (576)       92 2019-03-05 17:22:02.000000 hivclustering-1.6.4/hivclustering/__init__.py
-drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:24:20.891826 hivclustering-1.6.4/hivclustering/data/
-drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:24:20.902826 hivclustering-1.6.4/hivclustering/data/HBL/
--rw-r--r--   0 sweaver    (554) veg        (576)    11479 2019-03-05 17:22:02.000000 hivclustering-1.6.4/hivclustering/data/HBL/CycleSupport.bf
--rw-r--r--   0 sweaver    (554) veg        (576)     6622 2019-03-05 17:22:02.000000 hivclustering-1.6.4/hivclustering/data/HBL/DegreeDistributions.bf
--rw-r--r--   0 sweaver    (554) veg        (576)      616 2015-08-31 19:36:41.000000 hivclustering-1.6.4/hivclustering/data/HBL/ExtractACluster.bf
--rw-r--r--   0 sweaver    (554) veg        (576)      837 2019-03-05 17:22:02.000000 hivclustering-1.6.4/hivclustering/data/HBL/ExtractSequences.bf
--rw-r--r--   0 sweaver    (554) veg        (576)     8264 2015-08-31 19:36:41.000000 hivclustering-1.6.4/hivclustering/data/HBL/SimulateSequence.bf
--rw-r--r--   0 sweaver    (554) veg        (576)     3512 2020-07-20 19:37:54.000000 hivclustering-1.6.4/hivclustering/data/HBL/TriangleSupport.bf
--rw-r--r--   0 sweaver    (554) veg        (576)     5580 2019-09-04 16:11:50.000000 hivclustering-1.6.4/hivclustering/ll.py
--rw-r--r--   0 sweaver    (554) veg        (576)   107327 2020-07-20 19:37:54.000000 hivclustering-1.6.4/hivclustering/mtnetwork.py
--rwxr-xr-x   0 sweaver    (554) veg        (576)    43610 2020-07-20 19:37:54.000000 hivclustering-1.6.4/hivclustering/networkbuild.py
-drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:24:20.899826 hivclustering-1.6.4/hivclustering.egg-info/
--rw-r--r--   0 sweaver    (554) veg        (576)      225 2023-05-15 19:24:20.000000 hivclustering-1.6.4/hivclustering.egg-info/PKG-INFO
--rw-r--r--   0 sweaver    (554) veg        (576)      621 2023-05-15 19:24:20.000000 hivclustering-1.6.4/hivclustering.egg-info/SOURCES.txt
--rw-r--r--   0 sweaver    (554) veg        (576)        1 2023-05-15 19:24:20.000000 hivclustering-1.6.4/hivclustering.egg-info/dependency_links.txt
--rw-r--r--   0 sweaver    (554) veg        (576)       48 2023-05-15 19:24:20.000000 hivclustering-1.6.4/hivclustering.egg-info/requires.txt
--rw-r--r--   0 sweaver    (554) veg        (576)       14 2023-05-15 19:24:20.000000 hivclustering-1.6.4/hivclustering.egg-info/top_level.txt
-drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:24:20.903826 hivclustering-1.6.4/scripts/
--rwxr-xr-x   0 sweaver    (554) veg        (576)    23567 2019-03-05 17:22:02.000000 hivclustering-1.6.4/scripts/TNS
--rwxr-xr-x   0 sweaver    (554) veg        (576)     9069 2020-07-20 19:37:54.000000 hivclustering-1.6.4/scripts/hivnetworkannotate
--rwxr-xr-x   0 sweaver    (554) veg        (576)    33221 2020-07-20 19:41:22.000000 hivclustering-1.6.4/scripts/hivnetworkcsv
--rw-r--r--   0 sweaver    (554) veg        (576)       38 2023-05-15 19:24:20.904826 hivclustering-1.6.4/setup.cfg
--rw-r--r--   0 sweaver    (554) veg        (576)      778 2023-05-15 19:24:11.000000 hivclustering-1.6.4/setup.py
+drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:26:24.762285 hivclustering-1.6.5/
+-rw-r--r--   0 sweaver    (554) veg        (576)      225 2023-05-15 19:26:24.761285 hivclustering-1.6.5/PKG-INFO
+-rw-r--r--   0 sweaver    (554) veg        (576)     8869 2020-07-20 19:37:54.000000 hivclustering-1.6.5/README.md
+drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:26:24.759285 hivclustering-1.6.5/hivclustering/
+-rw-r--r--   0 sweaver    (554) veg        (576)       92 2019-03-05 17:22:02.000000 hivclustering-1.6.5/hivclustering/__init__.py
+drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:26:24.757285 hivclustering-1.6.5/hivclustering/data/
+drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:26:24.761285 hivclustering-1.6.5/hivclustering/data/HBL/
+-rw-r--r--   0 sweaver    (554) veg        (576)    11479 2019-03-05 17:22:02.000000 hivclustering-1.6.5/hivclustering/data/HBL/CycleSupport.bf
+-rw-r--r--   0 sweaver    (554) veg        (576)     6622 2019-03-05 17:22:02.000000 hivclustering-1.6.5/hivclustering/data/HBL/DegreeDistributions.bf
+-rw-r--r--   0 sweaver    (554) veg        (576)      616 2015-08-31 19:36:41.000000 hivclustering-1.6.5/hivclustering/data/HBL/ExtractACluster.bf
+-rw-r--r--   0 sweaver    (554) veg        (576)      837 2019-03-05 17:22:02.000000 hivclustering-1.6.5/hivclustering/data/HBL/ExtractSequences.bf
+-rw-r--r--   0 sweaver    (554) veg        (576)     8264 2015-08-31 19:36:41.000000 hivclustering-1.6.5/hivclustering/data/HBL/SimulateSequence.bf
+-rw-r--r--   0 sweaver    (554) veg        (576)     3512 2020-07-20 19:37:54.000000 hivclustering-1.6.5/hivclustering/data/HBL/TriangleSupport.bf
+-rw-r--r--   0 sweaver    (554) veg        (576)     5580 2019-09-04 16:11:50.000000 hivclustering-1.6.5/hivclustering/ll.py
+-rw-r--r--   0 sweaver    (554) veg        (576)   107327 2020-07-20 19:37:54.000000 hivclustering-1.6.5/hivclustering/mtnetwork.py
+-rwxr-xr-x   0 sweaver    (554) veg        (576)    43547 2023-05-15 19:26:02.000000 hivclustering-1.6.5/hivclustering/networkbuild.py
+drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:26:24.759285 hivclustering-1.6.5/hivclustering.egg-info/
+-rw-r--r--   0 sweaver    (554) veg        (576)      225 2023-05-15 19:26:24.000000 hivclustering-1.6.5/hivclustering.egg-info/PKG-INFO
+-rw-r--r--   0 sweaver    (554) veg        (576)      621 2023-05-15 19:26:24.000000 hivclustering-1.6.5/hivclustering.egg-info/SOURCES.txt
+-rw-r--r--   0 sweaver    (554) veg        (576)        1 2023-05-15 19:26:24.000000 hivclustering-1.6.5/hivclustering.egg-info/dependency_links.txt
+-rw-r--r--   0 sweaver    (554) veg        (576)       48 2023-05-15 19:26:24.000000 hivclustering-1.6.5/hivclustering.egg-info/requires.txt
+-rw-r--r--   0 sweaver    (554) veg        (576)       14 2023-05-15 19:26:24.000000 hivclustering-1.6.5/hivclustering.egg-info/top_level.txt
+drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:26:24.761285 hivclustering-1.6.5/scripts/
+-rwxr-xr-x   0 sweaver    (554) veg        (576)    23567 2019-03-05 17:22:02.000000 hivclustering-1.6.5/scripts/TNS
+-rwxr-xr-x   0 sweaver    (554) veg        (576)     9179 2023-05-15 19:26:02.000000 hivclustering-1.6.5/scripts/hivnetworkannotate
+-rwxr-xr-x   0 sweaver    (554) veg        (576)    33290 2023-05-15 19:26:02.000000 hivclustering-1.6.5/scripts/hivnetworkcsv
+-rw-r--r--   0 sweaver    (554) veg        (576)       38 2023-05-15 19:26:24.762285 hivclustering-1.6.5/setup.cfg
+-rw-r--r--   0 sweaver    (554) veg        (576)      778 2023-05-15 19:26:20.000000 hivclustering-1.6.5/setup.py
```

### Comparing `hivclustering-1.6.4/README.md` & `hivclustering-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.4/hivclustering/data/HBL/CycleSupport.bf` & `hivclustering-1.6.5/hivclustering/data/HBL/CycleSupport.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.4/hivclustering/data/HBL/DegreeDistributions.bf` & `hivclustering-1.6.5/hivclustering/data/HBL/DegreeDistributions.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.4/hivclustering/data/HBL/ExtractACluster.bf` & `hivclustering-1.6.5/hivclustering/data/HBL/ExtractACluster.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.4/hivclustering/data/HBL/ExtractSequences.bf` & `hivclustering-1.6.5/hivclustering/data/HBL/ExtractSequences.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.4/hivclustering/data/HBL/SimulateSequence.bf` & `hivclustering-1.6.5/hivclustering/data/HBL/SimulateSequence.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.4/hivclustering/data/HBL/TriangleSupport.bf` & `hivclustering-1.6.5/hivclustering/data/HBL/TriangleSupport.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.4/hivclustering/ll.py` & `hivclustering-1.6.5/hivclustering/ll.py`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.4/hivclustering/mtnetwork.py` & `hivclustering-1.6.5/hivclustering/mtnetwork.py`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.4/hivclustering/networkbuild.py` & `hivclustering-1.6.5/hivclustering/networkbuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 #!/usr/bin/env python3
 
 import csv
 import argparse
-import operator
 import sys
 import datetime
 import time
 import random
 import os.path
 import json
 import hppy as hy
 import re
-from math import log10, floor, sqrt, exp, log
+from math import sqrt, exp, log
 from hivclustering import *
-from functools import partial
-import multiprocessing
-import hppy as hy
-from operator import itemgetter
-
-
 
 run_settings = None
 uds_settings = None
 
 def settings():
     return run_settings
 
@@ -688,15 +681,17 @@
 
             if len (rec) == 1:
                 run_settings.threshold = rec[0][0]
             else:
                 if len (rec) > 1:
                     suggested_span = max (rec, key = lambda x: x[0])[0] - min (rec, key = lambda x: x[0])[0]
                     mean_diff = sum ([k[1] - profile[i-1][1] for i,k in enumerate(profile[1:])]) / (len (profile)-1)
-                    if (suggested_span / mean_diff < log (len (profile))):
+                    if mean_diff == 0.0:
+                        pass
+                    elif (suggested_span / mean_diff < log (len (profile))):
                         run_settings.threshold = rec[0][0]
 
             if run_settings.threshold is None:
                 if len (rec) == 0:
                     best_guess = sorted (profile, key = lambda r : r[-1], reverse = True)
                     print ('ERROR : Could not automatically determine a distance threshold; no sufficiently strong outlier, best guess %g (score %g)' % (best_guess[0][0], best_guess[0][-1]) , file = sys.stderr)
                 else:
```

### Comparing `hivclustering-1.6.4/hivclustering.egg-info/SOURCES.txt` & `hivclustering-1.6.5/hivclustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.4/scripts/TNS` & `hivclustering-1.6.5/scripts/TNS`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.4/scripts/hivnetworkannotate` & `hivclustering-1.6.5/scripts/hivnetworkannotate`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
 field_input_group.add_argument ('-f', '--field', help = 'Describe an argument to be added to invididual nodes as "name" "label" "type" "transform"; currently supported types are "String", "enum", "Date", "Number"; transform must be specified as a lambda, an empty string to use an identity map, or a python style dict to specify an enum; "fulldate" is a predefined option to reformat the date using the default hivtrace-viz format', nargs = 4, action = 'append')
 field_input_group.add_argument ('-g', '--fields-file', help = 'Read in fields from a JSON file', type = argparse.FileType('r'))
 
 import_settings = arguments.parse_args()
 
 results_json = json.load (import_settings.network)
 
+root_trace_results = False
+
 if('trace_results' in results_json.keys()):
     root_trace_results = True
 
 network_json    = ht_process_network_json(results_json)
 
 # set up record filtering
 
@@ -139,14 +141,15 @@
     index_on = 0
     if import_settings.index:
         index_on = fields.index (import_settings.index)
         if index_on < 0:
             raise "Invalid field to index on (%s)" % import_settings.index
 
     to_import = {}
+
     try:
         for line in csv_reader:
             to_import [line[index_on]] = {}
             total_records += 1
             for i, k in enumerate (line):
                 if i != index_on:
                      to_import [line[index_on]][fields[i]] = k
@@ -168,15 +171,15 @@
 for n, values in to_import.items():
     node_id = id_mapper (n)
     if node_id in nodes_indexed_by_id:
         node_dict = ensure_key (nodes_indexed_by_id[node_id], node_attribute_key)
         for k, val in values.items():
             if k in field_transformations:
                 store_this = field_transformations[k] (val)
-                if store_this is not None:
+                if store_this is not None and node_dict is not None:
                     node_dict[field_names[k]] = store_this
                     if node_id in uninjected_set[field_names[k]]:
                         uninjected_set[field_names[k]].remove (node_id)
 
 print ("\nImport summary", file = sys.stderr)
 print ("\t Records in file  : %d" % total_records, file = sys.stderr)
 print ("\t Nodes in network : %d" % len(network_json ["Nodes"]), file = sys.stderr)
@@ -193,19 +196,19 @@
             node_dict = ensure_key (nodes_indexed_by_id[node_id], node_attribute_key)
             node_dict[values[0]] = values[1]
 
 
 if import_settings.inplace and import_settings.network is not sys.stdin:
     import_settings.output = open (import_settings.network.name, "w")
     
-if 'Settings' in network_json and 'compact_json' in network_json['Settings']:
+if 'Settings' in network_json and 'compact_json' in network_json['Settings'] and network_json['Settings']['compact_json']:
      ht_compress_network_json (network_json)
 
 # Return with trace_results key
 to_return = {}
 if(root_trace_results):
     to_return["trace_results"] = network_json
 else:
     to_return = network_json
 
 
-json.dump(to_return, import_settings.output, separators=(',', ':'))
+json.dump(to_return, import_settings.output, indent=2, separators=(',', ':'))
```

### Comparing `hivclustering-1.6.4/scripts/hivnetworkcsv` & `hivclustering-1.6.5/scripts/hivnetworkcsv`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,16 @@
             for n in network.nodes:
                 n.cluster_id = n.original_cluster_id
                 del n.original_cluster_id
                 
                 
                 
         cluster_summary_info = None
-
+        prior_network_subclusters = None
+        
         if settings().prior is not None:
             try:
                 existing_nodes      = {} # node ID -> cluster ID
                 prior_network       = ht_process_network_json(json.load (settings().prior))
                 
                 
                 if "trace_results" in prior_network.keys():
@@ -613,9 +614,10 @@
 
     if settings().centralities:
         network.write_centralities(settings().centralities)
 
     return network
 
 if __name__ == '__main__':
+    __spec__ = None
     make_hiv_network()
```

### Comparing `hivclustering-1.6.4/setup.py` & `hivclustering-1.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from os.path import abspath, join, split
 from setuptools import setup
 
 sys.path.insert(0, join(split(abspath(__file__))[0], 'lib'))
 
 setup(name='hivclustering',
-      version="1.6.4",
+      version="1.6.5",
       description='HIV molecular clustering tools',
       author='Sergei Kosakovsky Pond',
       author_email='spond@ucsd.edu',
       url='http://github.com/veg/hivclustering',
       license='MIT License',
       packages=['hivclustering'],
       package_data={'hivclustering': [
```

