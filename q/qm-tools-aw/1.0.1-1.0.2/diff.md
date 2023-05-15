# Comparing `tmp/qm_tools_aw-1.0.1.tar.gz` & `tmp/qm_tools_aw-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qm_tools_aw-1.0.1.tar", last modified: Mon May  1 14:11:00 2023, max compression
+gzip compressed data, was "qm_tools_aw-1.0.2.tar", last modified: Mon May 15 17:14:28 2023, max compression
```

## Comparing `qm_tools_aw-1.0.1.tar` & `qm_tools_aw-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:11:00.382060 qm_tools_aw-1.0.1/
--rw-r--r--   0 austinwallace   (501) staff       (20)     1074 2023-03-27 20:06:41.000000 qm_tools_aw-1.0.1/LICENSE
--rw-r--r--   0 austinwallace   (501) staff       (20)      689 2023-05-01 14:11:00.382150 qm_tools_aw-1.0.1/PKG-INFO
--rw-r--r--   0 austinwallace   (501) staff       (20)      107 2023-03-27 20:06:41.000000 qm_tools_aw-1.0.1/README.md
--rw-r--r--   0 austinwallace   (501) staff       (20)      649 2023-05-01 14:10:54.000000 qm_tools_aw-1.0.1/pyproject.toml
--rw-r--r--   0 austinwallace   (501) staff       (20)      202 2023-05-01 14:11:00.382521 qm_tools_aw-1.0.1/setup.cfg
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:11:00.378329 qm_tools_aw-1.0.1/src/
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:11:00.379927 qm_tools_aw-1.0.1/src/qm_tools_aw/
--rw-r--r--   0 austinwallace   (501) staff       (20)       20 2023-03-27 20:06:41.000000 qm_tools_aw-1.0.1/src/qm_tools_aw/__init__.py
--rw-r--r--   0 austinwallace   (501) staff       (20)     6177 2023-03-27 20:06:41.000000 qm_tools_aw-1.0.1/src/qm_tools_aw/tools.py
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:11:00.381823 qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/
--rw-r--r--   0 austinwallace   (501) staff       (20)      689 2023-05-01 14:11:00.000000 qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/PKG-INFO
--rw-r--r--   0 austinwallace   (501) staff       (20)      323 2023-05-01 14:11:00.000000 qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/SOURCES.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-05-01 14:11:00.000000 qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/dependency_links.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)       32 2023-05-01 14:11:00.000000 qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/requires.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)       12 2023-05-01 14:11:00.000000 qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/top_level.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-03-27 20:27:35.000000 qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/zip-safe
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-15 17:14:28.272624 qm_tools_aw-1.0.2/
+-rw-r--r--   0 austinwallace   (501) staff       (20)     1074 2023-03-27 20:06:41.000000 qm_tools_aw-1.0.2/LICENSE
+-rw-r--r--   0 austinwallace   (501) staff       (20)      689 2023-05-15 17:14:28.272745 qm_tools_aw-1.0.2/PKG-INFO
+-rw-r--r--   0 austinwallace   (501) staff       (20)      107 2023-03-27 20:06:41.000000 qm_tools_aw-1.0.2/README.md
+-rw-r--r--   0 austinwallace   (501) staff       (20)      649 2023-05-15 17:14:23.000000 qm_tools_aw-1.0.2/pyproject.toml
+-rw-r--r--   0 austinwallace   (501) staff       (20)      202 2023-05-15 17:14:28.273233 qm_tools_aw-1.0.2/setup.cfg
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-15 17:14:28.268759 qm_tools_aw-1.0.2/src/
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-15 17:14:28.270557 qm_tools_aw-1.0.2/src/qm_tools_aw/
+-rw-r--r--   0 austinwallace   (501) staff       (20)       20 2023-03-27 20:06:41.000000 qm_tools_aw-1.0.2/src/qm_tools_aw/__init__.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     7725 2023-05-15 17:13:26.000000 qm_tools_aw-1.0.2/src/qm_tools_aw/tools.py
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-15 17:14:28.272369 qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/
+-rw-r--r--   0 austinwallace   (501) staff       (20)      689 2023-05-15 17:14:28.000000 qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/PKG-INFO
+-rw-r--r--   0 austinwallace   (501) staff       (20)      323 2023-05-15 17:14:28.000000 qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/SOURCES.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-05-15 17:14:28.000000 qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/dependency_links.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)       32 2023-05-15 17:14:28.000000 qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/requires.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)       12 2023-05-15 17:14:28.000000 qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/top_level.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-03-27 20:27:35.000000 qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/zip-safe
```

### Comparing `qm_tools_aw-1.0.1/LICENSE` & `qm_tools_aw-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qm_tools_aw-1.0.1/PKG-INFO` & `qm_tools_aw-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qm_tools_aw
-Version: 1.0.1
+Version: 1.0.2
 Summary: Provides some functions that I have found value in reusing for quantum chemistry related tasks.
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/qm_tools
 Project-URL: Bug Tracker, https://github.com/Awallace3/qm_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qm_tools_aw-1.0.1/pyproject.toml` & `qm_tools_aw-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qm_tools_aw"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Austin M. Wallace", email="awallace43@gatech.edu" },
 ]
 description = "Provides some functions that I have found value in reusing for quantum chemistry related tasks."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `qm_tools_aw-1.0.1/src/qm_tools_aw/tools.py` & `qm_tools_aw-1.0.2/src/qm_tools_aw/tools.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pickle
 import numpy as np
 from periodictable import elements
 import qcelemental as qcel
+import pandas as pd
 
 
 def create_pt_dict():
     """
     create_pt_dict creates dictionary for string elements to atomic number.
     """
     el_dc = {}
@@ -29,14 +30,28 @@
     for n, r in enumerate(carts):
         e, x, y, z = r
         line = "{:d}\t{:.10f}\t{:.10f}\t{:.10f}\n".format(int(e), x, y, z)
         w += line
     return w
 
 
+def convert_schr_row_to_mol(r) -> qcel.models.Molecule:
+    """
+    convert_schr_row_to_mol
+    """
+    ma, mb = r['monAs'], r['monBs']
+    g1, g2 = r['Geometry'][ma], r['Geometry'][mb]
+    m1 = f"{r['charges'][1][0]} {r['charges'][1][1]}\n"
+    m1 += print_cartesians_pos_carts(g1[:,0], g1[:,1:], only_results=True)
+    m2 = f"{r['charges'][2][0]} {r['charges'][2][1]}\n"
+    m2 += print_cartesians_pos_carts(g2[:,0], g2[:,1:], only_results=True)
+    mol = qcel.models.Molecule.from_data(m1 + "--\n" + m2)
+    return mol
+
+
 def string_carts_to_np(geom):
     geom = geom.split("\n")
     if geom[0] == "":
         geom = geom[1:]
     mols = []
     m = []
     charges = [[0, 1]]
@@ -98,14 +113,15 @@
     for a in arr:
         for i, elem in enumerate(a):
             if i == 0:
                 print("{} ".format(int(elem)), end="\t")
             else:
                 print("{:.10f} ".format(elem).rjust(3), end="\t")
         print(end="\n")
+    return
 
 
 def print_cartesians_dimer(geom, monAs, monBs, charges) -> str:
     """
     print_cartesians_dimer takes in dimer geometry and splits
     by monAs and monBs slicing to produce monomers. The
     charges are mult and charge.
@@ -117,37 +133,69 @@
     print_cartesians(m1)
     print(f"--")
     print(*c2)
     print_cartesians(m2)
     return
 
 
-def print_cartesians_pos_carts(pos: np.array, carts: np.array):
+def print_cartesians_pos_carts(pos: np.array, carts: np.array, only_results=False):
     """
     prints a 2-D numpy array in a nicer format
     """
-    print()
+    if not only_results:
+        print()
     lines = ""
     for n, r in enumerate(carts):
         x, y, z = r
         line = "{}\t{:.10f}\t{:.10f}\t{:.10f}".format(int(pos[n]), x, y, z)
         lines += line + "\n"
-        print(line)
-    print()
+        if not only_results:
+            print(line)
+    if not only_results:
+        print()
     return lines
 
+# def return_cartesians_pos_carts(pos: np.array, carts: np.array):
+#     """
+#     prints a 2-D numpy array in a nicer format
+#     """
+#     print()
+#     lines = ""
+#     for n, r in enumerate(carts):
+#         x, y, z = r
+#         line = "{}\t{:.10f}\t{:.10f}\t{:.10f}".format(int(pos[n]), x, y, z)
+#         lines += line + "\n"
+#         print(line)
+#     print()
+#     return lines
+
+def carts_to_xyz(pos: np.array, carts: np.array, el_dc=create_el_num_to_symbol()):
+    """
+    creates xyz file from pos and carts
+    """
+    out = ""
+    start = f"{len(pos)}\n\n"
+    out += start
+    for n, r in enumerate(carts):
+        x, y, z = r
+        line = "{}\t{:.10f}\t{:.10f}\t{:.10f}\n".format(el_dc[int(pos[n])], x, y, z)
+        out += line
+    return out
+
 
 def write_cartesians_to_xyz(pos: np.array, carts: np.array, fn="out.xyz"):
     """
     creates xyz file from pos and carts
     """
     el_dc = create_el_num_to_symbol()
     out = ""
     with open(fn, "w") as f:
-        f.write(f"{len(pos)}\n\n")
+        start = f"{len(pos)}\n\n"
+        out += start
+        f.write(start)
         for n, r in enumerate(carts):
             x, y, z = r
             line = "{}\t{:.10f}\t{:.10f}\t{:.10f}\n".format(el_dc[int(pos[n])], x, y, z)
             out += line
             f.write(line)
     return out
 
@@ -158,26 +206,29 @@
 
 
 def read_pickle(fname="data.pickle"):
     with open(fname, "rb") as handle:
         return pickle.load(handle)
 
 
-def read_xyz_to_pos_carts(xyz_path="mol.xyz") -> (np.array, np.array):
+def read_xyz_to_pos_carts(xyz_path="mol.xyz",) -> (np.array, np.array):
     """
     read_xyz_to_pos_carts reads xyz file and returns pos and carts
     """
     el_dc = create_pt_dict()
     with open(xyz_path, "r") as f:
         d = f.readlines()[2:]
 
     pos, carts = [], []
     for l in d:
         l = l.split()
-        el = el_dc[l[0]]
+        if l[0].isnumeric():
+            el = int(l[0])
+        else:
+            el = el_dc[l[0]]
         x, y, z = float(l[1]), float(l[2]), float(l[3])
         pos.append(el)
         carts.append([x, y, z])
     return np.array(pos), np.array(carts)
 
 
 def convert_geom_str_to_dimer_splits(geom, units_angstroms=True) -> [np.array, np.array, np.array, np.array]:
```

### Comparing `qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/PKG-INFO` & `qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qm-tools-aw
-Version: 1.0.1
+Version: 1.0.2
 Summary: Provides some functions that I have found value in reusing for quantum chemistry related tasks.
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/qm_tools
 Project-URL: Bug Tracker, https://github.com/Awallace3/qm_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

