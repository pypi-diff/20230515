# Comparing `tmp/brain-loop-search-0.1.3.tar.gz` & `tmp/brain-loop-search-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brain-loop-search-0.1.3.tar", last modified: Mon May 15 02:00:28 2023, max compression
+gzip compressed data, was "brain-loop-search-0.1.4.tar", last modified: Mon May 15 02:27:41 2023, max compression
```

## Comparing `brain-loop-search-0.1.3.tar` & `brain-loop-search-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 02:00:28.083319 brain-loop-search-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-05-15 02:00:27.719066 brain-loop-search-0.1.3/.github/
--rw-rw-rw-   0        0        0        6 2023-05-10 08:58:56.000000 brain-loop-search-0.1.3/.github/python-version.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 02:00:27.720063 brain-loop-search-0.1.3/.github/workflows/
--rw-rw-rw-   0        0        0     1447 2023-05-10 08:58:56.000000 brain-loop-search-0.1.3/.github/workflows/static.yml
--rw-rw-rw-   0        0        0     1935 2023-05-10 08:56:44.000000 brain-loop-search-0.1.3/.gitignore
--rw-rw-rw-   0        0        0     1096 2023-04-19 10:12:56.000000 brain-loop-search-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       22 2023-04-19 07:47:30.000000 brain-loop-search-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4968 2023-05-15 02:00:28.071345 brain-loop-search-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4291 2023-05-10 10:11:48.000000 brain-loop-search-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 02:00:27.789389 brain-loop-search-0.1.3/brain_loop_search/
--rw-rw-rw-   0        0        0      290 2023-05-10 05:16:54.000000 brain-loop-search-0.1.3/brain_loop_search/__init__.py
--rw-rw-rw-   0        0        0    10889 2023-05-10 09:11:32.000000 brain-loop-search-0.1.3/brain_loop_search/brain_utils.py
--rw-rw-rw-   0        0        0    12868 2023-05-15 01:59:19.000000 brain-loop-search-0.1.3/brain_loop_search/packing.py
--rw-rw-rw-   0        0        0    19645 2023-05-10 05:50:08.000000 brain-loop-search-0.1.3/brain_loop_search/search.py
--rw-rw-rw-   0        0        0    65506 2023-02-01 17:02:57.000000 brain-loop-search-0.1.3/brain_loop_search/structures.csv
-drwxrwxrwx   0        0        0        0 2023-05-15 02:00:27.809337 brain-loop-search-0.1.3/brain_loop_search.egg-info/
--rw-rw-rw-   0        0        0     4968 2023-05-15 02:00:27.000000 brain-loop-search-0.1.3/brain_loop_search.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-05-15 02:00:27.000000 brain-loop-search-0.1.3/brain_loop_search.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 02:00:27.000000 brain-loop-search-0.1.3/brain_loop_search.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-15 02:00:27.000000 brain-loop-search-0.1.3/brain_loop_search.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-15 02:00:27.000000 brain-loop-search-0.1.3/brain_loop_search.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      984 2023-05-10 08:55:45.000000 brain-loop-search-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 02:00:28.083319 brain-loop-search-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-15 02:00:28.057803 brain-loop-search-0.1.3/test/
--rw-rw-rw-   0        0        0   144508 2023-05-10 08:22:30.000000 brain-loop-search-0.1.3/test/test.png
--rw-rw-rw-   0        0        0   143835 2023-05-10 09:11:39.000000 brain-loop-search-0.1.3/test/test2.png
--rw-rw-rw-   0        0        0     1359 2023-05-10 05:50:08.000000 brain-loop-search-0.1.3/test/test_flow.py
--rw-rw-rw-   0        0        0     2818 2023-05-04 13:57:31.000000 brain-loop-search-0.1.3/test/test_graph_packing.py
--rw-rw-rw-   0        0        0     1128 2023-05-04 13:57:31.000000 brain-loop-search-0.1.3/test/test_ontology.py
--rw-rw-rw-   0        0        0     3588 2023-05-10 05:43:45.000000 brain-loop-search-0.1.3/test/test_sssp.py
--rw-rw-rw-   0        0        0     3400 2023-05-04 13:57:31.000000 brain-loop-search-0.1.3/test/test_vertex_packing.py
--rw-rw-rw-   0        0        0     1135 2023-05-10 08:35:20.000000 brain-loop-search-0.1.3/test/test_vis.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:27:41.194573 brain-loop-search-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-05-15 02:27:41.161795 brain-loop-search-0.1.4/.github/
+-rw-rw-rw-   0        0        0        6 2023-05-10 08:58:56.000000 brain-loop-search-0.1.4/.github/python-version.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 02:27:41.162830 brain-loop-search-0.1.4/.github/workflows/
+-rw-rw-rw-   0        0        0     1447 2023-05-10 08:58:56.000000 brain-loop-search-0.1.4/.github/workflows/static.yml
+-rw-rw-rw-   0        0        0     1935 2023-05-10 08:56:44.000000 brain-loop-search-0.1.4/.gitignore
+-rw-rw-rw-   0        0        0     1096 2023-04-19 10:12:56.000000 brain-loop-search-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-04-19 07:47:30.000000 brain-loop-search-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4968 2023-05-15 02:27:41.193977 brain-loop-search-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4291 2023-05-10 10:11:48.000000 brain-loop-search-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 02:27:41.171041 brain-loop-search-0.1.4/brain_loop_search/
+-rw-rw-rw-   0        0        0      290 2023-05-10 05:16:54.000000 brain-loop-search-0.1.4/brain_loop_search/__init__.py
+-rw-rw-rw-   0        0        0    10889 2023-05-10 09:11:32.000000 brain-loop-search-0.1.4/brain_loop_search/brain_utils.py
+-rw-rw-rw-   0        0        0    13576 2023-05-15 02:26:42.000000 brain-loop-search-0.1.4/brain_loop_search/packing.py
+-rw-rw-rw-   0        0        0    19645 2023-05-10 05:50:08.000000 brain-loop-search-0.1.4/brain_loop_search/search.py
+-rw-rw-rw-   0        0        0    65506 2023-02-01 17:02:57.000000 brain-loop-search-0.1.4/brain_loop_search/structures.csv
+drwxrwxrwx   0        0        0        0 2023-05-15 02:27:41.179839 brain-loop-search-0.1.4/brain_loop_search.egg-info/
+-rw-rw-rw-   0        0        0     4968 2023-05-15 02:27:40.000000 brain-loop-search-0.1.4/brain_loop_search.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-05-15 02:27:41.000000 brain-loop-search-0.1.4/brain_loop_search.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 02:27:40.000000 brain-loop-search-0.1.4/brain_loop_search.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-15 02:27:40.000000 brain-loop-search-0.1.4/brain_loop_search.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-15 02:27:40.000000 brain-loop-search-0.1.4/brain_loop_search.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      984 2023-05-10 08:55:45.000000 brain-loop-search-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-15 02:27:41.194573 brain-loop-search-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 02:27:41.192382 brain-loop-search-0.1.4/test/
+-rw-rw-rw-   0        0        0   144508 2023-05-10 08:22:30.000000 brain-loop-search-0.1.4/test/test.png
+-rw-rw-rw-   0        0        0   143835 2023-05-10 09:11:39.000000 brain-loop-search-0.1.4/test/test2.png
+-rw-rw-rw-   0        0        0     1359 2023-05-10 05:50:08.000000 brain-loop-search-0.1.4/test/test_flow.py
+-rw-rw-rw-   0        0        0     2818 2023-05-04 13:57:31.000000 brain-loop-search-0.1.4/test/test_graph_packing.py
+-rw-rw-rw-   0        0        0     1128 2023-05-04 13:57:31.000000 brain-loop-search-0.1.4/test/test_ontology.py
+-rw-rw-rw-   0        0        0     3588 2023-05-10 05:43:45.000000 brain-loop-search-0.1.4/test/test_sssp.py
+-rw-rw-rw-   0        0        0     3400 2023-05-04 13:57:31.000000 brain-loop-search-0.1.4/test/test_vertex_packing.py
+-rw-rw-rw-   0        0        0     1135 2023-05-10 08:35:20.000000 brain-loop-search-0.1.4/test/test_vis.py
```

### Comparing `brain-loop-search-0.1.3/.github/workflows/static.yml` & `brain-loop-search-0.1.4/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/.gitignore` & `brain-loop-search-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/LICENSE` & `brain-loop-search-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/PKG-INFO` & `brain-loop-search-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brain-loop-search
-Version: 0.1.3
+Version: 0.1.4
 Summary: Screen loops among brain structures(or any entities comprising a graph).
 Author-email: Zuohan Zhao <zzhmark@126.com>
 License: MIT License
 Project-URL: GitHub Project, https://github.com/SEU-ALLEN-codebase/brain-loop-search
 Project-URL: Documentation, https://SEU-ALLEN-codebase.github.io/brain-loop-search
 Keywords: neuron-morphology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `brain-loop-search-0.1.3/README.md` & `brain-loop-search-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/brain_loop_search/brain_utils.py` & `brain-loop-search-0.1.4/brain_loop_search/brain_utils.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/brain_loop_search/packing.py` & `brain-loop-search-0.1.4/brain_loop_search/packing.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     I used this as an abstract interface and make derivation for ccfv3 ontology in brain.
     You can follow my subclass for your own.
 
     I would recommend using pandas for tree representation for its speed and also because you can save some useful info
     as appended columns.
     """
+
     def __init__(self):
         """
         Here, some preprocessing can be done make other functions easier and faster to operate. Also, you need to
         ensure that this is actually a tree.
         """
         pass
 
@@ -105,45 +106,53 @@
         For retrieving the intermediate or final results. To remove mutability, it's turned to tuple. If you need a
         diversion of processing, you can retrieve the intermediate result and make a new pathway.
 
         :return: the stashed vertices' copy as a numpy array.
         """
         return self._vert.copy()
 
-    def filter_by_level(self, fro: int = None, to: int = None):
+    def filter_by_level(self, fro: int = None, to: int = None, invert=False):
         """
         Only retain the vertices within the level range, c style.
 
         Levels are the max count from the current node to its leaves in the tree, staring from 0.
 
         :param fro: the starting level, inclusive, default as None, meaning no limit.
         :param to: the ending level, exclusive, default as None, meaning no limit.
+        :param invert: whether retain the otherwise non-descendents
         """
         levels = self._ont.levels_of(self._vert)
         if fro is not None:
             levels = levels[levels >= fro]
         if to is not None:
             levels = levels[levels < to]
-        self._vert = levels.index
+        if invert:
+            self._vert = self._vert[~self._vert.isin(levels.index)]
+        else:
+            self._vert = levels.index
 
-    def filter_by_depth(self, fro: int = None, to: int = None):
+    def filter_by_depth(self, fro: int = None, to: int = None, invert=False):
         """
         Only retain the vertices within the depth range, c style.
 
         Depths are the count from the current node to its root in the tree, staring from 0.
 
         :param fro: the starting depth, inclusive, default as None, meaning no limit.
         :param to: the ending depth, exclusive, default as None, meaning no limit.
+        :param invert: whether retain the otherwise non-descendents
         """
         depths = self._ont.depths_of(self._vert)
         if fro is not None:
             depths = depths[depths >= fro]
         if to is not None:
             depths = depths[depths < to]
-        self._vert = depths.index
+        if invert:
+            self._vert = self._vert[~self._vert.isin(depths.index)]
+        else:
+            self._vert = depths.index
 
     def filter_super(self):
         """
         Remove any vertices that happen to be the ancestor of another.
         """
         un = set.union(*map(set, self._ont.ancestors_of(self._vert)))
         self._vert = self._vert[~self._vert.isin(un)]
@@ -152,35 +161,42 @@
         """
         Remove any vertices that happen to be the descendent of another.
         """
         vert = set(self._vert)
         tf = [vert.isdisjoint(i) for i in self._ont.ancestors_of(self._vert)]
         self._vert = self._vert[tf]
 
-    def filter_by_immediate_child_of(self, parents: typing.Iterable):
+    def filter_by_immediate_child_of(self, parents: typing.Iterable, invert=False):
         """
         Only retain the direct children under some vertices, which is convenient when you have a big super node with
         many branches below.
 
         :param parents: the direct parent vertices.
+        :param invert: whether retain the otherwise non-descendents
         """
         un = set.union(*map(set, self._ont.immediate_children_of(parents)))
-        self._vert = self._vert[self._vert.isin(un)]
+        if invert:
+            self._vert = self._vert[~self._vert.isin(un)]
+        else:
+            self._vert = self._vert[self._vert.isin(un)]
 
-    def filter_by_descendants_of(self, parents: typing.Iterable, include_parents=False):
+    def filter_by_descendants_of(self, parents: typing.Iterable, include_parents=False, invert=False):
         """
         Only retain the descendents of some vertices.
 
         :param parents: the ancestors.
         :param include_parents: whether to allow the parents to exist in the result, default as not.
+        :param invert: whether retain the otherwise non-descendents
         """
         parents = set(parents)
         tf = map(lambda p: not parents.isdisjoint(p), self._ont.ancestors_of(self._vert))
         if include_parents:
             tf = [*tf] | self._vert.isin(parents)
+        if invert:
+            tf = [not i for i in tf]
         self._vert = self._vert[tf]
 
     def merge_by_level(self, thr):
         """
         Merge the vertices until they are all above the min level or no merge can be done.
 
         Levels are the max count from the current node to its leaves in the tree, staring from 0.
@@ -220,14 +236,15 @@
 
     Taking brain graph as an example, a group of neurons project from regions to regions,
     meaning edge (a, b) can have redundant occurrences with different weights. This is where merging needs to be done.
 
     Sometimes, you want to look into their coarser regions' relations rather than the finer ones. This is where
     rearrangement needs to be done.
     """
+
     def __init__(self, adj_mat: pd.DataFrame, ontology: Ontology):
         """
         :param adj_mat: the adjacent matrix in pandas dataframe, the projection is from rows to columns.
         :param ontology: a derivation of the abstract class `Ontology`.
         """
         # check adjacent matrix
         assert ontology.check_include(adj_mat.index), f"rows contain unrecognizable ID "
```

### Comparing `brain-loop-search-0.1.3/brain_loop_search/search.py` & `brain-loop-search-0.1.4/brain_loop_search/search.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/brain_loop_search/structures.csv` & `brain-loop-search-0.1.4/brain_loop_search/structures.csv`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/brain_loop_search.egg-info/PKG-INFO` & `brain-loop-search-0.1.4/brain_loop_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brain-loop-search
-Version: 0.1.3
+Version: 0.1.4
 Summary: Screen loops among brain structures(or any entities comprising a graph).
 Author-email: Zuohan Zhao <zzhmark@126.com>
 License: MIT License
 Project-URL: GitHub Project, https://github.com/SEU-ALLEN-codebase/brain-loop-search
 Project-URL: Documentation, https://SEU-ALLEN-codebase.github.io/brain-loop-search
 Keywords: neuron-morphology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `brain-loop-search-0.1.3/brain_loop_search.egg-info/SOURCES.txt` & `brain-loop-search-0.1.4/brain_loop_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/pyproject.toml` & `brain-loop-search-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/test/test.png` & `brain-loop-search-0.1.4/test/test.png`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/test/test2.png` & `brain-loop-search-0.1.4/test/test2.png`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/test/test_flow.py` & `brain-loop-search-0.1.4/test/test_flow.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/test/test_graph_packing.py` & `brain-loop-search-0.1.4/test/test_graph_packing.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/test/test_ontology.py` & `brain-loop-search-0.1.4/test/test_ontology.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/test/test_sssp.py` & `brain-loop-search-0.1.4/test/test_sssp.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/test/test_vertex_packing.py` & `brain-loop-search-0.1.4/test/test_vertex_packing.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.3/test/test_vis.py` & `brain-loop-search-0.1.4/test/test_vis.py`

 * *Files identical despite different names*

