# Comparing `tmp/fenics-smart-0.1.10.tar.gz` & `tmp/fenics-smart-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenics-smart-0.1.10.tar", last modified: Tue May  2 01:45:52 2023, max compression
+gzip compressed data, was "fenics-smart-2.0.1.tar", last modified: Mon May 15 07:44:03 2023, max compression
```

## Comparing `fenics-smart-0.1.10.tar` & `fenics-smart-2.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 emmetf    (1000) emmetf    (1000)        0 2023-05-02 01:45:52.126594 fenics-smart-0.1.10/
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)     7370 2023-02-09 18:07:42.000000 fenics-smart-0.1.10/LICENSE
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)    14157 2023-05-02 01:45:52.121735 fenics-smart-0.1.10/PKG-INFO
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)     5774 2023-05-02 01:42:21.000000 fenics-smart-0.1.10/README.md
-drwxrwxrwx   0 emmetf    (1000) emmetf    (1000)        0 2023-05-02 01:45:51.697523 fenics-smart-0.1.10/fenics_smart.egg-info/
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)    14157 2023-05-02 01:45:51.000000 fenics-smart-0.1.10/fenics_smart.egg-info/PKG-INFO
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)      461 2023-05-02 01:45:51.000000 fenics-smart-0.1.10/fenics_smart.egg-info/SOURCES.txt
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)        1 2023-05-02 01:45:51.000000 fenics-smart-0.1.10/fenics_smart.egg-info/dependency_links.txt
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)      231 2023-05-02 01:45:51.000000 fenics-smart-0.1.10/fenics_smart.egg-info/requires.txt
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)        6 2023-05-02 01:45:51.000000 fenics-smart-0.1.10/fenics_smart.egg-info/top_level.txt
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)     2170 2023-05-02 01:42:21.000000 fenics-smart-0.1.10/pyproject.toml
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)       38 2023-05-02 01:45:52.126594 fenics-smart-0.1.10/setup.cfg
-drwxrwxrwx   0 emmetf    (1000) emmetf    (1000)        0 2023-05-02 01:45:51.986714 fenics-smart-0.1.10/smart/
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)      221 2023-05-02 01:42:21.000000 fenics-smart-0.1.10/smart/__init__.py
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)    21203 2023-05-02 01:42:21.000000 fenics-smart-0.1.10/smart/common.py
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)    11759 2023-05-02 01:42:21.000000 fenics-smart-0.1.10/smart/config.py
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)      764 2023-05-02 01:42:21.000000 fenics-smart-0.1.10/smart/deprecation.py
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)    16171 2023-05-02 01:42:21.000000 fenics-smart-0.1.10/smart/mesh.py
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)    85963 2023-05-02 01:42:21.000000 fenics-smart-0.1.10/smart/model.py
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)    50972 2023-05-02 01:42:21.000000 fenics-smart-0.1.10/smart/model_assembly.py
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)    22165 2023-05-02 01:42:21.000000 fenics-smart-0.1.10/smart/solvers.py
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)      564 2023-05-02 01:42:21.000000 fenics-smart-0.1.10/smart/units.py
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)     1522 2023-05-02 01:42:21.000000 fenics-smart-0.1.10/smart/utils.py
-drwxrwxrwx   0 emmetf    (1000) emmetf    (1000)        0 2023-05-02 01:45:52.043118 fenics-smart-0.1.10/tests/
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)     1459 2023-05-02 01:42:22.000000 fenics-smart-0.1.10/tests/test_compartment.py
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)     1702 2023-05-02 01:42:22.000000 fenics-smart-0.1.10/tests/test_species.py
--rwxrwxrwx   0 emmetf    (1000) emmetf    (1000)     4637 2023-05-02 01:42:22.000000 fenics-smart-0.1.10/tests/test_stubs_model_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:44:03.915598 fenics-smart-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-05-15 07:44:03.915598 fenics-smart-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:44:03.915598 fenics-smart-2.0.1/fenics_smart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-05-15 07:44:03.000000 fenics-smart-2.0.1/fenics_smart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-15 07:44:03.000000 fenics-smart-2.0.1/fenics_smart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:44:03.000000 fenics-smart-2.0.1/fenics_smart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 07:44:03.000000 fenics-smart-2.0.1/fenics_smart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 07:44:03.000000 fenics-smart-2.0.1/fenics_smart.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 07:44:03.915598 fenics-smart-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:44:03.915598 fenics-smart-2.0.1/smart/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85874 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50721 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/model_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25640 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:44:03.915598 fenics-smart-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/tests/test_compartment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/tests/test_species.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/tests/test_stubs_model_init.py
```

### Comparing `fenics-smart-0.1.10/LICENSE` & `fenics-smart-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fenics-smart-0.1.10/PKG-INFO` & `fenics-smart-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-smart
-Version: 0.1.10
+Version: 2.0.1
 Summary: SMART is a biophysical simulation library that provides a level of abstraction to models, making it easier for users to develop, share, and simulate their mathematical models
 Author-email: Justin Laughlin <justinglaughlin@gmail.com>
 License: GNU LESSER GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
         
@@ -58,14 +58,15 @@
         
         Each version is given a distinguishing version number. If the Library as you received it specifies that a certain numbered version of the GNU Lesser General Public License “or any later version” applies to it, you have the option of following the terms and conditions either of that published version or of any later version published by the Free Software Foundation. If the Library as you received it does not specify a version number of the GNU Lesser General Public License, you may choose any version of the GNU Lesser General Public License ever published by the Free Software Foundation.
         
         If the Library as you received it specifies that a proxy can decide whether future versions of the GNU Lesser General Public License shall apply, that proxy's public statement of acceptance of any version is permanent authorization for you to choose that version for the Library.
         
 Project-URL: homepage, https://rangamanilabucsd.github.io/smart
 Project-URL: repository, https://github.com/RangamaniLabUCSD/smart
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
 Spatial Modelling Algorithms for Reaction-Transport [systems|models|equations]
```

### Comparing `fenics-smart-0.1.10/README.md` & `fenics-smart-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fenics-smart-0.1.10/fenics_smart.egg-info/PKG-INFO` & `fenics-smart-2.0.1/fenics_smart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-smart
-Version: 0.1.10
+Version: 2.0.1
 Summary: SMART is a biophysical simulation library that provides a level of abstraction to models, making it easier for users to develop, share, and simulate their mathematical models
 Author-email: Justin Laughlin <justinglaughlin@gmail.com>
 License: GNU LESSER GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
         
@@ -58,14 +58,15 @@
         
         Each version is given a distinguishing version number. If the Library as you received it specifies that a certain numbered version of the GNU Lesser General Public License “or any later version” applies to it, you have the option of following the terms and conditions either of that published version or of any later version published by the Free Software Foundation. If the Library as you received it does not specify a version number of the GNU Lesser General Public License, you may choose any version of the GNU Lesser General Public License ever published by the Free Software Foundation.
         
         If the Library as you received it specifies that a proxy can decide whether future versions of the GNU Lesser General Public License shall apply, that proxy's public statement of acceptance of any version is permanent authorization for you to choose that version for the Library.
         
 Project-URL: homepage, https://rangamanilabucsd.github.io/smart
 Project-URL: repository, https://github.com/RangamaniLabUCSD/smart
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
 Spatial Modelling Algorithms for Reaction-Transport [systems|models|equations]
```

### Comparing `fenics-smart-0.1.10/pyproject.toml` & `fenics-smart-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "fenics-smart"
-version = "0.1.10"
+version = "2.0.1"
 description = "SMART is a biophysical simulation library that provides a level of abstraction to models, making it easier for users to develop, share, and simulate their mathematical models"
 authors = [{name = "Justin Laughlin", email = "justinglaughlin@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
+requires-python = ">=3.8"
 dependencies = [
     "matplotlib",
     "numpy>=1.16.0",
     "pandas",
     "Pint",
     "scipy>=1.1.0",
     "sympy",
```

### Comparing `fenics-smart-0.1.10/smart/common.py` & `fenics-smart-2.0.1/smart/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,29 +9,26 @@
 
 import dolfin as d
 import gmsh
 import meshio
 
 # import trimesh
 import numpy as np
-import pint
 
 import ufl
 from pytz import timezone
 from termcolor import colored
 
 from .deprecation import deprecated
 from .config import global_settings as gset, FancyFormatter
 from .units import unit
 
 __all__ = [
     "smart_expressions",
     "sub",
-    "pint_unit_to_quantity",
-    "pint_quantity_to_unit",
     "Stopwatch",
     "facet_topology",
     "cube_condition",
     "DemoCuboidsMesh",
     "DemoSpheresMesh",
     "write_mesh",
 ]
@@ -138,30 +135,14 @@
         else:
             return func[idx]
 
     else:
         raise ValueError(f"Unknown input type of {func=}")
 
 
-def pint_unit_to_quantity(pint_unit):
-    if not isinstance(pint_unit, pint.Unit):
-        raise TypeError("Input must be a pint unit")
-    # returning pint.Quantity(1, pint_unit) changes the unit
-    # registry which we do NOT want
-    return 1.0 * pint_unit
-
-
-def pint_quantity_to_unit(pint_quantity):
-    if not isinstance(pint_quantity, pint.Quantity):
-        raise TypeError("Input must be a pint quantity")
-    if pint_quantity.magnitude != 1.0:
-        raise ValueError("Trying to convert a pint quantity into a unit with magnitude != 1")
-    return pint_quantity.units
-
-
 # Write a stopwatch class to measure time elapsed
 # with a start, stop, and pause methods
 # Keep track of timings in a list of lists called
 # self.timings, each time the timer is paused,
 # the time elapsed since the last pause is added to
 # the sublist. Using stop resets the timer to zero
 # and beings a new list of timings.
```

### Comparing `fenics-smart-0.1.10/smart/config.py` & `fenics-smart-2.0.1/smart/config.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-0.1.10/smart/deprecation.py` & `fenics-smart-2.0.1/smart/deprecation.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-0.1.10/smart/mesh.py` & `fenics-smart-2.0.1/smart/mesh.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-0.1.10/smart/model.py` & `fenics-smart-2.0.1/smart/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1041,17 +1041,15 @@
                 self.u["u"],
                 self.Fblocks_all,
                 self.Jblocks_all,
                 self._active_compartments,
                 self._all_compartments,
                 self.stopwatches,
                 self.config.solver["print_assembly"],
-                self.mpi_comm_world,
             )
-            # self.problem = smartSNESProblem(self)
 
             self.problem.init_petsc_matnest()
             self.problem.init_petsc_vecnest()
             if len(self.problem.global_sizes) == 1:
                 self._ubackend = u[0].vector().vec().copy()
             else:
                 self._ubackend = PETSc.Vec().createNest([usub.vector().vec().copy() for usub in u])
```

### Comparing `fenics-smart-0.1.10/smart/model_assembly.py` & `fenics-smart-2.0.1/smart/model_assembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 """
 Classes for parameters, species, compartments, reactions, fluxes, and forms
 Model class contains functions to efficiently solve a system
 """
 import dataclasses
+import logging
 import numbers
 import sys
-import logging
 from collections import OrderedDict as odict
 from dataclasses import dataclass
 from pprint import pformat
 from textwrap import wrap
-from typing import Any, Union
+from typing import Any, List, Optional, Union
 
 import dolfin as d
 import numpy as np
-import numpy.typing as npt
 import pandas
 import pint
 import sympy as sym
 import ufl
 from cached_property import cached_property
 from sympy import Symbol, integrate
 from sympy.parsing.sympy_parser import parse_expr
 from tabulate import tabulate
 
 from . import common
-from .common import pint_quantity_to_unit, pint_unit_to_quantity, sub
 from .config import global_settings as gset
-from .units import unit
-
+from .units import quantity_to_unit, unit, unit_to_quantity
 
 __all__ = [
     "empty_sbmodel",
     "sbmodel_from_locals",
     "Compartment",
     "Parameter",
     "Reaction",
@@ -44,45 +41,14 @@
 rank = comm.rank
 size = comm.size
 root = 0
 
 logger = logging.getLogger(__name__)
 
 
-def _np_smart_hstack(
-    x1: Union[list, npt.ArrayLike], x2: Union[list, npt.ArrayLike]
-) -> npt.ArrayLike:
-    """
-    Quality of life function. Converts two (N,) numpy arrays or two lists into a
-    (Nx2) array
-
-    Params:
-        x1: First array
-        x2: Second array
-
-    Returns:
-        The stacked array
-
-    Examples:
-
-        .. highlight:: python
-        .. code-block:: python
-
-            a_list = [1,2,3,4]
-            a_np_array = np.array([x**2 for x in a_list])
-            _np_smart_hstack(a_list, a_np_array)
-    """
-    assert len(x1) == len(x2)  # confirm same size
-    if isinstance(x1, list):
-        x1 = np.array(x1)
-    if isinstance(x2, list):
-        x2 = np.array(x2)
-    return np.hstack([x1.reshape(-1, 1), x2.reshape(-1, 1)])
-
-
 # ====================================================
 # ====================================================
 # Base Classes
 # ====================================================
 # ====================================================
 
 
@@ -190,51 +156,59 @@
     # Mostly methods called by Model.initialize()
     # ==============================================================================
 
     # ==============================================================================
     # ObjectContainer - Printing/data-formatting related methods
     # ==============================================================================
 
-    def get_pandas_dataframe(self, properties_to_print=None, include_idx=True):
+    def get_pandas_dataframe(
+        self, properties_to_print: Optional[List[str]] = None, include_idx: bool = True
+    ) -> pandas.DataFrame:
+        """
+        Create a `pandas.DataFrame` of all items in the class (defined through `self.items`)
+
+        Params:
+            properties_to_print: If set only the listed properties (by attribute name)
+              is added to the series
+            include_index: If true, add index as the first column in the data-frame..
+
+
+
+        """
+
         df = pandas.DataFrame()
         if include_idx:
-            if properties_to_print and "idx" not in properties_to_print:
+            if properties_to_print is not None and "idx" not in properties_to_print:
                 properties_to_print.insert(0, "idx")
-            for idx, (name, instance) in enumerate(self.items):
+            for idx, (_, instance) in enumerate(self.items):
                 df = pandas.concat(
                     [
                         df,
                         instance.get_pandas_series(properties_to_print=properties_to_print, idx=idx)
                         .to_frame()
                         .T,
                     ]
                 )
         else:
-            for idx, (name, instance) in enumerate(self.items):
+            for idx, (_, instance) in enumerate(self.items):
                 df = pandas.concat(
                     [
                         df,
                         instance.get_pandas_series(properties_to_print=properties_to_print)
                         .to_frame()
                         .T,
                     ]
                 )
-        # # sometimes types are recast. change entries into their original types
-        # for dtypeName, dtype in self.dtypes.items():
-        #     if dtypeName in df.columns:
-        #         df = df.astype({dtypeName: dtype})
-
         return df
 
     def print_to_latex(
         self,
         properties_to_print=None,
         max_col_width=None,
         sig_figs=2,
-        latex_name_map=None,
         return_df=True,
     ):
         """Requires latex packages \siunitx and \longtable"""
 
         df = self.get_pandas_dataframe_formatted(
             properties_to_print=properties_to_print,
             max_col_width=max_col_width,
@@ -254,19 +228,22 @@
         if return_df:
             return df
         else:
             with pandas.option_context("max_colwidth", 1000):
                 logger.info(df.to_latex(escape=False, longtable=True, index=False))
 
     def get_pandas_dataframe_formatted(
-        self, properties_to_print=None, max_col_width=50, sig_figs=2
+        self,
+        properties_to_print: Optional[Union[str, List[str]]] = None,
+        max_col_width=50,
+        sig_figs=2,
     ):
         # Get the pandas dataframe with the properties we want to print
-        if properties_to_print:
-            if type(properties_to_print) != list:
+        if properties_to_print is not None:
+            if not isinstance(properties_to_print, list):
                 properties_to_print = [properties_to_print]
         elif hasattr(self, "properties_to_print"):
             properties_to_print = self.properties_to_print
         df = self.get_pandas_dataframe(properties_to_print=properties_to_print, include_idx=False)
         if properties_to_print:
             df = df[properties_to_print]
 
@@ -326,20 +303,14 @@
 
 class ObjectInstance:
     """
     Parent class containing general methods used by all smart
     "objects": i.e. parameters, species, compartments, reactions, fluxes, forms
     """
 
-    def _convert_pint_quantity_to_unit(self):
-        # strip the magnitude and keep the units. Warn if magnitude!=1
-        for name, attr in vars(self).items():
-            if isinstance(attr, pint.Quantity):
-                setattr(self, name, pint_quantity_to_unit(attr))
-
     def _check_input_type_validity(self):
         "Check that the inputs have the same type (or are convertible) to the type hint."
         for field in dataclasses.fields(self):
             value = getattr(self, field.name)
             if field.type == Any:
                 continue
             elif not isinstance(value, field.type):
@@ -348,36 +319,56 @@
                 except Exception:
                     raise TypeError(
                         f"Object {self.name!r} type error: the attribute {field.name!r} "
                         f"is expected to be {field.type}, got {type(value)} instead. "
                         "Conversion to the expected type was attempted but unsuccessful."
                     )
 
+    def _convert_pint_quantity_to_unit(self):
+        """
+        Convert all attributes of the class that is a `pint.Quantity` into a `pint.Unit`.
+        """
+        # strip the magnitude and keep the units. Warn if magnitude!=1
+        for name, attr in vars(self).items():
+            if isinstance(attr, pint.Quantity):
+                setattr(self, name, quantity_to_unit(attr))
+
     def _convert_pint_unit_to_quantity(self):
-        # convert pint units to quantity
+        """
+        Convert all attributes of the class that is a `pint.Unit` into a `pint.Quantity`.
+        """
         for name, attr in vars(self).items():
             if isinstance(attr, pint.Unit):
-                setattr(self, name, pint_unit_to_quantity(attr))
+                setattr(self, name, unit_to_quantity(attr))
 
-    def get_pandas_series(self, properties_to_print=None, idx=None):
-        if properties_to_print:
+    def get_pandas_series(
+        self, properties_to_print: Optional[List[str]] = None, idx: Optional[int] = None
+    ):
+        """
+        Convert attributes of the class into a `pandas.Series`.
+
+        Params:
+            properties_to_print: If set only the listed properties (by attribute name)
+                is added to the series
+            index: If set add to series
+        """
+        if properties_to_print is not None:
             dict_to_convert = odict({"idx": idx})
             dict_to_convert.update(
                 odict(
                     [
                         (key, val)
                         for (key, val) in self.__dict__.items()
                         if key in properties_to_print
                     ]
                 )
             )
         else:
             dict_to_convert = self.__dict__
         return pandas.Series(dict_to_convert, name=self.name)
-        # return pandas.Series(dict_to_convert)
 
     def print(self, properties_to_print=None):
         if rank == root:
             logger.info("Name: " + self.name)
             # if a custom list of properties to print is provided, only use those
             if properties_to_print:
                 dict_to_print = dict(
@@ -604,22 +595,19 @@
         super().print(tablefmt, self.properties_to_print, filename, max_col_width)
 
     def print_to_latex(
         self,
         properties_to_print=None,
         max_col_width=None,
         sig_figs=2,
-        latex_name_map=None,
         return_df=False,
     ):
         properties_to_print = ["_latex_name"]
         properties_to_print.extend(self.properties_to_print)
-        df = super().print_to_latex(
-            properties_to_print, max_col_width, sig_figs, latex_name_map, return_df=True
-        )
+        df = super().print_to_latex(properties_to_print, max_col_width, sig_figs, return_df=True)
         # fix dof_index
         for col in df.columns:
             if col == "dof_index":
                 df[col] = df[col].astype(int)
         # fix name
         # get the column of df that contains the name
         # this can be more robust
@@ -712,15 +700,15 @@
             raise ValueError(
                 f"Units of diffusion coefficient for species {self.name} must "
                 "be dimensionally equivalent to [length]^2/[time]."
             )
 
     @cached_property
     def vscalar(self):
-        return d.TestFunction(sub(self.compartment.V, 0, True))
+        return d.TestFunction(common.sub(self.compartment.V, 0, True))
 
     @property
     def dolfin_quantity(self):
         return self._usplit["u"] * self.concentration_units
 
     @property
     def initial_condition_quantity(self):
@@ -1277,15 +1265,15 @@
         return variables
 
     # @property
     # def equation_value(self):
     #     return self.equation_quantity.magnitude
     # @property
     # def equation_units(self):
-    #     return common.pint_unit_to_quantity(self.equation_quantity.units)
+    #     return unit_to_quantity(self.equation_quantity.units)
 
     def equation_lambda_eval(self, input_type="quantity"):
         """
         Evaluates the equation lambda function using either the quantity
         (value * units), the value, or the units.
         The values and units are evaluated separately and then combined
         because some expressions don't work well
@@ -1294,15 +1282,15 @@
         # This is an attempt to make the equation lambda work with pint quantities
         self._equation_quantity = self.equation_lambda(**self.equation_variables)
         if input_type == "quantity":
             return self._equation_quantity
         elif input_type == "value":
             return self._equation_quantity.magnitude
         elif input_type == "units":
-            return common.pint_unit_to_quantity(self._equation_quantity.units)
+            return unit_to_quantity(self._equation_quantity.units)
 
     # Seems like setting this as a @property doesn't cause fenics to recompile
 
     @property
     def form(self):
         """-1 factor because terms are defined as if they were on the
         lhs of the equation F(u;v)=0"""
@@ -1457,11 +1445,7 @@
     compartments.reverse()
     reactions.reverse()
     pc.add(parameters)
     sc.add(species)
     cc.add(compartments)
     rc.add(reactions)
     return pc, sc, cc, rc
-
-
-def nan_to_none(df):
-    return df.replace({np.nan: None})
```

### Comparing `fenics-smart-0.1.10/smart/solvers.py` & `fenics-smart-2.0.1/smart/solvers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,118 +1,173 @@
-# # Using PETSc to solve monolithic problem
+"""Interface to PETSc SNES solver"""
 import logging
-import dolfin as d
 import os
+from typing import Dict, List, Optional
+
+import dolfin as d
 import petsc4py.PETSc as p
 
+from .common import Stopwatch
+from .model_assembly import Compartment
 
 logger = logging.getLogger(__name__)
 
+__all__ = ["smartSNESProblem"]
+
+_stopwatch_keys = [
+    "snes jacobian assemble",
+    "snes residual assemble",
+    "snes initialize zero matrices",
+]
+
 
 class smartSNESProblem:
-    """To interface with PETSc SNES solver
+    """Interface to PETSc SNES solver.
 
-    Notes on the high-level dolfin solver d.solve()
-    when applied to Mixed Nonlinear problems:
+    Args:
+        u: The function containing the unknown dofs (is a function from a
+            :class:`dolfin.MixedFunctionSpace`)
+        Fforms: Nested list of forms for the residual ``F``. Number of
+            block rows in the rhs vector is given by the number of items in the outermost list.
+        Jforms_all: Nested list of forms for the Jacobian.
+
+            .. note::
+                Number of entries in the outermost list should be ``len(Fforms)**2``
+
+            Flattened such that ``J[i,j]=sum(Jforms_all[i*len(Fforms)+j])``,
+            ``i,j=0,..,len(Fforms)-1``.
+            The k-th entry of ``Jforms_all`` is a list of forms that are summed up in a given block.
+        active_compartments: List of compartments used in the variational form.
+
+            .. note::
+                This input is only used to get the compartment names, should we change the
+                input to only be the names?
+        all_compartments: List of all compartments in model.
+
+            .. note::
+                This is only used to get a map from mesh-id to name of compartment.
+                I think we should extract this information
+                from the active compartments.
+        stopwatches: Dictionary of stop-watches (stopwatch_name: stopwatch-class).
+
+            .. note::
+                Assumes that one has the entries:
+
+                - ``'snes jacobian assemble'``
+                - ``'snes residual assemble'``
+                - ``'snes initialize zero matrices'``
+        verbose: If True output logger info
+
+    .. note::
+        High-level dolfin solver ``d.solve()`` when applied to Mixed Nonlinear problems:
+        F is the sum of all forms, in smart this is:
+
+        .. highlight:: python
+        .. code-block:: python
+
+            Fsum = sum([f.lhs for f in model.forms]) # single form F0+F1+...+Fn
+            d.solve(Fsum==0, u)
 
-    F is the sum of all forms, in smart this is:
-    Fsum = sum([f.lhs for f in model.forms]) # single form F0+F1+...+Fn
-    d.solve(Fsum==0, u) roughly executes the following:
+        roughly executes the following:
 
+        .. highlight:: python
+        .. code-block:: python
 
-    * d.solve(Fsum==0, u)  [fem/solving.py]
-        * _solve_varproblem() [fem/solving.py]
+            d.solve(Fsum==0, u)  # [fem/solving.py]
+            _solve_varproblem()  # [fem/solving.py]
             eq, ... = _extract_args()
             # tuple of forms (F0, F1, ..., Fn)
             F = extract_blocks(eq.lhs) [fem/formmanipulations -> ufl/algorithms/formsplitter]
             for Fi in F:
                 for uj in u._functions:
                     Js.append(expand_derivatives(formmanipulations.derivative(Fi, uj)))
                     # [J00, J01, J02, etc...]
             problem = MixedNonlinearVariationalProblem(F, u._functions, bcs, Js)
             solver  = MixedNonlinearVariationalSolver(problem)
             solver.solve()
 
-    * MixedNonlinearVariationalProblem(F, u._functions, bcs, Js)     [fem/problem.py]
-        u_comps = [u[i]._cpp_object for i in range(len(u))]
+        .. highlight:: python
+        .. code-block:: python
 
-        # if len(F)!= len(u) -> Fill empty blocks of F with None
+            MixedNonlinearVariationalProblem(F, u._functions, bcs, Js)  # [fem/problem.py]
+            u_comps = [u[i]._cpp_object for i in range(len(u))]
 
-        # Check that len(J)==len(u)**2 and len(F)==len(u)
+            # if len(F)!= len(u) -> Fill empty blocks of F with None
+            # Check that len(J)==len(u)**2 and len(F)==len(u)
 
-        # use F to create Flist. Separate forms by domain:
-        # Flist[i] is a list of Forms separated by domain. E.g. if F1 consists of
-        # integrals on \Omega_1, \Omega_2, and \Omega_3
-        # then Flist[i] is a list with 3 forms
-        If Fi is None -> Flist[i] = cpp.fem.Form(1,0)
-        else -> Flist[i] = [Fi[domain=0], Fi[domain=1], ...]
-
-        # Do the same for J -> Jlist
-
-        cpp.fem.MixedNonlinearVariationalProblem.__init__(self, Flist, u_comps, bcs, Jlist)
-
-    ========
-    More notes:
-    ========
-    # on extract_blocks(F)
-    F  = sum([f.lhs for f in model.forms]) # single form
-    Fb = extract_blocks(F) # tuple of forms
-    Fb0 = Fb[0]
-
-    F0 = sum([f.lhs for f in model.forms if f.compartment.name=='cytosol'])
-    F0.equals(Fb0) -> False
-
-    I0 = F0.integrals()[0].integrand()
-    Ib0 = Fb0.integrals()[0].integrand()
-    (ufl.Indexed(Argument))) vs ufl.Indexed(ListTensor(ufl.Indexed(Argument)))
-    I0.ufl_operands[0] == Ib0.ufl_operands[0] -> False
-    I0.ufl_operands[1] == Ib0.ufl_operands[1] -> True
-    I0.ufl_operands[0] == Ib0.ufl_operands[0](1) -> True
-
-
-    # on d.functionspace
-    V.__repr__() shows the UFL coordinate element
-    (finite element over coordinate vector field) and finite element of the function space.
-    We can access individually with:
-    V.ufl_domain().ufl_coordinate_element()
-    V.ufl_element()
-
-    # on assembler
-    d.fem.assembling.assemble_mixed(form, tensor)
-    assembler = cpp.fem.MixedAssembler()
-
-
-    fem.assemble.cpp/assemble_mixed(GenericTensor& A, const Form& a, bool add)
-    MixedAssembler assembler;
-    assembler.add_values = add;
-    assembler.assemble(A, a);
+            # use F to create Flist. Separate forms by domain:
+            # Flist[i] is a list of Forms separated by domain. E.g. if F1 consists of
+            # integrals on \Omega_1, \Omega_2, and \Omega_3
+            # then Flist[i] is a list with 3 forms
+            If Fi is None -> Flist[i] = cpp.fem.Form(1,0)
+            else -> Flist[i] = [Fi[domain=0], Fi[domain=1], ...]
+
+            # Do the same for J -> Jlist
+            cpp.fem.MixedNonlinearVariationalProblem.__init__(self, Flist, u_comps, bcs, Jlist)
+
+    .. note::
+        .. highlight:: python
+        .. code-block:: python
+
+            # on extract_blocks(F)
+            F  = sum([f.lhs for f in model.forms]) # single form
+            Fb = extract_blocks(F) # tuple of forms
+            Fb0 = Fb[0]
+
+            F0 = sum([f.lhs for f in model.forms if f.compartment.name=='cytosol'])
+            F0.equals(Fb0) -> False
+
+            I0 = F0.integrals()[0].integrand()
+            Ib0 = Fb0.integrals()[0].integrand()
+            (ufl.Indexed(Argument))) vs ufl.Indexed(ListTensor(ufl.Indexed(Argument)))
+            I0.ufl_operands[0] == Ib0.ufl_operands[0] -> False
+            I0.ufl_operands[1] == Ib0.ufl_operands[1] -> True
+            I0.ufl_operands[0] == Ib0.ufl_operands[0](1) -> True
+
+        ``V.__repr__()`` shows the UFL coordinate element (finite element over coordinate
+        vector field) and finite element of the function space. We can access individually with:
+
+        .. highlight:: python
+        .. code-block:: python
+
+            V.ufl_domain().ufl_coordinate_element()
+            V.ufl_element()
+
+            # on assembler
+            d.fem.assembling.assemble_mixed(form, tensor)
+            assembler = cpp.fem.MixedAssembler()
+
+            fem.assemble.cpp/assemble_mixed(GenericTensor& A, const Form& a, bool add)
+            MixedAssembler assembler;
+            assembler.add_values = add;
+            assembler.assemble(A, a);
     """
 
-    # def __init__(self, model):
     def __init__(
         self,
-        u,
-        Fforms,
-        Jforms_all,
-        active_compartments,
-        all_compartments,
-        stopwatches,
-        print_assembly,
-        mpi_comm_world,
+        u: d.Function,
+        Fforms: List[List[d.Form]],
+        Jforms_all: List[List[d.Form]],
+        active_compartments: List[Compartment],
+        all_compartments: List[Compartment],
+        stopwatches: Dict[str, Stopwatch],
+        verbose: bool,
     ):
         self.u = u
         self.Fforms = Fforms
         self.Jforms_all = Jforms_all
-
         # for convenience, the mixed function space (model.V)
         self.W = [usub.function_space() for usub in u._functions]
         self.dim = len(self.Fforms)
 
         assert len(self.Jforms_all) == self.dim**2
-        self.comm = mpi_comm_world
+
+        # Extract MPI communicator from one of the underlying meshes
+        assert len(self.u._functions) >= 1
+        self.comm = self.u._functions[0].function_space().mesh().mpi_comm()
         self.rank = self.comm.rank
         self.size = self.comm.size
 
         # save sparsity patterns of block matrices
         self.tensors = [[None] * len(Jij_list) for Jij_list in self.Jforms_all]
 
         # Get local_to_global maps (len=number of owned dofs + ghost dofs) and
@@ -141,19 +196,21 @@
         # self.global_sizes = [c._num_dofs for c in active_compartments]
         self.is_single_domain = len(self.global_sizes) == 1
 
         self.active_compartment_names = [c.name for c in active_compartments]
         self.mesh_id_to_name = {c.mesh_id: c.name for c in all_compartments}
 
         # Should we print assembly info (can get very verbose)
-        self.print_assembly = print_assembly
+        self.verbose = verbose
 
         # Timings
+        for key in _stopwatch_keys:
+            if key not in stopwatches.keys():
+                raise ValueError(f"Stopwatch dictionary missing stopwatch {key}")
         self.stopwatches = stopwatches
-
         # Our custom assembler (something about dolfin's init_global_tensor was not
         # correct so we manually initialize the petsc matrix and then wrap with dolfin)
         # This assembly routine is the exact same as d.assemble_mixed() except
         # init_global_tensor() is commented out
         # Thanks to Prof. Kamensky and his student for the idea
         # https://github.com/hanzhao2020/PENGoLINS/blob/main/PENGoLINS/cpp/transfer_matrix.cpp
         os.path.dirname(os.path.realpath(__file__))
@@ -171,15 +228,15 @@
                 ij = i * self.dim + j
                 if all(
                     self.Jforms_all[ij][k].function_space(0) is None
                     for k in range(len(self.Jforms_all[ij]))
                 ):
                     self.empty_forms.append((i, j))
         if len(self.empty_forms) > 0:
-            if self.print_assembly:
+            if self.verbose:
                 logger.debug(
                     f"Forms {self.empty_forms} are empty. Skipping assembly.",
                     extra=dict(format_type="data"),
                 )
 
     def init_petsc_matnest(self):
         Jforms = self.Jforms_all
@@ -190,15 +247,15 @@
                 ij = i * dim + j
 
                 non_empty_forms = 0
                 for k in range(len(Jforms[ij])):
                     if Jforms[ij][k].function_space(0) is None:
                         # The only reason this is empty is because the whole form is empty
                         assert len(Jforms[ij]) == 1
-                        if self.print_assembly:
+                        if self.verbose:
                             logger.debug(
                                 f"{self.Jijk_name(i,j,k=None)} is empty",
                                 extra=dict(format_type="log"),
                             )
                         continue
                     else:
                         non_empty_forms += 1
@@ -214,15 +271,15 @@
                         extra=dict(format_type="log"),
                     )
 
                     d.assemble_mixed(Jforms[ij][k], tensor=self.tensors[ij][k])
 
                 if non_empty_forms == 0:
                     # If all forms are empty, we don't need to assemble. Initialize to zero matrix
-                    if self.print_assembly:
+                    if self.verbose:
                         logger.debug(
                             f"{self.Jijk_name(i,j)} is empty - initializing as "
                             f"empty PETSc Matrix with local size {self.local_sizes[i]}, "
                             f"{self.local_sizes[j]} "
                             f"and global size {self.global_sizes[i]}, {self.global_sizes[j]}",
                             extra=dict(format_type="log"),
                         )
@@ -261,23 +318,23 @@
         logger.info(f"Jpetsc_nest assembled, size = {self.Jpetsc_nest.size}")
 
     def d_to_p(self, dolfin_matrix):
         return d.as_backend_type(dolfin_matrix).mat()
 
     def init_petsc_vecnest(self):
         dim = self.dim
-        if self.print_assembly:
+        if self.verbose:
             logger.info("Initializing block residual vector", extra=dict(format_type="assembly"))
 
         Fpetsc = []
         for j in range(dim):
             Fsum = None
             for k in range(len(self.Fforms[j])):
                 if self.Fforms[j][k].function_space(0) is None:
-                    if self.print_assembly:
+                    if self.verbose:
                         logger.warning(
                             f"{self.Fjk_name(j,k)}] has no function space",
                             extra=dict(format_type="log"),
                         )
                     continue
 
                 tensor = d.PETScVector()
@@ -286,15 +343,15 @@
                     Fsum = d.assemble_mixed(self.Fforms[j][k], tensor=tensor)
                 else:
                     # Fsum.axpy(1, d.assemble_mixed(self.Fforms[j][k], tensor=tensor).vec(),
                     # structure=Fsum.Structure.DIFFERENT_NONZERO_PATTERN)
                     Fsum += d.assemble_mixed(self.Fforms[j][k], tensor=tensor)
 
             if Fsum is None:
-                if self.print_assembly:
+                if self.verbose:
                     logger.debug(
                         f"{self.Fjk_name(j)} is empty - initializing as empty PETSc "
                         f"Vector with local size {self.local_sizes[j]} "
                         f"and global size {self.global_sizes[j]}",
                         extra=dict(format_type="log"),
                     )
                 Fsum = d.PETScVector(self.init_petsc_vector(j, assemble=True))
@@ -314,15 +371,15 @@
         Parameters
         ----------
         Jnest : petsc4py.Mat
             PETSc nest matrix representing the Jacobian
 
         Jmats are created using assemble_mixed(Jform) and are dolfin.PETScMatrix types
         """
-        if self.print_assembly:
+        if self.verbose:
             logger.debug("Assembling block Jacobian", extra=dict(format_type="assembly"))
         self.stopwatches["snes jacobian assemble"].start()
         dim = self.dim
 
         Jform = self.Jforms_all
 
         # Get the petsc sub matrices, convert to dolfin wrapper, assemble forms using
@@ -337,40 +394,40 @@
                 # Extract petsc submatrix
                 if self.is_single_domain:
                     Jij_petsc = Jnest
                 else:
                     Jij_petsc = Jnest.getNestSubMatrix(i, j)
                 Jij_petsc.zeroEntries()  # this maintains sparse (non-zeros) structure
 
-                if self.print_assembly:
+                if self.verbose:
                     logger.debug(
                         f"Assembling {self.Jijk_name(i,j)}:",
                         extra=dict(format_type="assembly_sub"),
                     )
 
                 Jmats = []
                 # Jijk == dFi/duj(Omega_k)
                 for k in range(num_subforms):
                     # Check for empty form
                     if Jform[ij][k].function_space(0) is None:
-                        if self.print_assembly:
+                        if self.verbose:
                             logger.debug(
                                 f"{self.Jijk_name(i,j,k)} is empty. Skipping assembly.",
                                 extra=dict(format_type="data"),
                             )
                         continue
 
                     # if we have the sparsity pattern re-use it, if not save it for next time
                     # single domain can't re-use the tensor for some reason
                     if self.tensors[ij][k] is None and not self.is_single_domain:
                         raise AssertionError("I dont think this should happpen")
                     elif self.is_single_domain:
                         self.tensors[ij][k] = d.PETScMatrix(self.comm)
                     else:
-                        if self.print_assembly:
+                        if self.verbose:
                             logger.debug(
                                 f"Reusing tensor for {self.Jijk_name(i,j,k)}",
                                 extra=dict(format_type="data"),
                             )
                     # Assemble and append to the list of subforms
                     Jmats.append(d.assemble_mixed(Jform[ij][k], tensor=self.tensors[ij][k]))
                     # Print some useful info on assembled Jijk
@@ -390,15 +447,15 @@
 
         Jnest.assemble()
 
         self.stopwatches["snes jacobian assemble"].pause()
 
     def assemble_Fnest(self, Fnest):
         dim = self.dim
-        if self.print_assembly:
+        if self.verbose:
             logger.debug("Assembling block residual vector", extra=dict(format_type="assembly"))
         self.stopwatches["snes residual assemble"].start()
 
         if self.is_single_domain:
             Fj_petsc = [Fnest]
         else:
             Fj_petsc = Fnest.getNestSubVecs()
@@ -489,37 +546,60 @@
         V.setUp()
         # V.setLGMap(self.lgmaps_petsc[j])
 
         if assemble:
             V.assemble()
         return V
 
-    def Jijk_name(self, i, j, k=None):
-        ij = i * self.dim + j
+    def Jijk_name(self, i: int, j: int, k: Optional[int] = None):
+        """
+        Get a string representation of an entry of the Jacobian.
+
+        Args:
+            i: Row index
+            j: Column index
+            k: If the Jacobian entry is a sum of forms, get the name
+                of the domain in the `k`th entry.
+        """
         if k is None:
             return (
                 f"J{i}{j} = dF[{self.active_compartment_names[i]}]"
                 f"/du[{self.active_compartment_names[j]}]"
             )
         else:
+            ij = i * self.dim + j
+            if (num_entries := len(self.Jforms_all[ij])) <= k:
+                raise RuntimeError(f"J[{i},{j}] only consists of {num_entries} componets")
+
             domain_name = self.mesh_id_to_name[self.Jforms_all[ij][k].function_space(0).mesh().id()]
             return (
                 f"J{i}{j}{k} = dF[{self.active_compartment_names[i]}]"
                 f"/du[{self.active_compartment_names[j]}] (domain={domain_name})"
             )
 
-    def Fjk_name(self, j, k=None):
+    def Fjk_name(self, j: int, k: Optional[int] = None):
+        """
+        Get a string representation of an entry of the residual.
+
+        Args:
+            j: Block index
+            k: If the residual entry is a sum of forms, get the name
+                of the domain in the `k`th entry.
+        """
+
         if k is None:
             return f"F{j} = F[{self.active_compartment_names[j]}]"
         else:
+            if (num_entries := len(self.Fforms[j])) <= k:
+                raise RuntimeError(f"F[{j}] only consists of {num_entries} componets")
             domain_name = self.mesh_id_to_name[self.Fforms[j][k].function_space(0).mesh().id()]
             return f"F{j} = F[{self.active_compartment_names[j]}] (domain={domain_name})"
 
     def print_Jijk_info(self, i, j, k=None, tensor=None):
-        if not self.print_assembly:
+        if not self.verbose:
             return
         if tensor is None:
             return
         # Print some useful info on Jijk
         info = tensor.getInfo()
         # , block_size={int(info['block_size'])}
         info_str = (
```

### Comparing `fenics-smart-0.1.10/tests/test_compartment.py` & `fenics-smart-2.0.1/tests/test_compartment.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 @pytest.fixture(name="Cyto_kwargs")
 def example_compartment():
     kwargs = dict(
         dimensionality=3,
         name="Cyto",
-        compartment_units=smart.unit.um,
+        compartment_units=smart.units.unit.um,
         cell_marker=1,
     )
 
     Cyto = smart.model_assembly.Compartment(**kwargs)
     return (Cyto, kwargs)
```

### Comparing `fenics-smart-0.1.10/tests/test_species.py` & `fenics-smart-2.0.1/tests/test_species.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import smart
 
 
 @pytest.fixture(name="A_kwargs")
 def example_species():
     kwargs = dict(
-        concentration_units=smart.unit.uM,
-        diffusion_units=smart.unit.um**2 / smart.unit.sec,
+        concentration_units=smart.units.unit.uM,
+        diffusion_units=smart.units.unit.um**2 / smart.units.unit.sec,
         initial_condition=0.01,
         D=2.0,
         name="A",
         compartment_name="Cyto",
         group="Some group",
     )
 
@@ -27,19 +27,17 @@
     assert A.latex_name == kwargs["name"]
     assert str(A.sym) == kwargs["name"]
 
     assert math.isclose(A.initial_condition, kwargs["initial_condition"])
     assert (
         A.initial_condition_quantity == kwargs["initial_condition"] * kwargs["concentration_units"]
     )
-    assert A.concentration_units == smart.common.pint_unit_to_quantity(
-        kwargs["concentration_units"]
-    )
+    assert A.concentration_units == smart.units.unit_to_quantity(kwargs["concentration_units"])
     assert math.isclose(A.D, kwargs["D"])
-    assert A.diffusion_units == smart.common.pint_unit_to_quantity(kwargs["diffusion_units"])
+    assert A.diffusion_units == smart.units.unit_to_quantity(kwargs["diffusion_units"])
     assert A.D_quantity == kwargs["D"] * kwargs["diffusion_units"]
 
     assert A.compartment_name == kwargs["compartment_name"]
     assert A.group == kwargs["group"]
     assert A.dof_map is None
     assert A.ut is None
     assert A.v is None
```

### Comparing `fenics-smart-0.1.10/tests/test_stubs_model_init.py` & `fenics-smart-2.0.1/tests/test_stubs_model_init.py`

 * *Files identical despite different names*

