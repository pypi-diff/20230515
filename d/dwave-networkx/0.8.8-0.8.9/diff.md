# Comparing `tmp/dwave_networkx-0.8.8.tar.gz` & `tmp/dwave_networkx-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dwave_networkx-0.8.8.tar", last modified: Thu Sep 17 11:48:53 2020, max compression
+gzip compressed data, was "dist/dwave_networkx-0.8.9.tar", last modified: Thu Sep  9 21:31:48 2021, max compression
```

## Comparing `dwave_networkx-0.8.8.tar` & `dwave_networkx-0.8.9.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-17 11:48:53.000000 dwave_networkx-0.8.8/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1659 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-17 11:48:53.000000 dwave_networkx-0.8.8/dwave_networkx.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1228 2020-09-17 11:48:53.000000 dwave_networkx-0.8.8/dwave_networkx.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       15 2020-09-17 11:48:53.000000 dwave_networkx-0.8.8/dwave_networkx.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-09-17 11:48:53.000000 dwave_networkx-0.8.8/dwave_networkx.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2020-09-17 11:48:53.000000 dwave_networkx-0.8.8/dwave_networkx.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2555 2020-09-17 11:48:53.000000 dwave_networkx-0.8.8/dwave_networkx.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2020-09-17 11:48:53.000000 dwave_networkx-0.8.8/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2555 2020-09-17 11:48:53.000000 dwave_networkx-0.8.8/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1908 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-17 11:48:53.000000 dwave_networkx-0.8.8/dwave_networkx/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4632 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/default_sampler.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-17 11:48:53.000000 dwave_networkx-0.8.8/dwave_networkx/generators/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34412 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/generators/pegasus.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17585 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/generators/chimera.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4590 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/generators/markov.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      867 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/generators/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-17 11:48:53.000000 dwave_networkx-0.8.8/dwave_networkx/algorithms/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6835 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/algorithms/cover.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4884 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/algorithms/canonicalization.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28042 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/algorithms/elimination_ordering.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4358 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/algorithms/max_cut.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7027 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/algorithms/clique.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9401 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/algorithms/independent_set.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6944 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/algorithms/social.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7143 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/algorithms/markov.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13614 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/algorithms/coloring.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7321 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/algorithms/tsp.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12355 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/algorithms/matching.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1262 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/algorithms/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-17 11:48:53.000000 dwave_networkx-0.8.8/dwave_networkx/drawing/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12336 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/drawing/chimera_layout.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12205 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/drawing/pegasus_layout.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19379 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/drawing/qubit_layout.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39330 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/drawing/distinguishable_colors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/drawing/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1131 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      927 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/package_info.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-17 11:48:53.000000 dwave_networkx-0.8.8/dwave_networkx/utils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6291 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/utils/decorators.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      757 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/utils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1262 2020-09-17 11:48:36.000000 dwave_networkx-0.8.8/dwave_networkx/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:31:48.000000 dwave_networkx-0.8.9/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10059 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2460 2021-09-09 21:31:48.000000 dwave_networkx-0.8.9/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1648 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/README.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:31:48.000000 dwave_networkx-0.8.9/dwave_networkx/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1084 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:31:48.000000 dwave_networkx-0.8.9/dwave_networkx/algorithms/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1162 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/algorithms/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4850 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/algorithms/canonicalization.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6882 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/algorithms/clique.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13482 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/algorithms/coloring.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6735 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/algorithms/cover.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    27946 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/algorithms/elimination_ordering.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9355 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/algorithms/independent_set.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7252 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/algorithms/markov.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11670 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/algorithms/matching.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4969 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/algorithms/max_cut.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6680 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/algorithms/social.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7207 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/algorithms/tsp.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4532 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/default_sampler.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:31:48.000000 dwave_networkx-0.8.9/dwave_networkx/drawing/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      715 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/drawing/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12024 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/drawing/chimera_layout.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39229 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/drawing/distinguishable_colors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11851 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/drawing/pegasus_layout.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18974 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/drawing/qubit_layout.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1031 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/exceptions.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:31:48.000000 dwave_networkx-0.8.9/dwave_networkx/generators/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      767 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/generators/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17393 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/generators/chimera.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4449 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/generators/markov.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34219 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/generators/pegasus.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      827 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/package_info.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:31:48.000000 dwave_networkx-0.8.9/dwave_networkx/utils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      757 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/utils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6191 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/dwave_networkx/utils/decorators.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:31:48.000000 dwave_networkx-0.8.9/dwave_networkx.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2460 2021-09-09 21:31:48.000000 dwave_networkx-0.8.9/dwave_networkx.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1240 2021-09-09 21:31:48.000000 dwave_networkx-0.8.9/dwave_networkx.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-09-09 21:31:48.000000 dwave_networkx-0.8.9/dwave_networkx.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      101 2021-09-09 21:31:48.000000 dwave_networkx-0.8.9/dwave_networkx.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       15 2021-09-09 21:31:48.000000 dwave_networkx-0.8.9/dwave_networkx.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      107 2021-09-09 21:31:48.000000 dwave_networkx-0.8.9/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2021-09-09 21:31:24.000000 dwave_networkx-0.8.9/setup.py
```

### Comparing `dwave_networkx-0.8.8/README.rst` & `dwave_networkx-0.8.9/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 .. image:: https://img.shields.io/pypi/v/dwave-networkx.svg
-    :target: https://pypi.python.org/pypi/dwave-networkx
+    :target: https://pypi.org/project/dwave-networkx
 
 .. image:: https://readthedocs.com/projects/d-wave-systems-dwave-networkx/badge/?version=latest
     :target: https://docs.ocean.dwavesys.com/projects/dwave-networkx/en/latest/?badge=latest
 
-.. image:: https://codecov.io/gh/dwavesystems/dwave_networkx/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/dwavesystems/dwave_networkx
+.. image:: https://codecov.io/gh/dwavesystems/dwave-networkx/branch/main/graph/badge.svg
+    :target: https://codecov.io/gh/dwavesystems/dwave-networkx
 
-.. image:: https://circleci.com/gh/dwavesystems/dwave_networkx.svg?style=svg
-    :target: https://circleci.com/gh/dwavesystems/dwave_networkx
+.. image:: https://circleci.com/gh/dwavesystems/dwave-networkx.svg?style=svg
+    :target: https://circleci.com/gh/dwavesystems/dwave-networkx
 
 .. inclusion-marker-do-not-remove
 
 D-Wave NetworkX
 ===============
 
 .. index-start-marker
 
-D-Wave NetworkX is an extension of `NetworkX <http://networkx.github.io>`_\ ---a
+D-Wave NetworkX is an extension of `NetworkX <https://networkx.org>`_\ ---a
 Python language package for exploration and analysis of networks and network
 algorithms---for users of D-Wave Systems. It provides tools for working with
 Chimera graphs and implementations of graph-theory algorithms on the D-Wave
 system and other binary quadratic model samplers.
 
 The example below generates a graph for a Chimera unit cell (eight nodes in a 4-by-2
 bipartite architecture).
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx.egg-info/SOURCES.txt` & `dwave_networkx-0.8.9/dwave_networkx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.rst
 setup.cfg
 setup.py
 dwave_networkx/__init__.py
 dwave_networkx/default_sampler.py
 dwave_networkx/exceptions.py
 dwave_networkx/package_info.py
```

### Comparing `dwave_networkx-0.8.8/setup.py` & `dwave_networkx-0.8.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,50 +7,57 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 import os
-import sys
 
 from setuptools import setup
 
 # run from the base path
 my_loc = os.path.dirname(os.path.abspath(__file__))
 os.chdir(my_loc)
 
-# add __version__, __author__, __authoremail__, __description__ to this namespace
-_PY2 = sys.version_info.major == 2
-if _PY2:
-    execfile(os.path.join(".", "dwave_networkx", "package_info.py"))
-else:
-    exec(open(os.path.join(".", "dwave_networkx", "package_info.py")).read())
+exec(open(os.path.join(".", "dwave_networkx", "package_info.py")).read())
 
 packages = ['dwave_networkx',
             'dwave_networkx.algorithms',
             'dwave_networkx.utils',
             'dwave_networkx.drawing',
             'dwave_networkx.generators',
             ]
 
 install_requires = ['networkx>=2.0,<3.0',
                     'decorator>=4.1.0,<5.0.0',
-                    'dimod>=0.8.0',
+                    'dimod>=0.8.0,!=0.10.0,!=0.10.1,!=0.10.2,!=0.10.3,!=0.10.4',
                     ]
 
+python_requires = ">=3.6"
+
+classifiers = [
+    'License :: OSI Approved :: Apache Software License',
+    'Operating System :: OS Independent',
+    'Programming Language :: Python :: 3 :: Only',
+    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+]
+
 setup(
     name='dwave_networkx',
     version=__version__,
     author=__author__,
     author_email=__authoremail__,
     description=__description__,
     long_description=open('README.rst').read(),
     url='https://github.com/dwavesystems/dwave_networkx',
     download_url='https://github.com/dwavesystems/dwave_networkx/releases',
     packages=packages,
     license='Apache 2.0',
     install_requires=install_requires,
+    python_requires=python_requires,
+    classifiers=classifiers,
 )
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/default_sampler.py` & `dwave_networkx-0.8.9/dwave_networkx/default_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 """Sets a binary quadratic model sampler used by default
 for functions that require a sample when none is specified.
 
 A sampler is a process that samples
 from low-energy states in models defined by an Ising equation
 or a Quadratic Unconstrained Binary Optimization Problem
 (QUBO).
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/generators/pegasus.py` & `dwave_networkx-0.8.9/dwave_networkx/generators/pegasus.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,36 +7,29 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 """
 Generators for some graphs derived from the D-Wave System.
-
 """
 import re
 
 import networkx as nx
 
-from dwave_networkx import _PY2
 from dwave_networkx.exceptions import DWaveNetworkXException
 import warnings
 
 __all__ = ['pegasus_graph',
            'pegasus_coordinates',
            ]
 
-# compatibility for python 2/3
-if _PY2:
-    range = xrange
-
 
 def pegasus_graph(m, create_using=None, node_list=None, edge_list=None, data=True,
                   offset_lists=None, offsets_index=None, coordinates=False, fabric_only=True,
                   nice_coordinates=False):
     """
     Creates a Pegasus graph with size parameter `m`.
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/generators/chimera.py` & `dwave_networkx-0.8.9/dwave_networkx/generators/chimera.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,39 +7,33 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 """
 Generators for graphs derived from the D-Wave System.
 
 """
 import warnings
 
 import networkx as nx
 from networkx.algorithms.bipartite import color
 from networkx import diameter
 
-from dwave_networkx import _PY2
 from dwave_networkx.exceptions import DWaveNetworkXException
 
 __all__ = ['chimera_graph',
            'chimera_coordinates',
            'find_chimera_indices',
            'chimera_to_linear',
            'linear_to_chimera']
 
-# compatibility for python 2/3
-if _PY2:
-    range = xrange
-
 
 def chimera_graph(m, n=None, t=None, create_using=None, node_list=None, edge_list=None, data=True, coordinates=False):
     """Creates a Chimera lattice of size (m, n, t).
 
     Parameters
     ----------
     m : int
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/generators/markov.py` & `dwave_networkx-0.8.9/dwave_networkx/generators/markov.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,22 +7,17 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# =============================================================================
-import itertools
 
-try:
-    import collections.abc as abc
-except ImportError:
-    import collections as abc
+import itertools
+import collections.abc as abc
 
 from collections import namedtuple
 
 import networkx as nx
 
 
 __all__ = 'markov_network',
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/generators/__init__.py` & `dwave_networkx-0.8.9/dwave_networkx/generators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,12 +7,11 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 from dwave_networkx.generators.chimera import *
 from dwave_networkx.generators.markov import markov_network
 from dwave_networkx.generators.pegasus import *
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/algorithms/cover.py` & `dwave_networkx-0.8.9/dwave_networkx/algorithms/cover.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 from dwave_networkx.algorithms.independent_set import maximum_weighted_independent_set
 from dwave_networkx.utils import binary_quadratic_model_sampler
 
 __all__ = ['min_weighted_vertex_cover', 'min_vertex_cover', 'is_vertex_cover']
 
 
 @binary_quadratic_model_sampler(2)
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/algorithms/canonicalization.py` & `dwave_networkx-0.8.9/dwave_networkx/algorithms/canonicalization.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from __future__ import division
-
-
 import math
 
 from dwave_networkx.generators.chimera import chimera_coordinates
 
 __all__ = ['canonical_chimera_labeling']
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/algorithms/elimination_ordering.py` & `dwave_networkx-0.8.9/dwave_networkx/algorithms/elimination_ordering.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# =============================================================================
+
 import itertools
+
 from random import random, sample
 
 import networkx as nx
 
 from dwave_networkx.generators.pegasus import pegasus_coordinates
 
 __all__ = ['is_almost_simplicial',
@@ -890,15 +890,15 @@
     -------
     order : list
         An elimination order that provides an upper bound on the treewidth.
 
 
     .. [bbrr] Boothby, K., P. Bunky, J. Raymond, A. Roy. Next-Generation Topology
        of D-Wave Quantum Processors. Technical Report, Februrary 2019.
-       https://www.dwavesys.com/resources/publications?type=white#publication-987
+       https://www.dwavesys.com/resources/publications?type=white
 
     """
     m = n
     l = 12
 
     # ordering for horizontal qubits in each tile, from east to west:
     h_order = [4, 5, 6, 7, 0, 1, 2, 3, 8, 9, 10, 11]
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/algorithms/max_cut.py` & `dwave_networkx-0.8.9/dwave_networkx/algorithms/max_cut.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2018 D-Wave Systems Inc.
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+
 from dwave_networkx.exceptions import DWaveNetworkXException
 from dwave_networkx.utils import binary_quadratic_model_sampler
 
 __all__ = ["maximum_cut", "weighted_maximum_cut"]
 
 
 @binary_quadratic_model_sampler(1)
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/algorithms/clique.py` & `dwave_networkx-0.8.9/dwave_networkx/algorithms/clique.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,18 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
-from __future__ import division
+
 import networkx as nx
 import dwave_networkx as dnx
+
 from dwave_networkx.utils import binary_quadratic_model_sampler
 
 __all__ = ["maximum_clique", "clique_number", "is_clique"]
 
 @binary_quadratic_model_sampler(1)
 def maximum_clique(G, sampler=None, lagrange=2.0, **sampler_args):
     """
@@ -69,15 +68,15 @@
     Samplers by their nature may not return the optimal solution. This
     function does not attempt to confirm the quality of the returned
     sample.
 
     References
     ----------
 
-    `Maximum Clique on Wikipedia <https://en.wikipedia.org/wiki/Maximum_clique(graph_theory)>`_
+    `Maximum Clique on Wikipedia <https://en.wikipedia.org/wiki/Clique_(graph_theory)>`_
 
     `Independent Set on Wikipedia <https://en.wikipedia.org/wiki/Independent_set_(graph_theory)>`_
 
     `QUBO on Wikipedia <https://en.wikipedia.org/wiki/Quadratic_unconstrained_binary_optimization>`_
 
     .. [AL] Lucas, A. (2014). Ising formulations of many NP problems.
        Frontiers in Physics, Volume 2, Article 5.
@@ -138,15 +137,15 @@
     Samplers by their nature may not return the optimal solution. This
     function does not attempt to confirm the quality of the returned
     sample.
 
     References
     ----------
 
-    `Maximum Clique on Wikipedia <https://en.wikipedia.org/wiki/Maximum_clique(graph_theory)>`_
+    `Maximum Clique on Wikipedia <https://en.wikipedia.org/wiki/Clique_(graph_theory)>`_
     """
     return len(maximum_clique(G, sampler, lagrange, **sampler_args))
 
 def is_clique(G, clique_nodes):
     """Determines whether the given nodes form a clique.
 
     A clique is a subset of nodes of an undirected graph such that every two
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/algorithms/independent_set.py` & `dwave_networkx-0.8.9/dwave_networkx/algorithms/independent_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
-from __future__ import division
 
 from dwave_networkx.utils import binary_quadratic_model_sampler
 
-__all__ = ["maximum_weighted_independent_set", "maximum_independent_set", "is_independent_set"]
+__all__ = ["maximum_weighted_independent_set",
+           "maximum_weighted_independent_set_qubo",
+           "maximum_independent_set",
+           "is_independent_set",
+           ]
 
 
 @binary_quadratic_model_sampler(2)
 def maximum_weighted_independent_set(G, weight=None, sampler=None, lagrange=2.0, **sampler_args):
     """Returns an approximate maximum weighted independent set.
 
     Defines a QUBO with ground states corresponding to a
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/algorithms/social.py` & `dwave_networkx-0.8.9/dwave_networkx/algorithms/social.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,19 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 from dwave_networkx.utils import binary_quadratic_model_sampler
-from dwave_networkx import _PY2
 
 __all__ = ["structural_imbalance"]
 
-# compatibility for python 2/3
-if _PY2:
-    def iteritems(d): return d.iteritems()
-else:
-    def iteritems(d): return d.items()
-
 
 @binary_quadratic_model_sampler(1)
 def structural_imbalance(S, sampler=None, **sampler_args):
     """Returns an approximate set of frustrated edges and a bicoloring.
 
     A signed social network graph is a graph whose signed edges
     represent friendly/hostile interactions between nodes. A
@@ -113,15 +105,15 @@
     # use the sampler to find low energy states
     response = sampler.sample_ising(h, J, **sampler_args)
 
     # we want the lowest energy sample
     sample = next(iter(response))
 
     # spins determine the color
-    colors = {v: (spin + 1) // 2 for v, spin in iteritems(sample)}
+    colors = {v: (spin + 1) // 2 for v, spin in sample.items()}
 
     # frustrated edges are the ones that are violated
     frustrated_edges = {}
     for u, v, data in S.edges(data=True):
         sign = data['sign']
 
         if sign > 0 and colors[u] != colors[v]:
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/algorithms/markov.py` & `dwave_networkx-0.8.9/dwave_networkx/algorithms/markov.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,25 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# =============================================================================
 
 import dimod
+try:
+    from dwave.preprocessing import FixVariablesComposite
+except ImportError:
+    # fall back on dimod (<0.10) if dwave.preprocessing not installed
+    from dimod import FixedVariableComposite as FixVariablesComposite
 
 from dwave_networkx.utils import binary_quadratic_model_sampler
 
-__all__ = 'sample_markov_network', 'markov_network_bqm'
+__all__ = ['sample_markov_network', 'markov_network_bqm']
 
 
 ###############################################################################
 # The following code is partially based on https://github.com/tbabej/gibbs
 #
 # MIT License
 # ===========
@@ -137,16 +140,15 @@
     function does not attempt to confirm the quality of the returned
     sample.
 
     """
 
     bqm = markov_network_bqm(MN)
 
-    # use the FixedVar
-    fv_sampler = dimod.FixedVariableComposite(sampler)
+    fv_sampler = FixVariablesComposite(sampler)
 
     sampleset = fv_sampler.sample(bqm, fixed_variables=fixed_variables,
                                   **sampler_args)
 
     if return_sampleset:
         return sampleset
     else:
@@ -180,15 +182,15 @@
 
         # for single nodes we don't need to worry about order
 
         phi0 = potential[(0,)]
         phi1 = potential[(1,)]
 
         bqm.add_variable(v, phi1 - phi0)
-        bqm.add_offset(phi0)
+        bqm.offset += phi0
 
     # the interaction potentials
     for u, v, ddict in MN.edges(data=True, default=None):
         potential = ddict.get('potential', None)
 
         if potential is None:
             continue
@@ -202,10 +204,10 @@
         phi01 = potential[(0, 1)]
         phi10 = potential[(1, 0)]
         phi11 = potential[(1, 1)]
 
         bqm.add_variable(u, phi10 - phi00)
         bqm.add_variable(v, phi01 - phi00)
         bqm.add_interaction(u, v, phi11 - phi10 - phi01 + phi00)
-        bqm.add_offset(phi00)
+        bqm.offset += phi00
 
     return bqm
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/algorithms/coloring.py` & `dwave_networkx-0.8.9/dwave_networkx/algorithms/coloring.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# =============================================================================
-from __future__ import division
 
 import math
 import itertools
 
 import networkx as nx
 
 from dwave_networkx.utils import binary_quadratic_model_sampler
@@ -124,15 +121,15 @@
         A coloring for each vertex in G such that no adjacent nodes
         share the same color. A dict of the form {node: color, ...}
 
 
     References
     ----------
     .. [DWMP] Dahl, E., "Programming the D-Wave: Map Coloring Problem",
-       https://www.dwavesys.com/sites/default/files/Map%20Coloring%20WP2.pdf
+       https://www.dwavesys.com/media/htfgw5bk/map-coloring-wp2.pdf
 
     Notes
     -----
     Samplers by their nature may not return the optimal solution. This
     function does not attempt to confirm the quality of the returned
     sample.
 
@@ -307,15 +304,15 @@
     coloring : dict
         A coloring for each vertex in G such that no adjacent nodes
         share the same color. A dict of the form {node: color, ...}
 
     References
     ----------
     .. [DWMP] Dahl, E., "Programming the D-Wave: Map Coloring Problem",
-       https://www.dwavesys.com/sites/default/files/Map%20Coloring%20WP2.pdf
+       https://www.dwavesys.com/media/htfgw5bk/map-coloring-wp2.pdf
 
     Notes
     -----
     Samplers by their nature may not return the optimal solution. This
     function does not attempt to confirm the quality of the returned
     sample.
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/algorithms/tsp.py` & `dwave_networkx-0.8.9/dwave_networkx/algorithms/tsp.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# =============================================================================
-from __future__ import division
 
 import itertools
 
 from collections import defaultdict
 
 from dwave_networkx.utils import binary_quadratic_model_sampler
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/algorithms/matching.py` & `dwave_networkx-0.8.9/dwave_networkx/algorithms/matching.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,47 +7,195 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 import itertools
+import numbers
+import warnings
+
+import dimod
+import networkx as nx
 
 from dwave_networkx.utils import binary_quadratic_model_sampler
-from dwave_networkx import _PY2
 
-__all__ = ['min_maximal_matching', 'is_matching', 'is_maximal_matching']
+__all__ = ['is_matching',
+           'is_maximal_matching',
+           'matching_bqm',
+           'maximal_matching_bqm',
+           'min_maximal_matching',
+           'min_maximal_matching_bqm',
+           ]
+
+
+def matching_bqm(G):
+    """Find a binary quadratic model for the graph's matchings.
+
+    A matching is a subset of edges in which no node occurs more than
+    once. This function returns a binary quadratic model (BQM) with ground
+    states corresponding to the possible matchings of G.
+
+    Finding valid matchings can be done in polynomial time, so finding matching
+    with BQMs is generally inefficient.
+    This BQM may be useful when combined with other constraints and objectives.
+
+    Parameters
+    ----------
+    G : NetworkX graph
+        The graph on which to find a matching.
+
+    Returns
+    -------
+    bqm : :class:`dimod.BinaryQuadraticModel`
+        A binary quadratic model with ground states corresponding to a
+        matching. The variables of the BQM are the edges of `G` as frozensets.
+        The BQM's ground state energy is 0 by construction.
+        The energy of the first excited state is 1.
+
+    """
+    bqm = dimod.BinaryQuadraticModel.empty('BINARY')
+
+    # add the edges of G as variables
+    for edge in G.edges:
+        bqm.add_variable(frozenset(edge), 0)
+
+    for node in G:
+        for edge0, edge1 in itertools.combinations(G.edges(node), 2):
+            u = frozenset(edge0)
+            v = frozenset(edge1)
+            bqm.add_interaction(u, v, 1)
+
+    return bqm
+
+
+def maximal_matching_bqm(G, lagrange=None):
+    """Find a binary quadratic model for the graph's maximal matchings.
+
+    A matching is a subset of edges in which no node occurs more than
+    once. A maximal matching is one in which no edges from G can be
+    added without violating the matching rule.
+    This function returns a binary quadratic model (BQM) with ground
+    states corresponding to the possible maximal matchings of G.
+
+    Finding maximal matchings can be done in polynomial time, so finding
+    maximal matching with BQMs is generally inefficient.
+    This BQM may be useful when combined with other constraints and objectives.
+
+    Parameters
+    ----------
+    G : NetworkX graph
+        The graph on which to find a maximal matching.
+
+    lagrange : float (optional)
+        The Lagrange multiplier for the matching constraint. Should be positive
+        and greater than `max_degree - 2`.
+        Defaults to `1.25 * (max_degree - 2)`.
+
+    Returns
+    -------
+    bqm : :class:`dimod.BinaryQuadraticModel`
+        A binary quadratic model with ground states corresponding to a maximal
+        matching. The variables of the BQM are the edges of `G` as frozensets.
+        The BQM's ground state energy is 0 by construction.
+
+    """
+    bqm = matching_bqm(G)
+
+    if lagrange is None:
+        delta = max((G.degree[v] for v in G), default=0)
+        lagrange = max(1.25 * (delta - 2), 1)
+
+    bqm.scale(lagrange)
+
+    for node0, node1 in G.edges:
+        # (1 - y_v - y_u + y_v*y_u) <- see paper
+
+        bqm.offset += 1
+
+        for edge in G.edges(node0):
+            bqm.linear[frozenset(edge)] -= 1
+
+        for edge in G.edges(node1):
+            bqm.linear[frozenset(edge)] -= 1
+
+        for edge0 in G.edges(node0):
+            u = frozenset(edge0)
+            for edge1 in G.edges(node1):
+                v = frozenset(edge1)
+                if u == v:
+                    bqm.linear[u] += 1
+                else:
+                    bqm.add_interaction(u, v, 1)
+
+    return bqm
+
+
+def min_maximal_matching_bqm(G, maximal_lagrange=2, matching_lagrange=None):
+    """Find a binary quadratic model for the graph's minimum maximal matchings.
+
+    A matching is a subset of edges in which no node occurs more than
+    once. A maximal matching is one in which no edges from G can be
+    added without violating the matching rule. A minimum maximal matching
+    is a maximal matching that contains the smallest possible number of edges.
+    This function returns a binary quadratic model (BQM) with ground
+    states corresponding to the possible maximal matchings of G.
+
+    Parameters
+    ----------
+    G : NetworkX graph
+        The graph on which to find a minimum maximal matching.
+
+    maximal_lagrange : float (optional, default=2)
+        The Lagrange multiplier for the maximal constraint. Should be greater
+        than 1.
+
+    matching_lagrange : float (optional)
+        The Lagrange multiplier for the matching constraint. Should be positive
+        and greater than `maximal_lagrange * max_degree - 2`.
+        Defaults to `1.25 * (maximal_lagrange * max_degree - 2)`.
+
+    Returns
+    -------
+    bqm : :class:`dimod.BinaryQuadraticModel`
+        A binary quadratic model with ground states corresponding to a
+        minimum maximal matching. The variables of the BQM are the edges
+        of `G` as frozensets.
 
-# compatibility for python 2/3
-if _PY2:
-    range = xrange
+    """
 
-    def iteritems(d): return d.iteritems()
+    if matching_lagrange is not None:
+        # we're going to scale the bqm by maximal_matching so undo that
+        # for maximal_lagrange
+        matching_lagrange /= maximal_lagrange
+    bqm = maximal_matching_bqm(G, lagrange=matching_lagrange)
+    bqm.scale(maximal_lagrange)
 
-    def itervalues(d): return d.itervalues()
-else:
-    def iteritems(d): return d.items()
+    for v in bqm.variables:
+        bqm.linear[v] += 1
 
-    def itervalues(d): return d.values()
+    return bqm
 
 
 @binary_quadratic_model_sampler(1)
 def maximal_matching(G, sampler=None, **sampler_args):
     """Finds an approximate maximal matching.
 
     Defines a QUBO with ground states corresponding to a maximal
     matching and uses the sampler to sample from it.
 
     A matching is a subset of edges in which no node occurs more than
     once. A maximal matching is one in which no edges from G can be
     added without violating the matching rule.
 
+    Finding maximal matchings can be done is polynomial time, so this method
+    is only useful pedagogically.
+
     Parameters
     ----------
     G : NetworkX graph
         The graph on which to find a maximal matching.
 
     sampler
         A binary quadratic model sampler. A sampler is a process that
@@ -72,52 +220,30 @@
     Samplers by their nature may not return the optimal solution. This
     function does not attempt to confirm the quality of the returned
     sample.
 
     References
     ----------
 
-    `Matching on Wikipedia <https://en.wikipedia.org/wiki/Matching_(graph_theory)>`_
+    `Matching on Wikipedia <https://w.wiki/r9s>`_
 
-    `QUBO on Wikipedia <https://en.wikipedia.org/wiki/Quadratic_unconstrained_binary_optimization>`_
+    `QUBO on Wikipedia <https://w.wiki/r9t>`_
 
     Based on the formulation presented in [AL]_
 
     """
+    if not G.edges:
+        return set()
 
-    # the maximum degree
-    delta = max(G.degree(node) for node in G)
-
-    # use the maximum degree to determine the infeasible gaps
-    A = 1.
-    if delta == 2:
-        B = .75
-    else:
-        B = .75 * A / (delta - 2.)  # we want A > (delta - 2) * B
-
-    # each edge in G gets a variable, so let's create those
-    edge_mapping = _edge_mapping(G)
-
-    # build the QUBO
-    Q = _maximal_matching_qubo(G, edge_mapping, magnitude=B)
-    Qm = _matching_qubo(G, edge_mapping, magnitude=A)
-    for edge, bias in Qm.items():
-        if edge not in Q:
-            Q[edge] = bias
-        else:
-            Q[edge] += bias
-
-    # use the sampler to find low energy states
-    response = sampler.sample_qubo(Q, **sampler_args)
-
-    # we want the lowest energy sample
-    sample = next(iter(response))
+    bqm = maximal_matching_bqm(G)
+    sampleset = sampler.sample(bqm, **sampler_args)
+    sample = sampleset.first.sample
 
     # the matching are the edges that are 1 in the sample
-    return set(edge for edge in G.edges if sample[edge_mapping[edge]] > 0)
+    return set(tuple(edge) for edge, val in sample.items() if val > 0)
 
 
 @binary_quadratic_model_sampler(1)
 def min_maximal_matching(G, sampler=None, **sampler_args):
     """Returns an approximate minimum maximal matching.
 
     Defines a QUBO with ground states corresponding to a minimum
@@ -167,228 +293,59 @@
     Samplers by their nature may not return the optimal solution. This
     function does not attempt to confirm the quality of the returned
     sample.
 
     References
     ----------
 
-    `Matching on Wikipedia <https://en.wikipedia.org/wiki/Matching_(graph_theory)>`_
+    `Matching on Wikipedia <https://w.wiki/r9s>`_
 
-    `QUBO on Wikipedia <https://en.wikipedia.org/wiki/Quadratic_unconstrained_binary_optimization>`_
+    `QUBO on Wikipedia <https://w.wiki/r9t>`_
 
     .. [AL] Lucas, A. (2014). Ising formulations of many NP problems.
        Frontiers in Physics, Volume 2, Article 5.
 
     """
+    if not G.edges:
+        return set()
 
-    # the maximum degree
-    delta = max(G.degree(node) for node in G)
-
-    # use the maximum degree to determine the infeasible gaps
-    A = 1.
-    if delta == 2:
-        B = .75
-    else:
-        B = .75 * A / (delta - 2.)  # we want A > (delta - 2) * B
-    C = .75 * B  # we want B > C
-
-    # each edge in G gets a variable, so let's create those
-    edge_mapping = _edge_mapping(G)
-
-    # build the QUBO
-    Q = _maximal_matching_qubo(G, edge_mapping, magnitude=B)
-    Qm = _matching_qubo(G, edge_mapping, magnitude=A)
-    for edge, bias in Qm.items():
-        if edge not in Q:
-            Q[edge] = bias
-        else:
-            Q[edge] += bias
-
-    # to enforce the minimal constraint, we additionally add a small bias to
-    # each variable
-    for v in set(edge_mapping.values()):
-        if (v, v) not in Q:
-            Q[(v, v)] = C
-        else:
-            Q[(v, v)] += C
-
-    # use the sampler to find low energy states
-    response = sampler.sample_qubo(Q, **sampler_args)
-
-    # we want the lowest energy sample
-    sample = next(iter(response))
+    bqm = min_maximal_matching_bqm(G)
+    sampleset = sampler.sample(bqm, **sampler_args)
+    sample = sampleset.first.sample
 
     # the matching are the edges that are 1 in the sample
-    return set(edge for edge in G.edges if sample[edge_mapping[edge]] > 0)
+    return set(tuple(edge) for edge, val in sample.items() if val > 0)
 
 
 def is_matching(edges):
-    """Determines whether the given set of edges is a matching.
-
-    A matching is a subset of edges in which no node occurs more than
-    once.
-
-    Parameters
-    ----------
-    edges : iterable
-        A iterable of edges.
-
-    Returns
-    -------
-    is_matching : bool
-        True if the given edges are a matching.
-
-    Example
-    -------
-    This example checks two sets of edges, both derived from a
-    single Chimera unit cell, for a matching. Because every node in a Chimera
-    unit cell connects to four other nodes in the cell, the first set, which
-    contains all the edges, repeats each node 4 times; the second is a subset
-    of those edges found using the `min_maximal_matching()` function.
-
-    >>> import dwave_networkx as dnx
-    >>> G = dnx.chimera_graph(1, 1, 4)
-    >>> dnx.is_matching(G.edges())
-    False
-    >>> dnx.is_matching({(0, 4), (1, 5), (2, 7), (3, 6)})
-    True
+    """Determine whether the given set of edges is a matching.
 
+    Deprecated in favour of :func:`networkx.is_matching`.
     """
+    warnings.warn("This method is deprecated, please use NetworkX's"
+                  "nx.is_matching(G, edges) rather than dwave-networkx's "
+                  "dnx.is_matching(edges)", DeprecationWarning, stacklevel=2)
     return len(set().union(*edges)) == len(edges) * 2
 
 
 def is_maximal_matching(G, matching):
-    """Determines whether the given set of edges is a maximal matching.
-
-    A matching is a subset of edges in which no node occurs more than
-    once. The cardinality of a matching is the number of matched edges.
-    A maximal matching is one where one cannot add any more edges
-    without violating the matching rule.
-
-    Parameters
-    ----------
-    G : NetworkX graph
-        The graph on which to check the maximal matching.
-
-    edges : iterable
-        A iterable of edges.
-
-    Returns
-    -------
-    is_matching : bool
-        True if the given edges are a maximal matching.
-
-    Example
-    -------
-    This example checks two sets of edges, both derived from a
-    single Chimera unit cell, for a matching. The first set (a matching) is
-    a subset of the second, which was found using the `min_maximal_matching()`
-    function.
-
-    >>> import dwave_networkx as dnx
-    >>> G = dnx.chimera_graph(1, 1, 4)
-    >>> dnx.is_matching({(0, 4), (2, 7)})
-    True
-    >>> dnx.is_maximal_matching(G,{(0, 4), (2, 7)})
-    False
-    >>> dnx.is_maximal_matching(G,{(0, 4), (1, 5), (2, 7), (3, 6)})
-    True
+    """Determine whether the given set of edges is a maximal matching.
 
+    Deprecated in favour of :func:`networkx.is_matching`.
     """
+    warnings.warn("This method is deprecated, please use NetworkX's"
+                  "nx.is_maximal_matching(G, edges) rather than "
+                  "dwave-networkx's dnx.is_maximal_matching(G, edges)",
+                  DeprecationWarning, stacklevel=2)
     touched_nodes = set().union(*matching)
 
     # first check if a matching
     if len(touched_nodes) != len(matching) * 2:
         return False
 
     # now for each edge, check that at least one of its variables is
     # already in the matching
     for (u, v) in G.edges:
         if u not in touched_nodes and v not in touched_nodes:
             return False
 
     return True
-
-
-def _edge_mapping(G):
-    """Assigns a variable for each edge in G.
-    (u, v) and (v, u) map to the same variable.
-    """
-    edge_mapping = {edge: idx for idx, edge in enumerate(G.edges)}
-    edge_mapping.update({(e1, e0): idx for (e0, e1), idx in edge_mapping.items()})
-    return edge_mapping
-
-
-def _maximal_matching_qubo(G, edge_mapping, magnitude=1.):
-    """Generates a QUBO that when combined with one as generated by _matching_qubo,
-    induces a maximal matching on the given graph G.
-    The variables in the QUBO are the edges, as given my edge_mapping.
-
-    ground_energy = -1 * magnitude * |edges|
-    infeasible_gap >= magnitude
-    """
-    Q = {}
-
-    # for each node n in G, define a variable y_n to be 1 when n has a colored edge
-    # and 0 otherwise.
-    # for each edge (u, v) in the graph we want to enforce y_u OR y_v. This is because
-    # if both y_u == 0 and y_v == 0, then we could add (u, v) to the matching.
-    for (u, v) in G.edges:
-        # 1 - y_v - y_u + y_v*y_u
-
-        # for each edge connected to u
-        for edge in G.edges(u):
-            x = edge_mapping[edge]
-            if (x, x) not in Q:
-                Q[(x, x)] = -1 * magnitude
-            else:
-                Q[(x, x)] -= magnitude
-
-        # for each edge connected to v
-        for edge in G.edges(v):
-            x = edge_mapping[edge]
-            if (x, x) not in Q:
-                Q[(x, x)] = -1 * magnitude
-            else:
-                Q[(x, x)] -= magnitude
-
-        for e0 in G.edges(v):
-            x0 = edge_mapping[e0]
-            for e1 in G.edges(u):
-                x1 = edge_mapping[e1]
-
-                if x0 < x1:
-                    if (x0, x1) not in Q:
-                        Q[(x0, x1)] = magnitude
-                    else:
-                        Q[(x0, x1)] += magnitude
-                else:
-                    if (x1, x0) not in Q:
-                        Q[(x1, x0)] = magnitude
-                    else:
-                        Q[(x1, x0)] += magnitude
-
-    return Q
-
-
-def _matching_qubo(G, edge_mapping, magnitude=1.):
-    """Generates a QUBO that induces a matching on the given graph G.
-    The variables in the QUBO are the edges, as given my edge_mapping.
-
-    ground_energy = 0
-    infeasible_gap = magnitude
-    """
-    Q = {}
-
-    # We wish to enforce the behavior that no node has two colored edges
-    for node in G:
-
-        # for each pair of edges that contain node
-        for edge0, edge1 in itertools.combinations(G.edges(node), 2):
-
-            v0 = edge_mapping[edge0]
-            v1 = edge_mapping[edge1]
-
-            # penalize both being True
-            Q[(v0, v1)] = magnitude
-
-    return Q
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/algorithms/__init__.py` & `dwave_networkx-0.8.9/dwave_networkx/algorithms/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 from dwave_networkx.algorithms.independent_set import *
 from dwave_networkx.algorithms.canonicalization import *
 from dwave_networkx.algorithms.clique import *
 from dwave_networkx.algorithms.cover import *
 from dwave_networkx.algorithms.matching import *
 from dwave_networkx.algorithms.social import *
 from dwave_networkx.algorithms.elimination_ordering import *
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/drawing/chimera_layout.py` & `dwave_networkx-0.8.9/dwave_networkx/drawing/chimera_layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,42 +13,28 @@
 #    limitations under the License.
 #
 # ================================================================================================
 """
 Tools to visualize Chimera lattices and weighted graph problems on them.
 """
 
-from __future__ import division
-
 import networkx as nx
 from networkx import draw
 
-from dwave_networkx import _PY2
 from dwave_networkx.drawing.qubit_layout import draw_qubit_graph, draw_embedding, draw_yield
 from dwave_networkx.generators.chimera import chimera_graph, find_chimera_indices, chimera_coordinates
 
-# compatibility for python 2/3
-if _PY2:
-    range = xrange
-
-    def itervalues(d): return d.itervalues()
-
-    def iteritems(d): return d.iteritems()
-else:
-    def itervalues(d): return d.values()
-
-    def iteritems(d): return d.items()
 
 __all__ = ['chimera_layout', 'draw_chimera', 'draw_chimera_embedding', 'draw_chimera_yield']
 
 
 def chimera_layout(G, scale=1., center=None, dim=2):
     """Positions the nodes of graph G in a Chimera cross topology.
 
-    NumPy (http://scipy.org) is required for this function.
+    NumPy (https://scipy.org) is required for this function.
 
     Parameters
     ----------
     G : NetworkX graph
         Should be a Chimera graph or a subgraph of a
         Chimera graph. If every node in G has a `chimera_index`
         attribute, those are used to place the nodes. Otherwise makes
@@ -104,21 +90,21 @@
         if all('chimera_index' in dat for __, dat in G.nodes(data=True)):
             chimera_indices = {v: dat['chimera_index'] for v, dat in G.nodes(data=True)}
         else:
             chimera_indices = find_chimera_indices(G)
 
         # we could read these off of the name attribute for G, but we would want the values in
         # the nodes to override the name in case of conflict.
-        m = max(idx[0] for idx in itervalues(chimera_indices)) + 1
-        n = max(idx[1] for idx in itervalues(chimera_indices)) + 1
-        t = max(idx[3] for idx in itervalues(chimera_indices)) + 1
+        m = max(idx[0] for idx in chimera_indices.values()) + 1
+        n = max(idx[1] for idx in chimera_indices.values()) + 1
+        t = max(idx[3] for idx in chimera_indices.values()) + 1
         xy_coords = chimera_node_placer_2d(m, n, t, scale, center, dim)
 
         # compute our coordinates
-        pos = {v: xy_coords(i, j, u, k) for v, (i, j, u, k) in iteritems(chimera_indices)}
+        pos = {v: xy_coords(i, j, u, k) for v, (i, j, u, k) in chimera_indices.items()}
 
     return pos
 
 
 def chimera_node_placer_2d(m, n, t, scale=1., center=None, dim=2):
     """Generates a function that converts Chimera indices to x, y
     coordinates for a plot.
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/drawing/pegasus_layout.py` & `dwave_networkx-0.8.9/dwave_networkx/drawing/pegasus_layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,49 +7,38 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 """
 Tools to visualize Pegasus lattices and weighted graph problems on them.
 """
 
-from __future__ import division
-
 import networkx as nx
 from networkx import draw
 
-from dwave_networkx import _PY2
 from dwave_networkx.drawing.qubit_layout import draw_qubit_graph, draw_embedding, draw_yield
 from dwave_networkx.generators.pegasus import pegasus_graph, pegasus_coordinates
 from dwave_networkx.drawing.chimera_layout import chimera_node_placer_2d
 
-# compatibility for python 2/3
-if _PY2:
-    range = xrange
-
-    def itervalues(d): return d.itervalues()
-
-    def iteritems(d): return d.iteritems()
-else:
-    def itervalues(d): return d.values()
-
-    def iteritems(d): return d.items()
 
-__all__ = ['pegasus_layout', 'draw_pegasus', 'draw_pegasus_embedding', 'draw_pegasus_yield']
+__all__ = ['pegasus_layout',
+           'draw_pegasus',
+           'draw_pegasus_embedding',
+           'draw_pegasus_yield',
+           ]
 
 
 def pegasus_layout(G, scale=1., center=None, dim=2, crosses=False):
     """Positions the nodes of graph G in a Pegasus topology.
 
-    `NumPy <http://scipy.org>`_ is required for this function.
+    `NumPy <https://scipy.org>`_ is required for this function.
 
     Parameters
     ----------
     G : NetworkX graph
         A Pegasus graph or a subgraph of a Pegasus graph, as produced by
         the :func:`dwave_networkx.pegasus_graph` function.
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/drawing/qubit_layout.py` & `dwave_networkx-0.8.9/dwave_networkx/drawing/qubit_layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,43 +7,27 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 """
 Tools to visualize Chimera lattices and weighted graph problems on them.
 """
 
-from __future__ import division
-
 import math
 import random
 import networkx as nx
-from networkx import draw
 
-from dwave_networkx import _PY2
+from networkx import draw
 
 from dwave_networkx.drawing.distinguishable_colors import distinguishable_color_map
 
-# compatibility for python 2/3
-if _PY2:
-    range = xrange
-
-    def itervalues(d): return d.itervalues()
-
-    def iteritems(d): return d.iteritems()
-else:
-    def itervalues(d): return d.values()
-
-    def iteritems(d): return d.items()
-
 __all__ = ['draw_qubit_graph']
 
 
 def draw_qubit_graph(G, layout, linear_biases={}, quadratic_biases={},
                      nodelist=None, edgelist=None, cmap=None, edge_cmap=None, vmin=None, vmax=None,
                      edge_vmin=None, edge_vmax=None, midpoint=None,
                      **kwargs):
@@ -291,15 +275,15 @@
 
         for v, bag in bags.items():
             for i, x in enumerate(bag):
                 node_size_dict[(v, x)] = base_node_size * (len(bag) - i) ** 2
 
         kwargs['node_size'] = [node_size_dict[p] for p in G.nodes()]
 
-    qlabel = {q: v for v, chain in iteritems(emb) for q in chain}
+    qlabel = {q: v for v, chain in emb.items() for q in chain}
     edgelist = []
     edge_color = []
     background_edgelist = []
     background_edge_color = []
 
     if interaction_edges is not None:
         interactions = nx.Graph()
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/drawing/distinguishable_colors.py` & `dwave_networkx-0.8.9/dwave_networkx/drawing/distinguishable_colors.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 def distinguishable_color_map(num_colors):
     # Creates a matplotlib Colormap with num_colors visually distinct colors.
     try:
         from matplotlib.colors import LinearSegmentedColormap
     except ImportError:
         raise ImportError("Matplotlib required for distinguishable_color_map()")
     return LinearSegmentedColormap.from_list('dist_colors', distinguishable_colors[:min(num_colors, 1000)], num_colors)
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/drawing/__init__.py` & `dwave_networkx-0.8.9/dwave_networkx/drawing/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,11 +7,10 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 from dwave_networkx.drawing.chimera_layout import *
 from dwave_networkx.drawing.pegasus_layout import *
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/exceptions.py` & `dwave_networkx-0.8.9/dwave_networkx/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 """
 Base exceptions and errors for D-Wave NetworkX.
 
 All exceptions are derived from NetworkXException.
 
 """
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/package_info.py` & `dwave_networkx-0.8.9/dwave_networkx/package_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,13 +7,12 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
-__version__ = '0.8.8'
+
+__version__ = '0.8.9'
 __author__ = 'D-Wave Systems Inc.'
 __authoremail__ = 'acondello@dwavesys.com'
 __description__ = 'A NetworkX extension providing graphs and algorithms relevent to working with the D-Wave System'
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/utils/decorators.py` & `dwave_networkx-0.8.9/dwave_networkx/utils/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
+
 """
 Decorators allow for input checking and default parameter setting for
 algorithms.
 """
 
 from decorator import decorator
```

### Comparing `dwave_networkx-0.8.8/dwave_networkx/utils/__init__.py` & `dwave_networkx-0.8.9/dwave_networkx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave_networkx-0.8.8/dwave_networkx/__init__.py` & `dwave_networkx-0.8.9/dwave_networkx/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,14 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-#
-# ================================================================================================
-from __future__ import absolute_import
-
-import sys
-_PY2 = sys.version_info[0] == 2
 
 import dwave_networkx.generators
 from dwave_networkx.generators import *
 
 import dwave_networkx.algorithms
 from dwave_networkx.algorithms import *
 
@@ -29,8 +23,9 @@
 
 import dwave_networkx.default_sampler
 from dwave_networkx.default_sampler import *
 
 import dwave_networkx.drawing
 from dwave_networkx.drawing import *
 
-from dwave_networkx.package_info import __version__, __author__, __authoremail__, __description__
+from dwave_networkx.package_info import __version__, __author__, \
+    __authoremail__, __description__
```

