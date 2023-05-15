# Comparing `tmp/gctree-4.1.0.tar.gz` & `tmp/gctree-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gctree-4.1.0.tar", last modified: Sat May 13 21:10:34 2023, max compression
+gzip compressed data, was "gctree-4.1.1.tar", last modified: Mon May 15 16:43:34 2023, max compression
```

## Comparing `gctree-4.1.0.tar` & `gctree-4.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:10:34.653152 gctree-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-13 21:10:19.000000 gctree-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-13 21:10:19.000000 gctree-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-13 21:10:34.653152 gctree-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-13 21:10:19.000000 gctree-4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:10:34.653152 gctree-4.1.0/gctree/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-13 21:10:19.000000 gctree-4.1.0/gctree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-13 21:10:34.653152 gctree-4.1.0/gctree/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81899 2023-05-13 21:10:19.000000 gctree-4.1.0/gctree/branching_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-05-13 21:10:19.000000 gctree-4.1.0/gctree/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7706 2023-05-13 21:10:19.000000 gctree-4.1.0/gctree/deduplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-05-13 21:10:19.000000 gctree-4.1.0/gctree/isotype.py
--rw-r--r--   0 runner    (1001) docker     (123)    20657 2023-05-13 21:10:19.000000 gctree-4.1.0/gctree/isotyping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2381 2023-05-13 21:10:19.000000 gctree-4.1.0/gctree/mkconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    23106 2023-05-13 21:10:19.000000 gctree-4.1.0/gctree/mutation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-05-13 21:10:19.000000 gctree-4.1.0/gctree/phylip_parse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1158 2023-05-13 21:10:19.000000 gctree-4.1.0/gctree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:10:34.653152 gctree-4.1.0/gctree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-13 21:10:34.000000 gctree-4.1.0/gctree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-13 21:10:34.000000 gctree-4.1.0/gctree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 21:10:34.000000 gctree-4.1.0/gctree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-13 21:10:34.000000 gctree-4.1.0/gctree.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-13 21:10:34.000000 gctree-4.1.0/gctree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 21:10:34.000000 gctree-4.1.0/gctree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-13 21:10:34.653152 gctree-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-13 21:10:19.000000 gctree-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:10:34.653152 gctree-4.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-13 21:10:19.000000 gctree-4.1.0/tests/test_disambiguate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-13 21:10:19.000000 gctree-4.1.0/tests/test_isotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-13 21:10:19.000000 gctree-4.1.0/tests/test_likelihoods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-13 21:10:19.000000 gctree-4.1.0/tests/test_local_branching.py
--rw-r--r--   0 runner    (1001) docker     (123)    68590 2023-05-13 21:10:19.000000 gctree-4.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:43:34.941223 gctree-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-15 16:43:23.000000 gctree-4.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 16:43:23.000000 gctree-4.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-15 16:43:34.941223 gctree-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-15 16:43:23.000000 gctree-4.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:43:34.945223 gctree-4.1.1/gctree/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 16:43:23.000000 gctree-4.1.1/gctree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-15 16:43:34.945223 gctree-4.1.1/gctree/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81953 2023-05-15 16:43:23.000000 gctree-4.1.1/gctree/branching_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-05-15 16:43:23.000000 gctree-4.1.1/gctree/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7706 2023-05-15 16:43:23.000000 gctree-4.1.1/gctree/deduplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-05-15 16:43:23.000000 gctree-4.1.1/gctree/isotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20657 2023-05-15 16:43:23.000000 gctree-4.1.1/gctree/isotyping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2371 2023-05-15 16:43:23.000000 gctree-4.1.1/gctree/mkconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23106 2023-05-15 16:43:23.000000 gctree-4.1.1/gctree/mutation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-05-15 16:43:23.000000 gctree-4.1.1/gctree/phylip_parse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1158 2023-05-15 16:43:23.000000 gctree-4.1.1/gctree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:43:34.941223 gctree-4.1.1/gctree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-15 16:43:34.000000 gctree-4.1.1/gctree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-15 16:43:34.000000 gctree-4.1.1/gctree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:43:34.000000 gctree-4.1.1/gctree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-15 16:43:34.000000 gctree-4.1.1/gctree.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 16:43:34.000000 gctree-4.1.1/gctree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 16:43:34.000000 gctree-4.1.1/gctree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-15 16:43:34.945223 gctree-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-15 16:43:23.000000 gctree-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:43:34.941223 gctree-4.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-15 16:43:23.000000 gctree-4.1.1/tests/test_disambiguate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-15 16:43:23.000000 gctree-4.1.1/tests/test_isotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-15 16:43:23.000000 gctree-4.1.1/tests/test_likelihoods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-15 16:43:23.000000 gctree-4.1.1/tests/test_local_branching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68590 2023-05-15 16:43:23.000000 gctree-4.1.1/versioneer.py
```

### Comparing `gctree-4.1.0/LICENSE` & `gctree-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gctree-4.1.0/PKG-INFO` & `gctree-4.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: gctree
-Version: 4.1.0
+Version: 4.1.1
 Summary: phylogenetic inference of genotype-collapsed trees
 Home-page: https://github.com/matsengrp/gctree
 Author: Matsen Group
 Author-email: ematsen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="docs/_static/logo.png" width="400"/>
 
 Phylogenetic inference for sequence data with repeated genotypes.
```

### Comparing `gctree-4.1.0/README.md` & `gctree-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gctree-4.1.0/gctree/branching_processes.py` & `gctree-4.1.1/gctree/branching_processes.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,15 +429,15 @@
             self.tree.add_child(child)
 
         if root:
             # create list of (c, m) for each node
             self._build_cm_counts()
 
     def __repr__(self):
-        r"""return a string representation for printing."""
+        r"""Return a string representation for printing."""
         return str(self.tree)
 
     def render(
         self,
         outfile: str,
         scale: Optional[float] = None,
         branch_margin: float = 0,
@@ -1262,27 +1262,29 @@
                 )
 
         # Filter by likelihood, isotype parsimony, mutability,
         # and make ctrees, cforest, and render trees
         dagweight_kwargs = ll_dagfuncs + iso_funcs + mut_funcs + allele_funcs
         trimdag = dag.copy()
         trimdag.trim_optimal_weight(
-            **dagweight_kwargs, optimal_func=lambda l: min(l, key=minfunckey)
+            **dagweight_kwargs,
+            optimal_func=lambda l: min(l, key=minfunckey),  # noqa: E741
         )
         # make sure trimming worked as expected:
         min_weightcounter = trimdag.weight_count(**dagweight_kwargs)
         min_weightset = {minfunckey(key) for key in min_weightcounter}
         if len(min_weightset) != 1:
             raise RuntimeError(
                 "Filtering was not successful. After trimming, these weights are represented:",
                 min_weightset,
             )
 
         best_weighttuple = trimdag.optimal_weight_annotate(
-            **dagweight_kwargs, optimal_func=lambda l: min(l, key=minfunckey)
+            **dagweight_kwargs,
+            optimal_func=lambda l: min(l, key=minfunckey),  # noqa: E741
         )
         if summarize_forest:
             with open(outbase + ".forest_summary.log", "w") as fh:
                 independent_best = []
                 for kwargs in kwargls:
                     # Only summarize for stats for which information was
                     # provided (not just placeholders):
@@ -1343,15 +1345,15 @@
 
         if verbose:
             print_stats([best_weighttuple], "Stats for optimal trees")
 
         return (self._trimmed_self(trimdag), best_weighttuple)
 
     def likelihood_rankplot(self, outbase, p, q, img_type="svg"):
-        """save a rank plot of likelihoods to the file
+        """Save a rank plot of likelihoods to the file
         `[outbase].inference.likelihood_rank.[img_type]`."""
         ll_dagfuncs = _ll_genotype_dagfuncs(p, q)
         if self._forest is not None:
             dag_l = list(
                 float(ll) for ll in self._forest.weight_count(**ll_dagfuncs).elements()
             )
         else:
@@ -1583,15 +1585,15 @@
                     )
         else:
             warnings.warn("No validation was performed on tree")
 
         return ctree
 
     def __repr__(self):
-        r"""return a string representation for printing."""
+        r"""Return a string representation for printing."""
         return f"n_trees = {self.n_trees}\n" "\n".join([str(tree) for tree in self])
 
     def __iter__(self):
         if self._ctrees is not None:
             yield from self._ctrees
         elif self._forest is not None:
             for cladetree in self._forest.get_trees():
@@ -1611,15 +1613,15 @@
     ll: Callable[[np.float64, np.float64], Tuple[np.float64, np.ndarray]], **kwargs
 ) -> Tuple[np.float64, np.float64]:
     # initialization
     x_0 = (0.5, 0.5)
     bounds = ((1e-6, 1 - 1e-6), (1e-6, 1 - 1e-6))
 
     def f(x):
-        """negative log likelihood."""
+        """Negative log likelihood."""
         return tuple(-y for y in ll(*x, **kwargs))
 
     grad_check = sco.check_grad(lambda x: f(x)[0], lambda x: f(x)[1], x_0)
     if grad_check > 1e-3:
         warnings.warn(
             f"gradient mismatches finite difference approximation by {grad_check}",
             RuntimeWarning,
```

### Comparing `gctree-4.1.0/gctree/cli.py` & `gctree-4.1.1/gctree/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             plt.scatter([ps[i]], [qs[j]], c="black", marker="+")
     plt.savefig(args.outbase + ".2." + args.img_type)
 
     return
 
 
 def infer(args):
-    """inference subprogram."""
+    """Inference subprogram."""
 
     def isotype_add(forest):
         forest.add_isotypes(
             isotypemap_file=args.isotype_mapfile,
             idmap_file=args.idmapfile,
             isotype_names=args.isotype_names,
         )
```

### Comparing `gctree-4.1.0/gctree/deduplicate.py` & `gctree-4.1.1/gctree/deduplicate.py`

 * *Files identical despite different names*

### Comparing `gctree-4.1.0/gctree/isotype.py` & `gctree-4.1.1/gctree/isotype.py`

 * *Files identical despite different names*

### Comparing `gctree-4.1.0/gctree/isotyping.py` & `gctree-4.1.1/gctree/isotyping.py`

 * *Files identical despite different names*

### Comparing `gctree-4.1.0/gctree/mkconfig.py` & `gctree-4.1.1/gctree/mkconfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 r"""Read a PHYLIP-format file and produce an appropriate config file for passing
 to `dnapars`.
 
-`dnapars` doesn't play very well in a
-pipeline.  It prompts the user for configuration information and reads
-responses from stdin.  The config file generated by this script is
-meant to mimic the responses to the expected prompts.
+`dnapars` doesn't play very well in a pipeline.  It prompts the user for
+configuration information and reads responses from stdin.  The config
+file generated by this script is meant to mimic the responses to the
+expected prompts.
 
 Typical usage is,
 
-     $ mkconfig sequence.phy > dnapars.cfg
-     $ dnapars < dnapars.cfg
+$ mkconfig sequence.phy > dnapars.cfg $ dnapars < dnapars.cfg
 """
 import os
 import argparse
 
 
 def get_parser():
     parser = argparse.ArgumentParser(description=__doc__)
```

### Comparing `gctree-4.1.0/gctree/mutation_model.py` & `gctree-4.1.1/gctree/mutation_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                         {b: float(x) for b, x in zip("ACGT", fields[1:5])},
                     )
         else:
             self.context_model = None
 
     @staticmethod
     def _disambiguate(sequence):
-        r"""generator of all possible nt sequences implied by a sequence
+        r"""Generator of all possible nt sequences implied by a sequence
         containing ambiguous bases."""
         return _sequence_disambiguations(sequence)
 
     def mutability(self, kmer: str) -> Tuple[np.float64, np.float64]:
         r"""Returns the mutability of a central base of :math:`k`-mer, along
         with nucleotide bias averages over ambiguous ``"N"`` nucleotide
         identities.
```

### Comparing `gctree-4.1.0/gctree/phylip_parse.py` & `gctree-4.1.1/gctree/phylip_parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-
 """Given an outputfile from one of the PHYLIP tools - `dnaml` or `dnapars` -
 produce a CollapsedForest containing the trees in that outputfile."""
 
 import gctree.branching_processes as bp
 import gctree.utils
 
 from ete3 import Tree
@@ -96,15 +95,15 @@
     return seqs
 
 
 # parse the dnaml output file and return data structures containing a
 # list biopython.SeqRecords and a dict containing adjacency
 # relationships and distances between nodes.
 def parse_outfile(outfile, abundance_file=None, root="root", disambiguate=False):
-    """parse phylip outfile, and return dnapars trees."""
+    """Parse phylip outfile, and return dnapars trees."""
     if abundance_file is not None:
         counts = {
             line.split(",")[0]: int(line.split(",")[1]) for line in open(abundance_file)
         }
     # No count, just make an empty count dictionary:
     else:
         counts = None
```

### Comparing `gctree-4.1.0/gctree/utils.py` & `gctree-4.1.1/gctree/utils.py`

 * *Files identical despite different names*

### Comparing `gctree-4.1.0/gctree.egg-info/PKG-INFO` & `gctree-4.1.1/gctree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: gctree
-Version: 4.1.0
+Version: 4.1.1
 Summary: phylogenetic inference of genotype-collapsed trees
 Home-page: https://github.com/matsengrp/gctree
 Author: Matsen Group
 Author-email: ematsen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="docs/_static/logo.png" width="400"/>
 
 Phylogenetic inference for sequence data with repeated genotypes.
```

### Comparing `gctree-4.1.0/gctree.egg-info/SOURCES.txt` & `gctree-4.1.1/gctree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gctree-4.1.0/setup.py` & `gctree-4.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                                       "phylip_parse=gctree.phylip_parse:main"]},
     packages=['gctree'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.7, <3.10",
+    python_requires=">=3.7",
     install_requires=[
         "PyQt5",
         "ete3",
         "biopython",
         "matplotlib",
         "pandas",
         "scipy",
```

### Comparing `gctree-4.1.0/tests/test_disambiguate.py` & `gctree-4.1.1/tests/test_disambiguate.py`

 * *Files identical despite different names*

### Comparing `gctree-4.1.0/tests/test_isotype.py` & `gctree-4.1.1/tests/test_isotype.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         idmap_file="tests/example_output/original/idmap.txt",
     )
     # isotypemap_file=None,
     # idmap=None,
     # idmap_file=None,
     # isotype_names=None,
     tdag = dag.copy()
-    tdag.optimal_weight_annotate(**kwargs, optimal_func=lambda l: l[0])
+    tdag.optimal_weight_annotate(**kwargs, optimal_func=lambda l: l[0])  # noqa: E741
     for node in tdag.preorder():
         if node.attr is not None:
             node.attr["isotype"] = node._dp_data
     kwargs = _isotype_dagfuncs()
     c = tdag.weight_count(**kwargs)
     key = min(c)
     count = c[key]
```

### Comparing `gctree-4.1.0/tests/test_likelihoods.py` & `gctree-4.1.1/tests/test_likelihoods.py`

 * *Files identical despite different names*

### Comparing `gctree-4.1.0/tests/test_local_branching.py` & `gctree-4.1.1/tests/test_local_branching.py`

 * *Files identical despite different names*

### Comparing `gctree-4.1.0/versioneer.py` & `gctree-4.1.1/versioneer.py`

 * *Files identical despite different names*

