# Comparing `tmp/adaptive-0.9.0.tar.gz` & `tmp/adaptive-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adaptive-0.9.0.tar", last modified: Mon Oct  7 11:08:23 2019, max compression
+gzip compressed data, was "adaptive-1.0.0.tar", last modified: Mon May 15 18:09:01 2023, max compression
```

## Comparing `adaptive-0.9.0.tar` & `adaptive-1.0.0.tar`

### file list

```diff
@@ -1,52 +1,57 @@
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2019-10-07 11:08:23.000000 adaptive-0.9.0/
--rw-r--r--   0 basnijholt   (501) staff       (20)     1521 2019-05-24 18:30:02.000000 adaptive-0.9.0/LICENSE
--rw-r--r--   0 basnijholt   (501) staff       (20)       16 2019-05-24 18:30:02.000000 adaptive-0.9.0/MANIFEST.in
--rw-r--r--   0 basnijholt   (501) staff       (20)      527 2019-10-07 11:08:23.000000 adaptive-0.9.0/PKG-INFO
--rw-r--r--   0 basnijholt   (501) staff       (20)     6708 2019-07-10 17:13:09.000000 adaptive-0.9.0/README.rst
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2019-10-07 11:08:23.000000 adaptive-0.9.0/adaptive/
--rw-r--r--   0 basnijholt   (501) staff       (20)     1254 2019-08-31 12:53:57.000000 adaptive-0.9.0/adaptive/__init__.py
--rw-r--r--   0 basnijholt   (501) staff       (20)       60 2019-10-07 11:08:23.000000 adaptive-0.9.0/adaptive/_static_version.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     6066 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/_version.py
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2019-10-07 11:08:23.000000 adaptive-0.9.0/adaptive/learner/
--rw-r--r--   0 basnijholt   (501) staff       (20)      989 2019-08-31 12:53:57.000000 adaptive-0.9.0/adaptive/learner/__init__.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     4281 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/learner/average_learner.py
--rw-r--r--   0 basnijholt   (501) staff       (20)    16756 2019-09-05 09:15:26.000000 adaptive-0.9.0/adaptive/learner/balancing_learner.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     6108 2019-08-31 12:53:28.000000 adaptive-0.9.0/adaptive/learner/base_learner.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     3297 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/learner/data_saver.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     5961 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/learner/integrator_coeffs.py
--rw-r--r--   0 basnijholt   (501) staff       (20)    18883 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/learner/integrator_learner.py
--rw-r--r--   0 basnijholt   (501) staff       (20)    23555 2019-09-06 11:27:46.000000 adaptive-0.9.0/adaptive/learner/learner1D.py
--rw-r--r--   0 basnijholt   (501) staff       (20)    20126 2019-09-12 15:38:03.000000 adaptive-0.9.0/adaptive/learner/learner2D.py
--rw-r--r--   0 basnijholt   (501) staff       (20)    41228 2019-09-23 07:47:54.000000 adaptive-0.9.0/adaptive/learner/learnerND.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     4003 2019-08-31 12:53:57.000000 adaptive-0.9.0/adaptive/learner/sequence_learner.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     3670 2019-08-31 12:53:57.000000 adaptive-0.9.0/adaptive/learner/skopt_learner.py
--rw-r--r--   0 basnijholt   (501) staff       (20)    23259 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/learner/triangulation.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     8245 2019-08-31 12:59:50.000000 adaptive-0.9.0/adaptive/notebook_integration.py
--rw-r--r--   0 basnijholt   (501) staff       (20)    26353 2019-08-31 12:59:50.000000 adaptive-0.9.0/adaptive/runner.py
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2019-10-07 11:08:23.000000 adaptive-0.9.0/adaptive/tests/
--rw-r--r--   0 basnijholt   (501) staff       (20)        0 2019-05-24 18:30:02.000000 adaptive-0.9.0/adaptive/tests/__init__.py
--rw-r--r--   0 basnijholt   (501) staff       (20)    17993 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/tests/algorithm_4.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     1464 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/tests/test_average_learner.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     2171 2019-09-20 11:42:20.000000 adaptive-0.9.0/adaptive/tests/test_balancing_learner.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     8719 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/tests/test_cquad.py
--rw-r--r--   0 basnijholt   (501) staff       (20)    12104 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/tests/test_learner1d.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     1742 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/tests/test_learnernd.py
--rw-r--r--   0 basnijholt   (501) staff       (20)    19313 2019-09-20 11:42:20.000000 adaptive-0.9.0/adaptive/tests/test_learners.py
--rw-r--r--   0 basnijholt   (501) staff       (20)      529 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/tests/test_notebook_integration.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     2920 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/tests/test_runner.py
--rw-r--r--   0 basnijholt   (501) staff       (20)      731 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/tests/test_skopt_learner.py
--rw-r--r--   0 basnijholt   (501) staff       (20)    10029 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/tests/test_triangulation.py
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2019-10-07 11:08:23.000000 adaptive-0.9.0/adaptive/tests/unit/
--rw-r--r--   0 basnijholt   (501) staff       (20)        0 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/tests/unit/__init__.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     1324 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/tests/unit/test_learnernd.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     1909 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/tests/unit/test_learnernd_integration.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     2132 2019-07-10 17:13:09.000000 adaptive-0.9.0/adaptive/tests/unit/test_triangulation.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     1635 2019-08-31 12:59:50.000000 adaptive-0.9.0/adaptive/utils.py
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2019-10-07 11:08:22.000000 adaptive-0.9.0/adaptive.egg-info/
--rw-r--r--   0 basnijholt   (501) staff       (20)      527 2019-10-07 11:08:21.000000 adaptive-0.9.0/adaptive.egg-info/PKG-INFO
--rw-r--r--   0 basnijholt   (501) staff       (20)     1351 2019-10-07 11:08:21.000000 adaptive-0.9.0/adaptive.egg-info/SOURCES.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)        1 2019-10-07 11:08:21.000000 adaptive-0.9.0/adaptive.egg-info/dependency_links.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)      175 2019-10-07 11:08:21.000000 adaptive-0.9.0/adaptive.egg-info/requires.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)        9 2019-10-07 11:08:21.000000 adaptive-0.9.0/adaptive.egg-info/top_level.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)       38 2019-10-07 11:08:23.000000 adaptive-0.9.0/setup.cfg
--rw-r--r--   0 basnijholt   (501) staff       (20)     1837 2019-08-31 12:59:50.000000 adaptive-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:09:01.497214 adaptive-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-15 18:08:42.000000 adaptive-1.0.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-15 18:08:42.000000 adaptive-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 18:08:42.000000 adaptive-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-15 18:09:01.497214 adaptive-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-05-15 18:08:42.000000 adaptive-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:09:01.497214 adaptive-1.0.0/adaptive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-15 18:09:01.497214 adaptive-1.0.0/adaptive/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:09:01.493214 adaptive-1.0.0/adaptive/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/learner/average_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26147 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/learner/average_learner1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21987 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/learner/balancing_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/learner/base_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/learner/data_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/learner/integrator_coeffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23367 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/learner/integrator_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33332 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/learner/learner1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29018 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/learner/learner2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45314 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/learner/learnerND.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/learner/sequence_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/learner/skopt_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24593 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/learner/triangulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/notebook_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43778 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:09:01.497214 adaptive-1.0.0/adaptive/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19299 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/algorithm_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/test_average_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/test_average_learner1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/test_balancing_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/test_cquad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12699 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/test_learner1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/test_learnernd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24796 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/test_learners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/test_notebook_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/test_sequence_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/test_skopt_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/test_triangulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:09:01.497214 adaptive-1.0.0/adaptive/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/unit/test_learnernd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/unit/test_learnernd_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/tests/unit/test_triangulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-15 18:08:42.000000 adaptive-1.0.0/adaptive/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:09:01.493214 adaptive-1.0.0/adaptive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-15 18:09:01.000000 adaptive-1.0.0/adaptive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-15 18:09:01.000000 adaptive-1.0.0/adaptive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:09:01.000000 adaptive-1.0.0/adaptive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-15 18:09:01.000000 adaptive-1.0.0/adaptive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 18:09:01.000000 adaptive-1.0.0/adaptive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-15 18:08:42.000000 adaptive-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-15 18:09:01.497214 adaptive-1.0.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `adaptive-0.9.0/LICENSE` & `adaptive-1.0.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2017-2018, Adaptive authors
+Copyright (c) 2017-2023, Adaptive authors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `adaptive-0.9.0/adaptive/__init__.py` & `adaptive-1.0.0/adaptive/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-# -*- coding: utf-8 -*-
-
 from contextlib import suppress
 
-from adaptive import learner, runner, utils
 from adaptive._version import __version__
 from adaptive.learner import (
     AverageLearner,
+    AverageLearner1D,
     BalancingLearner,
     BaseLearner,
     DataSaver,
     IntegratorLearner,
     Learner1D,
     Learner2D,
     LearnerND,
-    make_datasaver,
     SequenceLearner,
+    make_datasaver,
 )
 from adaptive.notebook_integration import (
     active_plotting_tasks,
     live_plot,
     notebook_extension,
 )
 from adaptive.runner import AsyncRunner, BlockingRunner, Runner
 
+from adaptive import learner, runner, utils  # isort:skip
+
 __all__ = [
     "learner",
     "runner",
     "utils",
     "__version__",
     "AverageLearner",
     "BalancingLearner",
     "BaseLearner",
     "DataSaver",
     "IntegratorLearner",
     "Learner1D",
     "Learner2D",
     "LearnerND",
+    "AverageLearner1D",
     "make_datasaver",
     "SequenceLearner",
     "active_plotting_tasks",
     "live_plot",
     "notebook_extension",
     "AsyncRunner",
     "BlockingRunner",
@@ -48,10 +49,9 @@
 
 with suppress(ImportError):
     # Only available if 'scikit-optimize' is installed
     from adaptive.learner import SKOptLearner  # noqa: F401
 
     __all__.append("SKOptLearner")
 
-# to avoid confusion with `notebook_extension` and `__version__`
-del _version  # noqa: F821
-del notebook_integration  # noqa: F821
+# to avoid confusion with `notebook_extension`
+del notebook_integration  # type: ignore[name-defined] # noqa: F821
```

### Comparing `adaptive-0.9.0/adaptive/learner/base_learner.py` & `adaptive-1.0.0/adaptive/learner/base_learner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
 import abc
 from contextlib import suppress
-from copy import deepcopy
+from typing import TYPE_CHECKING, Any, Callable, TypeVar
+
+import cloudpickle
 
 from adaptive.utils import load, save
 
+if TYPE_CHECKING:
+    import pandas
+
 
-def uses_nth_neighbors(n):
+def uses_nth_neighbors(n: int):
     """Decorator to specify how many neighboring intervals the loss function uses.
 
     Wraps loss functions to indicate that they expect intervals together
     with ``n`` nearest neighbors
 
     The loss function will then receive the data of the N nearest neighbors
-    (``nth_neighbors``) aling with the data of the interval itself in a dict.
+    (``nth_neighbors``) along with the data of the interval itself in a dict.
     The `~adaptive.Learner1D` will also make sure that the loss is updated
     whenever one of the ``nth_neighbors`` changes.
 
     Examples
     --------
 
     The next function is a part of the `curvature_loss_function` function.
@@ -57,38 +62,43 @@
     def _wrapped(loss_per_interval):
         loss_per_interval.nth_neighbors = n
         return loss_per_interval
 
     return _wrapped
 
 
-class BaseLearner(metaclass=abc.ABCMeta):
+DataType = dict[Any, Any]
+
+
+class BaseLearner(abc.ABC):
     """Base class for algorithms for learning a function 'f: X → Y'.
 
     Attributes
     ----------
     function : callable: X → Y
-        The function to learn.
+        The function to learn. A subclass of BaseLearner might modify
+        the user's supplied function.
     data : dict: X → Y
         `function` evaluated at certain points.
-        The values can be 'None', which indicates that the point
-        will be evaluated, but that we do not have the result yet.
-    npoints : int, optional
-        The number of evaluated points that have been added to the learner.
-        Subclasses do not *have* to implement this attribute.
-    pending_points : set, optional
+    pending_points : set
         Points that have been requested but have not been evaluated yet.
-        Subclasses do not *have* to implement this attribute.
+    npoints : int
+        The number of evaluated points that have been added to the learner.
 
     Notes
     -----
     Subclasses may define a ``plot`` method that takes no parameters
     and returns a holoviews plot.
     """
 
+    data: DataType
+    npoints: int
+    pending_points: set
+    function: Callable[..., Any]
+
     def tell(self, x, y):
         """Tell the learner about a single value.
 
         Parameters
         ----------
         x : A value from the function domain
         y : A value from the function image
@@ -106,20 +116,18 @@
         for x, y in zip(xs, ys):
             self.tell(x, y)
 
     @abc.abstractmethod
     def tell_pending(self, x):
         """Tell the learner that 'x' has been requested such
         that it's not suggested again."""
-        pass
 
     @abc.abstractmethod
     def remove_unfinished(self):
         """Remove uncomputed data from the learner."""
-        pass
 
     @abc.abstractmethod
     def loss(self, real=True):
         """Return the loss for the current state of the learner.
 
         Parameters
         ----------
@@ -138,22 +146,26 @@
         n : int
             The number of points to choose.
         tell_pending : bool, default: True
             If True, add the chosen points to this learner's
             `pending_points`. Set this to False if you do not
             want to modify the state of the learner.
         """
+
+    @abc.abstractmethod
+    def _get_data(self) -> Any:
         pass
 
     @abc.abstractmethod
-    def _get_data(self):
+    def _set_data(self, data: Any) -> None:
         pass
 
     @abc.abstractmethod
-    def _set_data(self):
+    def new(self):
+        """Return a new learner with the same function and parameters."""
         pass
 
     def copy_from(self, other):
         """Copy over the data from another learner.
 
         Parameters
         ----------
@@ -187,12 +199,57 @@
             If the data is compressed when saved, one must load it
             with compression too.
         """
         with suppress(FileNotFoundError, EOFError):
             data = load(fname, compress)
             self._set_data(data)
 
+    @abc.abstractmethod
+    def to_dataframe(
+        self,
+        with_default_function_args: bool = True,
+        function_prefix: str = "function.",
+        **kwargs: Any,
+    ) -> pandas.DataFrame:
+        """Return the data as a `pandas.DataFrame`.
+
+        Parameters
+        ----------
+        with_default_function_args : bool, optional
+            Include the ``learner.function``'s default arguments as a
+            column, by default True
+        function_prefix : str, optional
+            Prefix to the ``learner.function``'s default arguments' names,
+            by default "function."
+        x_name : str, optional
+            Name of the input value, by default "x"
+        y_name : str, optional
+            Name of the output value, by default "y"
+
+        Returns
+        -------
+        pandas.DataFrame
+        """
+
+    @abc.abstractmethod
+    def load_dataframe(
+        self,
+        df: pandas.DataFrame,
+        with_default_function_args: bool = True,
+        function_prefix: str = "function.",
+        **kwargs: Any,
+    ) -> None:
+        """Load data from a `pandas.DataFrame`.
+
+        If ``with_default_function_args`` is True, then ``learner.function``'s
+        default arguments are set (using `functools.partial`) from the values
+        in the `pandas.DataFrame`.
+        """
+
     def __getstate__(self):
-        return deepcopy(self.__dict__)
+        return cloudpickle.dumps(self.__dict__)
 
     def __setstate__(self, state):
-        self.__dict__ = state
+        self.__dict__ = cloudpickle.loads(state)
+
+
+LearnerType = TypeVar("LearnerType", bound=BaseLearner)
```

### Comparing `adaptive-0.9.0/adaptive/learner/integrator_coeffs.py` & `adaptive-1.0.0/adaptive/learner/integrator_coeffs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# -*- coding: utf-8 -*-
 # Based on an adaptive quadrature algorithm by Pedro Gonnet
+from __future__ import annotations
 
 from collections import defaultdict
 from fractions import Fraction
+from functools import cache
 
 import numpy as np
 import scipy.linalg
 
 
-def legendre(n):
+def legendre(n: int) -> list[list[Fraction]]:
     """Return the first n Legendre polynomials.
 
     The polynomials have *standard* normalization, i.e.
     int_{-1}^1 dx L_n(x) L_m(x) = delta(m, n) * 2 / (2 * n + 1).
 
     The return value is a list of list of fraction.Fraction instances.
     """
@@ -25,15 +26,15 @@
         new[1:] = (r * (2 * i - 1) for r in result[-1])
         new[:-2] = (n - r * (i - 1) for n, r in zip(new[:-2], result[-2]))
         new[:] = (n / i for n in new)
         result.append(new)
     return result
 
 
-def newton(n):
+def newton(n: int) -> np.ndarray:
     """Compute the monomial coefficients of the Newton polynomial over the
     nodes of the n-point Clenshaw-Curtis quadrature rule.
     """
     # The nodes of the Clenshaw-Curtis rule are x_i = -cos(i * Pi / (n-1)).
     # Here, we calculate the coefficients c_i such that sum_i c_i * x^i
     # = prod_i (x - x_i).  The coefficients are thus sums of products of
     # cosines.
@@ -44,15 +45,15 @@
     #
     # The dictionary 'terms' descibes the terms that make up the
     # monomial coefficients.  Each item ((d, a), m) corresponds to a
     # term m * cos(a * Pi / n) to be added to prefactor of the
     # monomial x^(n-d).
 
     mod = 2 * (n - 1)
-    terms = defaultdict(int)
+    terms: dict[tuple[int, int], int] = defaultdict(int)
     terms[0, 0] += 1
 
     for i in range(n):
         newterms = []
         for (d, a), m in terms.items():
             for b in [i, -i]:
                 # In order to reduce the number of terms, cosine
@@ -82,15 +83,15 @@
     cf = np.array(c, float)
     assert all(int(cfe) == ce for cfe, ce in zip(cf, c)), "Precision loss"
 
     cf /= 2.0 ** np.arange(n, -1, -1)
     return cf
 
 
-def scalar_product(a, b):
+def scalar_product(a: list[Fraction], b: list[Fraction]) -> Fraction:
     """Compute the polynomial scalar product int_-1^1 dx a(x) b(x).
 
     The args must be sequences of polynomial coefficients.  This
     function is careful to use the input data type for calculations.
     """
     la = len(a)
     lc = len(b) + la + 1
@@ -100,18 +101,18 @@
     for i, bi in enumerate(b):
         if bi == 0:
             continue
         for j in range(i % 2, la, 2):
             c[i + j] += a[j] * bi
 
     # Calculate the definite integral from -1 to 1.
-    return 2 * sum(c[i] / (i + 1) for i in range(0, lc, 2))
+    return 2 * sum(c[i] / (i + 1) for i in range(0, lc, 2))  # type: ignore[return-value]
 
 
-def calc_bdef(ns):
+def calc_bdef(ns: tuple[int, int, int, int]) -> list[np.ndarray]:
     """Calculate the decompositions of Newton polynomials (over the nodes
     of the n-point Clenshaw-Curtis quadrature rule) in terms of
     Legandre polynomials.
 
     The parameter 'ns' is a sequence of numers of points of the
     quadrature rule.  The return value is a corresponding sequence of
     normalized Legendre polynomial coefficients.
@@ -129,52 +130,65 @@
             # orthonormal.)
             poly.append(np.sqrt((2 * len(b) - 1) / 2) * igral)
 
         result.append(np.array(poly))
     return result
 
 
-def calc_V(x, n):
+def calc_V(x: np.ndarray, n: int) -> np.ndarray:
     V = [np.ones(x.shape), x.copy()]
     for i in range(2, n):
         V.append((2 * i - 1) / i * x * V[-1] - (i - 1) / i * V[-2])
     for i in range(n):
         V[i] *= np.sqrt(i + 0.5)
     return np.array(V).T
 
 
-eps = np.spacing(1)
-
-# the nodes and Newton polynomials
-ns = (5, 9, 17, 33)
-xi = [-np.cos(np.linspace(0, np.pi, n)) for n in ns]
-
-# Make `xi` perfectly anti-symmetric, important for splitting the intervals
-xi = [(row - row[::-1]) / 2 for row in xi]
-
-# Compute the Vandermonde-like matrix and its inverse.
-V = [calc_V(x, n) for x, n in zip(xi, ns)]
-V_inv = list(map(scipy.linalg.inv, V))
-Vcond = [scipy.linalg.norm(a, 2) * scipy.linalg.norm(b, 2) for a, b in zip(V, V_inv)]
-
-# Compute the shift matrices.
-T_left, T_right = [V_inv[3] @ calc_V((xi[3] + a) / 2, ns[3]) for a in [-1, 1]]
-
-# If the relative difference between two consecutive approximations is
-# lower than this value, the error estimate is considered reliable.
-# See section 6.2 of Pedro Gonnet's thesis.
-hint = 0.1
-
-# Smallest acceptable relative difference of points in a rule.  This was chosen
-# such that no artifacts are apparent in plots of (i, log(a_i)), where a_i is
-# the sequence of estimates of the integral value of an interval and all its
-# ancestors..
-min_sep = 16 * eps
-
-ndiv_max = 20
-
-# set-up the downdate matrix
-k = np.arange(ns[3])
-alpha = np.sqrt((k + 1) ** 2 / (2 * k + 1) / (2 * k + 3))
-gamma = np.concatenate([[0, 0], np.sqrt(k[2:] ** 2 / (4 * k[2:] ** 2 - 1))])
-
-b_def = calc_bdef(ns)
+@cache
+def _coefficients():
+    """Compute the coefficients on demand, in order to avoid doing linear algebra on import."""
+    eps = np.spacing(1)
+
+    # the nodes and Newton polynomials
+    ns = (5, 9, 17, 33)
+    xi = [-np.cos(np.linspace(0, np.pi, n)) for n in ns]
+
+    # Make `xi` perfectly anti-symmetric, important for splitting the intervals
+    xi = [(row - row[::-1]) / 2 for row in xi]
+
+    # Compute the Vandermonde-like matrix and its inverse.
+    V = [calc_V(x, n) for x, n in zip(xi, ns)]
+    V_inv = list(map(scipy.linalg.inv, V))
+    Vcond = [
+        scipy.linalg.norm(a, 2) * scipy.linalg.norm(b, 2) for a, b in zip(V, V_inv)
+    ]
+
+    # Compute the shift matrices.
+    T_left, T_right = (V_inv[3] @ calc_V((xi[3] + a) / 2, ns[3]) for a in [-1, 1])
+
+    # If the relative difference between two consecutive approximations is
+    # lower than this value, the error estimate is considered reliable.
+    # See section 6.2 of Pedro Gonnet's thesis.
+    hint = 0.1
+
+    # Smallest acceptable relative difference of points in a rule.  This was chosen
+    # such that no artifacts are apparent in plots of (i, log(a_i)), where a_i is
+    # the sequence of estimates of the integral value of an interval and all its
+    # ancestors..
+    min_sep = 16 * eps
+
+    ndiv_max = 20
+
+    # set-up the downdate matrix
+    k = np.arange(ns[3])
+    alpha = np.sqrt((k + 1) ** 2 / (2 * k + 1) / (2 * k + 3))
+    gamma = np.concatenate([[0, 0], np.sqrt(k[2:] ** 2 / (4 * k[2:] ** 2 - 1))])
+
+    b_def = calc_bdef(ns)
+    return locals()
+
+
+def __getattr__(name):
+    try:
+        return _coefficients()[name]
+    except KeyError:
+        raise AttributeError(f"module {__name__} has no attribute {name}") from None
```

### Comparing `adaptive-0.9.0/adaptive/learner/integrator_learner.py` & `adaptive-1.0.0/adaptive/learner/integrator_learner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,69 @@
-# -*- coding: utf-8 -*-
 # Based on an adaptive quadrature algorithm by Pedro Gonnet
+from __future__ import annotations
 
 import sys
 from collections import defaultdict
 from math import sqrt
 from operator import attrgetter
+from typing import TYPE_CHECKING, Callable
 
+import cloudpickle
 import numpy as np
 from scipy.linalg import norm
 from sortedcontainers import SortedSet
 
+from adaptive.learner import integrator_coeffs as coeff
 from adaptive.learner.base_learner import BaseLearner
 from adaptive.notebook_integration import ensure_holoviews
-from adaptive.utils import cache_latest, restore
+from adaptive.utils import assign_defaults, cache_latest, restore
 
-from .integrator_coeffs import (
-    T_left,
-    T_right,
-    V_inv,
-    Vcond,
-    alpha,
-    b_def,
-    eps,
-    gamma,
-    hint,
-    min_sep,
-    ndiv_max,
-    ns,
-    xi,
-)
+try:
+    import pandas
 
+    with_pandas = True
 
-def _downdate(c, nans, depth):
+except ModuleNotFoundError:
+    with_pandas = False
+
+
+def _downdate(c: np.ndarray, nans: list[int], depth: int) -> np.ndarray:
     # This is algorithm 5 from the thesis of Pedro Gonnet.
-    b = b_def[depth].copy()
-    m = ns[depth] - 1
+    b = coeff.b_def[depth].copy()
+    m = coeff.ns[depth] - 1
     for i in nans:
-        b[m + 1] /= alpha[m]
-        xii = xi[depth][i]
-        b[m] = (b[m] + xii * b[m + 1]) / alpha[m - 1]
+        b[m + 1] /= coeff.alpha[m]
+        xii = coeff.xi[depth][i]
+        b[m] = (b[m] + xii * b[m + 1]) / coeff.alpha[m - 1]
         for j in range(m - 1, 0, -1):
-            b[j] = (b[j] + xii * b[j + 1] - gamma[j + 1] * b[j + 2]) / alpha[j - 1]
+            b[j] = (
+                b[j] + xii * b[j + 1] - coeff.gamma[j + 1] * b[j + 2]
+            ) / coeff.alpha[j - 1]
         b = b[1:]
 
         c[:m] -= c[m] / b[m] * b[:m]
         c[m] = 0
         m -= 1
     return c
 
 
-def _zero_nans(fx):
+def _zero_nans(fx: np.ndarray) -> list[int]:
     """Caution: this function modifies fx."""
     nans = []
     for i in range(len(fx)):
         if not np.isfinite(fx[i]):
             nans.append(i)
             fx[i] = 0.0
     return nans
 
 
-def _calc_coeffs(fx, depth):
+def _calc_coeffs(fx: np.ndarray, depth: int) -> np.ndarray:
     """Caution: this function modifies fx."""
     nans = _zero_nans(fx)
-    c_new = V_inv[depth] @ fx
+    c_new = coeff.V_inv[depth] @ fx
     if nans:
         fx[nans] = np.nan
         c_new = _downdate(c_new, nans, depth)
     return c_new
 
 
 class DivergentIntegralError(ValueError):
@@ -96,15 +93,15 @@
         The number of splits that the interval has gone through, starting at 1.
     ndiv : int
         A number that is used to determine whether the interval is divergent.
     parent : _Interval
         The parent interval.
     children : list of `_Interval`s
         The intervals resulting from a split.
-    done_points : dict
+    data : dict
         A dictionary with the x-values and y-values: `{x1: y1, x2: y2 ...}`.
     done : bool
         The integral and the error for the interval has been calculated.
     done_leaves : set or None
         Leaves used for the error and the integral estimation of this
         interval. None means that this information was already propagated to
         the ancestors of this interval.
@@ -129,137 +126,143 @@
         "igral",
         "err",
         "fx",
         "rdepth",
         "ndiv",
         "parent",
         "children",
-        "done_points",
+        "data",
         "done_leaves",
         "depth_complete",
         "removed",
     ]
 
-    def __init__(self, a, b, depth, rdepth):
-        self.children = []
-        self.done_points = {}
+    def __init__(self, a: int | float, b: int | float, depth: int, rdepth: int) -> None:
+        self.children: list[_Interval] = []
+        self.data: dict[float, float] = {}
         self.a = a
         self.b = b
         self.depth = depth
         self.rdepth = rdepth
-        self.done_leaves = set()
-        self.depth_complete = None
+        self.done_leaves: set[_Interval] | None = set()
+        self.depth_complete: int | None = None
         self.removed = False
+        if TYPE_CHECKING:
+            self.ndiv: int
+            self.parent: _Interval | None
+            self.err: float
+            self.c: np.ndarray
 
     @classmethod
-    def make_first(cls, a, b, depth=2):
+    def make_first(cls, a: int, b: int, depth: int = 2) -> _Interval:
         ival = _Interval(a, b, depth, rdepth=1)
         ival.ndiv = 0
         ival.parent = None
         ival.err = sys.float_info.max  # needed because inf/2 == inf
         return ival
 
     @property
-    def T(self):
+    def T(self) -> np.ndarray:
         """Get the correct shift matrix.
 
         Should only be called on children of a split interval.
         """
         assert self.parent is not None
         left = self.a == self.parent.a
         right = self.b == self.parent.b
         assert left != right
-        return T_left if left else T_right
+        return coeff.T_left if left else coeff.T_right
 
-    def refinement_complete(self, depth):
+    def refinement_complete(self, depth: int) -> bool:
         """The interval has all the y-values to calculate the intergral."""
-        if len(self.done_points) < ns[depth]:
+        if len(self.data) < coeff.ns[depth]:
             return False
-        return all(p in self.done_points for p in self.points(depth))
+        return all(p in self.data for p in self.points(depth))
 
-    def points(self, depth=None):
+    def points(self, depth: int | None = None) -> np.ndarray:
         if depth is None:
             depth = self.depth
         a = self.a
         b = self.b
-        return (a + b) / 2 + (b - a) * xi[depth] / 2
+        return (a + b) / 2 + (b - a) * coeff.xi[depth] / 2
 
-    def refine(self):
+    def refine(self) -> _Interval:
         self.depth += 1
         return self
 
-    def split(self):
+    def split(self) -> list[_Interval]:
         points = self.points()
         m = points[len(points) // 2]
         ivals = [
             _Interval(self.a, m, 0, self.rdepth + 1),
             _Interval(m, self.b, 0, self.rdepth + 1),
         ]
         self.children = ivals
         for ival in ivals:
             ival.parent = self
             ival.ndiv = self.ndiv
             ival.err = self.err / 2
 
         return ivals
 
-    def calc_igral(self):
+    def calc_igral(self) -> None:
         self.igral = (self.b - self.a) * self.c[0] / sqrt(2)
 
-    def update_heuristic_err(self, value):
+    def update_heuristic_err(self, value: float) -> None:
         """Sets the error of an interval using a heuristic (half the error of
         the parent) when the actual error cannot be calculated due to its
         parents not being finished yet. This error is propagated down to its
         children."""
         self.err = value
         for child in self.children:
             if child.depth_complete or (
                 child.depth_complete == 0 and self.depth_complete is not None
             ):
                 continue
             child.update_heuristic_err(value / 2)
 
-    def calc_err(self, c_old):
+    def calc_err(self, c_old: np.ndarray) -> float:
         c_new = self.c
         c_diff = np.zeros(max(len(c_old), len(c_new)))
         c_diff[: len(c_old)] = c_old
         c_diff[: len(c_new)] -= c_new
         c_diff = norm(c_diff)
         self.err = (self.b - self.a) * c_diff
         for child in self.children:
             if child.depth_complete is None:
                 child.update_heuristic_err(self.err / 2)
         return c_diff
 
-    def calc_ndiv(self):
+    def calc_ndiv(self) -> None:
+        assert self.parent is not None
         div = self.parent.c00 and self.c00 / self.parent.c00 > 2
-        self.ndiv += div
+        self.ndiv += int(div)
 
-        if self.ndiv > ndiv_max and 2 * self.ndiv > self.rdepth:
+        if self.ndiv > coeff.ndiv_max and 2 * self.ndiv > self.rdepth:
             raise DivergentIntegralError
 
         if div:
             for child in self.children:
                 child.update_ndiv_recursively()
 
-    def update_ndiv_recursively(self):
+    def update_ndiv_recursively(self) -> None:
         self.ndiv += 1
-        if self.ndiv > ndiv_max and 2 * self.ndiv > self.rdepth:
+        if self.ndiv > coeff.ndiv_max and 2 * self.ndiv > self.rdepth:
             raise DivergentIntegralError
 
         for child in self.children:
             child.update_ndiv_recursively()
 
-    def complete_process(self, depth):
+    def complete_process(self, depth: int) -> tuple[bool, bool] | tuple[bool, np.bool_]:
         """Calculate the integral contribution and error from this interval,
         and update the done leaves of all ancestor intervals."""
         assert self.depth_complete is None or self.depth_complete == depth - 1
         self.depth_complete = depth
 
-        fx = [self.done_points[k] for k in self.points(depth)]
+        fx = [self.data[k] for k in self.points(depth)]
         self.fx = np.array(fx)
         force_split = False  # This may change when refining
 
         first_ival = self.parent is None and depth == 2
 
         if depth and not first_ival:
             # Store for usage in refine
@@ -272,29 +275,31 @@
             return False, False
 
         self.calc_igral()
 
         if depth:
             # Refine
             c_diff = self.calc_err(c_old)
-            force_split = c_diff > hint * norm(self.c)
+            force_split = c_diff > coeff.hint * norm(self.c)
         else:
             # Split
             self.c00 = self.c[0]
-
+            assert self.parent is not None
             if self.parent.depth_complete is not None:
-                c_old = self.T[:, : ns[self.parent.depth_complete]] @ self.parent.c
+                c_old = (
+                    self.T[:, : coeff.ns[self.parent.depth_complete]] @ self.parent.c
+                )
                 self.calc_err(c_old)
                 self.calc_ndiv()
 
             for child in self.children:
                 if child.depth_complete is not None:
                     child.calc_ndiv()
                 if child.depth_complete == 0:
-                    c_old = child.T[:, : ns[self.depth_complete]] @ self.c
+                    c_old = child.T[:, : coeff.ns[self.depth_complete]] @ self.c
                     child.calc_err(c_old)
 
         if self.done_leaves is not None and not len(self.done_leaves):
             # This interval contributes to the integral estimate.
             self.done_leaves = {self}
 
             # Use this interval in the integral estimates of the ancestors
@@ -302,45 +307,45 @@
             ival = self.parent
             old_leaves = set()
             while ival is not None:
                 unused_children = [
                     child for child in ival.children if child.done_leaves is not None
                 ]
 
-                if not all(len(child.done_leaves) for child in unused_children):
+                if not all(len(child.done_leaves) for child in unused_children):  # type: ignore[arg-type]
                     break
 
                 if ival.done_leaves is None:
                     ival.done_leaves = set()
                 old_leaves.add(ival)
                 for child in ival.children:
                     if child.done_leaves is None:
                         continue
                     ival.done_leaves.update(child.done_leaves)
                     child.done_leaves = None
                 ival.done_leaves -= old_leaves
                 ival = ival.parent
 
-        remove = self.err < (abs(self.igral) * eps * Vcond[depth])
+        remove = self.err < (abs(self.igral) * coeff.eps * coeff.Vcond[depth])
 
         return force_split, remove
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         lst = [
             f"(a, b)=({self.a:.5f}, {self.b:.5f})",
             f"depth={self.depth}",
             f"rdepth={self.rdepth}",
             f"err={self.err:.5E}",
             "igral={:.5E}".format(self.igral if hasattr(self, "igral") else np.inf),
         ]
         return " ".join(lst)
 
 
 class IntegratorLearner(BaseLearner):
-    def __init__(self, function, bounds, tol):
+    def __init__(self, function: Callable, bounds: tuple[int, int], tol: float) -> None:
         """
         Parameters
         ----------
         function : callable: X → Y
             The function to learn.
         bounds : pair of reals
             The bounds of the interval on which to learn 'function'.
@@ -366,42 +371,49 @@
         Methods
         -------
         done : bool
             Returns whether the `tol` has been reached.
         plot : hv.Scatter
             Plots all the points that are evaluated.
         """
-        self.function = function
+        self.function = function  # type: ignore
         self.bounds = bounds
         self.tol = tol
         self.max_ivals = 1000
-        self.priority_split = []
-        self.done_points = {}
+        self.priority_split: list[_Interval] = []
+        self.data = {}
         self.pending_points = set()
-        self._stack = []
-        self.x_mapping = defaultdict(lambda: SortedSet([], key=attrgetter("rdepth")))
-        self.ivals = set()
+        self._stack: list[float] = []
+        self.x_mapping: dict[float, SortedSet] = defaultdict(
+            lambda: SortedSet([], key=attrgetter("rdepth"))
+        )
+        self.ivals: set[_Interval] = set()
         ival = _Interval.make_first(*self.bounds)
         self.add_ival(ival)
         self.first_ival = ival
 
+    def new(self) -> IntegratorLearner:
+        """Create a copy of `~adaptive.Learner2D` without the data."""
+        return IntegratorLearner(self.function, self.bounds, self.tol)
+
     @property
-    def approximating_intervals(self):
+    def approximating_intervals(self) -> set[_Interval]:
+        assert self.first_ival.done_leaves is not None
         return self.first_ival.done_leaves
 
-    def tell(self, point, value):
+    def tell(self, point: float, value: float) -> None:
         if point not in self.x_mapping:
             raise ValueError(f"Point {point} doesn't belong to any interval")
-        self.done_points[point] = value
+        self.data[point] = value
         self.pending_points.discard(point)
 
         # Select the intervals that have this point
         ivals = self.x_mapping[point]
         for ival in ivals:
-            ival.done_points[point] = value
+            ival.data[point] = value
 
             if ival.depth_complete is None:
                 from_depth = 0 if ival.parent is not None else 2
             else:
                 from_depth = ival.depth_complete + 1
 
             for depth in range(from_depth, ival.depth + 1):
@@ -420,71 +432,71 @@
                         # If it already has children it has already been split
                         assert ival in self.ivals
                         self.priority_split.append(ival)
 
     def tell_pending(self):
         pass
 
-    def propagate_removed(self, ival):
+    def propagate_removed(self, ival: _Interval) -> None:
         def _propagate_removed_down(ival):
             ival.removed = True
             self.ivals.discard(ival)
 
             for child in ival.children:
                 _propagate_removed_down(child)
 
         _propagate_removed_down(ival)
 
-    def add_ival(self, ival):
+    def add_ival(self, ival: _Interval) -> None:
         for x in ival.points():
             # Update the mappings
             self.x_mapping[x].add(ival)
-            if x in self.done_points:
-                self.tell(x, self.done_points[x])
+            if x in self.data:
+                self.tell(x, self.data[x])
             elif x not in self.pending_points:
                 self.pending_points.add(x)
                 self._stack.append(x)
         self.ivals.add(ival)
 
-    def ask(self, n, tell_pending=True):
+    def ask(self, n: int, tell_pending: bool = True) -> tuple[list[float], list[float]]:
         """Choose points for learners."""
         if not tell_pending:
             with restore(self):
                 return self._ask_and_tell_pending(n)
         else:
             return self._ask_and_tell_pending(n)
 
-    def _ask_and_tell_pending(self, n):
+    def _ask_and_tell_pending(self, n: int) -> tuple[list[float], list[float]]:
         points, loss_improvements = self.pop_from_stack(n)
         n_left = n - len(points)
         while n_left > 0:
             assert n_left >= 0
             try:
                 self._fill_stack()
             except ValueError:
-                raise RuntimeError("No way to improve the integral estimate.")
+                raise RuntimeError("No way to improve the integral estimate.") from None
             new_points, new_loss_improvements = self.pop_from_stack(n_left)
             points += new_points
             loss_improvements += new_loss_improvements
             n_left -= len(new_points)
 
         return points, loss_improvements
 
-    def pop_from_stack(self, n):
+    def pop_from_stack(self, n: int) -> tuple[list[float], list[float]]:
         points = self._stack[:n]
         self._stack = self._stack[n:]
         loss_improvements = [
             max(ival.err for ival in self.x_mapping[x]) for x in points
         ]
         return points, loss_improvements
 
     def remove_unfinished(self):
         pass
 
-    def _fill_stack(self):
+    def _fill_stack(self) -> list[float]:
         # XXX: to-do if all the ivals have err=inf, take the interval
         # with the lowest rdepth and no children.
         force_split = bool(self.priority_split)
         if force_split:
             ival = self.priority_split.pop()
         else:
             ival = max(self.ivals, key=lambda x: (x.err, x.a))
@@ -492,44 +504,44 @@
         assert not ival.children
 
         # If the interval points are smaller than machine precision, then
         # don't continue with splitting or refining.
         points = ival.points()
 
         if (
-            points[1] - points[0] < points[0] * min_sep
-            or points[-1] - points[-2] < points[-2] * min_sep
+            points[1] - points[0] < points[0] * coeff.min_sep
+            or points[-1] - points[-2] < points[-2] * coeff.min_sep
         ):
             self.ivals.remove(ival)
         elif ival.depth == 3 or force_split:
             # Always split when depth is maximal or if refining didn't help
             self.ivals.remove(ival)
-            for ival in ival.split():
-                self.add_ival(ival)
+            for iv in ival.split():
+                self.add_ival(iv)
         else:
             self.add_ival(ival.refine())
 
         # Remove the interval with the smallest error
         # if number of intervals is larger than max_ivals
         if len(self.ivals) > self.max_ivals:
             self.ivals.remove(min(self.ivals, key=lambda x: (x.err, x.a)))
 
         return self._stack
 
     @property
-    def npoints(self):
+    def npoints(self) -> int:  # type: ignore[override]
         """Number of evaluated points."""
-        return len(self.done_points)
+        return len(self.data)
 
     @property
-    def igral(self):
+    def igral(self) -> float:
         return sum(i.igral for i in self.approximating_intervals)
 
     @property
-    def err(self):
+    def err(self) -> float:
         if self.approximating_intervals:
             err = sum(i.err for i in self.approximating_intervals)
             if err > sys.float_info.max:
                 err = np.inf
         else:
             err = np.inf
         return err
@@ -548,43 +560,134 @@
     @cache_latest
     def loss(self, real=True):
         return abs(abs(self.igral) * self.tol - self.err)
 
     def plot(self):
         hv = ensure_holoviews()
         ivals = sorted(self.ivals, key=attrgetter("a"))
-        if not self.done_points:
+        if not self.data:
             return hv.Path([])
-        xs, ys = zip(
-            *[(x, y) for ival in ivals for x, y in sorted(ival.done_points.items())]
-        )
+        xs, ys = zip(*[(x, y) for ival in ivals for x, y in sorted(ival.data.items())])
         return hv.Path((xs, ys))
 
+    def to_numpy(self):
+        """Data as NumPy array of size (npoints, 2)."""
+        return np.array(sorted(self.data.items()))
+
+    def to_dataframe(  # type: ignore[override]
+        self,
+        with_default_function_args: bool = True,
+        function_prefix: str = "function.",
+        x_name: str = "x",
+        y_name: str = "y",
+    ) -> pandas.DataFrame:
+        """Return the data as a `pandas.DataFrame`.
+
+        Parameters
+        ----------
+        with_default_function_args : bool, optional
+            Include the ``learner.function``'s default arguments as a
+            column, by default True
+        function_prefix : str, optional
+            Prefix to the ``learner.function``'s default arguments' names,
+            by default "function."
+        x_name : str, optional
+            Name of the input value, by default "x"
+        y_name : str, optional
+            Name of the output value, by default "y"
+
+        Returns
+        -------
+        pandas.DataFrame
+
+        Raises
+        ------
+        ImportError
+            If `pandas` is not installed.
+        """
+        if not with_pandas:
+            raise ImportError("pandas is not installed.")
+        df = pandas.DataFrame(sorted(self.data.items()), columns=[x_name, y_name])
+        df.attrs["inputs"] = [x_name]
+        df.attrs["output"] = y_name
+        if with_default_function_args:
+            assign_defaults(self.function, df, function_prefix)
+        return df
+
+    def load_dataframe(  # type: ignore[override]
+        self,
+        df: pandas.DataFrame,
+        with_default_function_args: bool = True,
+        function_prefix: str = "function.",
+        x_name: str = "x",
+        y_name: str = "y",
+    ) -> None:
+        """Load data from a `pandas.DataFrame`.
+
+        If ``with_default_function_args`` is True, then ``learner.function``'s
+        default arguments are set (using `functools.partial`) from the values
+        in the `pandas.DataFrame`.
+
+        Parameters
+        ----------
+        with_default_function_args : bool, optional
+            Include the ``learner.function``'s default arguments as a
+            column, by default True
+        function_prefix : str, optional
+            Prefix to the ``learner.function``'s default arguments' names,
+            by default "function."
+        x_name : str, optional
+            Name of the input value, by default "x"
+        y_name : str, optional
+            Name of the output value, by default "y"
+        """
+        raise NotImplementedError
+
     def _get_data(self):
         # Change the defaultdict of SortedSets to a normal dict of sets.
         x_mapping = {k: set(v) for k, v in self.x_mapping.items()}
 
         return (
             self.priority_split,
-            self.done_points,
+            self.data,
             self.pending_points,
             self._stack,
             x_mapping,
             self.ivals,
             self.first_ival,
         )
 
     def _set_data(self, data):
-        self.priority_split, self.done_points, self.pending_points, self._stack, x_mapping, self.ivals, self.first_ival = (
-            data
-        )
+        (
+            self.priority_split,
+            self.data,
+            self.pending_points,
+            self._stack,
+            x_mapping,
+            self.ivals,
+            self.first_ival,
+        ) = data
 
         # Add the pending_points to the _stack such that they are evaluated again
         for x in self.pending_points:
             if x not in self._stack:
                 self._stack.append(x)
 
         # x_mapping is a data structure that can't easily be saved
         # so we recreate it here
         self.x_mapping = defaultdict(lambda: SortedSet([], key=attrgetter("rdepth")))
         for k, _set in x_mapping.items():
             self.x_mapping[k].update(_set)
+
+    def __getstate__(self):
+        return (
+            cloudpickle.dumps(self.function),
+            self.bounds,
+            self.tol,
+            self._get_data(),
+        )
+
+    def __setstate__(self, state):
+        function, bounds, tol, data = state
+        function = cloudpickle.loads(function)
+        self.__init__(function, bounds, tol)
+        self._set_data(data)
```

### Comparing `adaptive-0.9.0/adaptive/learner/learner2D.py` & `adaptive-1.0.0/adaptive/learner/learner2D.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,66 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
 import itertools
+import warnings
 from collections import OrderedDict
+from collections.abc import Iterable
 from copy import copy
 from math import sqrt
+from typing import Callable
 
+import cloudpickle
 import numpy as np
 from scipy import interpolate
+from scipy.interpolate.interpnd import LinearNDInterpolator
 
 from adaptive.learner.base_learner import BaseLearner
+from adaptive.learner.triangulation import simplex_volume_in_embedding
 from adaptive.notebook_integration import ensure_holoviews
-from adaptive.utils import cache_latest
+from adaptive.types import Bool, Float, Real
+from adaptive.utils import (
+    assign_defaults,
+    cache_latest,
+    partial_function_from_dataframe,
+)
+
+try:
+    import pandas
+
+    with_pandas = True
+
+except ModuleNotFoundError:
+    with_pandas = False
 
 # Learner2D and helper functions.
 
 
-def deviations(ip):
+def deviations(ip: LinearNDInterpolator) -> list[np.ndarray]:
     """Returns the deviation of the linear estimate.
 
     Is useful when defining custom loss functions.
 
     Parameters
     ----------
     ip : `scipy.interpolate.LinearNDInterpolator` instance
 
     Returns
     -------
-    numpy array
+    deviations : list
         The deviation per triangle.
     """
     values = ip.values / (ip.values.ptp(axis=0).max() or 1)
     gradients = interpolate.interpnd.estimate_gradients_2d_global(
         ip.tri, values, tol=1e-6
     )
 
-    p = ip.tri.points[ip.tri.vertices]
-    vs = values[ip.tri.vertices]
-    gs = gradients[ip.tri.vertices]
+    simplices = ip.tri.simplices
+    p = ip.tri.points[simplices]
+    vs = values[simplices]
+    gs = gradients[simplices]
 
     def deviation(p, v, g):
         dev = 0
         for j in range(3):
             vest = v[:, j, None] + (
                 (p[:, :, :] - p[:, j, None, :]) * g[:, j, None, :]
             ).sum(axis=-1)
@@ -48,114 +68,137 @@
         return dev
 
     n_levels = vs.shape[2]
     devs = [deviation(p, vs[:, :, i], gs[:, :, i]) for i in range(n_levels)]
     return devs
 
 
-def areas(ip):
+def areas(ip: LinearNDInterpolator) -> np.ndarray:
     """Returns the area per triangle of the triangulation inside
     a `LinearNDInterpolator` instance.
 
     Is useful when defining custom loss functions.
 
     Parameters
     ----------
     ip : `scipy.interpolate.LinearNDInterpolator` instance
 
     Returns
     -------
-    numpy array
+    areas : numpy.ndarray
         The area per triangle in ``ip.tri``.
     """
-    p = ip.tri.points[ip.tri.vertices]
+    p = ip.tri.points[ip.tri.simplices]
     q = p[:, :-1, :] - p[:, -1, None, :]
     areas = abs(q[:, 0, 0] * q[:, 1, 1] - q[:, 0, 1] * q[:, 1, 0]) / 2
     return areas
 
 
-def uniform_loss(ip):
+def uniform_loss(ip: LinearNDInterpolator) -> np.ndarray:
     """Loss function that samples the domain uniformly.
 
     Works with `~adaptive.Learner2D` only.
 
+    Parameters
+    ----------
+    ip : `scipy.interpolate.LinearNDInterpolator` instance
+
+    Returns
+    -------
+    losses : numpy.ndarray
+        Loss per triangle in ``ip.tri``.
+
     Examples
     --------
     >>> from adaptive.learner.learner2D import uniform_loss
     >>> def f(xy):
     ...     x, y = xy
     ...     return x**2 + y**2
     >>>
-    >>> learner = adaptive.Learner2D(f,
-    ...                              bounds=[(-1, -1), (1, 1)],
-    ...                              loss_per_triangle=uniform_loss)
+    >>> learner = adaptive.Learner2D(
+    ...     f,
+    ...     bounds=[(-1, -1), (1, 1)],
+    ...     loss_per_triangle=uniform_loss,
+    ... )
     >>>
     """
     return np.sqrt(areas(ip))
 
 
-def resolution_loss_function(min_distance=0, max_distance=1):
+def resolution_loss_function(
+    min_distance: float = 0, max_distance: float = 1
+) -> Callable[[LinearNDInterpolator], np.ndarray]:
     """Loss function that is similar to the `default_loss` function, but you
     can set the maximimum and minimum size of a triangle.
 
     Works with `~adaptive.Learner2D` only.
 
     The arguments `min_distance` and `max_distance` should be in between 0 and 1
     because the total area is normalized to 1.
 
+    Returns
+    -------
+    loss_function : callable
+
     Examples
     --------
     >>> def f(xy):
     ...     x, y = xy
     ...     return x**2 + y**2
     >>>
     >>> loss = resolution_loss_function(min_distance=0.01, max_distance=1)
-    >>> learner = adaptive.Learner2D(f,
-    ...                              bounds=[(-1, -1), (1, 1)],
-    ...                              loss_per_triangle=loss)
-    >>>
+    >>> learner = adaptive.Learner2D(f, bounds=[(-1, -1), (1, 1)], loss_per_triangle=loss)
     """
 
     def resolution_loss(ip):
         loss = default_loss(ip)
 
         A = areas(ip)
         # Setting areas with a small area to zero such that they won't be chosen again
-        loss[A < min_distance ** 2] = 0
+        loss[A < min_distance**2] = 0
 
         # Setting triangles that have a size larger than max_distance to infinite loss
         # such that these triangles will be picked
-        loss[A > max_distance ** 2] = np.inf
+        loss[A > max_distance**2] = np.inf
 
         return loss
 
     return resolution_loss
 
 
-def minimize_triangle_surface_loss(ip):
-    """Loss function that is similar to the default loss function in the
+def minimize_triangle_surface_loss(ip: LinearNDInterpolator) -> np.ndarray:
+    """Loss function that is similar to the distance loss function in the
     `~adaptive.Learner1D`. The loss is the area spanned by the 3D
     vectors of the vertices.
 
     Works with `~adaptive.Learner2D` only.
 
+    Parameters
+    ----------
+    ip : `scipy.interpolate.LinearNDInterpolator` instance
+
+    Returns
+    -------
+    losses : numpy.ndarray
+        Loss per triangle in ``ip.tri``.
+
     Examples
     --------
     >>> from adaptive.learner.learner2D import minimize_triangle_surface_loss
     >>> def f(xy):
     ...     x, y = xy
     ...     return x**2 + y**2
     >>>
     >>> learner = adaptive.Learner2D(f, bounds=[(-1, -1), (1, 1)],
     ...     loss_per_triangle=minimize_triangle_surface_loss)
     >>>
     """
     tri = ip.tri
-    points = tri.points[tri.vertices]
-    values = ip.values[tri.vertices]
+    points = tri.points[tri.simplices]
+    values = ip.values[tri.simplices]
     values = values / (ip.values.ptp(axis=0).max() or 1)
 
     def _get_vectors(points):
         delta = points - points[:, -1, :][:, None, :]
         vectors = delta[:, :2, :]
         return vectors[:, 0, :], vectors[:, 1, :]
 
@@ -164,41 +207,54 @@
 
     a = np.hstack([a_xy, a_z])
     b = np.hstack([b_xy, b_z])
 
     return np.linalg.norm(np.cross(a, b) / 2, axis=1)
 
 
-def default_loss(ip):
+def default_loss(ip: LinearNDInterpolator) -> np.ndarray:
+    """Loss function that combines `deviations` and `areas` of the triangles.
+
+    Works with `~adaptive.Learner2D` only.
+
+    Parameters
+    ----------
+    ip : `scipy.interpolate.LinearNDInterpolator` instance
+
+    Returns
+    -------
+    losses : numpy.ndarray
+        Loss per triangle in ``ip.tri``.
+    """
     dev = np.sum(deviations(ip), axis=0)
     A = areas(ip)
     losses = dev * np.sqrt(A) + 0.3 * A
     return losses
 
 
-def choose_point_in_triangle(triangle, max_badness):
+def choose_point_in_triangle(triangle: np.ndarray, max_badness: int) -> np.ndarray:
     """Choose a new point in inside a triangle.
 
     If the ratio of the longest edge of the triangle squared
     over the area is bigger than the `max_badness` the new point
     is chosen on the middle of the longest edge. Otherwise
     a point in the center of the triangle is chosen. The badness
     is 1 for a equilateral triangle.
 
     Parameters
     ----------
-    triangle : numpy array
-        The coordinates of a triangle with shape (3, 2)
+    triangle : numpy.ndarray
+        The coordinates of a triangle with shape (3, 2).
     max_badness : int
         The badness at which the point is either chosen on a edge or
         in the middle.
 
     Returns
     -------
-    point : numpy array
+    point : numpy.ndarray
         The x and y coordinate of the suggested new point.
     """
     a, b, c = triangle
     area = 0.5 * np.cross(b - a, c - a)
     triangle_roll = np.roll(triangle, 1, axis=0)
     edge_lengths = np.linalg.norm(triangle - triangle_roll, axis=1)
     i = edge_lengths.argmax()
@@ -208,14 +264,53 @@
     if badness > max_badness:
         point = (triangle_roll[i] + triangle[i]) / 2
     else:
         point = triangle.mean(axis=0)
     return point
 
 
+def triangle_loss(ip):
+    r"""Computes the average of the volumes of the simplex combined with each
+    neighbouring point.
+
+    Parameters
+    ----------
+    ip : `scipy.interpolate.LinearNDInterpolator` instance
+
+    Returns
+    -------
+    triangle_loss : list
+        The mean volume per triangle.
+
+    Notes
+    -----
+    This loss function is *extremely* slow. It is here because it gives the
+    same result as the `adaptive.LearnerND`\s
+    `~adaptive.learner.learnerND.triangle_loss`.
+    """
+    tri = ip.tri
+
+    def get_neighbors(i, ip):
+        n = np.array([tri.simplices[n] for n in tri.neighbors[i] if n != -1])
+        # remove the vertices that are in the simplex
+        c = np.setdiff1d(n.reshape(-1), tri.simplices[i])
+        return np.concatenate((tri.points[c], ip.values[c]), axis=-1)
+
+    simplices = np.concatenate(
+        [tri.points[tri.simplices], ip.values[tri.simplices]], axis=-1
+    )
+    neighbors = [get_neighbors(i, ip) for i in range(len(tri.simplices))]
+
+    return [
+        sum(simplex_volume_in_embedding(np.vstack([simplex, n])) for n in neighbors[i])
+        / len(neighbors[i])
+        for i, simplex in enumerate(simplices)
+    ]
+
+
 class Learner2D(BaseLearner):
     """Learns and predicts a function 'f: ℝ^2 → ℝ^N'.
 
     Parameters
     ----------
     function : callable
         The function to learn. Must take a tuple of two real
@@ -226,15 +321,14 @@
     loss_per_triangle : callable, optional
         A function that returns the loss for every triangle.
         If not provided, then a default is used, which uses
         the deviation from a linear estimate, as well as
         triangle area, to determine the loss. See the notes
         for more details.
 
-
     Attributes
     ----------
     data : dict
         Sampled points and values.
     pending_points : set
         Points that still have to be evaluated and are currently
         interpolated, see `data_combined`.
@@ -244,20 +338,14 @@
     aspect_ratio : float, int, default: 1
         Average ratio of ``x`` span over ``y`` span of a triangle. If
         there is more detail in either ``x`` or ``y`` the ``aspect_ratio``
         needs to be adjusted. When ``aspect_ratio > 1`` the
         triangles will be stretched along ``x``, otherwise
         along ``y``.
 
-    Methods
-    -------
-    data_combined : dict
-        Sampled points and values so far including
-        the unknown interpolated points in `pending_points`.
-
     Notes
     -----
     Adapted from an initial implementation by Pauli Virtanen.
 
     The sample points are chosen by estimating the point where the
     linear and cubic interpolants based on the existing points have
     maximal disagreement. This point is then taken as the next point
@@ -278,57 +366,160 @@
     These can be used to compute the loss. The functions
     `~adaptive.learner.learner2D.areas` and
     `~adaptive.learner.learner2D.deviations` to calculate the
     areas and deviations from a linear interpolation
     over each triangle.
     """
 
-    def __init__(self, function, bounds, loss_per_triangle=None):
+    def __init__(
+        self,
+        function: Callable,
+        bounds: tuple[tuple[Real, Real], tuple[Real, Real]],
+        loss_per_triangle: Callable | None = None,
+    ) -> None:
         self.ndim = len(bounds)
-        self._vdim = None
+        self._vdim: int | None = None
         self.loss_per_triangle = loss_per_triangle or default_loss
-        self.bounds = tuple((float(a), float(b)) for a, b in bounds)
+        self.bounds = (
+            (float(bounds[0][0]), float(bounds[0][1])),
+            (float(bounds[1][0]), float(bounds[1][1])),
+        )
         self.data = OrderedDict()
         self._stack = OrderedDict()
         self.pending_points = set()
 
         self.xy_mean = np.mean(self.bounds, axis=1)
         self._xy_scale = np.ptp(self.bounds, axis=1)
         self.aspect_ratio = 1
 
         self._bounds_points = list(itertools.product(*bounds))
         self._stack.update({p: np.inf for p in self._bounds_points})
-        self.function = function
+        self.function = function  # type: ignore
         self._ip = self._ip_combined = None
 
         self.stack_size = 10
 
+    def new(self) -> Learner2D:
+        return Learner2D(self.function, self.bounds, self.loss_per_triangle)
+
     @property
-    def xy_scale(self):
+    def xy_scale(self) -> np.ndarray:
         xy_scale = self._xy_scale
         if self.aspect_ratio == 1:
             return xy_scale
         else:
             return np.array([xy_scale[0], xy_scale[1] / self.aspect_ratio])
 
-    def _scale(self, points):
+    def to_numpy(self):
+        """Data as NumPy array of size ``(npoints, 3)`` if ``learner.function`` returns a scalar
+        and ``(npoints, 2+vdim)`` if ``learner.function`` returns a vector of length ``vdim``.
+        """
+        return np.array(
+            [(x, y, *np.atleast_1d(z)) for (x, y), z in sorted(self.data.items())]
+        )
+
+    def to_dataframe(  # type: ignore[override]
+        self,
+        with_default_function_args: bool = True,
+        function_prefix: str = "function.",
+        x_name: str = "x",
+        y_name: str = "y",
+        z_name: str = "z",
+    ) -> pandas.DataFrame:
+        """Return the data as a `pandas.DataFrame`.
+
+        Parameters
+        ----------
+        with_default_function_args : bool, optional
+            Include the ``learner.function``'s default arguments as a
+            column, by default True
+        function_prefix : str, optional
+            Prefix to the ``learner.function``'s default arguments' names,
+            by default "function."
+        seed_name : str, optional
+            Name of the seed parameter, by default "seed"
+        x_name : str, optional
+            Name of the input x value, by default "x"
+        y_name : str, optional
+            Name of the input y value, by default "y"
+        z_name : str, optional
+            Name of the output value, by default "z"
+
+        Returns
+        -------
+        pandas.DataFrame
+
+        Raises
+        ------
+        ImportError
+            If `pandas` is not installed.
+        """
+        if not with_pandas:
+            raise ImportError("pandas is not installed.")
+        data = sorted((x, y, z) for (x, y), z in self.data.items())
+        df = pandas.DataFrame(data, columns=[x_name, y_name, z_name])
+        df.attrs["inputs"] = [x_name, y_name]
+        df.attrs["output"] = z_name
+        if with_default_function_args:
+            assign_defaults(self.function, df, function_prefix)
+        return df
+
+    def load_dataframe(  # type: ignore[override]
+        self,
+        df: pandas.DataFrame,
+        with_default_function_args: bool = True,
+        function_prefix: str = "function.",
+        x_name: str = "x",
+        y_name: str = "y",
+        z_name: str = "z",
+    ):
+        """Load data from a `pandas.DataFrame`.
+
+        If ``with_default_function_args`` is True, then ``learner.function``'s
+        default arguments are set (using `functools.partial`) from the values
+        in the `pandas.DataFrame`.
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            The data to load.
+        with_default_function_args : bool, optional
+            The ``with_default_function_args`` used in ``to_dataframe()``,
+            by default True
+        function_prefix : str, optional
+            The ``function_prefix`` used in ``to_dataframe``, by default "function."
+        x_name : str, optional
+            The ``x_name`` used in ``to_dataframe``, by default "x"
+        y_name : str, optional
+            The ``y_name`` used in ``to_dataframe``, by default "y"
+        z_name : str, optional
+            The ``z_name`` used in ``to_dataframe``, by default "z"
+        """
+        data = df.set_index([x_name, y_name])[z_name].to_dict()
+        self._set_data(data)
+        if with_default_function_args:
+            self.function = partial_function_from_dataframe(
+                self.function, df, function_prefix
+            )
+
+    def _scale(self, points: list[tuple[float, float]] | np.ndarray) -> np.ndarray:
         points = np.asarray(points, dtype=float)
         return (points - self.xy_mean) / self.xy_scale
 
-    def _unscale(self, points):
+    def _unscale(self, points: np.ndarray) -> np.ndarray:
         points = np.asarray(points, dtype=float)
         return points * self.xy_scale + self.xy_mean
 
     @property
-    def npoints(self):
+    def npoints(self) -> int:  # type: ignore[override]
         """Number of evaluated points."""
         return len(self.data)
 
     @property
-    def vdim(self):
+    def vdim(self) -> int:
         """Length of the output of ``learner.function``.
         If the output is unsized (when it's a scalar)
         then `vdim = 1`.
 
         As long as no data is known `vdim = 1`.
         """
         if self._vdim is None and self.data:
@@ -336,117 +527,179 @@
                 value = next(iter(self.data.values()))
                 self._vdim = len(value)
             except TypeError:
                 self._vdim = 1
         return self._vdim or 1
 
     @property
-    def bounds_are_done(self):
+    def bounds_are_done(self) -> bool:
         return not any(
             (p in self.pending_points or p in self._stack) for p in self._bounds_points
         )
 
-    def _data_in_bounds(self):
+    def interpolated_on_grid(
+        self, n: int | None = None
+    ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """Get the interpolated data on a grid.
+
+        Parameters
+        ----------
+        n : int, optional
+            Number of points in x and y. If None (default) this number is
+            evaluated by looking at the size of the smallest triangle.
+
+        Returns
+        -------
+        xs : 1D numpy.ndarray
+        ys : 1D numpy.ndarray
+        interpolated_on_grid : 2D numpy.ndarray
+        """
+        ip = self.interpolator(scaled=True)
+        if n is None:
+            # Calculate how many grid points are needed.
+            # factor from A=√3/4 * a² (equilateral triangle)
+            n = int(0.658 / sqrt(areas(ip).min()))
+            n = max(n, 10)
+
+        # The bounds of the linspace should be (-0.5, 0.5) but because of
+        # numerical precision problems it could (for example) be
+        # (-0.5000000000000001, 0.49999999999999983), then any point at exact
+        # boundary would be outside of the domain. See #181.
+        eps = 1e-13
+        xs = ys = np.linspace(-0.5 + eps, 0.5 - eps, n)
+        zs = ip(xs[:, None], ys[None, :] * self.aspect_ratio).squeeze()
+        xs, ys = self._unscale(np.vstack([xs, ys]).T).T
+        return xs, ys, zs
+
+    def _data_in_bounds(self) -> tuple[np.ndarray, np.ndarray]:
         if self.data:
             points = np.array(list(self.data.keys()))
             values = np.array(list(self.data.values()), dtype=float)
             ll, ur = np.reshape(self.bounds, (2, 2)).T
             inds = np.all(np.logical_and(ll <= points, points <= ur), axis=1)
             return points[inds], values[inds].reshape(-1, self.vdim)
         return np.zeros((0, 2)), np.zeros((0, self.vdim), dtype=float)
 
-    def _data_interp(self):
+    def _data_interp(self) -> tuple[np.ndarray | list[tuple[float, float]], np.ndarray]:
         if self.pending_points:
             points = list(self.pending_points)
             if self.bounds_are_done:
-                values = self.ip()(self._scale(points))
+                ip = self.interpolator(scaled=True)
+                values = ip(self._scale(points))
             else:
                 # Without the bounds the interpolation cannot be done properly,
                 # so we just set everything to zero.
                 values = np.zeros((len(points), self.vdim))
             return points, values
         return np.zeros((0, 2)), np.zeros((0, self.vdim), dtype=float)
 
-    def _data_combined(self):
+    def _data_combined(self) -> tuple[np.ndarray, np.ndarray]:
         points, values = self._data_in_bounds()
         if not self.pending_points:
             return points, values
         points_interp, values_interp = self._data_interp()
         points_combined = np.vstack([points, points_interp])
         values_combined = np.vstack([values, values_interp])
         return points_combined, values_combined
 
-    def data_combined(self):
-        """Like `data`, however this includes the points in
-        `pending_points` for which the values are interpolated."""
-        # Interpolate the unfinished points
-        points, values = self._data_combined()
-        return {tuple(k): v for k, v in zip(points, values)}
+    def ip(self) -> LinearNDInterpolator:
+        """Deprecated, use `self.interpolator(scaled=True)`"""
+        warnings.warn(
+            "`learner.ip()` is deprecated, use `learner.interpolator(scaled=True)`."
+            " This will be removed in v1.0.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.interpolator(scaled=True)
 
-    def ip(self):
+    def interpolator(self, *, scaled: bool = False) -> LinearNDInterpolator:
         """A `scipy.interpolate.LinearNDInterpolator` instance
-        containing the learner's data."""
-        if self._ip is None:
+        containing the learner's data.
+
+        Parameters
+        ----------
+        scaled : bool
+            Use True if all points are inside the
+            unit-square [(-0.5, 0.5), (-0.5, 0.5)] or False if
+            the data points are inside the ``learner.bounds``.
+
+        Returns
+        -------
+        interpolator : `scipy.interpolate.LinearNDInterpolator`
+
+        Examples
+        --------
+        >>> xs, ys = [np.linspace(*b, num=100) for b in learner.bounds]
+        >>> ip = learner.interpolator()
+        >>> zs = ip(xs[:, None], ys[None, :])
+        """
+        if scaled:
+            if self._ip is None:
+                points, values = self._data_in_bounds()
+                points = self._scale(points)
+                self._ip = interpolate.LinearNDInterpolator(points, values)
+            return self._ip
+        else:
             points, values = self._data_in_bounds()
-            points = self._scale(points)
-            self._ip = interpolate.LinearNDInterpolator(points, values)
-        return self._ip
+            return interpolate.LinearNDInterpolator(points, values)
 
-    def ip_combined(self):
+    def _interpolator_combined(self) -> LinearNDInterpolator:
         """A `scipy.interpolate.LinearNDInterpolator` instance
         containing the learner's data *and* interpolated data of
         the `pending_points`."""
         if self._ip_combined is None:
             points, values = self._data_combined()
             points = self._scale(points)
             self._ip_combined = interpolate.LinearNDInterpolator(points, values)
         return self._ip_combined
 
-    def inside_bounds(self, xy):
+    def inside_bounds(self, xy: tuple[float, float]) -> Bool:
         x, y = xy
         (xmin, xmax), (ymin, ymax) = self.bounds
         return xmin <= x <= xmax and ymin <= y <= ymax
 
-    def tell(self, point, value):
-        point = tuple(point)
+    def tell(self, point: tuple[float, float], value: float | Iterable[float]) -> None:
+        point = tuple(point)  # type: ignore[assignment]
         self.data[point] = value
         if not self.inside_bounds(point):
             return
         self.pending_points.discard(point)
         self._ip = None
         self._stack.pop(point, None)
 
-    def tell_pending(self, point):
-        point = tuple(point)
+    def tell_pending(self, point: tuple[float, float]) -> None:
+        point = tuple(point)  # type: ignore[assignment]
         if not self.inside_bounds(point):
             return
         self.pending_points.add(point)
         self._ip_combined = None
         self._stack.pop(point, None)
 
-    def _fill_stack(self, stack_till=1):
+    def _fill_stack(
+        self, stack_till: int = 1
+    ) -> tuple[list[tuple[float, float]], list[float]]:
         if len(self.data) + len(self.pending_points) < self.ndim + 1:
             raise ValueError("too few points...")
 
         # Interpolate
-        ip = self.ip_combined()
+        ip = self._interpolator_combined()
 
         losses = self.loss_per_triangle(ip)
 
         points_new = []
         losses_new = []
-        for j, _ in enumerate(losses):
+        for _j, _ in enumerate(losses):
             jsimplex = np.argmax(losses)
-            triangle = ip.tri.points[ip.tri.vertices[jsimplex]]
+            triangle = ip.tri.points[ip.tri.simplices[jsimplex]]
             point_new = choose_point_in_triangle(triangle, max_badness=5)
             point_new = tuple(self._unscale(point_new))
 
             # np.clip results in numerical precision problems
             # https://github.com/python-adaptive/adaptive/issues/7
-            clip = lambda x, l, u: max(l, min(u, x))  # noqa: E731
+            clip = lambda x, lo, up: max(lo, min(up, x))  # noqa: E731
             point_new = (
                 clip(point_new[0], *self.bounds[0]),
                 clip(point_new[1], *self.bounds[1]),
             )
 
             loss_new = losses[jsimplex]
 
@@ -458,15 +711,17 @@
             if len(self._stack) >= stack_till:
                 break
             else:
                 losses[jsimplex] = -np.inf
 
         return points_new, losses_new
 
-    def ask(self, n, tell_pending=True):
+    def ask(
+        self, n: int, tell_pending: bool = True
+    ) -> tuple[list[tuple[float, float] | np.ndarray], list[float]]:
         # Even if tell_pending is False we add the point such that _fill_stack
         # will return new points, later we remove these points if needed.
         points = list(self._stack.keys())
         loss_improvements = list(self._stack.values())
         n_left = n - len(points)
         for p in points[:n]:
             self.tell_pending(p)
@@ -489,22 +744,22 @@
             self._stack = OrderedDict(zip(points[: self.stack_size], loss_improvements))
             for point in points[:n]:
                 self.pending_points.discard(point)
 
         return points[:n], loss_improvements[:n]
 
     @cache_latest
-    def loss(self, real=True):
+    def loss(self, real: bool = True) -> float:
         if not self.bounds_are_done:
             return np.inf
-        ip = self.ip() if real else self.ip_combined()
+        ip = self.interpolator(scaled=True) if real else self._interpolator_combined()
         losses = self.loss_per_triangle(ip)
         return losses.max()
 
-    def remove_unfinished(self):
+    def remove_unfinished(self) -> None:
         self.pending_points = set()
         for p in self._bounds_points:
             if p not in self.data:
                 self._stack[p] = np.inf
 
     def plot(self, n=None, tri_alpha=0):
         r"""Plot the Learner2D's current state.
@@ -537,62 +792,62 @@
         vector *cannot* be used with the live_plotting functionality.
         """
         hv = ensure_holoviews()
         x, y = self.bounds
         lbrt = x[0], y[0], x[1], y[1]
 
         if len(self.data) >= 4:
-            ip = self.ip()
-
-            if n is None:
-                # Calculate how many grid points are needed.
-                # factor from A=√3/4 * a² (equilateral triangle)
-                n = int(0.658 / sqrt(areas(ip).min()))
-                n = max(n, 10)
-
-            # The bounds of the linspace should be (-0.5, 0.5) but because of
-            # numerical precision problems it could (for example) be
-            # (-0.5000000000000001, 0.49999999999999983), then any point at exact
-            # boundary would be outside of the domain. See #181.
-            eps = 1e-13
-            x = y = np.linspace(-0.5 + eps, 0.5 - eps, n)
-            z = ip(x[:, None], y[None, :] * self.aspect_ratio).squeeze()
+            ip = self.interpolator(scaled=True)
+            x, y, z = self.interpolated_on_grid(n)
 
             if self.vdim > 1:
                 ims = {
                     i: hv.Image(np.rot90(z[:, :, i]), bounds=lbrt)
                     for i in range(z.shape[-1])
                 }
                 im = hv.HoloMap(ims)
             else:
                 im = hv.Image(np.rot90(z), bounds=lbrt)
 
             if tri_alpha:
-                points = self._unscale(ip.tri.points[ip.tri.vertices])
+                points = self._unscale(ip.tri.points[ip.tri.simplices])
                 points = np.pad(
                     points[:, [0, 1, 2, 0], :],
                     pad_width=((0, 0), (0, 1), (0, 0)),
                     mode="constant",
                     constant_values=np.nan,
                 ).reshape(-1, 2)
                 tris = hv.EdgePaths([points])
             else:
                 tris = hv.EdgePaths([])
         else:
             im = hv.Image([], bounds=lbrt)
             tris = hv.EdgePaths([])
+        return im.opts(cmap="viridis") * tris.opts(
+            line_width=0.5, alpha=tri_alpha, tools=[]
+        )
 
-        im_opts = dict(cmap="viridis")
-        tri_opts = dict(line_width=0.5, alpha=tri_alpha)
-        no_hover = dict(plot=dict(inspection_policy=None, tools=[]))
-
-        return im.opts(style=im_opts) * tris.opts(style=tri_opts, **no_hover)
-
-    def _get_data(self):
+    def _get_data(self) -> dict[tuple[float, float], Float | np.ndarray]:
         return self.data
 
-    def _set_data(self, data):
+    def _set_data(self, data: dict[tuple[float, float], Float | np.ndarray]) -> None:
         self.data = data
         # Remove points from stack if they already exist
         for point in copy(self._stack):
             if point in self.data:
                 self._stack.pop(point)
+
+    def __getstate__(self):
+        return (
+            cloudpickle.dumps(self.function),
+            self.bounds,
+            self.loss_per_triangle,
+            self._stack,
+            self._get_data(),
+        )
+
+    def __setstate__(self, state):
+        function, bounds, loss_per_triangle, _stack, data = state
+        function = cloudpickle.loads(function)
+        self.__init__(function, bounds, loss_per_triangle)
+        self._set_data(data)
+        self._stack = _stack
```

### Comparing `adaptive-0.9.0/adaptive/learner/learnerND.py` & `adaptive-1.0.0/adaptive/learner/learnerND.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
 import functools
 import itertools
 import random
 from collections import OrderedDict
 from collections.abc import Iterable
+from copy import deepcopy
 
 import numpy as np
 import scipy.spatial
 from scipy import interpolate
 from sortedcontainers import SortedKeyList
 
 from adaptive.learner.base_learner import BaseLearner, uses_nth_neighbors
@@ -16,15 +17,28 @@
     Triangulation,
     circumsphere,
     fast_det,
     point_in_simplex,
     simplex_volume_in_embedding,
 )
 from adaptive.notebook_integration import ensure_holoviews, ensure_plotly
-from adaptive.utils import cache_latest, restore
+from adaptive.utils import (
+    assign_defaults,
+    cache_latest,
+    partial_function_from_dataframe,
+    restore,
+)
+
+try:
+    import pandas
+
+    with_pandas = True
+
+except ModuleNotFoundError:
+    with_pandas = False
 
 
 def to_list(inp):
     if isinstance(inp, Iterable):
         return list(inp)
     return [inp]
 
@@ -129,15 +143,15 @@
         Each entry is one point of the simplex.
     values : list of values
         The scaled function values of each of the simplex points.
     value_scale : float
         The scale of values, where ``values = function_values * value_scale``.
     neighbors : list of tuples
         The neighboring points of the simplex, ordered such that simplex[0]
-        exacly opposes neighbors[0], etc.
+        exactly opposes neighbors[0], etc.
     neighbor_values : list of values
         The function values for each of the neighboring points.
 
     Returns
     -------
     loss : float
     """
@@ -167,15 +181,15 @@
             Each entry is one point of the simplex.
         values : list of values
             The scaled function values of each of the simplex points.
         value_scale : float
             The scale of values, where ``values = function_values * value_scale``.
         neighbors : list of tuples
             The neighboring points of the simplex, ordered such that simplex[0]
-            exacly opposes neighbors[0], etc.
+            exactly opposes neighbors[0], etc.
         neighbor_values : list of values
             The scaled function values for each of the neighboring points.
 
         Returns
         -------
         loss : float
         """
@@ -311,41 +325,43 @@
 
         self.data = OrderedDict()
         self.pending_points = set()
 
         self.bounds = bounds
         if isinstance(bounds, scipy.spatial.ConvexHull):
             hull_points = bounds.points[bounds.vertices]
-            self._bounds_points = sorted(list(map(tuple, hull_points)))
+            self._bounds_points = sorted(map(tuple, hull_points))
             self._bbox = tuple(zip(hull_points.min(axis=0), hull_points.max(axis=0)))
             self._interior = scipy.spatial.Delaunay(self._bounds_points)
         else:
-            self._bounds_points = sorted(list(map(tuple, itertools.product(*bounds))))
+            self._bounds_points = sorted(map(tuple, itertools.product(*bounds)))
             self._bbox = tuple(tuple(map(float, b)) for b in bounds)
+            self._interior = None
 
         self.ndim = len(self._bbox)
 
         self.function = func
         self._tri = None
-        self._losses = dict()
+        self._losses = {}
 
-        self._pending_to_simplex = dict()  # vertex → simplex
+        self._pending_to_simplex = {}  # vertex → simplex
 
         # triangulation of the pending points inside a specific simplex
-        self._subtriangulations = dict()  # simplex → triangulation
+        self._subtriangulations = {}  # simplex → triangulation
 
         # scale to unit hypercube
         # for the input
         self._transform = np.linalg.inv(np.diag(np.diff(self._bbox).flat))
         # for the output
         self._min_value = None
         self._max_value = None
+        self._old_scale = None
         self._output_multiplier = (
-            1
-        )  # If we do not know anything, do not scale the values
+            1  # If we do not know anything, do not scale the values
+        )
         self._recompute_losses_factor = 1.1
 
         # create a private random number generator with fixed seed
         self._random = random.Random(1)
 
         # all real triangles that have not been subdivided and the pending
         # triangles heap of tuples (-loss, real simplex, sub_simplex or None)
@@ -356,14 +372,18 @@
         # _simplex_queue may contain simplices that have been deleted, this is
         #  because deleting those items from the heap is an expensive operation,
         # so when popping an item, you should check that the simplex that has
         # been returned has not been deleted. This checking is done by
         # _pop_highest_existing_simplex
         self._simplex_queue = SortedKeyList(key=_simplex_evaluation_priority)
 
+    def new(self) -> LearnerND:
+        """Create a new learner with the same function and bounds."""
+        return LearnerND(self.function, self.bounds, self.loss_per_simplex)
+
     @property
     def npoints(self):
         """Number of evaluated points."""
         return len(self.data)
 
     @property
     def vdim(self):
@@ -377,14 +397,101 @@
             try:
                 value = next(iter(self.data.values()))
                 self._vdim = len(value)
             except TypeError:
                 self._vdim = 1
         return self._vdim if self._vdim is not None else 1
 
+    def to_numpy(self):
+        """Data as NumPy array of size ``(npoints, dim+vdim)``, where ``dim`` is the
+        size of the input dimension and ``vdim`` is the length of the return value
+        of ``learner.function``."""
+        return np.array([(*p, *np.atleast_1d(v)) for p, v in sorted(self.data.items())])
+
+    def to_dataframe(  # type: ignore[override]
+        self,
+        with_default_function_args: bool = True,
+        function_prefix: str = "function.",
+        point_names: tuple[str, ...] = ("x", "y", "z"),
+        value_name: str = "value",
+    ) -> pandas.DataFrame:
+        """Return the data as a `pandas.DataFrame`.
+
+        Parameters
+        ----------
+        with_default_function_args : bool, optional
+            Include the ``learner.function``'s default arguments as a
+            column, by default True
+        function_prefix : str, optional
+            Prefix to the ``learner.function``'s default arguments' names,
+            by default "function."
+        point_names : tuple[str, ...], optional
+            Names of the input points, should be the same length as number
+            of input parameters by default ("x", "y", "z" )
+        value_name : str, optional
+            Name of the output value, by default "value"
+
+        Returns
+        -------
+        pandas.DataFrame
+
+        Raises
+        ------
+        ImportError
+            If `pandas` is not installed.
+        """
+        if not with_pandas:
+            raise ImportError("pandas is not installed.")
+        if len(point_names) != self.ndim:
+            raise ValueError(
+                f"point_names ({point_names}) should have the"
+                f" same length as learner.ndims ({self.ndim})"
+            )
+        data = [(*x, y) for x, y in self.data.items()]
+        df = pandas.DataFrame(data, columns=[*point_names, value_name])
+        df.attrs["inputs"] = list(point_names)
+        df.attrs["output"] = value_name
+        if with_default_function_args:
+            assign_defaults(self.function, df, function_prefix)
+        return df
+
+    def load_dataframe(  # type: ignore[override]
+        self,
+        df: pandas.DataFrame,
+        with_default_function_args: bool = True,
+        function_prefix: str = "function.",
+        point_names: tuple[str, ...] = ("x", "y", "z"),
+        value_name: str = "value",
+    ):
+        """Load data from a `pandas.DataFrame`.
+
+        If ``with_default_function_args`` is True, then ``learner.function``'s
+        default arguments are set (using `functools.partial`) from the values
+        in the `pandas.DataFrame`.
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            The data to load.
+        with_default_function_args : bool, optional
+            The ``with_default_function_args`` used in ``to_dataframe()``,
+            by default True
+        function_prefix : str, optional
+            The ``function_prefix`` used in ``to_dataframe``, by default "function."
+        point_names : str, optional
+            The ``point_names`` used in ``to_dataframe``, by default ("x", "y", "z")
+        value_name : str, optional
+            The ``value_name`` used in ``to_dataframe``, by default "value"
+        """
+        self.tell_many(df[list(point_names)].values, df[value_name].values)
+        if with_default_function_args:
+            self.function = partial_function_from_dataframe(
+                self.function, df, function_prefix
+            )
+
     @property
     def bounds_are_done(self):
         return all(p in self.data for p in self._bounds_points)
 
     def _ip(self):
         """A `scipy.interpolate.LinearNDInterpolator` instance
         containing the learner's data."""
@@ -445,15 +552,15 @@
 
     def _simplex_exists(self, simplex):
         simplex = tuple(sorted(simplex))
         return simplex in self.tri.simplices
 
     def inside_bounds(self, point):
         """Check whether a point is inside the bounds."""
-        if hasattr(self, "_interior"):
+        if self._interior is not None:
             return self._interior.find_simplex(point, tol=1e-8) >= 0
         else:
             eps = 1e-8
             return all(
                 (mn - eps) <= p <= (mx + eps) for p, (mn, mx) in zip(point, self._bbox)
             )
 
@@ -754,22 +861,22 @@
             self._recompute_all_losses()
             return True
         return False
 
     @cache_latest
     def loss(self, real=True):
         # XXX: compute pending loss if real == False
-        losses = self._losses if self.tri is not None else dict()
+        losses = self._losses if self.tri is not None else {}
         return max(losses.values()) if losses else float("inf")
 
     def remove_unfinished(self):
         # XXX: implement this method
         self.pending_points = set()
-        self._subtriangulations = dict()
-        self._pending_to_simplex = dict()
+        self._subtriangulations = {}
+        self._pending_to_simplex = {}
 
     ##########################
     # Plotting related stuff #
     ##########################
 
     def plot(self, n=None, tri_alpha=0):
         """Plot the function we want to learn, only works in 2D.
@@ -821,20 +928,17 @@
                 ).reshape(-1, 2)
                 tris = hv.EdgePaths([points])
             else:
                 tris = hv.EdgePaths([])
         else:
             im = hv.Image([], bounds=lbrt)
             tris = hv.EdgePaths([])
-
-        im_opts = dict(cmap="viridis")
-        tri_opts = dict(line_width=0.5, alpha=tri_alpha)
-        no_hover = dict(plot=dict(inspection_policy=None, tools=[]))
-
-        return im.opts(style=im_opts) * tris.opts(style=tri_opts, **no_hover)
+        return im.opts(cmap="viridis") * tris.opts(
+            line_width=0.5, alpha=tri_alpha, tools=[]
+        )
 
     def plot_slice(self, cut_mapping, n=None):
         """Plot a 1D or 2D interpolated slice of a N-dimensional function.
 
         Parameters
         ----------
         cut_mapping : dict (int → float)
@@ -847,35 +951,35 @@
         hv = ensure_holoviews()
         plot_dim = self.ndim - len(cut_mapping)
         if plot_dim == 1:
             if not self.data:
                 return hv.Scatter([]) * hv.Path([])
             elif self.vdim > 1:
                 raise NotImplementedError(
-                    "multidimensional output not yet" " supported by `plot_slice`"
+                    "multidimensional output not yet supported by `plot_slice`"
                 )
             n = n or 201
             values = [
                 cut_mapping.get(i, np.linspace(*self._bbox[i], n))
                 for i in range(self.ndim)
             ]
             ind = next(i for i in range(self.ndim) if i not in cut_mapping)
             x = values[ind]
             y = self._ip()(*values)
             p = hv.Path((x, y))
 
             # Plot with 5% margins such that the boundary points are visible
             margin = 0.05 / self._transform[ind, ind]
             plot_bounds = (x.min() - margin, x.max() + margin)
-            return p.redim(x=dict(range=plot_bounds))
+            return p.redim(x={"range": plot_bounds})
 
         elif plot_dim == 2:
             if self.vdim > 1:
                 raise NotImplementedError(
-                    "holoviews currently does not support" " 3D surface plots in bokeh."
+                    "holoviews currently does not support 3D surface plots in bokeh."
                 )
             if n is None:
                 # Calculate how many grid points are needed.
                 # factor from A=√3/4 * a² (equilateral triangle)
                 scale_factor = np.product(np.diag(self._transform))
                 a_sq = np.sqrt(np.min(self.tri.volumes()) * scale_factor)
                 n = max(10, int(0.658 / a_sq))
@@ -894,28 +998,31 @@
 
             if len(self.data) >= 4:
                 z = self._ip()(*values).squeeze()
                 im = hv.Image(np.rot90(z), bounds=lbrt)
             else:
                 im = hv.Image([], bounds=lbrt)
 
-            return im.opts(style=dict(cmap="viridis"))
+            return im.opts(cmap="viridis")
         else:
             raise ValueError("Only 1 or 2-dimensional plots can be generated.")
 
-    def plot_3D(self, with_triangulation=False):
+    def plot_3D(self, with_triangulation=False, return_fig=False):
         """Plot the learner's data in 3D using plotly.
 
         Does *not* work with the
         `adaptive.notebook_integration.live_plot` functionality.
 
         Parameters
         ----------
         with_triangulation : bool, default: False
             Add the verticices to the plot.
+        return_fig : bool, default: False
+            Return the `plotly.graph_objs.Figure` object instead of showing
+            the rendered plot (default).
 
         Returns
         -------
         plot : `plotly.offline.iplot` object
             The 3D plot of ``learner.data``.
         """
         plotly = ensure_plotly()
@@ -933,89 +1040,82 @@
 
             plots.append(
                 plotly.graph_objs.Scatter3d(
                     x=Xe,
                     y=Ye,
                     z=Ze,
                     mode="lines",
-                    line=dict(color="rgb(125,125,125)", width=1),
+                    line={"color": "rgb(125,125,125)", "width": 1},
                     hoverinfo="none",
                 )
             )
 
         Xn, Yn, Zn = zip(*vertices)
         colors = [self.data[p] for p in self.tri.vertices]
-        marker = dict(
-            symbol="circle",
-            size=3,
-            color=colors,
-            colorscale="Viridis",
-            line=dict(color="rgb(50,50,50)", width=0.5),
-        )
+        marker = {
+            "symbol": "circle",
+            "size": 3,
+            "color": colors,
+            "colorscale": "Viridis",
+            "line": {"color": "rgb(50,50,50)", "width": 0.5},
+        }
 
         plots.append(
             plotly.graph_objs.Scatter3d(
                 x=Xn,
                 y=Yn,
                 z=Zn,
                 mode="markers",
                 name="actors",
                 marker=marker,
                 hoverinfo="text",
             )
         )
 
-        axis = dict(
-            showbackground=False,
-            showline=False,
-            zeroline=False,
-            showgrid=False,
-            showticklabels=False,
-            title="",
-        )
+        axis = {
+            "showbackground": False,
+            "showline": False,
+            "zeroline": False,
+            "showgrid": False,
+            "showticklabels": False,
+            "title": "",
+        }
 
         layout = plotly.graph_objs.Layout(
             showlegend=False,
-            scene=dict(xaxis=axis, yaxis=axis, zaxis=axis),
-            margin=dict(t=100),
+            scene={"xaxis": axis, "yaxis": axis, "zaxis": axis},
+            margin={"t": 100},
             hovermode="closest",
         )
 
         fig = plotly.graph_objs.Figure(data=plots, layout=layout)
 
-        return plotly.offline.iplot(fig)
-
-    def _get_data(self):
-        return self.data
-
-    def _set_data(self, data):
-        if data:
-            self.tell_many(*zip(*data.items()))
+        return fig if return_fig else plotly.offline.iplot(fig)
 
     def _get_iso(self, level=0.0, which="surface"):
         if which == "surface":
             if self.ndim != 3 or self.vdim != 1:
                 raise Exception(
                     "Isosurface plotting is only supported"
                     " for a 3D input and 1D output"
                 )
             get_surface = True
             get_line = False
         elif which == "line":
             if self.ndim != 2 or self.vdim != 1:
                 raise Exception(
-                    "Isoline plotting is only supported" " for a 2D input and 1D output"
+                    "Isoline plotting is only supported for a 2D input and 1D output"
                 )
             get_surface = False
             get_line = True
 
         vertices = []  # index -> (x,y,z)
         faces_or_lines = []  # tuple of indices of the corner points
 
-        @functools.lru_cache()
+        @functools.lru_cache
         def _get_vertex_index(a, b):
             vertex_a = self.tri.vertices[a]
             vertex_b = self.tri.vertices[b]
             value_a = self.data[vertex_a]
             value_b = self.data[vertex_b]
 
             da = abs(value_a - level)
@@ -1086,24 +1186,21 @@
         hv = ensure_holoviews()
         if n == -1:
             plot = hv.Path([])
         else:
             plot = self.plot(n=n, tri_alpha=tri_alpha)
 
         if isinstance(level, Iterable):
-            for l in level:
-                plot = plot * self.plot_isoline(level=l, n=-1)
+            for lvl in level:
+                plot = plot * self.plot_isoline(level=lvl, n=-1)
             return plot
 
         vertices, lines = self._get_iso(level, which="line")
         paths = [[vertices[i], vertices[j]] for i, j in lines]
-        contour = hv.Path(paths)
-
-        contour_opts = dict(color="black")
-        contour = contour.opts(style=contour_opts)
+        contour = hv.Path(paths).opts(color="black")
         return plot * contour
 
     def plot_isosurface(self, level=0.0, hull_opacity=0.2):
         """Plots a linearly interpolated isosurface.
 
         This is the 3D analog of an isoline. Does *not* work with the
         `adaptive.notebook_integration.live_plot` functionality.
@@ -1126,15 +1223,21 @@
         x, y, z = zip(*vertices)
 
         fig = plotly.figure_factory.create_trisurf(
             x=x, y=y, z=z, plot_edges=False, simplices=faces, title="Isosurface"
         )
         isosurface = fig.data[0]
         isosurface.update(
-            lighting=dict(ambient=1, diffuse=1, roughness=1, specular=0, fresnel=0)
+            lighting={
+                "ambient": 1,
+                "diffuse": 1,
+                "roughness": 1,
+                "specular": 0,
+                "fresnel": 0,
+            }
         )
 
         if hull_opacity < 1e-3:
             # Do not compute the hull_mesh.
             return plotly.offline.iplot(fig)
 
         hull_mesh = self._get_hull_mesh(opacity=hull_opacity)
@@ -1162,19 +1265,32 @@
             color_dict[simplex] = tuple(random.randint(0, 255) for _ in range(3))
             return color_dict[simplex]
 
         colors = [_get_plane_color(simplex) for simplex in hull.simplices]
 
         x, y, z = zip(*self._bounds_points)
         i, j, k = hull.simplices.T
-        lighting = dict(ambient=1, diffuse=1, roughness=1, specular=0, fresnel=0)
+        lighting = {
+            "ambient": 1,
+            "diffuse": 1,
+            "roughness": 1,
+            "specular": 0,
+            "fresnel": 0,
+        }
         return plotly.graph_objs.Mesh3d(
             x=x,
             y=y,
             z=z,
             i=i,
             j=j,
             k=k,
             facecolor=colors,
             opacity=opacity,
             lighting=lighting,
         )
+
+    def _get_data(self):
+        return deepcopy(self.__dict__)
+
+    def _set_data(self, state):
+        for k, v in state.items():
+            setattr(self, k, v)
```

### Comparing `adaptive-0.9.0/adaptive/learner/triangulation.py` & `adaptive-1.0.0/adaptive/learner/triangulation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,48 @@
-import math
 from collections import Counter
 from collections.abc import Iterable, Sized
 from itertools import chain, combinations
-from math import factorial
+from math import factorial, sqrt
 
-import numpy as np
 import scipy.spatial
+from numpy import abs as np_abs
+from numpy import (
+    array,
+    asarray,
+    average,
+    concatenate,
+    dot,
+    eye,
+    mean,
+    ones,
+    square,
+    subtract,
+    zeros,
+)
+from numpy import sum as np_sum
+from numpy.linalg import det as ndet
+from numpy.linalg import matrix_rank, norm, slogdet, solve
 
 
 def fast_norm(v):
-    # notice this method can be even more optimised
-    if len(v) == 2:
-        return math.sqrt(v[0] * v[0] + v[1] * v[1])
-    if len(v) == 3:
-        return math.sqrt(v[0] * v[0] + v[1] * v[1] + v[2] * v[2])
-    return math.sqrt(np.dot(v, v))
+    """Take the vector norm for len 2, 3 vectors.
+    Defaults to a square root of the dot product for larger vectors.
+
+    Note that for large vectors, it is possible for integer overflow to occur.
+    For instance:
+    vec = [49024, 59454, 12599, -63721, 18517, 27961]
+    dot(vec, vec) = -1602973744
+
+    """
+    len_v = len(v)
+    if len_v == 2:
+        return sqrt(v[0] * v[0] + v[1] * v[1])
+    if len_v == 3:
+        return sqrt(v[0] * v[0] + v[1] * v[1] + v[2] * v[2])
+    return sqrt(dot(v, v))
 
 
 def fast_2d_point_in_simplex(point, simplex, eps=1e-8):
     (p0x, p0y), (p1x, p1y), (p2x, p2y) = simplex
     px, py = point
 
     area = 0.5 * (-p1y * p2x + p0y * (p2x - p1x) + p1x * p2y + p0x * (p1y - p2y))
@@ -31,17 +55,17 @@
     return (t >= -eps) and (s + t <= 1 + eps)
 
 
 def point_in_simplex(point, simplex, eps=1e-8):
     if len(point) == 2:
         return fast_2d_point_in_simplex(point, simplex, eps)
 
-    x0 = np.array(simplex[0], dtype=float)
-    vectors = np.array(simplex[1:], dtype=float) - x0
-    alpha = np.linalg.solve(vectors.T, point - x0)
+    x0 = array(simplex[0], dtype=float)
+    vectors = array(simplex[1:], dtype=float) - x0
+    alpha = solve(vectors.T, point - x0)
 
     return all(alpha > -eps) and sum(alpha) < 1 + eps
 
 
 def fast_2d_circumcircle(points):
     """Compute the center and radius of the circumscribed circle of a triangle
 
@@ -49,17 +73,17 @@
     ----------
     points: 2D array-like
         the points of the triangle to investigate
 
     Returns
     -------
     tuple
-        (center point : tuple(int), radius: int)
+        (center point : tuple(float), radius: float)
     """
-    points = np.array(points)
+    points = array(points)
     # transform to relative coordinates
     pts = points[1:] - points[0]
 
     (x1, y1), (x2, y2) = pts
     # compute the length squared
     l1 = x1 * x1 + y1 * y1
     l2 = x2 * x2 + y2 * y2
@@ -69,33 +93,33 @@
     dy = -l1 * x2 + l2 * x1
     aa = +x1 * y2 - x2 * y1
     a = 2 * aa
 
     # compute center
     x = dx / a
     y = dy / a
-    radius = math.sqrt(x * x + y * y)  # radius = norm([x, y])
+    radius = sqrt(x * x + y * y)  # radius = norm([x, y])
 
     return (x + points[0][0], y + points[0][1]), radius
 
 
 def fast_3d_circumcircle(points):
-    """Compute the center and radius of the circumscribed shpere of a simplex.
+    """Compute the center and radius of the circumscribed sphere of a simplex.
 
     Parameters
     ----------
     points: 2D array-like
         the points of the triangle to investigate
 
     Returns
     -------
     tuple
-        (center point : tuple(int), radius: int)
+        (center point : tuple(float), radius: float)
     """
-    points = np.array(points)
+    points = array(points)
     pts = points[1:] - points[0]
 
     (x1, y1, z1), (x2, y2, z2), (x3, y3, z3) = pts
 
     l1 = x1 * x1 + y1 * y1 + z1 * z1
     l2 = x2 * x2 + y2 * y2 + z2 * z2
     l3 = x3 * x3 + y3 * y3 + z3 * z3
@@ -115,46 +139,68 @@
         center[2] + points[0][2],
     )
 
     return center, radius
 
 
 def fast_det(matrix):
-    matrix = np.asarray(matrix, dtype=float)
+    matrix = asarray(matrix, dtype=float)
     if matrix.shape == (2, 2):
         return matrix[0][0] * matrix[1][1] - matrix[1][0] * matrix[0][1]
     elif matrix.shape == (3, 3):
         a, b, c, d, e, f, g, h, i = matrix.ravel()
         return a * (e * i - f * h) - b * (d * i - f * g) + c * (d * h - e * g)
     else:
-        return np.linalg.det(matrix)
+        return ndet(matrix)
 
 
 def circumsphere(pts):
+    """Compute the center and radius of a N dimension sphere which touches each point in pts.
+
+    Parameters
+    ----------
+    pts : array-like, of shape (N-dim + 1, N-dim)
+        The points for which we would like to compute a circumsphere.
+
+    Returns
+    -------
+    center : tuple of floats of size N-dim
+    radius : a positive float
+    A valid center and radius, if a circumsphere is possible, and no points are repeated.
+    If points are repeated, or a circumsphere is not possible, will return nans, and a
+    ZeroDivisionError may occur.
+    Will fail for matrices which are not (N-dim + 1, N-dim) in size due to non-square determinants:
+    will raise numpy.linalg.LinAlgError.
+    May fail for points that are integers (due to 32bit integer overflow).
+    """
+
     dim = len(pts) - 1
     if dim == 2:
         return fast_2d_circumcircle(pts)
     if dim == 3:
         return fast_3d_circumcircle(pts)
 
     # Modified method from http://mathworld.wolfram.com/Circumsphere.html
-    mat = [[np.sum(np.square(pt)), *pt, 1] for pt in pts]
-
-    center = []
+    mat = array([[np_sum(square(pt)), *pt, 1] for pt in pts])
+    center = zeros(dim)
+    a = 1 / (2 * ndet(mat[:, 1:]))
+    factor = a
+    # Use ind to index into the matrix columns
+    ind = ones((dim + 2,), bool)
     for i in range(1, len(pts)):
-        r = np.delete(mat, i, 1)
-        factor = (-1) ** (i + 1)
-        center.append(factor * fast_det(r))
-
-    a = fast_det(np.delete(mat, 0, 1))
-    center = [x / (2 * a) for x in center]
+        ind[i - 1] = True
+        ind[i] = False
+        center[i - 1] = factor * ndet(mat[:, ind])
+        factor *= -1
 
+    # Use subtract as we don't know the type of x0.
     x0 = pts[0]
-    vec = np.subtract(center, x0)
-    radius = fast_norm(vec)
+    vec = subtract(center, x0)
+    # Vector norm.
+    radius = sqrt(dot(vec, vec))
 
     return tuple(center), radius
 
 
 def orientation(face, origin):
     """Compute the orientation of the face with respect to a point, origin.
 
@@ -170,16 +216,16 @@
     -------
     0 if the origin lies in the same hyperplane as face,
     -1 or 1 to indicate left or right orientation
 
     If two points lie on the same side of the face, the orientation will
     be equal, if they lie on the other side of the face, it will be negated.
     """
-    vectors = np.array(face)
-    sign, logdet = np.linalg.slogdet(vectors - origin)
+    vectors = array(face)
+    sign, logdet = slogdet(vectors - origin)
     if logdet < -50:  # assume it to be zero when it's close to zero
         return 0
     return sign
 
 
 def is_iterable_and_sized(obj):
     return isinstance(obj, Iterable) and isinstance(obj, Sized)
@@ -194,53 +240,53 @@
 
     Parameters
     ----------
     vertices : 2D arraylike of floats
 
     Returns
     -------
-    volume : int
+    volume : float
         the volume of the simplex with given vertices.
 
     Raises
     ------
     ValueError
         if the vertices do not form a simplex (for example,
         because they are coplanar, colinear or coincident).
     """
     # Implements http://mathworld.wolfram.com/Cayley-MengerDeterminant.html
     # Modified from https://codereview.stackexchange.com/questions/77593/calculating-the-volume-of-a-tetrahedron
 
-    vertices = np.asarray(vertices, dtype=float)
+    vertices = asarray(vertices, dtype=float)
     dim = len(vertices[0])
     if dim == 2:
         # Heron's formula
         a, b, c = scipy.spatial.distance.pdist(vertices, metric="euclidean")
         s = 0.5 * (a + b + c)
-        return math.sqrt(s * (s - a) * (s - b) * (s - c))
+        return sqrt(s * (s - a) * (s - b) * (s - c))
 
     # β_ij = |v_i - v_k|²
     sq_dists = scipy.spatial.distance.pdist(vertices, metric="sqeuclidean")
 
     # Add border while compressed
     num_verts = scipy.spatial.distance.num_obs_y(sq_dists)
-    bordered = np.concatenate((np.ones(num_verts), sq_dists))
+    bordered = concatenate((ones(num_verts), sq_dists))
 
     # Make matrix and find volume
     sq_dists_mat = scipy.spatial.distance.squareform(bordered)
 
-    coeff = -(-2) ** (num_verts - 1) * factorial(num_verts - 1) ** 2
+    coeff = -((-2) ** (num_verts - 1)) * factorial(num_verts - 1) ** 2
     vol_square = fast_det(sq_dists_mat) / coeff
 
     if vol_square < 0:
-        if abs(vol_square) < 1e-15:
+        if vol_square > -1e-15:
             return 0
         raise ValueError("Provided vertices do not form a simplex")
 
-    return np.sqrt(vol_square)
+    return sqrt(vol_square)
 
 
 class Triangulation:
     """A triangulation object.
 
     Parameters
     ----------
@@ -283,16 +329,16 @@
         if dim == 1:
             raise ValueError("Triangulation class only supports dim >= 2")
 
         if len(coords) < dim + 1:
             raise ValueError("Please provide at least one simplex")
 
         coords = list(map(tuple, coords))
-        vectors = np.subtract(coords[1:], coords[0])
-        if np.linalg.matrix_rank(vectors) < dim:
+        vectors = subtract(coords[1:], coords[0])
+        if matrix_rank(vectors) < dim:
             raise ValueError(
                 "Initial simplex has zero volumes "
                 "(the points are linearly dependent)"
             )
 
         self.vertices = list(coords)
         self.simplices = set()
@@ -334,17 +380,17 @@
             Indices of vertices of the simplex to which the vertex belongs.
             An empty list indicates that the vertex is outside the simplex.
         """
         # XXX: in the end we want to lose this method
         if len(simplex) != self.dim + 1:
             # We are checking whether point belongs to a face.
             simplex = self.containing(simplex).pop()
-        x0 = np.array(self.vertices[simplex[0]])
-        vectors = np.array(self.get_vertices(simplex[1:])) - x0
-        alpha = np.linalg.solve(vectors.T, point - x0)
+        x0 = array(self.vertices[simplex[0]])
+        vectors = array(self.get_vertices(simplex[1:])) - x0
+        alpha = solve(vectors.T, point - x0)
         if any(alpha < -eps) or sum(alpha) > 1 + eps:
             return []
 
         result = [i for i, a in enumerate(alpha, 1) if a > eps]
         if sum(alpha) < 1 - eps:
             result.insert(0, 0)
 
@@ -399,15 +445,15 @@
         multiplicities = Counter(face for face in self.faces())
         hull_faces = [face for face, count in multiplicities.items() if count == 1]
 
         # compute the center of the convex hull, this center lies in the hull
         # we do not really need the center, we only need a point that is
         # guaranteed to lie strictly within the hull
         hull_points = self.get_vertices(self.hull)
-        pt_center = np.average(hull_points, axis=0)
+        pt_center = average(hull_points, axis=0)
 
         pt_index = len(self.vertices)
         self.vertices.append(new_vertex)
 
         new_simplices = set()
         for face in hull_faces:
             # do orientation check, if orientation is the same, it lies on
@@ -443,29 +489,29 @@
             the simplex to investigate
 
         Returns
         -------
         tuple (center point, radius)
             The center and radius of the circumscribed circle
         """
-        pts = np.dot(self.get_vertices(simplex), transform)
+        pts = dot(self.get_vertices(simplex), transform)
         return circumsphere(pts)
 
     def point_in_cicumcircle(self, pt_index, simplex, transform):
         # return self.fast_point_in_circumcircle(pt_index, simplex, transform)
         eps = 1e-8
 
         center, radius = self.circumscribed_circle(simplex, transform)
-        pt = np.dot(self.get_vertices([pt_index]), transform)[0]
+        pt = dot(self.get_vertices([pt_index]), transform)[0]
 
-        return np.linalg.norm(center - pt) < (radius * (1 + eps))
+        return norm(center - pt) < (radius * (1 + eps))
 
     @property
     def default_transform(self):
-        return np.eye(self.dim)
+        return eye(self.dim)
 
     def bowyer_watson(self, pt_index, containing_simplex=None, transform=None):
         """Modified Bowyer-Watson point adding algorithm.
 
         Create a hole in the triangulation around the new point,
         then retriangulate this hole.
 
@@ -528,18 +574,18 @@
 
     def _relative_volume(self, simplex):
         """Compute the volume of a simplex divided by the average (Manhattan)
         distance of its vertices. The advantage of this is that the relative
         volume is only dependent on the shape of the simplex and not on the
         absolute size. Due to the weird scaling, the only use of this method
         is to check that a simplex is almost flat."""
-        vertices = np.array(self.get_vertices(simplex))
+        vertices = array(self.get_vertices(simplex))
         vectors = vertices[1:] - vertices[0]
-        average_edge_length = np.mean(np.abs(vectors))
-        return self.volume(simplex) / (average_edge_length ** self.dim)
+        average_edge_length = mean(np_abs(vectors))
+        return self.volume(simplex) / (average_edge_length**self.dim)
 
     def add_point(self, point, simplex=None, transform=None):
         """Add a new vertex and create simplices as appropriate.
 
         Parameters
         ----------
         point : float vector
@@ -583,16 +629,16 @@
             raise ValueError("Point already in triangulation.")
         else:
             pt_index = len(self.vertices)
             self.vertices.append(point)
             return self.bowyer_watson(pt_index, actual_simplex, transform)
 
     def volume(self, simplex):
-        prefactor = np.math.factorial(self.dim)
-        vertices = np.array(self.get_vertices(simplex))
+        prefactor = factorial(self.dim)
+        vertices = array(self.get_vertices(simplex))
         vectors = vertices[1:] - vertices[0]
         return float(abs(fast_det(vectors)) / prefactor)
 
     def volumes(self):
         return [self.volume(sim) for sim in self.simplices]
 
     def reference_invariant(self):
```

### Comparing `adaptive-0.9.0/adaptive/notebook_integration.py` & `adaptive-1.0.0/adaptive/notebook_integration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
 import asyncio
 import datetime
 import importlib
 import random
 import warnings
 from contextlib import suppress
@@ -29,70 +29,76 @@
         if not _holoviews_enabled:
             import holoviews
 
             holoviews.notebook_extension("bokeh", logo=False, inline=_inline_js)
             _holoviews_enabled = True
     except ModuleNotFoundError:
         warnings.warn(
-            "holoviews is not installed; plotting " "is disabled.", RuntimeWarning
+            "holoviews is not installed; plotting is disabled.",
+            RuntimeWarning,
+            stacklevel=2,
         )
 
     # Load ipywidgets
     try:
         if not _ipywidgets_enabled:
             import ipywidgets  # noqa: F401
 
             _ipywidgets_enabled = True
     except ModuleNotFoundError:
         warnings.warn(
-            "ipywidgets is not installed; live_info " "is disabled.", RuntimeWarning
+            "ipywidgets is not installed; live_info is disabled.",
+            RuntimeWarning,
+            stacklevel=2,
         )
 
     # Enable asyncio integration
     if not _async_enabled:
         get_ipython().magic("gui asyncio")  # noqa: F821
         _async_enabled = True
 
 
 def ensure_holoviews():
     try:
         return importlib.import_module("holoviews")
     except ModuleNotFoundError:
-        raise RuntimeError("holoviews is not installed; plotting is disabled.")
+        raise RuntimeError(
+            "holoviews is not installed; plotting is disabled."
+        ) from None
 
 
 def ensure_plotly():
     global _plotly_enabled
     try:
         import plotly
 
         if not _plotly_enabled:
-            import plotly.graph_objs
             import plotly.figure_factory
+            import plotly.graph_objs
             import plotly.offline
 
             # This injects javascript and should happen only once
             plotly.offline.init_notebook_mode()
             _plotly_enabled = True
         return plotly
-    except ModuleNotFoundError:
-        raise RuntimeError("plotly is not installed; plotting is disabled.")
+    except ModuleNotFoundError as e:
+        raise RuntimeError("plotly is not installed; plotting is disabled.") from e
 
 
-def in_ipynb():
+def in_ipynb() -> bool:
     try:
         # If we are running in IPython, then `get_ipython()` is always a global
-        return get_ipython().__class__.__name__ == "ZMQInteractiveShell"
+        return get_ipython().__class__.__name__ == "ZMQInteractiveShell"  # type: ignore[name-defined]
     except NameError:
         return False
 
 
 # Fancy displays in the Jupyter notebook
 
-active_plotting_tasks = dict()
+active_plotting_tasks: dict[str, asyncio.Task] = {}
 
 
 def live_plot(runner, *, plotter=None, update_interval=2, name=None, normalize=True):
     """Live plotting of the learner's data.
 
     Parameters
     ----------
@@ -157,15 +163,15 @@
         # see https://github.com/pyviz/holoviews/issues/3564
         try:
             while not runner.task.done():
                 event()
                 await asyncio.sleep(update_interval)
             event()  # fire off one last update before we die
         finally:
-            if active_plotting_tasks[name] is asyncio.Task.current_task():
+            if active_plotting_tasks[name] is asyncio.current_task():
                 active_plotting_tasks.pop(name, None)
             cancel_button.layout.display = "none"  # remove cancel button
 
     def cancel(_):
         with suppress(KeyError):
             active_plotting_tasks[name].cancel()
 
@@ -184,15 +190,15 @@
         # Make sure to only keep all the messages when the notebook
         # is viewed, this means 'buffer_size == 1'. However, when not
         # viewing the notebook the buffer fills up. When this happens
         # we decide to only add messages to it when a certain probability.
         # i.e. we're offline for 12h, with an update_interval of 0.5s,
         # and without the reduced probability, we have buffer_size=86400.
         # With the correction this is np.log(86400) / np.log(1.1) = 119.2
-        return 1.1 ** buffer_size * random.random() < 1
+        return 1.1**buffer_size * random.random() < 1
     except Exception:
         # We catch any Exception because we are using a private API.
         return True
 
 
 def live_info(runner, *, update_interval=0.5):
     """Display live information about the runner.
@@ -226,47 +232,54 @@
                 await asyncio.sleep(0.05)
 
         status.value = _info_html(runner)
         cancel.layout.display = "none"
 
     runner.ioloop.create_task(update())
 
-    display(
-        ipywidgets.HBox(
-            (status, cancel),
-            layout=ipywidgets.Layout(
-                border="solid 1px", width="200px", align_items="center"
-            ),
-        )
-    )
+    display(ipywidgets.VBox((status, cancel)))
+
+
+def _table_row(i, key, value):
+    """Style the rows of a table. Based on the default Jupyterlab table style."""
+    style = "text-align: right; padding: 0.5em 0.5em; line-height: 1.0;"
+    if i % 2 == 1:
+        style += " background: var(--md-grey-100);"
+    return f'<tr><th style="{style}">{key}</th><th style="{style}">{value}</th></tr>'
 
 
 def _info_html(runner):
     status = runner.status()
 
     color = {
         "cancelled": "orange",
         "failed": "red",
         "running": "blue",
         "finished": "green",
     }[status]
 
+    overhead = runner.overhead()
+    red_level = max(0, min(int(255 * overhead / 100), 255))
+    overhead_color = f"#{red_level:02x}{255 - red_level:02x}{0:02x}"
+
     info = [
         ("status", f'<font color="{color}">{status}</font>'),
         ("elapsed time", datetime.timedelta(seconds=runner.elapsed_time())),
-        ("overhead", f"{runner.overhead():.2f}%"),
+        ("overhead", f'<font color="{overhead_color}">{overhead:.2f}%</font>'),
     ]
 
     with suppress(Exception):
         info.append(("# of points", runner.learner.npoints))
 
     with suppress(Exception):
+        info.append(("# of samples", runner.learner.nsamples))
+
+    with suppress(Exception):
         info.append(("latest loss", f'{runner.learner._cache["loss"]:.3f}'))
 
-    template = '<dt class="ignore-css">{}</dt><dd>{}</dd>'
-    table = "\n".join(template.format(k, v) for k, v in info)
+    table = "\n".join(_table_row(i, k, v) for i, (k, v) in enumerate(info))
 
     return f"""
-        <dl>
+        <table>
         {table}
-        </dl>
+        </table>
     """
```

### Comparing `adaptive-0.9.0/adaptive/runner.py` & `adaptive-1.0.0/adaptive/runner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,140 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
 import abc
 import asyncio
 import concurrent.futures as concurrent
+import functools
 import inspect
-import os
+import itertools
+import pickle
+import platform
 import sys
 import time
 import traceback
 import warnings
 from contextlib import suppress
-
+from datetime import datetime, timedelta
+from importlib.util import find_spec
+from typing import TYPE_CHECKING, Any, Callable, Literal, Optional, Union
+
+import loky
+
+from adaptive import (
+    BalancingLearner,
+    DataSaver,
+    IntegratorLearner,
+    SequenceLearner,
+)
+from adaptive.learner.base_learner import LearnerType
 from adaptive.notebook_integration import in_ipynb, live_info, live_plot
+from adaptive.utils import SequentialExecutor
 
-try:
-    import ipyparallel
+ExecutorTypes: TypeAlias = Union[
+    concurrent.ProcessPoolExecutor,
+    concurrent.ThreadPoolExecutor,
+    SequentialExecutor,
+    loky.reusable_executor._ReusablePoolExecutor,
+]
+FutureTypes: TypeAlias = Union[concurrent.Future, asyncio.Future, asyncio.Task]
 
-    with_ipyparallel = True
-except ModuleNotFoundError:
-    with_ipyparallel = False
-
-try:
-    import distributed
-
-    with_distributed = True
-except ModuleNotFoundError:
-    with_distributed = False
-
-try:
-    import mpi4py.futures
-
-    with_mpi4py = True
-except ModuleNotFoundError:
-    with_mpi4py = False
+if TYPE_CHECKING:
+    import holoviews
 
-with suppress(ModuleNotFoundError):
-    import uvloop
 
-    asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+if sys.version_info >= (3, 10):
+    from typing import TypeAlias
+else:
+    from typing_extensions import TypeAlias
+
+
+with_ipyparallel = find_spec("ipyparallel") is not None
+with_distributed = find_spec("distributed") is not None
+with_mpi4py = find_spec("mpi4py") is not None
 
+if TYPE_CHECKING:
+    ExecutorTypes = Optional[()]
+    FutureTypes = Optional[()]
 
-if os.name == "nt":
     if with_distributed:
-        _default_executor = distributed.Client
-        _default_executor_kwargs = {"address": distributed.LocalCluster()}
-    else:
-        _windows_executor_msg = (
-            "The default executor on Windows for 'adaptive.Runner' cannot "
-            "be used because the package 'distributed' is not installed. "
-            "Either install 'distributed' or explicitly specify an executor "
-            "when using 'adaptive.Runner'."
-        )
+        import distributed
 
-        _default_executor_kwargs = {}
+        ExecutorTypes = Optional[
+            Union[
+                ExecutorTypes, distributed.Client, distributed.cfexecutor.ClientExecutor
+            ]
+        ]
+
+    if with_mpi4py:
+        import mpi4py.futures
+
+        ExecutorTypes = Optional[Union[ExecutorTypes, mpi4py.futures.MPIPoolExecutor]]
+
+    if with_ipyparallel:
+        import ipyparallel
+        from ipyparallel.client.asyncresult import AsyncResult
+
+        ExecutorTypes = Optional[
+            Union[
+                ExecutorTypes, ipyparallel.Client, ipyparallel.client.view.ViewExecutor
+            ]
+        ]
+        FutureTypes = Optional[Union[FutureTypes, AsyncResult]]
 
-        def _default_executor(*args, **kwargs):
-            raise RuntimeError(_windows_executor_msg)
+with suppress(ModuleNotFoundError):
+    import uvloop
+
+    asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
-        warnings.warn(_windows_executor_msg)
 
+# -- Runner definitions
+if platform.system() == "Linux":
+    _default_executor = concurrent.ProcessPoolExecutor  # type: ignore[misc]
 else:
-    _default_executor = concurrent.ProcessPoolExecutor
-    _default_executor_kwargs = {}
+    # On Windows and MacOS functions, the __main__ module must be
+    # importable by worker subprocesses. This means that
+    # ProcessPoolExecutor will not work in the interactive interpreter.
+    # On Linux the whole process is forked, so the issue does not appear.
+    # See https://docs.python.org/3/library/concurrent.futures.html#processpoolexecutor
+    # and https://github.com/python-adaptive/adaptive/issues/301
+    _default_executor = loky.get_reusable_executor  # type: ignore[misc]
 
 
 class BaseRunner(metaclass=abc.ABCMeta):
-    r"""Base class for runners that use `concurrent.futures.Executors`.
+    r"""Base class for runners that use `concurrent.futures.Executor`\'s.
 
     Parameters
     ----------
     learner : `~adaptive.BaseLearner` instance
-    goal : callable
+    goal : callable, optional
         The end condition for the calculation. This function must take
         the learner as its sole argument, and return True when we should
         stop requesting more points.
+    loss_goal : float, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the loss is smaller than this value.
+    npoints_goal : int, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the number of points is larger or
+        equal than this value.
+    end_time_goal : datetime, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the current time is larger or equal than this
+        value.
+    duration_goal : timedelta or number, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the current time is larger or equal than
+        ``start_time + duration_goal``. ``duration_goal`` can be a number
+        indicating the number of seconds.
     executor : `concurrent.futures.Executor`, `distributed.Client`,\
-               `mpi4py.futures.MPIPoolExecutor`, or `ipyparallel.Client`, optional
+               `mpi4py.futures.MPIPoolExecutor`, `ipyparallel.Client` or\
+               `loky.get_reusable_executor`, optional
         The executor in which to evaluate the function to be learned.
-        If not provided, a new `~concurrent.futures.ProcessPoolExecutor`
-        is used on Unix systems while on Windows a `distributed.Client`
-        is used if `distributed` is installed.
+        If not provided, a new `~concurrent.futures.ProcessPoolExecutor` on
+        Linux, and a `loky.get_reusable_executor` on MacOS and Windows.
     ntasks : int, optional
         The number of concurrent function evaluations. Defaults to the number
         of cores available in `executor`.
     log : bool, default: False
         If True, record the method calls made to the learner by this runner.
     shutdown_executor : bool, default: False
         If True, shutdown the executor when the runner has completed. If
@@ -91,104 +142,130 @@
         by the runner is shut down, regardless of this parameter.
     retries : int, default: 0
         Maximum amount of retries of a certain point ``x`` in
         ``learner.function(x)``. After `retries` is reached for ``x``
         the point is present in ``runner.failed``.
     raise_if_retries_exceeded : bool, default: True
         Raise the error after a point ``x`` failed `retries`.
+    allow_running_forever : bool, default: False
+        Allow the runner to run forever when the goal is None.
 
     Attributes
     ----------
     learner : `~adaptive.BaseLearner` instance
         The underlying learner. May be queried for its state.
     log : list or None
         Record of the method calls made to the learner, in the format
         ``(method_name, *args)``.
-    to_retry : dict
-        Mapping of ``{point: n_fails, ...}``. When a point has failed
+    to_retry : list of tuples
+        List of ``(point, n_fails)``. When a point has failed
         ``runner.retries`` times it is removed but will be present
         in ``runner.tracebacks``.
-    tracebacks : dict
-        A mapping of point to the traceback if that point failed.
-    pending_points : dict
-        A mapping of `~concurrent.futures.Future`\s to points.
+    tracebacks : list of tuples
+        List of of ``(point, tb)`` for points that failed.
+    pending_points : list of tuples
+        A list of tuples with ``(concurrent.futures.Future, point)``.
 
     Methods
     -------
     overhead : callable
         The overhead in percent of using Adaptive. Essentially, this is
         ``100 * (1 - total_elapsed_function_time / self.elapsed_time())``.
 
     """
 
     def __init__(
         self,
-        learner,
-        goal,
+        learner: LearnerType,
+        goal: Callable[[LearnerType], bool] | None = None,
         *,
-        executor=None,
-        ntasks=None,
-        log=False,
-        shutdown_executor=False,
-        retries=0,
-        raise_if_retries_exceeded=True,
+        loss_goal: float | None = None,
+        npoints_goal: int | None = None,
+        end_time_goal: datetime | None = None,
+        duration_goal: timedelta | int | float | None = None,
+        executor: ExecutorTypes | None = None,
+        ntasks: int | None = None,
+        log: bool = False,
+        shutdown_executor: bool = False,
+        retries: int = 0,
+        raise_if_retries_exceeded: bool = True,
+        allow_running_forever: bool = False,
     ):
-
         self.executor = _ensure_executor(executor)
-        self.goal = goal
+        self.goal = _goal(
+            learner,
+            goal,
+            loss_goal,
+            npoints_goal,
+            end_time_goal,
+            duration_goal,
+            allow_running_forever,
+        )
 
         self._max_tasks = ntasks
 
-        self.pending_points = {}
+        self._pending_tasks: dict[concurrent.Future, int] = {}
 
         # if we instantiate our own executor, then we are also responsible
         # for calling 'shutdown'
         self.shutdown_executor = shutdown_executor or (executor is None)
 
         self.learner = learner
-        self.log = [] if log else None
+        self.log: list | None = [] if log else None
 
         # Timing
         self.start_time = time.time()
-        self.end_time = None
+        self.end_time: float | None = None
         self._elapsed_function_time = 0
 
         # Error handling attributes
         self.retries = retries
         self.raise_if_retries_exceeded = raise_if_retries_exceeded
-        self.to_retry = {}
-        self.tracebacks = {}
+        self._to_retry: dict[int, int] = {}
+        self._tracebacks: dict[int, str] = {}
 
-    def _get_max_tasks(self):
+        self._id_to_point: dict[int, Any] = {}
+        self._next_id: Callable[[], int] = functools.partial(  # type: ignore[assignment]
+            next, itertools.count()
+        )  # some unique id to be associated with each point
+
+    def _get_max_tasks(self) -> int:
         return self._max_tasks or _get_ncores(self.executor)
 
-    def _do_raise(self, e, x):
-        tb = self.tracebacks[x]
+    def _do_raise(self, e: Exception, pid: int) -> None:
+        tb = self._tracebacks[pid]
+        x = self._id_to_point[pid]
         raise RuntimeError(
             "An error occured while evaluating "
             f'"learner.function({x})". '
             f"See the traceback for details.:\n\n{tb}"
         ) from e
 
     @property
-    def do_log(self):
+    def do_log(self) -> bool:
         return self.log is not None
 
-    def _ask(self, n):
-        points = [
-            p for p in self.to_retry.keys() if p not in self.pending_points.values()
-        ][:n]
-        loss_improvements = len(points) * [float("inf")]
-        if len(points) < n:
-            new_points, new_losses = self.learner.ask(n - len(points))
-            points += new_points
+    def _ask(self, n: int) -> tuple[list[int], list[float]]:
+        pending_ids = self._pending_tasks.values()
+        # using generator here because we only need until `n`
+        pids_gen = (pid for pid in self._to_retry.keys() if pid not in pending_ids)
+        pids = list(itertools.islice(pids_gen, n))
+
+        loss_improvements = len(pids) * [float("inf")]
+
+        if len(pids) < n:
+            new_points, new_losses = self.learner.ask(n - len(pids))
             loss_improvements += new_losses
-        return points, loss_improvements
+            for point in new_points:
+                pid = self._next_id()
+                self._id_to_point[pid] = point
+                pids.append(pid)
+        return pids, loss_improvements
 
-    def overhead(self):
+    def overhead(self) -> float:
         """Overhead of using Adaptive and the executor in percent.
 
         This is measured as ``100 * (1 - t_function / t_elapsed)``.
 
         Notes
         -----
         This includes the overhead of the executor that is being used.
@@ -203,109 +280,147 @@
         if t_function == 0:
             # When no function is done executing, the overhead cannot
             # reliably be determined, so 0 is the best we can do.
             return 0
         t_total = self.elapsed_time()
         return (1 - t_function / t_total) * 100
 
-    def _process_futures(self, done_futs):
+    def _process_futures(
+        self,
+        done_futs: set[FutureTypes],
+    ) -> None:
         for fut in done_futs:
-            x = self.pending_points.pop(fut)
+            pid = self._pending_tasks.pop(fut)
             try:
                 y = fut.result()
                 t = time.time() - fut.start_time  # total execution time
             except Exception as e:
-                self.tracebacks[x] = traceback.format_exc()
-                self.to_retry[x] = self.to_retry.get(x, 0) + 1
-                if self.to_retry[x] > self.retries:
-                    self.to_retry.pop(x)
+                self._tracebacks[pid] = traceback.format_exc()
+                self._to_retry[pid] = self._to_retry.get(pid, 0) + 1
+                if self._to_retry[pid] > self.retries:
+                    self._to_retry.pop(pid)
                     if self.raise_if_retries_exceeded:
-                        self._do_raise(e, x)
+                        self._do_raise(e, pid)
             else:
                 self._elapsed_function_time += t / self._get_max_tasks()
-                self.to_retry.pop(x, None)
-                self.tracebacks.pop(x, None)
+                self._to_retry.pop(pid, None)
+                self._tracebacks.pop(pid, None)
+                x = self._id_to_point.pop(pid)
                 if self.do_log:
-                    self.log.append(("tell", x, y))
+                    self.log.append(("tell", x, y))  # type: ignore[union-attr]
                 self.learner.tell(x, y)
 
-    def _get_futures(self):
+    def _get_futures(
+        self,
+    ) -> list[FutureTypes]:
         # Launch tasks to replace the ones that completed
         # on the last iteration, making sure to fill workers
         # that have started since the last iteration.
-        n_new_tasks = max(0, self._get_max_tasks() - len(self.pending_points))
+        n_new_tasks = max(0, self._get_max_tasks() - len(self._pending_tasks))
 
         if self.do_log:
-            self.log.append(("ask", n_new_tasks))
+            self.log.append(("ask", n_new_tasks))  # type: ignore[union-attr]
 
-        points, _ = self._ask(n_new_tasks)
+        pids, _ = self._ask(n_new_tasks)
 
-        for x in points:
+        for pid in pids:
             start_time = time.time()  # so we can measure execution time
-            fut = self._submit(x)
+            point = self._id_to_point[pid]
+            fut = self._submit(point)
             fut.start_time = start_time
-            self.pending_points[fut] = x
+            self._pending_tasks[fut] = pid
 
         # Collect and results and add them to the learner
-        futures = list(self.pending_points.keys())
+        futures = list(self._pending_tasks.keys())
         return futures
 
-    def _remove_unfinished(self):
+    def _remove_unfinished(self) -> list[FutureTypes]:
         # remove points with 'None' values from the learner
         self.learner.remove_unfinished()
         # cancel any outstanding tasks
-        remaining = list(self.pending_points.keys())
+        remaining = list(self._pending_tasks.keys())
         for fut in remaining:
             fut.cancel()
         return remaining
 
-    def _cleanup(self):
+    def _cleanup(self) -> None:
         if self.shutdown_executor:
-            # XXX: temporary set wait=True for Python 3.7
+            # XXX: temporary set wait=True because of a bug with Python ≥3.7
+            # and loky in any Python version.
             # see https://github.com/python-adaptive/adaptive/issues/156
             # and https://github.com/python-adaptive/adaptive/pull/164
-            self.executor.shutdown(wait=True if sys.version_info >= (3, 7) else False)
+            # and https://bugs.python.org/issue36281
+            # and https://github.com/joblib/loky/issues/241
+            self.executor.shutdown(wait=True)
         self.end_time = time.time()
 
     @property
-    def failed(self):
-        """Set of points that failed ``runner.retries`` times."""
-        return set(self.tracebacks) - set(self.to_retry)
+    def failed(self) -> set[int]:
+        """Set of points ids that failed ``runner.retries`` times."""
+        return set(self._tracebacks) - set(self._to_retry)
 
     @abc.abstractmethod
     def elapsed_time(self):
         """Return the total time elapsed since the runner
         was started.
 
         Is called in `overhead`.
         """
-        pass
 
     @abc.abstractmethod
     def _submit(self, x):
         """Is called in `_get_futures`."""
-        pass
+
+    @property
+    def tracebacks(self) -> list[tuple[int, str]]:
+        return [(self._id_to_point[pid], tb) for pid, tb in self._tracebacks.items()]
+
+    @property
+    def to_retry(self) -> list[tuple[int, int]]:
+        return [(self._id_to_point[pid], n) for pid, n in self._to_retry.items()]
+
+    @property
+    def pending_points(self) -> list[tuple[FutureTypes, Any]]:
+        return [
+            (fut, self._id_to_point[pid]) for fut, pid in self._pending_tasks.items()
+        ]
 
 
 class BlockingRunner(BaseRunner):
     """Run a learner synchronously in an executor.
 
     Parameters
     ----------
     learner : `~adaptive.BaseLearner` instance
-    goal : callable
+    goal : callable, optional
         The end condition for the calculation. This function must take
         the learner as its sole argument, and return True when we should
         stop requesting more points.
+    loss_goal : float, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the loss is smaller than this value.
+    npoints_goal : int, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the number of points is larger or
+        equal than this value.
+    end_time_goal : datetime, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the current time is larger or equal than this
+        value.
+    duration_goal : timedelta or number, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the current time is larger or equal than
+        ``start_time + duration_goal``. ``duration_goal`` can be a number
+        indicating the number of seconds.
     executor : `concurrent.futures.Executor`, `distributed.Client`,\
-               `mpi4py.futures.MPIPoolExecutor`, or `ipyparallel.Client`, optional
+               `mpi4py.futures.MPIPoolExecutor`, `ipyparallel.Client` or\
+               `loky.get_reusable_executor`, optional
         The executor in which to evaluate the function to be learned.
-        If not provided, a new `~concurrent.futures.ProcessPoolExecutor`
-        is used on Unix systems while on Windows a `distributed.Client`
-        is used if `distributed` is installed.
+        If not provided, a new `~concurrent.futures.ProcessPoolExecutor` on
+        Linux, and a `loky.get_reusable_executor` on MacOS and Windows.
     ntasks : int, optional
         The number of concurrent function evaluations. Defaults to the number
         of cores available in `executor`.
     log : bool, default: False
         If True, record the method calls made to the learner by this runner.
     shutdown_executor : bool, default: False
         If True, shutdown the executor when the runner has completed. If
@@ -321,22 +436,22 @@
     Attributes
     ----------
     learner : `~adaptive.BaseLearner` instance
         The underlying learner. May be queried for its state.
     log : list or None
         Record of the method calls made to the learner, in the format
         ``(method_name, *args)``.
-    to_retry : dict
-        Mapping of ``{point: n_fails, ...}``. When a point has failed
+    to_retry : list of tuples
+        List of ``(point, n_fails)``. When a point has failed
         ``runner.retries`` times it is removed but will be present
         in ``runner.tracebacks``.
-    tracebacks : dict
-        A mapping of point to the traceback if that point failed.
-    pending_points : dict
-        A mapping of `~concurrent.futures.Future`\to points.
+    tracebacks : list of tuples
+        List of of ``(point, tb)`` for points that failed.
+    pending_points : list of tuples
+        A list of tuples with ``(concurrent.futures.Future, point)``.
 
     Methods
     -------
     elapsed_time : callable
         A method that returns the time elapsed since the runner
         was started.
     overhead : callable
@@ -344,61 +459,72 @@
         overhead of the executor. Essentially, this is
         ``100 * (1 - total_elapsed_function_time / self.elapsed_time())``.
 
     """
 
     def __init__(
         self,
-        learner,
-        goal,
+        learner: LearnerType,
+        goal: Callable[[LearnerType], bool] | None = None,
         *,
-        executor=None,
-        ntasks=None,
-        log=False,
-        shutdown_executor=False,
-        retries=0,
-        raise_if_retries_exceeded=True,
-    ):
+        loss_goal: float | None = None,
+        npoints_goal: int | None = None,
+        end_time_goal: datetime | None = None,
+        duration_goal: timedelta | int | float | None = None,
+        executor: (ExecutorTypes | None) = None,
+        ntasks: int | None = None,
+        log: bool = False,
+        shutdown_executor: bool = False,
+        retries: int = 0,
+        raise_if_retries_exceeded: bool = True,
+    ) -> None:
         if inspect.iscoroutinefunction(learner.function):
-            raise ValueError(
-                "Coroutine functions can only be used " "with 'AsyncRunner'."
-            )
+            raise ValueError("Coroutine functions can only be used with 'AsyncRunner'.")
         super().__init__(
             learner,
-            goal,
+            goal=goal,
+            loss_goal=loss_goal,
+            npoints_goal=npoints_goal,
+            end_time_goal=end_time_goal,
+            duration_goal=duration_goal,
             executor=executor,
             ntasks=ntasks,
             log=log,
             shutdown_executor=shutdown_executor,
             retries=retries,
             raise_if_retries_exceeded=raise_if_retries_exceeded,
+            allow_running_forever=False,
         )
         self._run()
 
-    def _submit(self, x):
+    def _submit(self, x: tuple[float, ...] | float | int) -> FutureTypes:
         return self.executor.submit(self.learner.function, x)
 
-    def _run(self):
+    def _run(self) -> None:
         first_completed = concurrent.FIRST_COMPLETED
 
         if self._get_max_tasks() < 1:
             raise RuntimeError("Executor has no workers")
 
         try:
             while not self.goal(self.learner):
                 futures = self._get_futures()
                 done, _ = concurrent.wait(futures, return_when=first_completed)
                 self._process_futures(done)
         finally:
             remaining = self._remove_unfinished()
             if remaining:
                 concurrent.wait(remaining)
+                # Some futures get their result set, despite being cancelled.
+                # see https://github.com/python-adaptive/adaptive/issues/319
+                with_result = {f for f in remaining if not f.cancelled() and f.done()}
+                self._process_futures(with_result)
             self._cleanup()
 
-    def elapsed_time(self):
+    def elapsed_time(self) -> float:
         """Return the total time elapsed since the runner
         was started."""
         if self.end_time is None:
             # This shouldn't happen if the BlockingRunner
             # correctly finished.
             self.end_time = time.time()
         return self.end_time - self.start_time
@@ -409,22 +535,39 @@
 
     Parameters
     ----------
     learner : `~adaptive.BaseLearner` instance
     goal : callable, optional
         The end condition for the calculation. This function must take
         the learner as its sole argument, and return True when we should
-        stop requesting more points. If not provided, the runner will run
-        forever, or until ``self.task.cancel()`` is called.
+        stop requesting more points.
+        If not provided, the runner will run forever (or stop when no more
+        points can be added), or until ``runner.task.cancel()`` is called.
+    loss_goal : float, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the loss is smaller than this value.
+    npoints_goal : int, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the number of points is larger or
+        equal than this value.
+    end_time_goal : datetime, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the current time is larger or equal than this
+        value.
+    duration_goal : timedelta or number, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the current time is larger or equal than
+        ``start_time + duration_goal``. ``duration_goal`` can be a number
+        indicating the number of seconds.
     executor : `concurrent.futures.Executor`, `distributed.Client`,\
-               `mpi4py.futures.MPIPoolExecutor`, or `ipyparallel.Client`, optional
+               `mpi4py.futures.MPIPoolExecutor`, `ipyparallel.Client` or\
+               `loky.get_reusable_executor`, optional
         The executor in which to evaluate the function to be learned.
-        If not provided, a new `~concurrent.futures.ProcessPoolExecutor`
-        is used on Unix systems while on Windows a `distributed.Client`
-        is used if `distributed` is installed.
+        If not provided, a new `~concurrent.futures.ProcessPoolExecutor` on
+        Linux, and a `loky.get_reusable_executor` on MacOS and Windows.
     ntasks : int, optional
         The number of concurrent function evaluations. Defaults to the number
         of cores available in `executor`.
     log : bool, default: False
         If True, record the method calls made to the learner by this runner.
     shutdown_executor : bool, default: False
         If True, shutdown the executor when the runner has completed. If
@@ -435,32 +578,34 @@
         the default event loop is used.
     retries : int, default: 0
         Maximum amount of retries of a certain point ``x`` in
         ``learner.function(x)``. After `retries` is reached for ``x``
         the point is present in ``runner.failed``.
     raise_if_retries_exceeded : bool, default: True
         Raise the error after a point ``x`` failed `retries`.
+    allow_running_forever : bool, default: True
+        If True, the runner will run forever if the goal is not provided.
 
     Attributes
     ----------
     task : `asyncio.Task`
         The underlying task. May be cancelled in order to stop the runner.
     learner : `~adaptive.BaseLearner` instance
         The underlying learner. May be queried for its state.
     log : list or None
         Record of the method calls made to the learner, in the format
         ``(method_name, *args)``.
-    to_retry : dict
-        Mapping of ``{point: n_fails, ...}``. When a point has failed
+    to_retry : list of tuples
+        List of ``(point, n_fails)``. When a point has failed
         ``runner.retries`` times it is removed but will be present
         in ``runner.tracebacks``.
-    tracebacks : dict
-        A mapping of point to the traceback if that point failed.
-    pending_points : dict
-        A mapping of `~concurrent.futures.Future`\s to points.
+    tracebacks : list of tuples
+        List of of ``(point, tb)`` for points that failed.
+    pending_points : list of tuples
+        A list of tuples with ``(concurrent.futures.Future, point)``.
 
     Methods
     -------
     elapsed_time : callable
         A method that returns the time elapsed since the runner
         was started.
     overhead : callable
@@ -473,73 +618,92 @@
     This runner can be used when an async function (defined with
     ``async def``) has to be learned. In this case the function will be
     run directly on the event loop (and not in the executor).
     """
 
     def __init__(
         self,
-        learner,
-        goal=None,
+        learner: LearnerType,
+        goal: Callable[[LearnerType], bool] | None = None,
         *,
-        executor=None,
-        ntasks=None,
-        log=False,
-        shutdown_executor=False,
+        loss_goal: float | None = None,
+        npoints_goal: int | None = None,
+        end_time_goal: datetime | None = None,
+        duration_goal: timedelta | int | float | None = None,
+        executor: (ExecutorTypes | None) = None,
+        ntasks: int | None = None,
+        log: bool = False,
+        shutdown_executor: bool = False,
         ioloop=None,
-        retries=0,
-        raise_if_retries_exceeded=True,
-    ):
-
-        if goal is None:
-
-            def goal(_):
-                return False
+        retries: int = 0,
+        raise_if_retries_exceeded: bool = True,
+    ) -> None:
+        if (
+            executor is None
+            and _default_executor is concurrent.ProcessPoolExecutor
+            and not inspect.iscoroutinefunction(learner.function)
+        ):
+            try:
+                pickle.dumps(learner.function)
+            except pickle.PicklingError as e:
+                raise ValueError(
+                    "`learner.function` cannot be pickled (is it a lamdba function?)"
+                    " and therefore does not work with the default executor."
+                    " Either make sure the function is pickleble or use an executor"
+                    " that might work with 'hard to pickle'-functions"
+                    " , e.g. `ipyparallel` with `dill`."
+                ) from e
 
         super().__init__(
             learner,
-            goal,
+            goal=goal,
+            loss_goal=loss_goal,
+            npoints_goal=npoints_goal,
+            end_time_goal=end_time_goal,
+            duration_goal=duration_goal,
             executor=executor,
             ntasks=ntasks,
             log=log,
             shutdown_executor=shutdown_executor,
             retries=retries,
             raise_if_retries_exceeded=raise_if_retries_exceeded,
+            allow_running_forever=True,
         )
         self.ioloop = ioloop or asyncio.get_event_loop()
-        self.task = None
 
         # When the learned function is 'async def', we run it
         # directly on the event loop, and not in the executor.
         # The *whole point* of allowing learning of async functions is so that
         # the user can have more fine-grained control over the parallelism.
         if inspect.iscoroutinefunction(learner.function):
             if executor:  # user-provided argument
                 raise RuntimeError(
-                    "Cannot use an executor when learning an " "async function."
+                    "Cannot use an executor when learning an async function."
                 )
             self.executor.shutdown()  # Make sure we don't shoot ourselves later
 
         self.task = self.ioloop.create_task(self._run())
-        self.saving_task = None
+        self.saving_task: asyncio.Task | None = None
         if in_ipynb() and not self.ioloop.is_running():
             warnings.warn(
                 "The runner has been scheduled, but the asyncio "
                 "event loop is not running! If you are "
                 "in a Jupyter notebook, remember to run "
-                "'adaptive.notebook_extension()'"
+                "'adaptive.notebook_extension()'",
+                stacklevel=2,
             )
 
-    def _submit(self, x):
+    def _submit(self, x: Any) -> asyncio.Task | asyncio.Future:
         ioloop = self.ioloop
         if inspect.iscoroutinefunction(self.learner.function):
             return ioloop.create_task(self.learner.function(x))
         else:
             return ioloop.run_in_executor(self.executor, self.learner.function, x)
 
-    def status(self):
+    def status(self) -> str:
         """Return the runner status as a string.
 
         The possible statuses are: running, cancelled, failed, and finished.
         """
         try:
             self.task.result()
         except asyncio.CancelledError:
@@ -547,22 +711,29 @@
         except asyncio.InvalidStateError:
             return "running"
         except Exception:
             return "failed"
         else:
             return "finished"
 
-    def cancel(self):
+    def cancel(self) -> None:
         """Cancel the runner.
 
         This is equivalent to calling ``runner.task.cancel()``.
         """
         self.task.cancel()
 
-    def live_plot(self, *, plotter=None, update_interval=2, name=None, normalize=True):
+    def live_plot(
+        self,
+        *,
+        plotter: Callable[[LearnerType], holoviews.Element] | None = None,
+        update_interval: float = 2.0,
+        name: str | None = None,
+        normalize: bool = True,
+    ) -> holoviews.DynamicMap:
         """Live plotting of the learner's data.
 
         Parameters
         ----------
         runner : `~adaptive.Runner`
         plotter : function
             A function that takes the learner as a argument and returns a
@@ -578,116 +749,176 @@
 
         Returns
         -------
         dm : `holoviews.core.DynamicMap`
             The plot that automatically updates every `update_interval`.
         """
         return live_plot(
-            self, plotter=plotter, update_interval=update_interval, name=name
+            self,
+            plotter=plotter,
+            update_interval=update_interval,
+            name=name,
+            normalize=normalize,
         )
 
-    def live_info(self, *, update_interval=0.1):
+    def live_info(self, *, update_interval: float = 0.1) -> None:
         """Display live information about the runner.
 
         Returns an interactive ipywidget that can be
         visualized in a Jupyter notebook.
         """
         return live_info(self, update_interval=update_interval)
 
-    async def _run(self):
+    async def _run(self) -> None:
         first_completed = asyncio.FIRST_COMPLETED
 
         if self._get_max_tasks() < 1:
             raise RuntimeError("Executor has no workers")
 
         try:
             while not self.goal(self.learner):
                 futures = self._get_futures()
-                done, _ = await asyncio.wait(
-                    futures, return_when=first_completed, loop=self.ioloop
-                )
+                kw = {"loop": self.ioloop} if sys.version_info[:2] < (3, 10) else {}
+                done, _ = await asyncio.wait(futures, return_when=first_completed, **kw)  # type: ignore[arg-type]
                 self._process_futures(done)
         finally:
             remaining = self._remove_unfinished()
             if remaining:
                 await asyncio.wait(remaining)
             self._cleanup()
 
-    def elapsed_time(self):
+    def elapsed_time(self) -> float:
         """Return the total time elapsed since the runner
         was started."""
         if self.task.done():
             end_time = self.end_time
             if end_time is None:
                 # task was cancelled before it began
                 assert self.task.cancelled()
                 return 0
         else:
             end_time = time.time()
         return end_time - self.start_time
 
-    def start_periodic_saving(self, save_kwargs, interval):
+    def start_periodic_saving(
+        self,
+        save_kwargs: dict[str, Any] | None = None,
+        interval: int = 30,
+        method: Callable[[LearnerType], None] | None = None,
+    ):
         """Periodically save the learner's data.
 
         Parameters
         ----------
         save_kwargs : dict
             Key-word arguments for ``learner.save(**save_kwargs)``.
+            Only used if ``method=None``.
         interval : int
             Number of seconds between saving the learner.
+        method : callable
+            The method to use for saving the learner. If None, the default
+            saves the learner using "pickle" which calls
+            ``learner.save(**save_kwargs)``. Otherwise provide a callable
+            that takes the learner and saves the learner.
 
         Example
         -------
         >>> runner = Runner(learner)
         >>> runner.start_periodic_saving(
         ...     save_kwargs=dict(fname='data/test.pickle'),
         ...     interval=600)
         """
 
-        async def _saver(save_kwargs=save_kwargs, interval=interval):
+        def default_save(learner):
+            learner.save(**save_kwargs)
+
+        if method is None:
+            method = default_save
+            if save_kwargs is None:
+                raise ValueError("Must provide `save_kwargs` if method=None.")
+
+        async def _saver():
             while self.status() == "running":
-                self.learner.save(**save_kwargs)
+                method(self.learner)
                 await asyncio.sleep(interval)
-            self.learner.save(**save_kwargs)  # one last time
+            method(self.learner)  # one last time
 
         self.saving_task = self.ioloop.create_task(_saver())
         return self.saving_task
 
 
 # Default runner
 Runner = AsyncRunner
 
 
-def simple(learner, goal):
+def simple(
+    learner: LearnerType,
+    goal: Callable[[LearnerType], bool] | None = None,
+    *,
+    loss_goal: float | None = None,
+    npoints_goal: int | None = None,
+    end_time_goal: datetime | None = None,
+    duration_goal: timedelta | int | float | None = None,
+):
     """Run the learner until the goal is reached.
 
     Requests a single point from the learner, evaluates
     the function to be learned, and adds the point to the
     learner, until the goal is reached, blocking the current
     thread.
 
     This function is useful for extracting error messages,
     as the learner's function is evaluated in the same thread,
     meaning that exceptions can simple be caught an inspected.
 
     Parameters
     ----------
     learner : ~`adaptive.BaseLearner` instance
-    goal : callable
-        The end condition for the calculation. This function must take the
-        learner as its sole argument, and return True if we should stop.
+    goal : callable, optional
+        The end condition for the calculation. This function must take
+        the learner as its sole argument, and return True when we should
+        stop requesting more points.
+    loss_goal : float, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the loss is smaller than this value.
+    npoints_goal : int, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the number of points is larger or
+        equal than this value.
+    end_time_goal : datetime, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the current time is larger or equal than this
+        value.
+    duration_goal : timedelta or number, optional
+        Convenience argument, use instead of ``goal``. The end condition for the
+        calculation. Stop when the current time is larger or equal than
+        ``start_time + duration_goal``. ``duration_goal`` can be a number
+        indicating the number of seconds.
     """
+    goal = _goal(
+        learner,
+        goal,
+        loss_goal,
+        npoints_goal,
+        end_time_goal,
+        duration_goal,
+        allow_running_forever=False,
+    )
+    assert goal is not None
     while not goal(learner):
         xs, _ = learner.ask(1)
         for x in xs:
             y = learner.function(x)
             learner.tell(x, y)
 
 
-def replay_log(learner, log):
+def replay_log(
+    learner: LearnerType,
+    log: list[tuple[Literal["tell"], Any, Any] | tuple[Literal["ask"], int]],
+) -> None:
     """Apply a sequence of method calls to a learner.
 
     This is useful for debugging runners.
 
     Parameters
     ----------
     learner : `~adaptive.BaseLearner` instance
@@ -695,62 +926,236 @@
     log : list
         contains tuples: ``(method_name, *args)``.
     """
     for method, *args in log:
         getattr(learner, method)(*args)
 
 
-class SequentialExecutor(concurrent.Executor):
-    """A trivial executor that runs functions synchronously.
-
-    This executor is mainly for testing.
-    """
-
-    def submit(self, fn, *args, **kwargs):
-        fut = concurrent.Future()
-        try:
-            fut.set_result(fn(*args, **kwargs))
-        except Exception as e:
-            fut.set_exception(e)
-        return fut
-
-    def map(self, fn, *iterable, timeout=None, chunksize=1):
-        return map(fn, iterable)
-
-    def shutdown(self, wait=True):
-        pass
+# -- Internal executor-related, things
 
 
-def _ensure_executor(executor):
+def _ensure_executor(executor: ExecutorTypes | None) -> concurrent.Executor:
+    if with_ipyparallel:
+        import ipyparallel
+    if with_distributed:
+        import distributed
     if executor is None:
-        executor = _default_executor(**_default_executor_kwargs)
-
+        executor = _default_executor()
     if isinstance(executor, concurrent.Executor):
         return executor
     elif with_ipyparallel and isinstance(executor, ipyparallel.Client):
         return executor.executor()
     elif with_distributed and isinstance(executor, distributed.Client):
         return executor.get_executor()
     else:
         raise TypeError(
+            # TODO: check if this is correct. Isn't MPI,loky supported?
             "Only a concurrent.futures.Executor, distributed.Client,"
             " or ipyparallel.Client can be used."
         )
 
 
-def _get_ncores(ex):
+def _get_ncores(
+    ex: (ExecutorTypes),
+) -> int:
     """Return the maximum  number of cores that an executor can use."""
+    if with_ipyparallel:
+        import ipyparallel
+    if with_distributed:
+        import distributed
+    if with_mpi4py:
+        import mpi4py.futures
     if with_ipyparallel and isinstance(ex, ipyparallel.client.view.ViewExecutor):
         return len(ex.view)
     elif isinstance(
         ex, (concurrent.ProcessPoolExecutor, concurrent.ThreadPoolExecutor)
     ):
-        return ex._max_workers  # not public API!
+        return ex._max_workers  # type: ignore[union-attr]
+    elif isinstance(ex, loky.reusable_executor._ReusablePoolExecutor):
+        return ex._max_workers  # type: ignore[union-attr]
     elif isinstance(ex, SequentialExecutor):
         return 1
     elif with_distributed and isinstance(ex, distributed.cfexecutor.ClientExecutor):
         return sum(n for n in ex._client.ncores().values())
     elif with_mpi4py and isinstance(ex, mpi4py.futures.MPIPoolExecutor):
         ex.bootup()  # wait until all workers are up and running
         return ex._pool.size  # not public API!
     else:
         raise TypeError(f"Cannot get number of cores for {ex.__class__}")
+
+
+# --- Useful runner goals
+
+
+# TODO: deprecate
+def stop_after(*, seconds=0, minutes=0, hours=0) -> Callable[[LearnerType], bool]:
+    """Stop a runner after a specified time.
+
+    For example, to specify a runner that should stop after
+    5 minutes, one could do the following:
+
+    >>> runner = Runner(learner, goal=stop_after(minutes=5))
+
+    To stop a runner after 2 hours, 10 minutes and 3 seconds,
+    one could do the following:
+
+    >>> runner = Runner(learner, goal=stop_after(hours=2, minutes=10, seconds=3))
+
+    Parameters
+    ----------
+    seconds, minutes, hours : float, default: 0
+        If more than one is specified, then they are added together
+
+    Returns
+    -------
+    goal : callable
+        Can be used as the ``goal`` parameter when constructing
+        a `Runner`.
+
+    Notes
+    -----
+    The duration specified is only a *lower bound* on the time that the
+    runner will run for, because the runner only checks its goal when
+    it adds points to its learner
+    """
+    stop_time = time.time() + seconds + 60 * minutes + 3600 * hours
+    return lambda _: time.time() > stop_time
+
+
+class _TimeGoal:
+    def __init__(self, dt: timedelta | datetime | int | float):
+        self.dt = dt if isinstance(dt, (timedelta, datetime)) else timedelta(seconds=dt)
+        self.start_time = None
+
+    def __call__(self, _):
+        if isinstance(self.dt, timedelta):
+            if self.start_time is None:
+                self.start_time = datetime.now()
+            return datetime.now() - self.start_time > self.dt
+        if isinstance(self.dt, datetime):
+            return datetime.now() > self.dt
+        raise TypeError(f"`dt={self.dt}` is not a datetime, timedelta, or number.")
+
+
+def auto_goal(
+    *,
+    loss: float | None = None,
+    npoints: int | None = None,
+    end_time: datetime | None = None,
+    duration: timedelta | int | float | None = None,
+    learner: LearnerType | None = None,
+    allow_running_forever: bool = True,
+) -> Callable[[LearnerType], bool]:
+    """Extract a goal from the learners.
+
+    Parameters
+    ----------
+    loss : float, optional
+        Stop when the loss is smaller than this value.
+    npoints : int, optional
+        Stop when the number of points is larger or equal than this value.
+    end_time : datetime, optional
+        Stop when the current time is larger or equal than this value.
+    duration : timedelta or number, optional
+        Stop when the current time is larger or equal than
+        ``start_time + duration``. ``duration`` can be a number
+        indicating the number of seconds.
+    learner
+        Learner for which to determine the goal. Only used if the learner type
+        is `BalancingLearner`, `DataSaver`, `SequenceLearner`, or `IntegratorLearner`.
+    allow_running_forever
+        If True, and the goal is None and the learner is not a SequenceLearner,
+        then a goal that never stops is returned, otherwise an exception is raised.
+
+    Returns
+    -------
+    Callable[[adaptive.BaseLearner], bool]
+    """
+    opts = (loss, npoints, end_time, duration)  # all are mutually exclusive
+    if sum(v is not None for v in opts) > 1:
+        raise ValueError(
+            "Only one of loss, npoints, end_time, duration can be specified."
+        )
+
+    if loss is not None:
+        return lambda learner: learner.loss() <= loss
+    if isinstance(learner, BalancingLearner):
+        # Note that the float loss goal is more efficiently implemented in the
+        # BalancingLearner itself. That is why the previous if statement is
+        # above this one.
+        goals = [
+            auto_goal(
+                learner=lrn,
+                loss=loss,
+                npoints=npoints,
+                end_time=end_time,
+                duration=duration,
+                allow_running_forever=allow_running_forever,
+            )
+            for lrn in learner.learners
+        ]
+        return lambda learner: all(
+            goal(lrn) for lrn, goal in zip(learner.learners, goals)  # type: ignore[attr-defined]
+        )
+    if npoints is not None:
+        return lambda learner: learner.npoints >= npoints  # type: ignore[operator]
+    if end_time is not None:
+        return _TimeGoal(end_time)
+    if duration is not None:
+        return _TimeGoal(duration)
+    if isinstance(learner, DataSaver):
+        assert learner is not None
+        return auto_goal(
+            learner=learner.learner,
+            loss=loss,
+            npoints=npoints,
+            end_time=end_time,
+            duration=duration,
+            allow_running_forever=allow_running_forever,
+        )
+    if all(v is None for v in opts):
+        if isinstance(learner, SequenceLearner):
+            return SequenceLearner.done  # type: ignore[return-value]
+        if isinstance(learner, IntegratorLearner):
+            return IntegratorLearner.done  # type: ignore[return-value]
+        if not allow_running_forever:
+            raise ValueError(
+                "Goal is None which means the learners"
+                " continue forever and this is not allowed."
+            )
+        warnings.warn(
+            "Goal is None which means the learners continue forever!", stacklevel=2
+        )
+        return lambda _: False
+    raise ValueError("Cannot determine goal from {goal}.")
+
+
+def _goal(
+    learner: LearnerType | None,
+    goal: Callable[[LearnerType], bool] | None,
+    loss_goal: float | None,
+    npoints_goal: int | None,
+    end_time_goal: datetime | None,
+    duration_goal: timedelta | int | float | None,
+    allow_running_forever: bool,
+):
+    if callable(goal):
+        return goal
+
+    if goal is not None and (
+        loss_goal is not None
+        or npoints_goal is not None
+        or end_time_goal is not None
+        or duration_goal is not None
+    ):
+        raise ValueError(
+            "Either goal, loss_goal, npoints_goal, end_time_goal or"
+            " duration_goal can be specified, not multiple."
+        )
+    return auto_goal(
+        learner=learner,
+        loss=loss_goal,
+        npoints=npoints_goal,
+        end_time=end_time_goal,
+        duration=duration_goal,
+        allow_running_forever=allow_running_forever,
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adaptive-0.9.0/adaptive/tests/algorithm_4.py` & `adaptive-1.0.0/adaptive/tests/algorithm_4.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 # Copyright 2010 Pedro Gonnet
 # Copyright 2017 Christoph Groth
+from __future__ import annotations
 
 from collections import defaultdict
-from fractions import Fraction as Frac
+from fractions import Fraction
+from typing import Callable
 
 import numpy as np
 from numpy.testing import assert_allclose
 from scipy.linalg import inv, norm
 
+from adaptive.types import Real
+
 eps = np.spacing(1)
 
 
-def legendre(n):
+def legendre(n: int) -> list[list[Fraction]]:
     """Return the first n Legendre polynomials.
 
     The polynomials have *standard* normalization, i.e.
     int_{-1}^1 dx L_n(x) L_m(x) = delta(m, n) * 2 / (2 * n + 1).
 
     The return value is a list of list of fraction.Fraction instances.
     """
-    result = [[Frac(1)], [Frac(0), Frac(1)]]
+    result = [[Fraction(1)], [Fraction(0), Fraction(1)]]
     if n <= 2:
         return result[:n]
     for i in range(2, n):
         # Use Bonnet's recursion formula.
-        new = (i + 1) * [Frac(0)]
+        new = (i + 1) * [Fraction(0)]
         new[1:] = (r * (2 * i - 1) for r in result[-1])
         new[:-2] = (n - r * (i - 1) for n, r in zip(new[:-2], result[-2]))
         new[:] = (n / i for n in new)
         result.append(new)
     return result
 
 
-def newton(n):
+def newton(n: int) -> np.ndarray:
     """Compute the monomial coefficients of the Newton polynomial over the
     nodes of the n-point Clenshaw-Curtis quadrature rule.
     """
     # The nodes of the Clenshaw-Curtis rule are x_i = -cos(i * Pi / (n-1)).
     # Here, we calculate the coefficients c_i such that sum_i c_i * x^i
     # = prod_i (x - x_i).  The coefficients are thus sums of products of
     # cosines.
@@ -47,15 +51,15 @@
     #
     # The dictionary 'terms' descibes the terms that make up the
     # monomial coefficients.  Each item ((d, a), m) corresponds to a
     # term m * cos(a * Pi / n) to be added to prefactor of the
     # monomial x^(n-d).
 
     mod = 2 * (n - 1)
-    terms = defaultdict(int)
+    terms: dict[tuple[int, int], int] = defaultdict(int)
     terms[0, 0] += 1
 
     for i in range(n):
         newterms = []
         for (d, a), m in terms.items():
             for b in [i, -i]:
                 # In order to reduce the number of terms, cosine
@@ -85,15 +89,15 @@
     cf = np.array(c, float)
     assert all(int(cfe) == ce for cfe, ce in zip(cf, c)), "Precision loss"
 
     cf /= 2.0 ** np.arange(n, -1, -1)
     return cf
 
 
-def scalar_product(a, b):
+def scalar_product(a: list[Fraction], b: list[Fraction]) -> Fraction:
     """Compute the polynomial scalar product int_-1^1 dx a(x) b(x).
 
     The args must be sequences of polynomial coefficients.  This
     function is careful to use the input data type for calculations.
     """
     la = len(a)
     lc = len(b) + la + 1
@@ -103,31 +107,31 @@
     for i, bi in enumerate(b):
         if bi == 0:
             continue
         for j in range(i % 2, la, 2):
             c[i + j] += a[j] * bi
 
     # Calculate the definite integral from -1 to 1.
-    return 2 * sum(c[i] / (i + 1) for i in range(0, lc, 2))
+    return 2 * sum(c[i] / (i + 1) for i in range(0, lc, 2))  # type: ignore[return-value]
 
 
-def calc_bdef(ns):
+def calc_bdef(ns: tuple[int, int, int, int]) -> list[np.ndarray]:
     """Calculate the decompositions of Newton polynomials (over the nodes
     of the n-point Clenshaw-Curtis quadrature rule) in terms of
     Legandre polynomials.
 
     The parameter 'ns' is a sequence of numers of points of the
     quadrature rule.  The return value is a corresponding sequence of
     normalized Legendre polynomial coefficients.
     """
     legs = legendre(max(ns) + 1)
     result = []
     for n in ns:
         poly = []
-        a = list(map(Frac, newton(n)))
+        a = list(map(Fraction, newton(n)))
         for b in legs[: n + 1]:
             igral = scalar_product(a, b)
 
             # Normalize & store.  (The polynomials returned by
             # legendre() have standard normalization that is not
             # orthonormal.)
             poly.append(np.sqrt((2 * len(b) - 1) / 2) * igral)
@@ -141,15 +145,15 @@
 xi = [-np.cos(np.arange(n[j]) / (n[j] - 1) * np.pi) for j in range(4)]
 # Make `xi` perfectly anti-symmetric, important for splitting the intervals
 xi = [(row - row[::-1]) / 2 for row in xi]
 
 b_def = calc_bdef(n)
 
 
-def calc_V(xi, n):
+def calc_V(xi: np.ndarray, n: int) -> np.ndarray:
     V = [np.ones(xi.shape), xi.copy()]
     for i in range(2, n):
         V.append((2 * i - 1) / i * xi * V[-1] - (i - 1) / i * V[-2])
     for i in range(n):
         V[i] *= np.sqrt(i + 0.5)
     return np.array(V).T
 
@@ -179,15 +183,15 @@
 
 
 k = np.arange(n[3])
 alpha = np.sqrt((k + 1) ** 2 / (2 * k + 1) / (2 * k + 3))
 gamma = np.concatenate([[0, 0], np.sqrt(k[2:] ** 2 / (4 * k[2:] ** 2 - 1))])
 
 
-def _downdate(c, nans, depth):
+def _downdate(c: np.ndarray, nans: list[int], depth: int) -> None:
     # This is algorithm 5 from the thesis of Pedro Gonnet.
     b = b_def[depth].copy()
     m = n[depth] - 1
     for i in nans:
         b[m + 1] /= alpha[m]
         xii = xi[depth][i]
         b[m] = (b[m] + xii * b[m + 1]) / alpha[m - 1]
@@ -196,77 +200,92 @@
         b = b[1:]
 
         c[:m] -= c[m] / b[m] * b[:m]
         c[m] = 0
         m -= 1
 
 
-def _zero_nans(fx):
+def _zero_nans(fx: np.ndarray) -> list[int]:
     nans = []
     for i in range(len(fx)):
         if not np.isfinite(fx[i]):
             nans.append(i)
             fx[i] = 0.0
     return nans
 
 
-def _calc_coeffs(fx, depth):
+def _calc_coeffs(fx: np.ndarray, depth: int) -> np.ndarray:
     """Caution: this function modifies fx."""
     nans = _zero_nans(fx)
     c_new = V_inv[depth] @ fx
     if nans:
         fx[nans] = np.nan
         _downdate(c_new, nans, depth)
     return c_new
 
 
 class DivergentIntegralError(ValueError):
-    def __init__(self, msg, igral, err, nr_points):
+    def __init__(self, msg: str, igral: float, err: None, nr_points: int) -> None:
         self.igral = igral
         self.err = err
         self.nr_points = nr_points
         super().__init__(msg)
 
 
 class _Interval:
     __slots__ = ["a", "b", "c", "fx", "igral", "err", "depth", "rdepth", "ndiv", "c00"]
 
-    def __init__(self, a, b, depth, rdepth):
+    a: Real
+    b: Real
+    c: np.ndarray
+    fx: np.ndarray
+    igral: Real
+    err: Real
+    depth: int
+    rdepth: int
+    ndiv: int
+    c00: Real
+
+    def __init__(self, a: Real, b: Real, depth: int, rdepth: int) -> None:
         self.a = a
         self.b = b
         self.depth = depth
         self.rdepth = rdepth
 
-    def points(self):
+    def points(self) -> np.ndarray:
         a = self.a
         b = self.b
         return (a + b) / 2 + (b - a) * xi[self.depth] / 2
 
     @classmethod
-    def make_first(cls, f, a, b, depth=2):
+    def make_first(
+        cls, f: Callable, a: int, b: int, depth: int = 2
+    ) -> tuple[_Interval, int]:
         ival = _Interval(a, b, depth, 1)
         fx = f(ival.points())
         ival.c = _calc_coeffs(fx, depth)
         ival.c00 = 0.0
         ival.fx = fx
         ival.ndiv = 0
         return ival, n[depth]
 
-    def calc_igral_and_err(self, c_old):
+    def calc_igral_and_err(self, c_old: np.ndarray) -> float:
         self.c = c_new = _calc_coeffs(self.fx, self.depth)
         c_diff = np.zeros(max(len(c_old), len(c_new)))
         c_diff[: len(c_old)] = c_old
         c_diff[: len(c_new)] -= c_new
         c_diff = norm(c_diff)
         w = self.b - self.a
         self.igral = w * c_new[0] * sqrt_one_half
         self.err = w * c_diff
         return c_diff
 
-    def split(self, f):
+    def split(
+        self, f: Callable
+    ) -> tuple[tuple[float, float, float], int] | tuple[list[_Interval], int]:
         m = (self.a + self.b) / 2
         f_center = self.fx[(len(self.fx) - 1) // 2]
 
         rdepth = self.rdepth + 1
         ivals = [_Interval(self.a, m, 0, rdepth), _Interval(m, self.b, 0, rdepth)]
         points = np.concatenate([ival.points()[1:-1] for ival in ivals])
         nr_points = len(points)
@@ -276,34 +295,36 @@
         fxs[:, 1:-1] = f(points).reshape((2, -1))
 
         for ival, fx, T in zip(ivals, fxs, T_lr):
             ival.fx = fx
             ival.calc_igral_and_err(T[:, : self.c.shape[0]] @ self.c)
 
             ival.c00 = ival.c[0]
-            ival.ndiv = self.ndiv + (self.c00 and ival.c00 / self.c00 > 2)
+            ival.ndiv = self.ndiv + (self.c00 and ival.c00 / self.c00 > 2)  # type: ignore[assignment]
             if ival.ndiv > ndiv_max and 2 * ival.ndiv > ival.rdepth:
                 # Signal a divergent integral.
                 return (ival.a, ival.b, ival.b - ival.a), nr_points
 
         return ivals, nr_points
 
-    def refine(self, f):
+    def refine(self, f: Callable) -> tuple[np.ndarray, bool, int]:
         """Increase degree of interval."""
         self.depth = depth = self.depth + 1
         points = self.points()
         fx = np.empty(n[depth])
         fx[0 : n[depth] : 2] = self.fx
         fx[1 : n[depth] - 1 : 2] = f(points[1 : n[depth] - 1 : 2])
         self.fx = fx
         split = self.calc_igral_and_err(self.c) > hint * norm(self.c)
         return points, split, n[depth] - n[depth - 1]
 
 
-def algorithm_4(f, a, b, tol, N_loops=int(1e9)):
+def algorithm_4(
+    f: Callable, a: int, b: int, tol: float, N_loops: int = int(1e9)  # noqa: B008
+) -> tuple[float, float, int, list[_Interval]]:
     """ALGORITHM_4 evaluates an integral using adaptive quadrature. The
     algorithm uses Clenshaw-Curtis quadrature rules of increasing
     degree in each interval and bisects the interval if either the
     function does not appear to be smooth or a rule of maximum degree
     has been reached. The error estimate is computed from the L2-norm
     of the difference between two successive interpolations of the
     integrand over the nodes of the respective quadrature rules.
@@ -327,17 +348,17 @@
         Using Explicit Interpolants", P. Gonnet, ACM Transactions on
         Mathematical Software, 37 (3), art. no. 26, 2008.
     """
 
     ival, nr_points = _Interval.make_first(f, a, b)
 
     ivals = [ival]
-    igral_excess = 0
-    err_excess = 0
-    i_max = 0
+    igral_excess: float = 0
+    err_excess: float = 0
+    i_max: int = 0
 
     for _ in range(N_loops):
         if ivals[i_max].depth == 3:
             split = True
         else:
             points, split, nr_points_inc = ivals[i_max].refine(f)
             nr_points += nr_points_inc
@@ -399,45 +420,45 @@
             or (err_excess > abs(igral) * tol and err - err_excess < abs(igral) * tol)
             or not ivals
         ):
             return igral, err, nr_points, ivals
     return igral, err, nr_points, ivals
 
 
-################ Tests ################
+# ############### Tests ################
 
 
-def f0(x):
+def f0(x: float | np.ndarray) -> float | np.ndarray:
     return x * np.sin(1 / x) * np.sqrt(abs(1 - x))
 
 
 def f7(x):
-    return x ** -0.5
+    return x**-0.5
 
 
-def f24(x):
+def f24(x: float | np.ndarray) -> float | np.ndarray:
     return np.floor(np.exp(x))
 
 
-def f21(x):
+def f21(x: float | np.ndarray) -> float | np.ndarray:
     y = 0
     for i in range(1, 4):
-        y += 1 / np.cosh(20 ** i * (x - 2 * i / 10))
+        y += 1 / np.cosh(20**i * (x - 2 * i / 10))
     return y
 
 
-def f63(x, alpha, beta):
+def f63(x: float | np.ndarray, alpha: float, beta: float) -> float | np.ndarray:
     return abs(x - beta) ** alpha
 
 
 def F63(x, alpha, beta):
     return (x - beta) * abs(x - beta) ** alpha / (alpha + 1)
 
 
-def fdiv(x):
+def fdiv(x: float | np.ndarray) -> float | np.ndarray:
     return abs(x - 0.987654321) ** -1.1
 
 
 def f_one_with_nan(x):
     x = np.asarray(x)
     result = np.ones(x.shape)
     result[x == 0] = np.inf
@@ -457,15 +478,17 @@
 
 
 def test_scalar_product(n=33):
     legs = legendre(n)
     selection = [0, 5, 7, n - 1]
     for i in selection:
         for j in selection:
-            assert scalar_product(legs[i], legs[j]) == ((i == j) and Frac(2, 2 * i + 1))
+            assert scalar_product(legs[i], legs[j]) == (
+                (i == j) and Fraction(2, 2 * i + 1)
+            )
 
 
 def simple_newton(n):
     """Slower than 'newton()' and prone to numerical error."""
     from itertools import combinations
 
     nodes = -np.cos(np.arange(n) / (n - 1) * np.pi)
@@ -561,15 +584,15 @@
         except DivergentIntegralError:
             assert alpha < -0.8
             false_negatives += alpha > -1
         else:
             if alpha <= -1:
                 false_positives += 1
             else:
-                igral_exact = F(1) - F(0)
+                igral_exact = F(1, alpha, beta) - F(0, alpha, beta)
                 assert alpha < -0.7 or abs(igral - igral_exact) < err
 
     assert false_negatives < 0.05 * n
     assert false_positives < 0.05 * n
 
     np.seterr(**old_settings)
```

### Comparing `adaptive-0.9.0/adaptive/tests/test_average_learner.py` & `adaptive-1.0.0/adaptive/tests/test_average_learner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,43 @@
-# -*- coding: utf-8 -*-
-
 import random
+from typing import TYPE_CHECKING
 
+import flaky
 import numpy as np
 
 from adaptive.learner import AverageLearner
+from adaptive.runner import simple
+
+if TYPE_CHECKING:
+    pass
+
+
+def f_unused(seed):
+    raise NotImplementedError("This function shouldn't be used.")
 
 
 def test_only_returns_new_points():
-    learner = AverageLearner(lambda x: x, atol=None, rtol=0.01)
+    learner = AverageLearner(f_unused, atol=None, rtol=0.01)
 
     # Only tell it n = 5...10
     for i in range(5, 10):
         learner.tell(i, 1)
 
     learner.tell_pending(0)  # This means it shouldn't return 0 anymore
 
     assert learner.ask(1)[0][0] == 1
     assert learner.ask(1)[0][0] == 2
     assert learner.ask(1)[0][0] == 3
     assert learner.ask(1)[0][0] == 4
     assert learner.ask(1)[0][0] == 10
 
 
+@flaky.flaky(max_runs=5)
 def test_avg_std_and_npoints():
-    learner = AverageLearner(lambda x: x, atol=None, rtol=0.01)
+    learner = AverageLearner(f_unused, atol=None, rtol=0.01)
 
     for i in range(300):
         # This will add 5000 points at random values of n.
         # It could try to readd already evaluated points.
 
         n = random.randint(0, 2 * 300)
         value = random.random()
@@ -40,9 +49,29 @@
             learner.tell_pending(n)
 
         if i > 2 and i % 10 == 0:
             # We need more than two points for 'learner.std' to be defined.
             values = np.array(list(learner.data.values()))
             std = np.sqrt(sum((values - values.mean()) ** 2) / (len(values) - 1))
             assert learner.npoints == len(learner.data)
-            assert abs(learner.sum_f - values.sum()) < 1e-13
-            assert abs(learner.std - std) < 1e-13
+            assert abs(learner.sum_f - values.sum()) < 1e-12
+            assert abs(learner.std - std) < 1e-12
+
+
+def test_min_npoints():
+    def constant_function(seed):
+        return 0.1
+
+    for min_npoints in [1, 2, 3]:
+        learner = AverageLearner(
+            constant_function, atol=0.01, rtol=0.01, min_npoints=min_npoints
+        )
+        simple(learner, loss_goal=1.0)
+        assert learner.npoints >= max(2, min_npoints)
+
+
+def test_zero_mean():
+    # see https://github.com/python-adaptive/adaptive/issues/275
+    learner = AverageLearner(f_unused, rtol=0.01)
+    learner.tell(0, -1)
+    learner.tell(1, 1)
+    learner.loss()
```

### Comparing `adaptive-0.9.0/adaptive/tests/test_balancing_learner.py` & `adaptive-1.0.0/adaptive/tests/test_balancing_learner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
 import pytest
 
 from adaptive.learner import BalancingLearner, Learner1D
 from adaptive.runner import simple
 
-
 strategies = ["loss", "loss_improvements", "npoints", "cycle"]
 
 
 def test_balancing_learner_loss_cache():
     learner = Learner1D(lambda x: x, bounds=(-1, 1))
     learner.tell(-1, -1)
     learner.tell(1, 1)
@@ -49,19 +48,19 @@
     learners = [Learner1D(lambda x: x, bounds=(-1, 1)) for i in range(10)]
     learner = BalancingLearner(learners, strategy=strategy)
     points, _ = learner.ask(0)
     assert len(points) == 0
 
 
 @pytest.mark.parametrize(
-    "strategy, goal",
+    "strategy, goal_type, goal",
     [
-        ("loss", lambda l: l.loss() < 0.1),
-        ("loss_improvements", lambda l: l.loss() < 0.1),
-        ("npoints", lambda bl: all(l.npoints > 10 for l in bl.learners)),
-        ("cycle", lambda l: l.loss() < 0.1),
+        ("loss", "loss_goal", 0.1),
+        ("loss_improvements", "loss_goal", 0.1),
+        ("npoints", "goal", lambda bl: all(lrn.npoints > 10 for lrn in bl.learners)),
+        ("cycle", "loss_goal", 0.1),
     ],
 )
-def test_strategies(strategy, goal):
+def test_strategies(strategy, goal_type, goal):
     learners = [Learner1D(lambda x: x, bounds=(-1, 1)) for i in range(10)]
     learner = BalancingLearner(learners, strategy=strategy)
-    simple(learner, goal=goal)
+    simple(learner, **{goal_type: goal})
```

### Comparing `adaptive-0.9.0/adaptive/tests/test_cquad.py` & `adaptive-1.0.0/adaptive/tests/test_cquad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# -*- coding: utf-8 -*-
-
 from functools import partial
 from operator import attrgetter
 
 import numpy as np
 import pytest
 
+import adaptive.learner.integrator_coeffs as coeff
 from adaptive.learner import IntegratorLearner
-from adaptive.learner.integrator_coeffs import ns
 from adaptive.learner.integrator_learner import DivergentIntegralError
 
 from .algorithm_4 import DivergentIntegralError as A4DivergentIntegralError
 from .algorithm_4 import algorithm_4, f0, f7, f21, f24, f63, fdiv
 
 eps = np.spacing(1)
 
@@ -34,25 +32,25 @@
     slots = set(ival.__slots__).intersection(other.__slots__)
     same_slots = []
     for s in slots:
         a = getattr(ival, s)
         b = getattr(other, s)
         is_equal = np.allclose(a, b, rtol=0, atol=eps, equal_nan=True)
         if verbose and not is_equal:
-            print("ival.{} - other.{} = {}".format(s, s, a - b))
+            print(f"ival.{s} - other.{s} = {a - b}")
         same_slots.append(is_equal)
 
     return all(same_slots)
 
 
 def equal_ivals(ivals, other, *, verbose=False):
     """Note: `other` is a list of ivals."""
     if len(ivals) != len(other):
         if verbose:
-            print("len(ivals)={} != len(other)={}".format(len(ivals), len(other)))
+            print(f"len(ivals)={len(ivals)} != len(other)={len(other)}")
         return False
 
     ivals = [sorted(i, key=attrgetter("a")) for i in [ivals, other]]
     return all(
         equal_ival(ival, other_ival, verbose=verbose)
         for ival, other_ival in zip(*ivals)
     )
@@ -136,39 +134,39 @@
     xs, _ = learner.ask(17)
     skip_x = xs[1]
 
     for x in xs:
         if x != skip_x:
             learner.tell(x, learner.function(x))
 
-    for i in range(1000):
+    for _i in range(1000):
         xs, _ = learner.ask(1)
         for x in xs:
             if x != skip_x:
                 learner.tell(x, learner.function(x))
 
     # Now add the point that was skipped
     learner.tell(skip_x, learner.function(skip_x))
 
     # Create a learner with the same number of points, which should
     # give an identical igral value.
     learner2 = IntegratorLearner(f24, bounds=(0, 3), tol=1e-10)
-    for i in range(1017):
+    for _i in range(1017):
         xs, _ = learner2.ask(1)
         for x in xs:
             learner2.tell(x, learner2.function(x))
 
     np.testing.assert_almost_equal(learner.igral, learner2.igral)
 
 
 # XXX: This *should* pass (https://github.com/python-adaptive/adaptive/issues/55)
 @pytest.mark.xfail
 def test_tell_in_random_order(first_add_33=False):
-    from operator import attrgetter
     import random
+    from operator import attrgetter
 
     tol = 1e-10
     for f, a, b in ([f0, 0, 3], [f21, 0, 1], [f24, 0, 3], [f7, 0, 1]):
         learners = []
 
         for shuffle in [True, False]:
             learner = IntegratorLearner(f, bounds=(a, b), tol=tol)
@@ -184,39 +182,39 @@
                 random.shuffle(xs)
             for x in xs:
                 learner.tell(x, f(x))
 
             learners.append(learner)
 
         # Check whether the points of the learners are identical
-        assert set(learners[0].done_points) == set(learners[1].done_points)
+        assert set(learners[0].data) == set(learners[1].data)
 
         # Test whether approximating_intervals gives a complete set of intervals
         for learner in learners:
-            ivals = sorted(learner.approximating_intervals, key=lambda l: l.a)
+            ivals = sorted(learner.approximating_intervals, key=lambda lrn: lrn.a)
             for i in range(len(ivals) - 1):
                 assert ivals[i].b == ivals[i + 1].a, (ivals[i], ivals[i + 1])
 
         # Test if approximating_intervals is the same for random order of adding the point
         ivals = [
             sorted(ival, key=attrgetter("a"))
-            for ival in [l.approximating_intervals for l in learners]
+            for ival in [lrn.approximating_intervals for lrn in learners]
         ]
         assert all(ival.a == other_ival.a for ival, other_ival in zip(*ivals))
 
         # Test if the approximating_intervals are the same
-        ivals = [{(i.a, i.b) for i in l.approximating_intervals} for l in learners]
+        ivals = [{(i.a, i.b) for i in lrn.approximating_intervals} for lrn in learners]
         assert ivals[0] == ivals[1]
 
         # Test whether the igral is identical
         assert np.allclose(learners[0].igral, learners[1].igral), f
 
         # Compare if the errors are in line with the sequential case
         igral, err, *_ = algorithm_4(f, a, b, tol=tol)
-        assert all((l.err + err >= abs(l.igral - igral)) for l in learners)
+        assert all((lrn.err + err >= abs(lrn.igral - igral)) for lrn in learners)
 
         # Check that the errors are finite
         for learner in learners:
             assert np.isfinite(learner.err)
 
 
 # XXX: This *should* pass (https://github.com/python-adaptive/adaptive/issues/55)
@@ -231,36 +229,36 @@
     learner = IntegratorLearner(f24, bounds=(0, 3), tol=1e-10)
 
     xs, _ = learner.ask(10000)
     random.shuffle(xs)
     for x in xs:
         learner.tell(x, f24(x))
 
-    ivals = sorted(learner.approximating_intervals, key=lambda l: l.a)
+    ivals = sorted(learner.approximating_intervals, key=lambda lrn: lrn.a)
     for i in range(len(ivals) - 1):
         assert ivals[i].b == ivals[i + 1].a, (ivals[i], ivals[i + 1])
 
 
 # XXX: This *should* pass (https://github.com/python-adaptive/adaptive/issues/96)
 @pytest.mark.xfail
 def test_removed_choose_mutiple_points_at_once():
     """Given that a high-precision interval that was split into 2 low-precision ones,
-       we should use the high-precision interval.
+    we should use the high-precision interval.
     """
     learner = IntegratorLearner(np.exp, bounds=(0, 1), tol=1e-15)
-    n = ns[-1] + 2 * (ns[0] - 2)  # first + two children (33+6=39)
+    n = coeff.ns[-1] + 2 * (coeff.ns[0] - 2)  # first + two children (33+6=39)
     xs, _ = learner.ask(n)
     for x in xs:
         learner.tell(x, learner.function(x))
     assert list(learner.approximating_intervals)[0] == learner.first_ival
 
 
 def test_removed_ask_one_by_one():
     with pytest.raises(RuntimeError):
         # This test should raise because integrating np.exp should be done
         # after the 33th point
         learner = IntegratorLearner(np.exp, bounds=(0, 1), tol=1e-15)
-        n = ns[-1] + 2 * (ns[0] - 2)  # first + two children (33+6=39)
+        n = coeff.ns[-1] + 2 * (coeff.ns[0] - 2)  # first + two children (33+6=39)
         for _ in range(n):
             xs, _ = learner.ask(1)
             for x in xs:
                 learner.tell(x, learner.function(x))
```

### Comparing `adaptive-0.9.0/adaptive/tests/test_learner1d.py` & `adaptive-1.0.0/adaptive/tests/test_learner1d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,31 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
 import random
+import time
+from typing import TYPE_CHECKING
 
+import flaky
 import numpy as np
 
 from adaptive.learner import Learner1D
 from adaptive.learner.learner1D import curvature_loss_function
-from adaptive.runner import simple
+from adaptive.runner import BlockingRunner, simple
+
+if TYPE_CHECKING:
+    pass
+
+
+def flat_middle(x):
+    x *= 1e7
+    xs = np.array([0.0, 0.1, 0.9, 1.0])
+    ys = [0, 1, 1, 0]
+    if x < xs[1] or x > xs[-2]:
+        time.sleep(1)
+    return np.interp(x, xs, ys)
 
 
 def test_pending_loss_intervals():
     # https://github.com/python-adaptive/adaptive/issues/40
     learner = Learner1D(lambda x: x, (0, 4))
 
     learner.tell(0, 0)
@@ -90,15 +105,15 @@
 
 
 def test_loss_interpolation():
     learner = Learner1D(lambda _: 0, bounds=(-1, 1))
 
     learner.tell(-1, 0)
     learner.tell(1, 0)
-    for i in range(100):
+    for _i in range(100):
         # Add a 100 points with either None or 0
         if random.random() < 0.9:
             learner.tell_pending(random.uniform(-1, 1))
         else:
             learner.tell(random.uniform(-1, 1), 0)
 
     for (x1, x2), loss in learner.losses_combined.items():
@@ -115,15 +130,14 @@
         (x,), _ = learner.ask(1)
         learner.tell(x, learner.function(x))
 
     return learner
 
 
 def test_termination_on_discontinuities():
-
     learner = _run_on_discontinuity(0, (-1, 1))
     smallest_interval = min(abs(a - b) for a, b in learner.losses.keys())
     assert smallest_interval >= np.finfo(float).eps
 
     learner = _run_on_discontinuity(1, (-2, 2))
     smallest_interval = min(abs(a - b) for a, b in learner.losses.keys())
     assert smallest_interval >= np.finfo(float).eps
@@ -154,15 +168,15 @@
 def test_loss_at_machine_precision_interval_is_zero():
     """The loss of an interval smaller than _dx_eps
     should be set to zero."""
 
     def f(x):
         return 1 if x == 0 else 0
 
-    def goal(l):
+    def goal(learner):
         return learner.loss() < 0.01 or learner.npoints >= 1000
 
     learner = Learner1D(f, bounds=(-1, 1))
     simple(learner, goal=goal)
 
     # this means loss < 0.01 was reached
     assert learner.npoints != 1000
@@ -181,15 +195,15 @@
     learner = Learner1D(small_deviations, bounds=(1 - eps, 1 + eps))
 
     # Some non-determinism is needed to make this test fail so we keep
     # a list of points that will be evaluated later to emulate
     # parallel execution
     stash = []
 
-    for i in range(100):
+    for _i in range(100):
         xs, _ = learner.ask(10)
 
         # Save 5 random points out of `xs` for later
         random.shuffle(xs)
         for _ in range(5):
             stash.append(xs.pop())
 
@@ -244,35 +258,36 @@
 def test_ask_does_not_return_known_points_when_returning_bounds():
     learner = Learner1D(lambda x: None, (-1, 1))
     learner.tell(0, 0)
     points, _ = learner.ask(3)
     assert 0 not in points
 
 
+@flaky.flaky(max_runs=3)
 def test_tell_many():
     def f(x, offset=0.123214):
         a = 0.01
         return (
-            np.sin(x ** 2)
-            + np.sin(x ** 5)
-            + a ** 2 / (a ** 2 + (x - offset) ** 2)
-            + x ** 2
-            + 1e-5 * x ** 3
+            np.sin(x**2)
+            + np.sin(x**5)
+            + a**2 / (a**2 + (x - offset) ** 2)
+            + x**2
+            + 1e-5 * x**3
         )
 
     def f_vec(x, offset=0.123214):
         a = 0.01
-        y = x + a ** 2 / (a ** 2 + (x - offset) ** 2)
-        return [y, 0.5 * y, y ** 2]
+        y = x + a**2 / (a**2 + (x - offset) ** 2)
+        return [y, 0.5 * y, y**2]
 
     def assert_equal_dicts(d1, d2):
         xs1, ys1 = zip(*sorted(d1.items()))
         xs2, ys2 = zip(*sorted(d2.items()))
-        ys1 = np.array(ys1, dtype=np.float)
-        ys2 = np.array(ys2, dtype=np.float)
+        ys1 = np.array(ys1, dtype=np.float64)
+        ys2 = np.array(ys2, dtype=np.float64)
         np.testing.assert_almost_equal(xs1, xs2)
         np.testing.assert_almost_equal(ys1, ys2)
 
     def test_equal(l1, l2):
         assert_equal_dicts(l1.neighbors, l2.neighbors)
         assert_equal_dicts(l1.neighbors_combined, l2.neighbors_combined)
         assert_equal_dicts(l1.data, l2.data)
@@ -284,15 +299,15 @@
         np.testing.assert_almost_equal(l1._bbox[1], l1._bbox[1])
         assert l1._scale == l2._scale
         assert l1._bbox[0] == l2._bbox[0]
 
     for function in [f, f_vec]:
         learner = Learner1D(function, bounds=(-1, 1))
         learner2 = Learner1D(function, bounds=(-1, 1))
-        simple(learner, goal=lambda l: l.npoints > 200)
+        simple(learner, npoints_goal=200)
         xs, ys = zip(*learner.data.items())
 
         # Make the scale huge to no get a scale doubling
         x = 1e-6
         max_value = 1e6 if learner.vdim == 1 else np.array(learner.vdim * [1e6])
         learner.tell(x, max_value)
         learner2.tell(x, max_value)
@@ -310,15 +325,15 @@
             # Make the scale huge to no get a scale doubling
             x = 1e-6
             max_value = 1e6
             learner.tell(x, max_value)
             learner2.tell(x, max_value)
 
         stash = []
-        for i in range(10):
+        for _i in range(10):
             xs, _ = learner.ask(10)
             for x in xs:
                 learner2.tell_pending(x)
 
             # Save 5 random points out of `xs` for later
             random.shuffle(xs)
             for _ in range(5):
@@ -360,32 +375,44 @@
 def test_curvature_loss():
     def f(x):
         return np.tanh(20 * x)
 
     loss = curvature_loss_function()
     assert loss.nth_neighbors == 1
     learner = Learner1D(f, (-1, 1), loss_per_interval=loss)
-    simple(learner, goal=lambda l: l.npoints > 100)
-    assert learner.npoints > 100
+    simple(learner, npoints_goal=100)
+    assert learner.npoints >= 100
 
 
 def test_curvature_loss_vectors():
     def f(x):
         return np.tanh(20 * x), np.tanh(20 * (x - 0.4))
 
     loss = curvature_loss_function()
     assert loss.nth_neighbors == 1
     learner = Learner1D(f, (-1, 1), loss_per_interval=loss)
-    simple(learner, goal=lambda l: l.npoints > 100)
-    assert learner.npoints > 100
+    simple(learner, npoints_goal=100)
+    assert learner.npoints >= 100
 
 
 def test_NaN_loss():
     # see https://github.com/python-adaptive/adaptive/issues/145
     def f(x):
         a = 0.01
         if random.random() < 0.2:
             return np.NaN
-        return x + a ** 2 / (a ** 2 + x ** 2)
+        return x + a**2 / (a**2 + x**2)
 
     learner = Learner1D(f, bounds=(-1, 1))
-    simple(learner, lambda l: l.npoints > 100)
+    simple(learner, npoints_goal=100)
+
+
+def test_inf_loss_with_missing_bounds():
+    learner = Learner1D(
+        flat_middle,
+        bounds=(0, 1e-7),
+        loss_per_interval=curvature_loss_function(),
+    )
+    # must be done in parallel because otherwise the bounds will be evaluated first
+    BlockingRunner(learner, loss_goal=0.01)
+
+    assert learner.npoints >= 5
```

### Comparing `adaptive-0.9.0/adaptive/tests/test_learners.py` & `adaptive-1.0.0/adaptive/tests/test_learners.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-# -*- coding: utf-8 -*-
-
 import collections
 import functools as ft
 import inspect
 import itertools as it
 import math
 import operator
 import os
 import random
 import shutil
 import tempfile
+import time
 
+import flaky
 import numpy as np
 import pytest
 import scipy.spatial
 
 import adaptive
 from adaptive.learner import (
     AverageLearner,
+    AverageLearner1D,
     BalancingLearner,
     DataSaver,
     IntegratorLearner,
     Learner1D,
     Learner2D,
     LearnerND,
     SequenceLearner,
 )
+from adaptive.learner.learner1D import with_pandas
 from adaptive.runner import simple
 
 try:
-    from adaptive.learner import SKOptLearner
-except ModuleNotFoundError:
-    SKOptLearner = None
+    from adaptive.learner.skopt_learner import SKOptLearner
+except (ModuleNotFoundError, ImportError):
+    # XXX: catch the ImportError because of https://github.com/scikit-optimize/scikit-optimize/issues/902
+    SKOptLearner = None  # type: ignore[assignment,misc]
 
 
 LOSS_FUNCTIONS = {
     Learner1D: (
         "loss_per_interval",
         (
             adaptive.learner.learner1D.default_loss,
@@ -82,14 +85,31 @@
     return ft.partial(f, **realization)
 
 
 def uniform(a, b):
     return lambda: random.uniform(a, b)
 
 
+def simple_run(learner, n):
+    def get_goal(learner):
+        if hasattr(learner, "nsamples"):
+            return lambda lrn: lrn.nsamples > n
+        else:
+            return lambda lrn: lrn.npoints > n
+
+    def goal():
+        if isinstance(learner, BalancingLearner):
+            return get_goal(learner.learners[0])
+        elif isinstance(learner, DataSaver):
+            return get_goal(learner.learner)
+        return get_goal(learner)
+
+    simple(learner, goal=goal())
+
+
 # Library of functions and associated learners.
 
 learner_function_combos = collections.defaultdict(list)
 
 
 def learn_with(learner_type, **init_kwargs):
     def _(f):
@@ -108,46 +128,59 @@
 
 
 # All parameters except the first must be annotated with a callable that
 # returns a random value for that parameter.
 
 
 @learn_with(Learner1D, bounds=(-1, 1))
-def quadratic(x, m: uniform(0, 10), b: uniform(0, 1)):
-    return m * x ** 2 + b
+def quadratic(x, m: uniform(1, 4), b: uniform(0, 1)):  # type: ignore[valid-type]
+    return m * x**2 + b
 
 
 @learn_with(Learner1D, bounds=(-1, 1))
 @learn_with(SequenceLearner, sequence=np.linspace(-1, 1, 201))
-def linear_with_peak(x, d: uniform(-1, 1)):
+def linear_with_peak(x, d: uniform(-1, 1)):  # type: ignore[valid-type]
     a = 0.01
-    return x + a ** 2 / (a ** 2 + (x - d) ** 2)
+    return x + a**2 / (a**2 + (x - d) ** 2)
 
 
 @learn_with(LearnerND, bounds=((-1, 1), (-1, 1)))
 @learn_with(Learner2D, bounds=((-1, 1), (-1, 1)))
 @learn_with(SequenceLearner, sequence=np.random.rand(1000, 2))
-def ring_of_fire(xy, d: uniform(0.2, 1)):
+def ring_of_fire(xy, d: uniform(0.2, 1)):  # type: ignore[valid-type]
     a = 0.2
     x, y = xy
-    return x + math.exp(-(x ** 2 + y ** 2 - d ** 2) ** 2 / a ** 4)
+    return x + math.exp(-((x**2 + y**2 - d**2) ** 2) / a**4)
 
 
 @learn_with(LearnerND, bounds=((-1, 1), (-1, 1), (-1, 1)))
 @learn_with(SequenceLearner, sequence=np.random.rand(1000, 3))
-def sphere_of_fire(xyz, d: uniform(0.2, 1)):
+def sphere_of_fire(xyz, d: uniform(0.2, 0.5)):  # type: ignore[valid-type]
     a = 0.2
     x, y, z = xyz
-    return x + math.exp(-(x ** 2 + y ** 2 + z ** 2 - d ** 2) ** 2 / a ** 4) + z ** 2
+    return x + math.exp(-((x**2 + y**2 + z**2 - d**2) ** 2) / a**4) + z**2
 
 
 @learn_with(SequenceLearner, sequence=range(1000))
 @learn_with(AverageLearner, rtol=1)
-def gaussian(n):
-    return random.gauss(0, 1)
+def gaussian(n):  # type: ignore[valid-type]
+    return random.gauss(1, 1)
+
+
+@learn_with(AverageLearner1D, bounds=(-2, 2))
+def noisy_peak(  # type: ignore[valid-type]
+    seed_x,
+    sigma: uniform(1.5, 2.5),  # type: ignore[valid-type]
+    peak_width: uniform(0.04, 0.06),  # type: ignore[valid-type]
+    offset: uniform(-0.6, -0.3),  # type: ignore[valid-type]
+):
+    seed, x = seed_x
+    y = x**3 - x + 3 * peak_width**2 / (peak_width**2 + (x - offset) ** 2)
+    noise = np.random.normal(0, sigma)
+    return y + noise
 
 
 # Decorators for tests.
 
 
 # Create a sequence of learner parameters by adding all
 # possible loss functions to an existing parameter set.
@@ -229,44 +262,44 @@
     n = math.sqrt(len(points))
     xbounds, ybounds = learner_kwargs["bounds"]
     r = math.sqrt((ybounds[1] - ybounds[0]) / (xbounds[1] - xbounds[0]))
     xs, dx = np.linspace(*xbounds, int(n / r), retstep=True)
     ys, dy = np.linspace(*ybounds, int(n * r), retstep=True)
 
     distances, neighbors = tree.query(list(it.product(xs, ys)), k=1)
-    assert max(distances) < math.sqrt(dx ** 2 + dy ** 2)
+    assert max(distances) < math.sqrt(dx**2 + dy**2)
 
 
 @pytest.mark.parametrize(
     "learner_type, bounds",
     [
         (Learner1D, (-1, 1)),
-        (Learner2D, [(-1, 1), (-1, 1)]),
-        (LearnerND, [(-1, 1), (-1, 1), (-1, 1)]),
+        (Learner2D, ((-1, 1), (-1, 1))),
+        (LearnerND, ((-1, 1), (-1, 1), (-1, 1))),
     ],
 )
 def test_learner_accepts_lists(learner_type, bounds):
     def f(x):
         return [0, 1]
 
     learner = learner_type(f, bounds=bounds)
-    simple(learner, goal=lambda l: l.npoints > 10)
+    simple_run(learner, 10)
 
 
-@run_with(Learner1D, Learner2D, LearnerND, SequenceLearner)
+@run_with(Learner1D, Learner2D, LearnerND, SequenceLearner, AverageLearner1D)
 def test_adding_existing_data_is_idempotent(learner_type, f, learner_kwargs):
     """Adding already existing data is an idempotent operation.
 
     Either it is idempotent, or it is an error.
     This is the only sane behaviour.
     """
     f = generate_random_parametrization(f)
     learner = learner_type(f, **learner_kwargs)
-    control = learner_type(f, **learner_kwargs)
-    if learner_type is Learner1D:
+    control = learner.new()
+    if learner_type in (Learner1D, AverageLearner1D):
         learner._recompute_losses_factor = 1
         control._recompute_losses_factor = 1
 
     N = random.randint(10, 30)
     control.ask(N)
     xs, _ = learner.ask(N)
     points = [(x, learner.function(x)) for x in xs]
@@ -295,21 +328,28 @@
     else:
         # Point ordering is not defined, so compare as sets
         assert set(pls) == set(cpls)
 
 
 # XXX: This *should* pass (https://github.com/python-adaptive/adaptive/issues/55)
 #      but we xfail it now, as Learner2D will be deprecated anyway
-@run_with(Learner1D, xfail(Learner2D), LearnerND, AverageLearner, SequenceLearner)
+@run_with(
+    Learner1D,
+    xfail(Learner2D),
+    LearnerND,
+    AverageLearner,
+    AverageLearner1D,
+    SequenceLearner,
+)
 def test_adding_non_chosen_data(learner_type, f, learner_kwargs):
     """Adding data for a point that was not returned by 'ask'."""
     # XXX: learner, control and bounds are not defined
     f = generate_random_parametrization(f)
     learner = learner_type(f, **learner_kwargs)
-    control = learner_type(f, **learner_kwargs)
+    control = learner.new()
 
     if learner_type is Learner2D:
         # If the stack_size is bigger then the number of points added,
         # ask will return a point from the _stack.
         learner.stack_size = 1
         control.stack_size = 1
 
@@ -337,29 +377,31 @@
         assert indices == cindices
     else:
         # Point ordering within a single call to 'ask'
         # is not guaranteed to be the same by the API.
         assert set(pls) == set(cpls)
 
 
-@run_with(Learner1D, xfail(Learner2D), xfail(LearnerND), AverageLearner)
+@run_with(
+    Learner1D, xfail(Learner2D), xfail(LearnerND), AverageLearner, AverageLearner1D
+)
 def test_point_adding_order_is_irrelevant(learner_type, f, learner_kwargs):
     """The order of calls to 'tell' between calls to 'ask'
     is arbitrary.
 
     This test will fail for the Learner2D because
     `interpolate.interpnd.estimate_gradients_2d_global` will give different
     outputs based on the order of the triangles and values in
     (ip.tri, ip.values). Therefore the _stack will contain different points.
     """
     f = generate_random_parametrization(f)
     learner = learner_type(f, **learner_kwargs)
-    control = learner_type(f, **learner_kwargs)
+    control = learner.new()
 
-    if learner_type is Learner1D:
+    if learner_type in (Learner1D, AverageLearner1D):
         learner._recompute_losses_factor = 1
         control._recompute_losses_factor = 1
 
     N = random.randint(10, 30)
     control.ask(N)
     xs, _ = learner.ask(N)
     points = [(x, learner.function(x)) for x in xs]
@@ -368,103 +410,125 @@
         control.tell(*p)
 
     random.shuffle(points)
     for p in points:
         learner.tell(*p)
 
     M = random.randint(10, 30)
-    pls = zip(*learner.ask(M))
-    cpls = zip(*control.ask(M))
+    pls = sorted(zip(*learner.ask(M)))
+    cpls = sorted(zip(*control.ask(M)))
     # Point ordering within a single call to 'ask'
     # is not guaranteed to be the same by the API.
     # We compare the sorted points instead of set, because the points
     # should only be identical up to machine precision.
-    np.testing.assert_almost_equal(sorted(pls), sorted(cpls))
+    if isinstance(pls[0][0], tuple):
+        # This is the case for AverageLearner1D
+        pls = [(*x, y) for x, y in pls]
+        cpls = [(*x, y) for x, y in cpls]
+    np.testing.assert_almost_equal(pls, cpls)
 
 
 # XXX: the Learner2D fails with ~50% chance
 # see https://github.com/python-adaptive/adaptive/issues/55
-@run_with(Learner1D, xfail(Learner2D), LearnerND, AverageLearner)
+@run_with(Learner1D, xfail(Learner2D), LearnerND, AverageLearner, AverageLearner1D)
 def test_expected_loss_improvement_is_less_than_total_loss(
     learner_type, f, learner_kwargs
 ):
     """The estimated loss improvement can never be greater than the total loss."""
     f = generate_random_parametrization(f)
     learner = learner_type(f, **learner_kwargs)
-    N = random.randint(50, 100)
-    xs, loss_improvements = learner.ask(N)
-
-    for x in xs:
-        learner.tell(x, learner.function(x))
+    for _ in range(2):
+        # We do this twice to make sure that the AverageLearner1D
+        # has two different points in `x`.
+        N = random.randint(50, 100)
+        xs, loss_improvements = learner.ask(N)
+        for x in xs:
+            learner.tell(x, learner.function(x))
 
     M = random.randint(50, 100)
     _, loss_improvements = learner.ask(M)
 
     if learner_type is Learner2D:
-        assert sum(loss_improvements) < sum(learner.loss_per_triangle(learner.ip()))
-    elif learner_type is Learner1D:
+        assert sum(loss_improvements) < sum(
+            learner.loss_per_triangle(learner.interpolator(scaled=True))
+        )
+    elif learner_type in (Learner1D, AverageLearner1D):
         assert sum(loss_improvements) < sum(learner.losses.values())
     elif learner_type is AverageLearner:
         assert sum(loss_improvements) < learner.loss()
 
 
 # XXX: This *should* pass (https://github.com/python-adaptive/adaptive/issues/55)
 #      but we xfail it now, as Learner2D will be deprecated anyway
-@run_with(Learner1D, xfail(Learner2D), LearnerND)
+@run_with(Learner1D, xfail(Learner2D), LearnerND, AverageLearner1D)
 def test_learner_performance_is_invariant_under_scaling(
     learner_type, f, learner_kwargs
 ):
     """Learners behave identically under transformations that leave
        the loss invariant.
 
     This is a statement that the learner makes decisions based solely
     on the loss function.
     """
     # for now we just scale X and Y by random factors
     f = generate_random_parametrization(f)
+    if learner_type is AverageLearner1D:
+        # no noise for AverageLearner1D to make it deterministic
+        f = ft.partial(f, sigma=0)
 
     control_kwargs = dict(learner_kwargs)
     control = learner_type(f, **control_kwargs)
 
     xscale = 1000 * random.random()
     yscale = 1000 * random.random()
 
     l_kwargs = dict(learner_kwargs)
-    l_kwargs["bounds"] = xscale * np.array(l_kwargs["bounds"])
-    learner = learner_type(lambda x: yscale * f(np.array(x) / xscale), **l_kwargs)
+    bounds = xscale * np.array(l_kwargs["bounds"])
+    bounds = tuple((bounds).tolist())  # to satisfy typeguard tests
+    l_kwargs["bounds"] = bounds
+
+    def scale_x(x):
+        if isinstance(learner, AverageLearner1D):
+            seed, x = x
+            return (seed, x / xscale)
+        return np.array(x) / xscale
+
+    learner = learner_type(lambda x: yscale * f(scale_x(x)), **l_kwargs)
 
-    if learner_type in [Learner1D, LearnerND]:
+    if learner_type in [Learner1D, LearnerND, AverageLearner1D]:
         learner._recompute_losses_factor = 1
         control._recompute_losses_factor = 1
 
     npoints = random.randrange(300, 500)
 
     if learner_type is LearnerND:
         # Because the LearnerND is slow
         npoints //= 10
 
-    for n in range(npoints):
+    for _n in range(npoints):
         cxs, _ = control.ask(1)
         xs, _ = learner.ask(1)
         control.tell_many(cxs, [control.function(x) for x in cxs])
         learner.tell_many(xs, [learner.function(x) for x in xs])
 
         # Check whether the points returned are the same
-        xs_unscaled = np.array(xs) / xscale
+        xs_unscaled = [scale_x(x) for x in xs]
         assert np.allclose(xs_unscaled, cxs)
 
     # Check if the losses are close
     assert math.isclose(learner.loss(), control.loss(), rel_tol=1e-10)
 
 
+@flaky.flaky(max_runs=10)
 @run_with(
     Learner1D,
     Learner2D,
     LearnerND,
     AverageLearner,
+    AverageLearner1D,
     SequenceLearner,
     with_all_loss_functions=False,
 )
 def test_balancing_learner(learner_type, f, learner_kwargs):
     """Test if the BalancingLearner works with the different types of learners."""
     learners = [
         learner_type(generate_random_parametrization(f), **learner_kwargs)
@@ -472,15 +536,15 @@
     ]
 
     learner = BalancingLearner(learners)
 
     # Emulate parallel execution
     stash = []
 
-    for i in range(100):
+    for _i in range(100):
         n = random.randint(1, 10)
         m = random.randint(0, n)
         xs, _ = learner.ask(n, tell_pending=False)
 
         # Save 'm' random points out of `xs` for later
         random.shuffle(xs)
         for _ in range(m):
@@ -491,120 +555,128 @@
 
         # Evaluate and add 'm' random points from `stash`
         random.shuffle(stash)
         for _ in range(m):
             x = stash.pop()
             learner.tell(x, learner.function(x))
 
-    assert all(l.npoints > 10 for l in learner.learners), [
-        l.npoints for l in learner.learners
-    ]
+    if learner_type is AverageLearner1D:
+        nsamples = [lrn.nsamples for lrn in learner.learners]
+        assert all(lrn.nsamples > 5 for lrn in learner.learners), nsamples
+    else:
+        npoints = [lrn.npoints for lrn in learner.learners]
+        assert all(lrn.npoints > 5 for lrn in learner.learners), npoints
 
 
 @run_with(
     Learner1D,
     Learner2D,
     LearnerND,
     AverageLearner,
+    AverageLearner1D,
     maybe_skip(SKOptLearner),
     IntegratorLearner,
     SequenceLearner,
     with_all_loss_functions=False,
 )
 def test_saving(learner_type, f, learner_kwargs):
     f = generate_random_parametrization(f)
     learner = learner_type(f, **learner_kwargs)
-    control = learner_type(f, **learner_kwargs)
-    if learner_type is Learner1D:
+    control = learner.new()
+    if learner_type in (Learner1D, AverageLearner1D):
         learner._recompute_losses_factor = 1
         control._recompute_losses_factor = 1
-    simple(learner, lambda l: l.npoints > 100)
+    simple_run(learner, 100)
     fd, path = tempfile.mkstemp()
+    os.close(fd)
     try:
         learner.save(path)
         control.load(path)
 
         np.testing.assert_almost_equal(learner.loss(), control.loss())
 
         # Try if the control is runnable
-        simple(control, lambda l: l.npoints > 200)
+        simple_run(control, 200)
     finally:
         os.remove(path)
 
 
 @run_with(
     Learner1D,
     Learner2D,
     LearnerND,
     AverageLearner,
+    AverageLearner1D,
     maybe_skip(SKOptLearner),
     IntegratorLearner,
     SequenceLearner,
     with_all_loss_functions=False,
 )
 def test_saving_of_balancing_learner(learner_type, f, learner_kwargs):
     f = generate_random_parametrization(f)
     learner = BalancingLearner([learner_type(f, **learner_kwargs)])
-    control = BalancingLearner([learner_type(f, **learner_kwargs)])
+    control = learner.new()
 
-    if learner_type is Learner1D:
-        for l, c in zip(learner.learners, control.learners):
-            l._recompute_losses_factor = 1
+    if learner_type in (Learner1D, AverageLearner1D):
+        for lrn, c in zip(learner.learners, control.learners):
+            lrn._recompute_losses_factor = 1
             c._recompute_losses_factor = 1
 
-    simple(learner, lambda l: l.learners[0].npoints > 100)
+    simple_run(learner, 100)
     folder = tempfile.mkdtemp()
 
     def fname(learner):
         return folder + "test"
 
     try:
         learner.save(fname=fname)
         control.load(fname=fname)
 
         np.testing.assert_almost_equal(learner.loss(), control.loss())
 
         # Try if the control is runnable
-        simple(control, lambda l: l.learners[0].npoints > 200)
+        simple_run(control, 200)
     finally:
         shutil.rmtree(folder)
 
 
 @run_with(
     Learner1D,
     Learner2D,
     LearnerND,
     AverageLearner,
+    AverageLearner1D,
     maybe_skip(SKOptLearner),
     IntegratorLearner,
     with_all_loss_functions=False,
 )
 def test_saving_with_datasaver(learner_type, f, learner_kwargs):
     f = generate_random_parametrization(f)
     g = lambda x: {"y": f(x), "t": random.random()}  # noqa: E731
     arg_picker = operator.itemgetter("y")
     learner = DataSaver(learner_type(g, **learner_kwargs), arg_picker)
-    control = DataSaver(learner_type(g, **learner_kwargs), arg_picker)
+    control = learner.new()
 
-    if learner_type is Learner1D:
+    if learner_type in (Learner1D, AverageLearner1D):
         learner.learner._recompute_losses_factor = 1
         control.learner._recompute_losses_factor = 1
 
-    simple(learner, lambda l: l.npoints > 100)
+    simple_run(learner, 100)
     fd, path = tempfile.mkstemp()
+    os.close(fd)
     try:
         learner.save(path)
         control.load(path)
 
         np.testing.assert_almost_equal(learner.loss(), control.loss())
 
         assert learner.extra_data == control.extra_data
 
         # Try if the control is runnable
-        simple(control, lambda l: l.npoints > 200)
+        simple_run(learner, 200)
     finally:
         os.remove(path)
 
 
 @pytest.mark.xfail
 @run_with(Learner1D, Learner2D, LearnerND)
 def test_convergence_for_arbitrary_ordering(learner_type, f, learner_kwargs):
@@ -617,10 +689,111 @@
     raise NotImplementedError()
 
 
 @pytest.mark.xfail
 @run_with(Learner1D, Learner2D, LearnerND)
 def test_learner_subdomain(learner_type, f, learner_kwargs):
     """Learners that never receive data outside of a subdomain should
-       perform 'similarly' to learners defined on that subdomain only."""
+    perform 'similarly' to learners defined on that subdomain only."""
     # XXX: not sure how to implement this. How do we measure "performance"?
     raise NotImplementedError()
+
+
+def add_time(f):
+    @ft.wraps(f)
+    def wrapper(*args, **kwargs):
+        t0 = time.time()
+        result = f(*args, **kwargs)
+        return {"result": result, "time": time.time() - t0}
+
+    return wrapper
+
+
+@pytest.mark.skipif(not with_pandas, reason="pandas is not installed")
+@run_with(
+    Learner1D,
+    Learner2D,
+    LearnerND,
+    AverageLearner,
+    AverageLearner1D,
+    SequenceLearner,
+    IntegratorLearner,
+    with_all_loss_functions=False,
+)
+def test_to_dataframe(learner_type, f, learner_kwargs):
+    import pandas
+
+    if learner_type is LearnerND:
+        kw = {"point_names": tuple("xyz")[: len(learner_kwargs["bounds"])]}
+    else:
+        kw = {}
+
+    learner = learner_type(generate_random_parametrization(f), **learner_kwargs)
+
+    # Test empty dataframe
+    df = learner.to_dataframe(**kw)
+    assert len(df) == 0
+    assert "inputs" in df.attrs
+    assert "output" in df.attrs
+
+    # Run the learner
+    simple_run(learner, 100)
+    df = learner.to_dataframe(**kw)
+    assert isinstance(df, pandas.DataFrame)
+    if learner_type is AverageLearner1D:
+        assert len(df) == learner.nsamples
+    else:
+        assert len(df) == learner.npoints
+
+    # Add points from the DataFrame to a new empty learner
+    learner2 = learner.new()
+    learner2.load_dataframe(df, **kw)
+    assert learner2.npoints == learner.npoints
+
+    # Test this for a learner in a BalancingLearner
+    learners = [
+        learner_type(generate_random_parametrization(f), **learner_kwargs)
+        for _ in range(2)
+    ]
+    bal_learner = BalancingLearner(learners)
+    simple_run(bal_learner, 100)
+    df_bal = bal_learner.to_dataframe(**kw)
+    assert isinstance(df_bal, pandas.DataFrame)
+
+    if learner_type is not AverageLearner1D:
+        assert len(df_bal) == bal_learner.npoints
+
+    # Test loading from a DataFrame into the BalancingLearner
+    learners2 = [
+        learner_type(generate_random_parametrization(f), **learner_kwargs)
+        for _ in range(2)
+    ]
+    bal_learner2 = BalancingLearner(learners2)
+    bal_learner2.load_dataframe(df_bal, **kw)
+    assert bal_learner2.npoints == bal_learner.npoints
+
+    if learner_type is SequenceLearner:
+        # We do not test the DataSaver with the SequenceLearner
+        # because the DataSaver is not compatible with the SequenceLearner.
+        return
+
+    # Test with DataSaver
+    learner = learner_type(
+        add_time(generate_random_parametrization(f)), **learner_kwargs
+    )
+    data_saver = DataSaver(learner, operator.itemgetter("result"))
+    df = data_saver.to_dataframe(**kw)  # test if empty dataframe works
+    simple_run(data_saver, 100)
+    df = data_saver.to_dataframe(**kw)
+    if learner_type is AverageLearner1D:
+        assert len(df) == data_saver.nsamples
+    else:
+        assert len(df) == data_saver.npoints
+
+    # Test loading from a DataFrame into a new DataSaver
+    data_saver2 = data_saver.new()
+    data_saver2.load_dataframe(df, **kw)
+    assert data_saver2.extra_data.keys() == data_saver.extra_data.keys()
+    assert all(
+        data_saver2.extra_data[k] == data_saver.extra_data[k]
+        for k in data_saver.extra_data.keys()
+    )
```

### Comparing `adaptive-0.9.0/adaptive/tests/test_skopt_learner.py` & `adaptive-1.0.0/adaptive/tests/test_skopt_learner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,48 @@
-# -*- coding: utf-8 -*-
-
 import numpy as np
 import pytest
 
 try:
-    from adaptive.learner import SKOptLearner
+    from adaptive.learner.skopt_learner import SKOptLearner
 
     with_scikit_optimize = True
 except ModuleNotFoundError:
     with_scikit_optimize = False
 
 
 @pytest.mark.skipif(not with_scikit_optimize, reason="scikit-optimize is not installed")
 def test_skopt_learner_runs():
     """The SKOptLearner provides very few guarantees about its
-       behaviour, so we only test the most basic usage
+    behaviour, so we only test the most basic usage
     """
 
     def g(x, noise_level=0.1):
-        return np.sin(5 * x) * (1 - np.tanh(x ** 2)) + np.random.randn() * noise_level
+        return np.sin(5 * x) * (1 - np.tanh(x**2)) + np.random.randn() * noise_level
 
     learner = SKOptLearner(g, dimensions=[(-2.0, 2.0)])
 
     for _ in range(11):
         (x,), _ = learner.ask(1)
         learner.tell(x, learner.function(x))
+
+
+@pytest.mark.skipif(not with_scikit_optimize, reason="scikit-optimize is not installed")
+def test_skopt_learner_4D_runs():
+    """The SKOptLearner provides very few guarantees about its
+    behaviour, so we only test the most basic usage
+    In this case we test also for 4D domain
+    """
+
+    def g(x, noise_level=0.1):
+        return (
+            np.sin(5 * (x[0] + x[1] + x[2] + x[3]))
+            * (1 - np.tanh(x[0] ** 2 + x[1] ** 2 + x[2] ** 2 + x[3] ** 2))
+            + np.random.randn() * noise_level
+        )
+
+    learner = SKOptLearner(
+        g, dimensions=[(-2.0, 2.0), (-2.0, 2.0), (-2.0, 2.0), (-2.0, 2.0)]
+    )
+
+    for _ in range(11):
+        (x,), _ = learner.ask(1)
+        learner.tell(x, learner.function(x))
```

### Comparing `adaptive-0.9.0/adaptive/tests/test_triangulation.py` & `adaptive-1.0.0/adaptive/tests/test_triangulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 import itertools
 from collections import Counter
 from math import factorial
 
 import numpy as np
 import pytest
```

### Comparing `adaptive-0.9.0/adaptive/tests/unit/test_learnernd.py` & `adaptive-1.0.0/adaptive/tests/unit/test_learnernd.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from adaptive.learner.learnerND import LearnerND, curvature_loss_function
 
 
 def ring_of_fire(xy):
     a = 0.2
     d = 0.7
     x, y = xy
-    return x + math.exp(-(x ** 2 + y ** 2 - d ** 2) ** 2 / a ** 4)
+    return x + math.exp(-((x**2 + y**2 - d**2) ** 2) / a**4)
 
 
 def test_learnerND_inits_loss_depends_on_neighbors_correctly():
     learner = LearnerND(ring_of_fire, bounds=[(-1, 1), (-1, 1)])
     assert learner.nth_neighbors == 0
```

### Comparing `adaptive-0.9.0/adaptive/tests/unit/test_learnernd_integration.py` & `adaptive-1.0.0/adaptive/tests/unit/test_learnernd_integration.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,42 +7,42 @@
 from adaptive.runner import BlockingRunner
 from adaptive.runner import simple as SimpleRunner
 
 
 def ring_of_fire(xy, d=0.75):
     a = 0.2
     x, y = xy
-    return x + math.exp(-(x ** 2 + y ** 2 - d ** 2) ** 2 / a ** 4)
+    return x + math.exp(-((x**2 + y**2 - d**2) ** 2) / a**4)
 
 
 def test_learnerND_runs_to_10_points():
     learner = LearnerND(ring_of_fire, bounds=[(-1, 1), (-1, 1)])
-    SimpleRunner(learner, goal=lambda l: l.npoints >= 10)
+    SimpleRunner(learner, npoints_goal=10)
     assert learner.npoints == 10
 
 
 @pytest.mark.parametrize("execution_number", range(5))
 def test_learnerND_runs_to_10_points_Blocking(execution_number):
     learner = LearnerND(ring_of_fire, bounds=[(-1, 1), (-1, 1)])
-    BlockingRunner(learner, goal=lambda l: l.npoints >= 10)
+    BlockingRunner(learner, npoints_goal=10)
     assert learner.npoints >= 10
 
 
 def test_learnerND_curvature_runs_to_10_points():
     loss = curvature_loss_function()
     learner = LearnerND(ring_of_fire, bounds=[(-1, 1), (-1, 1)], loss_per_simplex=loss)
-    SimpleRunner(learner, goal=lambda l: l.npoints >= 10)
+    SimpleRunner(learner, npoints_goal=10)
     assert learner.npoints == 10
 
 
 @pytest.mark.parametrize("execution_number", range(5))
 def test_learnerND_curvature_runs_to_10_points_Blocking(execution_number):
     loss = curvature_loss_function()
     learner = LearnerND(ring_of_fire, bounds=[(-1, 1), (-1, 1)], loss_per_simplex=loss)
-    BlockingRunner(learner, goal=lambda l: l.npoints >= 10)
+    BlockingRunner(learner, npoints_goal=10)
     assert learner.npoints >= 10
 
 
 def test_learnerND_log_works():
     loss = curvature_loss_function()
     learner = LearnerND(ring_of_fire, bounds=[(-1, 1), (-1, 1)], loss_per_simplex=loss)
     learner.ask(4)
```

### Comparing `adaptive-0.9.0/adaptive.egg-info/SOURCES.txt` & `adaptive-1.0.0/adaptive.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,50 @@
+AUTHORS.md
 LICENSE
 MANIFEST.in
-README.rst
-setup.py
+README.md
+pyproject.toml
+setup.cfg
 adaptive/__init__.py
-adaptive/_static_version.py
 adaptive/_version.py
 adaptive/notebook_integration.py
 adaptive/runner.py
+adaptive/types.py
 adaptive/utils.py
 adaptive.egg-info/PKG-INFO
 adaptive.egg-info/SOURCES.txt
 adaptive.egg-info/dependency_links.txt
 adaptive.egg-info/requires.txt
 adaptive.egg-info/top_level.txt
 adaptive/learner/__init__.py
 adaptive/learner/average_learner.py
+adaptive/learner/average_learner1D.py
 adaptive/learner/balancing_learner.py
 adaptive/learner/base_learner.py
 adaptive/learner/data_saver.py
 adaptive/learner/integrator_coeffs.py
 adaptive/learner/integrator_learner.py
 adaptive/learner/learner1D.py
 adaptive/learner/learner2D.py
 adaptive/learner/learnerND.py
 adaptive/learner/sequence_learner.py
 adaptive/learner/skopt_learner.py
 adaptive/learner/triangulation.py
 adaptive/tests/__init__.py
 adaptive/tests/algorithm_4.py
 adaptive/tests/test_average_learner.py
+adaptive/tests/test_average_learner1d.py
 adaptive/tests/test_balancing_learner.py
 adaptive/tests/test_cquad.py
 adaptive/tests/test_learner1d.py
 adaptive/tests/test_learnernd.py
 adaptive/tests/test_learners.py
 adaptive/tests/test_notebook_integration.py
+adaptive/tests/test_pickling.py
 adaptive/tests/test_runner.py
+adaptive/tests/test_sequence_learner.py
 adaptive/tests/test_skopt_learner.py
 adaptive/tests/test_triangulation.py
 adaptive/tests/unit/__init__.py
 adaptive/tests/unit/test_learnernd.py
 adaptive/tests/unit/test_learnernd_integration.py
 adaptive/tests/unit/test_triangulation.py
```

