# Comparing `tmp/baseflow-0.0.6.tar.gz` & `tmp/baseflow-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseflow-0.0.6.tar", last modified: Wed Apr 26 08:34:16 2023, max compression
+gzip compressed data, was "baseflow-0.0.7.tar", last modified: Mon May 15 18:13:35 2023, max compression
```

## Comparing `baseflow-0.0.6.tar` & `baseflow-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 08:34:16.311876 baseflow-0.0.6/
--rw-rw-rw-   0        0        0     2696 2023-04-26 08:34:16.311876 baseflow-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2036 2023-03-20 14:16:11.000000 baseflow-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 08:34:16.295880 baseflow-0.0.6/baseflow/
--rw-rw-rw-   0        0        0      251 2023-03-20 14:08:26.000000 baseflow-0.0.6/baseflow/__init__.py
--rw-rw-rw-   0        0        0     3502 2023-02-16 04:15:40.000000 baseflow-0.0.6/baseflow/comparision.py
--rw-rw-rw-   0        0        0   678801 2021-11-26 09:44:13.000000 baseflow-0.0.6/baseflow/example.csv
-drwxrwxrwx   0        0        0        0 2023-04-26 08:34:16.310877 baseflow-0.0.6/baseflow/methods/
--rw-rw-rw-   0        0        0      686 2023-02-09 18:09:45.000000 baseflow-0.0.6/baseflow/methods/Boughton.py
--rw-rw-rw-   0        0        0      611 2023-02-09 17:52:56.000000 baseflow-0.0.6/baseflow/methods/CM.py
--rw-rw-rw-   0        0        0      630 2023-02-09 17:52:56.000000 baseflow-0.0.6/baseflow/methods/Chapman.py
--rw-rw-rw-   0        0        0      633 2023-02-09 18:12:19.000000 baseflow-0.0.6/baseflow/methods/EWMA.py
--rw-rw-rw-   0        0        0      710 2023-02-09 18:09:15.000000 baseflow-0.0.6/baseflow/methods/Eckhardt.py
--rw-rw-rw-   0        0        0      660 2023-04-26 08:31:08.000000 baseflow-0.0.6/baseflow/methods/Fixed.py
--rw-rw-rw-   0        0        0      684 2023-02-09 18:10:00.000000 baseflow-0.0.6/baseflow/methods/Furey.py
--rw-rw-rw-   0        0        0      949 2023-02-09 17:52:56.000000 baseflow-0.0.6/baseflow/methods/LH.py
--rw-rw-rw-   0        0        0     1568 2023-04-26 08:31:14.000000 baseflow-0.0.6/baseflow/methods/Local.py
--rw-rw-rw-   0        0        0      796 2023-04-26 08:31:49.000000 baseflow-0.0.6/baseflow/methods/Slide.py
--rw-rw-rw-   0        0        0     1552 2023-04-26 08:31:56.000000 baseflow-0.0.6/baseflow/methods/UKIH.py
--rw-rw-rw-   0        0        0      810 2023-02-09 18:10:14.000000 baseflow-0.0.6/baseflow/methods/Willems.py
--rw-rw-rw-   0        0        0      458 2021-09-23 13:22:08.000000 baseflow-0.0.6/baseflow/methods/__init__.py
--rw-rw-rw-   0        0        0     2838 2023-04-26 08:30:39.000000 baseflow-0.0.6/baseflow/param_estimate.py
--rw-rw-rw-   0        0        0     2464 2023-03-20 15:16:19.000000 baseflow-0.0.6/baseflow/separation.py
--rw-rw-rw-   0        0        0     3842 2023-02-21 18:18:24.000000 baseflow-0.0.6/baseflow/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-26 08:34:16.299878 baseflow-0.0.6/baseflow.egg-info/
--rw-rw-rw-   0        0        0     2696 2023-04-26 08:34:16.000000 baseflow-0.0.6/baseflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-04-26 08:34:16.000000 baseflow-0.0.6/baseflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 08:34:16.000000 baseflow-0.0.6/baseflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-26 08:34:16.000000 baseflow-0.0.6/baseflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-26 08:34:16.000000 baseflow-0.0.6/baseflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 08:34:16.311876 baseflow-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     3997 2023-04-26 08:32:45.000000 baseflow-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 18:13:35.818788 baseflow-0.0.7/
+-rw-rw-rw-   0        0        0     2696 2023-05-15 18:13:35.817788 baseflow-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1964 2023-04-25 17:32:50.000000 baseflow-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 18:13:35.801788 baseflow-0.0.7/baseflow/
+-rw-rw-rw-   0        0        0      243 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/__init__.py
+-rw-rw-rw-   0        0        0     3424 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/comparision.py
+-rw-rw-rw-   0        0        0   644797 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/example.csv
+drwxrwxrwx   0        0        0        0 2023-05-15 18:13:35.816788 baseflow-0.0.7/baseflow/methods/
+-rw-rw-rw-   0        0        0      661 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Boughton.py
+-rw-rw-rw-   0        0        0      587 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/CM.py
+-rw-rw-rw-   0        0        0      606 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Chapman.py
+-rw-rw-rw-   0        0        0      609 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/EWMA.py
+-rw-rw-rw-   0        0        0      685 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Eckhardt.py
+-rw-rw-rw-   0        0        0      644 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Fixed.py
+-rw-rw-rw-   0        0        0      659 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Furey.py
+-rw-rw-rw-   0        0        0      914 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/LH.py
+-rw-rw-rw-   0        0        0     1534 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Local.py
+-rw-rw-rw-   0        0        0      781 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Slide.py
+-rw-rw-rw-   0        0        0     1510 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/UKIH.py
+-rw-rw-rw-   0        0        0      783 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Willems.py
+-rw-rw-rw-   0        0        0      446 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/__init__.py
+-rw-rw-rw-   0        0        0     2766 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/param_estimate.py
+-rw-rw-rw-   0        0        0     2393 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/separation.py
+-rw-rw-rw-   0        0        0     3729 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 18:13:35.805787 baseflow-0.0.7/baseflow.egg-info/
+-rw-rw-rw-   0        0        0     2696 2023-05-15 18:13:35.000000 baseflow-0.0.7/baseflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-05-15 18:13:35.000000 baseflow-0.0.7/baseflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 18:13:35.000000 baseflow-0.0.7/baseflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-15 18:13:35.000000 baseflow-0.0.7/baseflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 18:13:35.000000 baseflow-0.0.7/baseflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 18:13:35.818788 baseflow-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     3863 2023-05-15 18:11:53.000000 baseflow-0.0.7/setup.py
```

### Comparing `baseflow-0.0.6/PKG-INFO` & `baseflow-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseflow
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python package for baseflow separation
 Home-page: https://github.com/xiejx5/baseflow
 Author: Cody James
 Author-email: xiejx5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `baseflow-0.0.6/README.md` & `baseflow-0.0.7/baseflow.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: baseflow
+Version: 0.0.7
+Summary: A python package for baseflow separation
+Home-page: https://github.com/xiejx5/baseflow
+Author: Cody James
+Author-email: xiejx5@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+Provides-Extra: fancy feature
+
+
 <div align="center">
 
 # baseflow
 
 An open-source Python package for baseflow separation 🔥<br>
 
 </div>
```

### Comparing `baseflow-0.0.6/baseflow/comparision.py` & `baseflow-0.0.7/baseflow/comparision.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import numpy as np
-
-
-def strict_baseflow(Q, ice=None):
-    dQ = (Q[2:] - Q[:-2]) / 2
-
-    # 1. flow data associated with positive and zero values of dy / dt
-    wet1 = np.concatenate([[True], dQ >= 0, [True]])
-
-    # 2. previous 2 points before points with dy/dt≥0, as well as the next 3 points
-    idx_first = np.where(wet1[1:].astype(int) - wet1[:-1].astype(int) == 1)[0] + 1
-    idx_last = np.where(wet1[1:].astype(int) - wet1[:-1].astype(int) == -1)[0]
-    idx_before = np.repeat([idx_first], 2) - np.tile(range(1, 3), idx_first.shape)
-    idx_next = np.repeat([idx_last], 3) + np.tile(range(1, 4), idx_last.shape)
-    idx_remove = np.concatenate([idx_before, idx_next])
-    wet2 = np.full(Q.shape, False)
-    wet2[idx_remove.clip(min=0, max=Q.shape[0] - 1)] = True
-
-    # 3. five data points after major events (90th quantile)
-    growing = np.concatenate([[True], (Q[1:] - Q[:-1]) >= 0, [True]])
-    idx_major = np.where((Q >= np.quantile(Q, 0.9)) & growing[:-1] & ~growing[1:])[0]
-    idx_after = np.repeat([idx_major], 5) + np.tile(range(1, 6), idx_major.shape)
-    wet3 = np.full(Q.shape, False)
-    wet3[idx_after.clip(min=0, max=Q.shape[0] - 1)] = True
-
-    # 4. flow data followed by a data point with a larger value of -dy / dt
-    wet4 = np.concatenate([[True], dQ[1:] - dQ[:-1] < 0, [True, True]])
-
-    # dry points, namely strict baseflow
-    dry = ~(wet1 + wet2 + wet3 + wet4)
-
-   # avoid ice conditions which invalidate the groundwater-baseflow relationship
-    if ice is not None:
-        dry[ice] = False
-
-    return dry
-
-
-def KGE(simulations, evaluation):
-    """Original Kling-Gupta Efficiency (KGE) and its three components
-    (r, α, β) as per `Gupta et al., 2009
-    <https://doi.org/10.1016/j.jhydrol.2009.08.003>`_.
-    Note, all four values KGE, r, α, β are returned, in this order.
-    :Calculation Details:
-        .. math::
-           E_{\\text{KGE}} = 1 - \\sqrt{[r - 1]^2 + [\\alpha - 1]^2
-           + [\\beta - 1]^2}
-        .. math::
-           r = \\frac{\\text{cov}(e, s)}{\\sigma({e}) \\cdot \\sigma(s)}
-        .. math::
-           \\alpha = \\frac{\\sigma(s)}{\\sigma(e)}
-        .. math::
-           \\beta = \\frac{\\mu(s)}{\\mu(e)}
-        where *e* is the *evaluation* series, *s* is (one of) the
-        *simulations* series, *cov* is the covariance, *σ* is the
-        standard deviation, and *μ* is the arithmetic mean.
-    """
-    # calculate error in timing and dynamics r
-    # (Pearson's correlation coefficient)
-    sim_mean = np.mean(simulations, axis=0, dtype=np.float64)
-    obs_mean = np.mean(evaluation, axis=0, dtype=np.float64)
-
-    r_num = np.sum((simulations - sim_mean) * (evaluation - obs_mean),
-                   axis=0, dtype=np.float64)
-    r_den = np.sqrt(np.sum((simulations - sim_mean) ** 2,
-                           axis=0, dtype=np.float64)
-                    * np.sum((evaluation - obs_mean) ** 2,
-                             axis=0, dtype=np.float64))
-    r = r_num / (r_den + 1e-10)
-    # calculate error in spread of flow alpha
-    alpha = np.std(simulations, axis=0) / (np.std(evaluation, axis=0) + 1e-10)
-    # calculate error in volume beta (bias of mean discharge)
-    beta = (np.sum(simulations, axis=0, dtype=np.float64)
-            / (np.sum(evaluation, axis=0, dtype=np.float64) + 1e-10))
-    # calculate the Kling-Gupta Efficiency KGE
-    kge_ = 1 - np.sqrt((r - 1) ** 2 + (alpha - 1) ** 2 + (beta - 1) ** 2)
-
-    return kge_
+import numpy as np
+
+
+def strict_baseflow(Q, ice=None):
+    dQ = (Q[2:] - Q[:-2]) / 2
+
+    # 1. flow data associated with positive and zero values of dy / dt
+    wet1 = np.concatenate([[True], dQ >= 0, [True]])
+
+    # 2. previous 2 points before points with dy/dt≥0, as well as the next 3 points
+    idx_first = np.where(wet1[1:].astype(int) - wet1[:-1].astype(int) == 1)[0] + 1
+    idx_last = np.where(wet1[1:].astype(int) - wet1[:-1].astype(int) == -1)[0]
+    idx_before = np.repeat([idx_first], 2) - np.tile(range(1, 3), idx_first.shape)
+    idx_next = np.repeat([idx_last], 3) + np.tile(range(1, 4), idx_last.shape)
+    idx_remove = np.concatenate([idx_before, idx_next])
+    wet2 = np.full(Q.shape, False)
+    wet2[idx_remove.clip(min=0, max=Q.shape[0] - 1)] = True
+
+    # 3. five data points after major events (90th quantile)
+    growing = np.concatenate([[True], (Q[1:] - Q[:-1]) >= 0, [True]])
+    idx_major = np.where((Q >= np.quantile(Q, 0.9)) & growing[:-1] & ~growing[1:])[0]
+    idx_after = np.repeat([idx_major], 5) + np.tile(range(1, 6), idx_major.shape)
+    wet3 = np.full(Q.shape, False)
+    wet3[idx_after.clip(min=0, max=Q.shape[0] - 1)] = True
+
+    # 4. flow data followed by a data point with a larger value of -dy / dt
+    wet4 = np.concatenate([[True], dQ[1:] - dQ[:-1] < 0, [True, True]])
+
+    # dry points, namely strict baseflow
+    dry = ~(wet1 + wet2 + wet3 + wet4)
+
+   # avoid ice conditions which invalidate the groundwater-baseflow relationship
+    if ice is not None:
+        dry[ice] = False
+
+    return dry
+
+
+def KGE(simulations, evaluation):
+    """Original Kling-Gupta Efficiency (KGE) and its three components
+    (r, α, β) as per `Gupta et al., 2009
+    <https://doi.org/10.1016/j.jhydrol.2009.08.003>`_.
+    Note, all four values KGE, r, α, β are returned, in this order.
+    :Calculation Details:
+        .. math::
+           E_{\\text{KGE}} = 1 - \\sqrt{[r - 1]^2 + [\\alpha - 1]^2
+           + [\\beta - 1]^2}
+        .. math::
+           r = \\frac{\\text{cov}(e, s)}{\\sigma({e}) \\cdot \\sigma(s)}
+        .. math::
+           \\alpha = \\frac{\\sigma(s)}{\\sigma(e)}
+        .. math::
+           \\beta = \\frac{\\mu(s)}{\\mu(e)}
+        where *e* is the *evaluation* series, *s* is (one of) the
+        *simulations* series, *cov* is the covariance, *σ* is the
+        standard deviation, and *μ* is the arithmetic mean.
+    """
+    # calculate error in timing and dynamics r
+    # (Pearson's correlation coefficient)
+    sim_mean = np.mean(simulations, axis=0, dtype=np.float64)
+    obs_mean = np.mean(evaluation, axis=0, dtype=np.float64)
+
+    r_num = np.sum((simulations - sim_mean) * (evaluation - obs_mean),
+                   axis=0, dtype=np.float64)
+    r_den = np.sqrt(np.sum((simulations - sim_mean) ** 2,
+                           axis=0, dtype=np.float64)
+                    * np.sum((evaluation - obs_mean) ** 2,
+                             axis=0, dtype=np.float64))
+    r = r_num / (r_den + 1e-10)
+    # calculate error in spread of flow alpha
+    alpha = np.std(simulations, axis=0) / (np.std(evaluation, axis=0) + 1e-10)
+    # calculate error in volume beta (bias of mean discharge)
+    beta = (np.sum(simulations, axis=0, dtype=np.float64)
+            / (np.sum(evaluation, axis=0, dtype=np.float64) + 1e-10))
+    # calculate the Kling-Gupta Efficiency KGE
+    kge_ = 1 - np.sqrt((r - 1) ** 2 + (alpha - 1) ** 2 + (beta - 1) ** 2)
+
+    return kge_
```

### Comparing `baseflow-0.0.6/baseflow/methods/Boughton.py` & `baseflow-0.0.7/baseflow/methods/Boughton.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import numpy as np
-from numba import njit
-
-
-@njit
-def Boughton(Q, b_LH, a, C, return_exceed=False):
-    """Boughton doulbe-parameter filter (Boughton, 2004)
-
-    Args:
-        Q (np.array): streamflow
-        a (float): recession coefficient
-        C (float): calibrated in baseflow.param_estimate
-    """
-    if return_exceed:
-        b = np.zeros(Q.shape[0] + 1)
-    else:
-        b = np.zeros(Q.shape[0])
-    b[0] = b_LH[0]
-    for i in range(Q.shape[0] - 1):
-        b[i + 1] = a / (1 + C) * b[i] + C / (1 + C) * Q[i + 1]
-        if b[i + 1] > Q[i + 1]:
-            b[i + 1] = Q[i + 1]
-            if return_exceed:
-                b[-1] += 1
-    return b
+import numpy as np
+from numba import njit
+
+
+@njit
+def Boughton(Q, b_LH, a, C, return_exceed=False):
+    """Boughton doulbe-parameter filter (Boughton, 2004)
+
+    Args:
+        Q (np.array): streamflow
+        a (float): recession coefficient
+        C (float): calibrated in baseflow.param_estimate
+    """
+    if return_exceed:
+        b = np.zeros(Q.shape[0] + 1)
+    else:
+        b = np.zeros(Q.shape[0])
+    b[0] = b_LH[0]
+    for i in range(Q.shape[0] - 1):
+        b[i + 1] = a / (1 + C) * b[i] + C / (1 + C) * Q[i + 1]
+        if b[i + 1] > Q[i + 1]:
+            b[i + 1] = Q[i + 1]
+            if return_exceed:
+                b[-1] += 1
+    return b
```

### Comparing `baseflow-0.0.6/baseflow/methods/CM.py` & `baseflow-0.0.7/baseflow/methods/CM.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import numpy as np
-from numba import njit
-
-
-@njit
-def CM(Q, b_LH, a, return_exceed=False):
-    """CM filter (Chapman & Maxwell, 1996)
-
-    Args:
-        Q (np.array): streamflow
-        a (float): recession coefficient
-    """
-    if return_exceed:
-        b = np.zeros(Q.shape[0] + 1)
-    else:
-        b = np.zeros(Q.shape[0])
-    b[0] = b_LH[0]
-    for i in range(Q.shape[0] - 1):
-        b[i + 1] = a / (2 - a) * b[i] + (1 - a) / (2 - a) * Q[i + 1]
-        if b[i + 1] > Q[i + 1]:
-            b[i + 1] = Q[i + 1]
-            if return_exceed:
-                b[-1] += 1
-    return b
+import numpy as np
+from numba import njit
+
+
+@njit
+def CM(Q, b_LH, a, return_exceed=False):
+    """CM filter (Chapman & Maxwell, 1996)
+
+    Args:
+        Q (np.array): streamflow
+        a (float): recession coefficient
+    """
+    if return_exceed:
+        b = np.zeros(Q.shape[0] + 1)
+    else:
+        b = np.zeros(Q.shape[0])
+    b[0] = b_LH[0]
+    for i in range(Q.shape[0] - 1):
+        b[i + 1] = a / (2 - a) * b[i] + (1 - a) / (2 - a) * Q[i + 1]
+        if b[i + 1] > Q[i + 1]:
+            b[i + 1] = Q[i + 1]
+            if return_exceed:
+                b[-1] += 1
+    return b
```

### Comparing `baseflow-0.0.6/baseflow/methods/Chapman.py` & `baseflow-0.0.7/baseflow/methods/Chapman.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import numpy as np
-from numba import njit
-
-
-@njit
-def Chapman(Q, b_LH, a, return_exceed=False):
-    """Chapman filter (Chapman, 1991)
-
-    Args:
-        Q (np.array): streamflow
-        a (float): recession coefficient
-    """
-    if return_exceed:
-        b = np.zeros(Q.shape[0] + 1)
-    else:
-        b = np.zeros(Q.shape[0])
-    b[0] = b_LH[0]
-    for i in range(Q.shape[0] - 1):
-        b[i + 1] = (3 * a - 1) / (3 - a) * b[i] + (1 - a) / (3 - a) * (Q[i + 1] + Q[i])
-        if b[i + 1] > Q[i + 1]:
-            b[i + 1] = Q[i + 1]
-            if return_exceed:
-                b[-1] += 1
-    return b
+import numpy as np
+from numba import njit
+
+
+@njit
+def Chapman(Q, b_LH, a, return_exceed=False):
+    """Chapman filter (Chapman, 1991)
+
+    Args:
+        Q (np.array): streamflow
+        a (float): recession coefficient
+    """
+    if return_exceed:
+        b = np.zeros(Q.shape[0] + 1)
+    else:
+        b = np.zeros(Q.shape[0])
+    b[0] = b_LH[0]
+    for i in range(Q.shape[0] - 1):
+        b[i + 1] = (3 * a - 1) / (3 - a) * b[i] + (1 - a) / (3 - a) * (Q[i + 1] + Q[i])
+        if b[i + 1] > Q[i + 1]:
+            b[i + 1] = Q[i + 1]
+            if return_exceed:
+                b[-1] += 1
+    return b
```

### Comparing `baseflow-0.0.6/baseflow/methods/EWMA.py` & `baseflow-0.0.7/baseflow/methods/EWMA.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import numpy as np
-from numba import njit
-
-
-@njit
-def EWMA(Q, b_LH, a, e, return_exceed=False):
-    """exponential weighted moving average (EWMA) filter (Tularam & Ilahee, 2008)
-
-    Args:
-        Q (np.array): streamflow
-        e (float): smoothing parameter
-    """
-    if return_exceed:
-        b = np.zeros(Q.shape[0] + 1)
-    else:
-        b = np.zeros(Q.shape[0])
-    b[0] = b_LH[0]
-    for i in range(Q.shape[0] - 1):
-        b[i + 1] = (1 - e) * b[i] + e * Q[i + 1]
-        if b[i + 1] > Q[i + 1]:
-            b[i + 1] = Q[i + 1]
-            if return_exceed:
-                b[-1] += 1
-    return b
+import numpy as np
+from numba import njit
+
+
+@njit
+def EWMA(Q, b_LH, a, e, return_exceed=False):
+    """exponential weighted moving average (EWMA) filter (Tularam & Ilahee, 2008)
+
+    Args:
+        Q (np.array): streamflow
+        e (float): smoothing parameter
+    """
+    if return_exceed:
+        b = np.zeros(Q.shape[0] + 1)
+    else:
+        b = np.zeros(Q.shape[0])
+    b[0] = b_LH[0]
+    for i in range(Q.shape[0] - 1):
+        b[i + 1] = (1 - e) * b[i] + e * Q[i + 1]
+        if b[i + 1] > Q[i + 1]:
+            b[i + 1] = Q[i + 1]
+            if return_exceed:
+                b[-1] += 1
+    return b
```

### Comparing `baseflow-0.0.6/baseflow/methods/Eckhardt.py` & `baseflow-0.0.7/baseflow/methods/Furey.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import numpy as np
-from numba import njit
-
-
-@njit
-def Eckhardt(Q, b_LH, a, BFImax, return_exceed=False):
-    """Eckhardt filter (Eckhardt, 2005)
-
-    Args:
-        Q (np.array): streamflow
-        a (float): recession coefficient
-        BFImax (float): maximum value of baseflow index (BFI)
-    """
-    if return_exceed:
-        b = np.zeros(Q.shape[0] + 1)
-    else:
-        b = np.zeros(Q.shape[0])
-    b[0] = b_LH[0]
-    for i in range(Q.shape[0] - 1):
-        b[i + 1] = ((1 - BFImax) * a * b[i] + (1 - a) * BFImax * Q[i + 1]) / (1 - a * BFImax)
-        if b[i + 1] > Q[i + 1]:
-            b[i + 1] = Q[i + 1]
-            if return_exceed:
-                b[-1] += 1
-    return b
+import numpy as np
+from numba import njit
+
+
+@njit
+def Furey(Q, b_LH, a, A, return_exceed=False):
+    """Furey digital filter (Furey & Gupta, 2001, 2003)
+
+    Args:
+        Q (np.array): streamflow
+        a (float): recession coefficient
+        A (float): calibrated in baseflow.param_estimate
+    """
+    if return_exceed:
+        b = np.zeros(Q.shape[0] + 1)
+    else:
+        b = np.zeros(Q.shape[0])
+    b[0] = b_LH[0]
+    for i in range(Q.shape[0] - 1):
+        b[i + 1] = (a - A * (1 - a)) * b[i] + A * (1 - a) * Q[i]
+        if b[i + 1] > Q[i + 1]:
+            b[i + 1] = Q[i + 1]
+            if return_exceed:
+                b[-1] += 1
+    return b
```

### Comparing `baseflow-0.0.6/baseflow/methods/Slide.py` & `baseflow-0.0.7/baseflow/methods/Slide.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import numpy as np
-from numba import njit
-from baseflow.methods.Local import hysep_interval
-
-
-def Slide(Q, area):
-    """Slide interval graphical method from HYSEP program (Sloto & Crouse, 1996)
-
-    Args:
-        Q (np.array): streamflow
-        area (float): basin area in km^2
-    """
-    inN = hysep_interval(area)
-    return Slide_interpolation(Q, inN)
-
-
-@njit
-def Slide_interpolation(Q, inN):
-    b = np.zeros(Q.shape[0])
-    for i in range(np.int64((inN - 1) / 2), np.int64(Q.shape[0] - (inN - 1) / 2)):
-        b[i] = np.min(Q[np.int64(i - (inN - 1) / 2):np.int64(i + (inN + 1) / 2)])
-    b[:np.int64((inN - 1) / 2)] = np.min(Q[:np.int64((inN - 1) / 2)])
-    b[np.int64(Q.shape[0] - (inN - 1) / 2):] = np.min(Q[np.int64(Q.shape[0] - (inN - 1) / 2):])
-    return b
+import numpy as np
+from numba import njit, prange
+from baseflow.methods.Local import hysep_interval
+
+
+def Slide(Q, area):
+    """Slide interval graphical method from HYSEP program (Sloto & Crouse, 1996)
+
+    Args:
+        Q (np.array): streamflow
+        area (float): basin area in km^2
+    """
+    inN = hysep_interval(area)
+    return Slide_interpolation(Q, inN)
+
+
+@njit
+def Slide_interpolation(Q, inN):
+    b = np.zeros(Q.shape[0])
+    for i in prange(np.int64((inN - 1) / 2), np.int64(Q.shape[0] - (inN - 1) / 2)):
+        b[i] = np.min(Q[np.int64(i - (inN - 1) / 2):np.int64(i + (inN + 1) / 2)])
+    b[:np.int64((inN - 1) / 2)] = np.min(Q[:np.int64((inN - 1) / 2)])
+    b[np.int64(Q.shape[0] - (inN - 1) / 2):] = np.min(Q[np.int64(Q.shape[0] - (inN - 1) / 2):])
+    return b
```

### Comparing `baseflow-0.0.6/baseflow/param_estimate.py` & `baseflow-0.0.7/baseflow/param_estimate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import numpy as np
-from numba import njit
-from baseflow.utils import NSE, moving_average, multi_arange
-
-
-def recession_coefficient(Q, strict):
-    cQ, dQ = Q[1:-1], (Q[2:] - Q[:-2]) / 2
-    cQ, dQ = cQ[strict[1:-1]], dQ[strict[1:-1]]
-
-    idx = np.argsort(-dQ / cQ)[np.floor(dQ.shape[0] * 0.05).astype(int)]
-    K = - cQ[idx] / dQ[idx]
-    return np.exp(-1 / K)
-
-
-def param_calibrate(param_range, method, Q, b_LH, a):
-    idx_rec = recession_period(Q)
-    idx_oth = np.full(Q.shape[0], True)
-    idx_oth[idx_rec] = False
-    return param_calibrate_jit(param_range, method, Q, b_LH, a, idx_rec, idx_oth)
-
-
-@njit
-def param_calibrate_jit(param_range, method, Q, b_LH, a, idx_rec, idx_oth):
-    logQ = np.log1p(Q)
-    loss = np.zeros(param_range.shape)
-    for i in range(param_range.shape[0]):
-        p = param_range[i]
-        b_exceed = method(Q, b_LH, a, p, return_exceed=True)
-        f_exd, logb = b_exceed[-1] / Q.shape[0], np.log1p(b_exceed[:-1])
-        NSE_rec = NSE(logQ[idx_rec], logb[idx_rec])
-        NSE_oth = NSE(logQ[idx_oth], logb[idx_oth])
-        loss[i] = 1 - (1 - (1 - NSE_rec) / (1 - NSE_oth)) * (1 - f_exd)
-    return param_range[np.argmin(loss)]
-
-
-def recession_period(Q):
-    idx_dec = np.zeros(Q.shape[0] - 1, dtype=np.int64)
-    Q_ave = moving_average(Q, 3)
-    idx_dec[1:-1] = (Q_ave[:-1] - Q_ave[1:]) > 0
-    idx_beg = np.where(idx_dec[:-1] - idx_dec[1:] == -1)[0] + 1
-    idx_end = np.where(idx_dec[:-1] - idx_dec[1:] == 1)[0] + 1
-    idx_keep = (idx_end - idx_beg) >= 10
-    idx_beg = idx_beg[idx_keep]
-    idx_end = idx_end[idx_keep]
-    duration = idx_end - idx_beg
-    idx_beg = idx_beg + np.ceil(duration * 0.6).astype(np.int64)
-    return multi_arange(idx_beg, idx_end)
-
-
-def maxmium_BFI(Q, b_LH, a, date=None):
-    b = Backward(Q, b_LH, a)
-
-    if date is None:
-        idx_end = b.shape[0] // 365 * 365
-        annual_b = np.mean(b[:idx_end].reshape(-1, 365), axis=1)
-        annual_Q = np.mean(Q[:idx_end].reshape(-1, 365), axis=1)
-        annual_BFI = annual_b / annual_Q
-    else:
-        idx_year = date.Y - date.Y.min()
-        counts = np.bincount(idx_year)
-        idx_valid = counts > 0
-        annual_b = np.bincount(idx_year, weights=b)[idx_valid] / counts[idx_valid]
-        annual_Q = np.bincount(idx_year, weights=Q)[idx_valid] / counts[idx_valid]
-        annual_BFI = annual_b / annual_Q
-
-    BFI_max = np.max(annual_BFI)
-    BFI_max = BFI_max if BFI_max < 0.9 else np.sum(annual_b) / np.sum(annual_Q)
-    return BFI_max
-
-
-@njit
-def Backward(Q, b_LH, a):
-    b = np.zeros(Q.shape[0])
-    b[-1] = b_LH[-1]
-    for i in range(Q.shape[0] - 1, 0, -1):
-        b[i - 1] = b[i] / a
-        if b[i] == 0:
-            b[i - 1] = Q[i - 1]
-        if b[i - 1] > Q[i - 1]:
-            b[i - 1] = Q[i - 1]
-    return b
+import numpy as np
+from numba import njit, prange
+from baseflow.utils import NSE, moving_average, multi_arange
+
+
+def recession_coefficient(Q, strict):
+    cQ, dQ = Q[1:-1], (Q[2:] - Q[:-2]) / 2
+    cQ, dQ = cQ[strict[1:-1]], dQ[strict[1:-1]]
+
+    idx = np.argsort(-dQ / cQ)[np.floor(dQ.shape[0] * 0.05).astype(int)]
+    K = - cQ[idx] / dQ[idx]
+    return np.exp(-1 / K)
+
+
+def param_calibrate(param_range, method, Q, b_LH, a):
+    idx_rec = recession_period(Q)
+    idx_oth = np.full(Q.shape[0], True)
+    idx_oth[idx_rec] = False
+    return param_calibrate_jit(param_range, method, Q, b_LH, a, idx_rec, idx_oth)
+
+
+@njit
+def param_calibrate_jit(param_range, method, Q, b_LH, a, idx_rec, idx_oth):
+    logQ = np.log1p(Q)
+    loss = np.zeros(param_range.shape)
+    for i in prange(param_range.shape[0]):
+        p = param_range[i]
+        b_exceed = method(Q, b_LH, a, p, return_exceed=True)
+        f_exd, logb = b_exceed[-1] / Q.shape[0], np.log1p(b_exceed[:-1])
+        NSE_rec = NSE(logQ[idx_rec], logb[idx_rec])
+        NSE_oth = NSE(logQ[idx_oth], logb[idx_oth])
+        loss[i] = 1 - (1 - (1 - NSE_rec) / (1 - NSE_oth)) * (1 - f_exd)
+    return param_range[np.argmin(loss)]
+
+
+def recession_period(Q):
+    idx_dec = np.zeros(Q.shape[0] - 1, dtype=np.int64)
+    Q_ave = moving_average(Q, 3)
+    idx_dec[1:-1] = (Q_ave[:-1] - Q_ave[1:]) > 0
+    idx_beg = np.where(idx_dec[:-1] - idx_dec[1:] == -1)[0] + 1
+    idx_end = np.where(idx_dec[:-1] - idx_dec[1:] == 1)[0] + 1
+    idx_keep = (idx_end - idx_beg) >= 10
+    idx_beg = idx_beg[idx_keep]
+    idx_end = idx_end[idx_keep]
+    duration = idx_end - idx_beg
+    idx_beg = idx_beg + np.ceil(duration * 0.6).astype(np.int64)
+    return multi_arange(idx_beg, idx_end)
+
+
+def maxmium_BFI(Q, b_LH, a, date=None):
+    b = Backward(Q, b_LH, a)
+
+    if date is None:
+        idx_end = b.shape[0] // 365 * 365
+        annual_b = np.mean(b[:idx_end].reshape(-1, 365), axis=1)
+        annual_Q = np.mean(Q[:idx_end].reshape(-1, 365), axis=1)
+        annual_BFI = annual_b / annual_Q
+    else:
+        idx_year = date.Y - date.Y.min()
+        counts = np.bincount(idx_year)
+        idx_valid = counts > 0
+        annual_b = np.bincount(idx_year, weights=b)[idx_valid] / counts[idx_valid]
+        annual_Q = np.bincount(idx_year, weights=Q)[idx_valid] / counts[idx_valid]
+        annual_BFI = annual_b / annual_Q
+
+    BFI_max = np.max(annual_BFI)
+    BFI_max = BFI_max if BFI_max < 0.9 else np.sum(annual_b) / np.sum(annual_Q)
+    return BFI_max
+
+
+@njit
+def Backward(Q, b_LH, a):
+    b = np.zeros(Q.shape[0])
+    b[-1] = b_LH[-1]
+    for i in range(Q.shape[0] - 1, 0, -1):
+        b[i - 1] = b[i] / a
+        if b[i] == 0:
+            b[i - 1] = Q[i - 1]
+        if b[i - 1] > Q[i - 1]:
+            b[i - 1] = Q[i - 1]
+    return b
```

### Comparing `baseflow-0.0.6/baseflow/utils.py` & `baseflow-0.0.7/baseflow/utils.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-import numpy as np
-from numba import njit
-
-
-def load_streamflow(path):
-    """load streamflow into memory
-
-    Args:
-        path (str|DataFrame): path of streamflow csv file, or pandas DataFrame
-
-    Returns:
-        tuple: (date of np.datetime64, streamflow of float)
-    """
-    if isinstance(path, str):
-        date, Q = np.loadtxt(path, delimiter=',', skiprows=1, unpack=True,
-                             dtype=[('date', 'datetime64[D]'), ('Q', float)],
-                             converters={0: np.datetime64}, encoding='utf8')
-        year = date.astype('datetime64[Y]').astype(int) + int(str(np.datetime64(0, 'Y')))
-        month = date.astype('datetime64[M]').astype(int) % 12 + 1
-        day = (date - date.astype('datetime64[M]')).astype(int) + 1
-        date = np.rec.fromarrays([year, month, day], dtype=[('Y', 'i4'), ('M', 'i4'), ('D', 'i4')])
-    elif len(path.shape) > 1:
-        df_date = path.iloc[:, 0].astype('datetime64')
-        date = np.rec.fromarrays([df_date.dt.year, df_date.dt.month, df_date.dt.day],
-                                 dtype=[('Y', 'i4'), ('M', 'i4'), ('D', 'i4')])
-        Q = path.iloc[:, 1].values.astype(float)
-    else:
-        date = np.rec.fromarrays([path.index.year, path.index.month, path.index.day],
-                                 dtype=[('Y', 'i4'), ('M', 'i4'), ('D', 'i4')])
-        Q = path.values.astype(float)
-    return clean_streamflow(date, Q)
-
-
-def clean_streamflow(date, Q):
-    Q = np.abs(Q)
-    year = date['Y']
-    year_unique = np.unique(year)
-    year_delete = clean_streamflow_jit(year, year_unique, Q)
-    idx_delete = np.isin(year, year_delete) | np.isnan(Q)
-    return Q[~idx_delete], date[~idx_delete]
-
-
-@njit
-def clean_streamflow_jit(year, year_unique, Q):
-    year_delete = []
-    for y in year_unique:
-        if (Q[year == y] >= 0).sum() < 120:
-            year_delete.append(y)
-    return year_delete
-
-
-def exist_ice(date, ice_period):
-    if (date is None) or (ice_period is None):
-        return None
-
-    if isinstance(ice_period, np.ndarray):
-        return np.isin(date.M, np.where(ice_period)[0] + 1)
-
-    beg, end = ice_period
-    if (end[0] > beg[0]) or ((end[0] == beg[0]) & (end[1] > beg[1])):
-        ice = (((date.M > beg[0]) & (date.M < end[0])) |
-               ((date.M == beg[0]) & (date.D >= beg[1])) |
-               ((date.M == end[0]) & (date.D <= end[1])))
-    else:
-        ice = (((date.M > beg[0]) | (date.M < end[0])) |
-               ((date.M == beg[0]) & (date.D >= beg[1])) |
-               ((date.M == end[0]) & (date.D <= end[1])))
-    return ice
-
-
-def moving_average(x, w):
-    res = np.convolve(x, np.ones(w)) / w
-    return res[w - 1:-w + 1]
-
-
-@njit
-def multi_arange_steps(starts, stops, steps):
-    pos = 0
-    cnt = np.sum((stops - starts + steps - np.sign(steps)) // steps, dtype=np.int64)
-    res = np.zeros((cnt,), dtype=np.int64)
-    for i in range(starts.size):
-        v, stop, step = starts[i], stops[i], steps[i]
-        if step > 0:
-            while v < stop:
-                res[pos] = v
-                pos += 1
-                v += step
-        elif step < 0:
-            while v > stop:
-                res[pos] = v
-                pos += 1
-                v += step
-    assert pos == cnt
-    return res
-
-
-@njit
-def multi_arange(starts, stops):
-    pos = 0
-    cnt = np.sum(stops - starts, dtype=np.int64)
-    res = np.zeros((cnt,), dtype=np.int64)
-    for i in range(starts.size):
-        num = stops[i] - starts[i]
-        res[pos:pos + num] = np.arange(starts[i], stops[i])
-        pos += num
-    return res
-
-
-@njit
-def NSE(Q_obs, Q_sim):
-    SS_res = np.sum(np.square(Q_obs - Q_sim))
-    SS_tot = np.sum(np.square(Q_obs - np.mean(Q_obs)))
-    return (1 - SS_res / (SS_tot + 1e-10)) - 1e-10
+import numpy as np
+from numba import njit
+
+
+def load_streamflow(path):
+    """load streamflow into memory
+
+    Args:
+        path (str|DataFrame): path of streamflow csv file, or pandas DataFrame
+
+    Returns:
+        tuple: (date of np.datetime64, streamflow of float)
+    """
+    if isinstance(path, str):
+        date, Q = np.loadtxt(path, delimiter=',', skiprows=1, unpack=True,
+                             dtype=[('date', 'datetime64[D]'), ('Q', float)],
+                             converters={0: np.datetime64}, encoding='utf8')
+        year = date.astype('datetime64[Y]').astype(int) + int(str(np.datetime64(0, 'Y')))
+        month = date.astype('datetime64[M]').astype(int) % 12 + 1
+        day = (date - date.astype('datetime64[M]')).astype(int) + 1
+        date = np.rec.fromarrays([year, month, day], dtype=[('Y', 'i4'), ('M', 'i4'), ('D', 'i4')])
+    elif len(path.shape) > 1:
+        df_date = path.iloc[:, 0].astype('datetime64')
+        date = np.rec.fromarrays([df_date.dt.year, df_date.dt.month, df_date.dt.day],
+                                 dtype=[('Y', 'i4'), ('M', 'i4'), ('D', 'i4')])
+        Q = path.iloc[:, 1].values.astype(float)
+    else:
+        date = np.rec.fromarrays([path.index.year, path.index.month, path.index.day],
+                                 dtype=[('Y', 'i4'), ('M', 'i4'), ('D', 'i4')])
+        Q = path.values.astype(float)
+    return clean_streamflow(date, Q)
+
+
+def clean_streamflow(date, Q):
+    Q = np.abs(Q)
+    year = date['Y']
+    year_unique = np.unique(year)
+    year_delete = clean_streamflow_jit(year, year_unique, Q)
+    idx_delete = np.isin(year, year_delete) | np.isnan(Q)
+    return Q[~idx_delete], date[~idx_delete]
+
+
+@njit
+def clean_streamflow_jit(year, year_unique, Q):
+    year_delete = []
+    for y in year_unique:
+        if (Q[year == y] >= 0).sum() < 120:
+            year_delete.append(y)
+    return year_delete
+
+
+def exist_ice(date, ice_period):
+    if (date is None) or (ice_period is None):
+        return None
+
+    if isinstance(ice_period, np.ndarray):
+        return np.isin(date.M, np.where(ice_period)[0] + 1)
+
+    beg, end = ice_period
+    if (end[0] > beg[0]) or ((end[0] == beg[0]) & (end[1] > beg[1])):
+        ice = (((date.M > beg[0]) & (date.M < end[0])) |
+               ((date.M == beg[0]) & (date.D >= beg[1])) |
+               ((date.M == end[0]) & (date.D <= end[1])))
+    else:
+        ice = (((date.M > beg[0]) | (date.M < end[0])) |
+               ((date.M == beg[0]) & (date.D >= beg[1])) |
+               ((date.M == end[0]) & (date.D <= end[1])))
+    return ice
+
+
+def moving_average(x, w):
+    res = np.convolve(x, np.ones(w)) / w
+    return res[w - 1:-w + 1]
+
+
+@njit
+def multi_arange_steps(starts, stops, steps):
+    pos = 0
+    cnt = np.sum((stops - starts + steps - np.sign(steps)) // steps, dtype=np.int64)
+    res = np.zeros((cnt,), dtype=np.int64)
+    for i in range(starts.size):
+        v, stop, step = starts[i], stops[i], steps[i]
+        if step > 0:
+            while v < stop:
+                res[pos] = v
+                pos += 1
+                v += step
+        elif step < 0:
+            while v > stop:
+                res[pos] = v
+                pos += 1
+                v += step
+    assert pos == cnt
+    return res
+
+
+@njit
+def multi_arange(starts, stops):
+    pos = 0
+    cnt = np.sum(stops - starts, dtype=np.int64)
+    res = np.zeros((cnt,), dtype=np.int64)
+    for i in range(starts.size):
+        num = stops[i] - starts[i]
+        res[pos:pos + num] = np.arange(starts[i], stops[i])
+        pos += num
+    return res
+
+
+@njit
+def NSE(Q_obs, Q_sim):
+    SS_res = np.sum(np.square(Q_obs - Q_sim))
+    SS_tot = np.sum(np.square(Q_obs - np.mean(Q_obs)))
+    return (1 - SS_res / (SS_tot + 1e-10)) - 1e-10
```

### Comparing `baseflow-0.0.6/baseflow.egg-info/PKG-INFO` & `baseflow-0.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,72 @@
-Metadata-Version: 2.1
-Name: baseflow
-Version: 0.0.6
-Summary: A python package for baseflow separation
-Home-page: https://github.com/xiejx5/baseflow
-Author: Cody James
-Author-email: xiejx5@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-Provides-Extra: fancy feature
-
-
-<div align="center">
-
-# baseflow
-
-An open-source Python package for baseflow separation 🔥<br>
-
-</div>
-<br>
-
-<div align="center">
-
-![Global Baseflow Index Distribution from 12 Separation Methods](https://user-images.githubusercontent.com/29588684/226364211-3fd46152-3b9a-4de9-8d77-f1b59747a0f4.jpg)
-
-</div>
-<br>
-
-
-## ⚡&nbsp;&nbsp;Usage
-
-### Install
-```bash
-pip install baseflow
-```
-<br>
-
-
-### Example
-```python
-import baseflow
-
-Q, date = baseflow.load_streamflow(baseflow.example)
-b, KGEs = baseflow.separation(Q, date, area=276)
-print(f'Best Method: {b.dtype.names[KGEs.argmax()]}')
-```
-<br>
-
-
-
-## Project Structure
-The directory structure of baseflow looks like this:
-```
-├── methods                 <- implements for 12 baseflow separation methods
-│
-├── recession_analysis      <- tools for estimating recession coefficiency
-│
-├── param_estimate          <- backward and calibration approaches to estimate other parameters
-│
-├── comparison              <- an evaluation criterion to comparison different methods
-│
-├── requirements.txt        <- File for installing baseflow dependencies
-│
-└── README.md
-```
-<br>
-
-## 📌&nbsp;&nbsp;Todo
-
-
-### Nolinear reservoir assumption
-- Implement the nolinear reservoir assumption from the [paper](https://github.com/xiejx5/watershed_delineation/releases)
-- Employ a time-varing recession coefficiency for baseflow separation
-<br>
-
-### Applicable to other time scales
-1. The current version only applies to the daily scale
-2. The package needs to be updated to support hourly baseflow separation
-<br>
-
-## 🚀&nbsp;&nbsp;Publications
-
-### The following articles detail the 12 baseflow separation methods and their evaluation criterion.
-- Xie, J., Liu, X., Wang, K., Yang, T., Liang, K., & Liu, C. (2020). Evaluation of typical methods for baseflow separation in the contiguous United States. Journal of Hydrology, 583, 124628. https://doi.org/10.1016/j.jhydrol.2020.124628
+<div align="center">
+
+# baseflow
+
+An open-source Python package for baseflow separation 🔥<br>
+
+</div>
+<br>
+
+<div align="center">
+
+![Global Baseflow Index Distribution from 12 Separation Methods](https://user-images.githubusercontent.com/29588684/226364211-3fd46152-3b9a-4de9-8d77-f1b59747a0f4.jpg)
+
+</div>
+<br>
+
+
+## ⚡&nbsp;&nbsp;Usage
+
+### Install
+```bash
+pip install baseflow
+```
+<br>
+
+
+### Example
+```python
+import baseflow
+
+Q, date = baseflow.load_streamflow(baseflow.example)
+b, KGEs = baseflow.separation(Q, date, area=276)
+print(f'Best Method: {b.dtype.names[KGEs.argmax()]}')
+```
+<br>
+
+
+
+## Project Structure
+The directory structure of baseflow looks like this:
+```
+├── methods                 <- implements for 12 baseflow separation methods
+│
+├── recession_analysis      <- tools for estimating recession coefficiency
+│
+├── param_estimate          <- backward and calibration approaches to estimate other parameters
+│
+├── comparison              <- an evaluation criterion to comparison different methods
+│
+├── requirements.txt        <- File for installing baseflow dependencies
+│
+└── README.md
+```
+<br>
+
+## 📌&nbsp;&nbsp;Todo
+
+
+### Nolinear reservoir assumption
+- Implement the nolinear reservoir assumption from the [paper](https://github.com/xiejx5/watershed_delineation/releases)
+- Employ a time-varing recession coefficiency for baseflow separation
+<br>
+
+### Applicable to other time scales
+1. The current version only applies to the daily scale
+2. The package needs to be updated to support hourly baseflow separation
+<br>
+
+## 🚀&nbsp;&nbsp;Publications
+
+### The following articles detail the 12 baseflow separation methods and their evaluation criterion.
+- Xie, J., Liu, X., Wang, K., Yang, T., Liang, K., & Liu, C. (2020). Evaluation of typical methods for baseflow separation in the contiguous United States. Journal of Hydrology, 583, 124628. https://doi.org/10.1016/j.jhydrol.2020.124628
```

### Comparing `baseflow-0.0.6/baseflow.egg-info/SOURCES.txt` & `baseflow-0.0.7/baseflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.6/setup.py` & `baseflow-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Note: To use the 'upload' functionality of this file, you must:
-#   $ pipenv install twine --dev
-
-import io
-import os
-import sys
-from shutil import rmtree
-
-from setuptools import find_packages, setup, Command
-
-# Package meta-data.
-NAME = 'baseflow'
-DESCRIPTION = 'A python package for baseflow separation'
-URL = 'https://github.com/xiejx5/baseflow'
-EMAIL = 'xiejx5@gmail.com'
-AUTHOR = 'Cody James'
-REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.6'
-
-# What packages are required for this module to be executed?
-REQUIRED = [
-    'numpy', 'numba',
-]
-
-# What packages are optional?
-EXTRAS = {
-    'fancy feature': ['pandas', 'matplotlib', 'scipy'],
-}
-
-# The rest you shouldn't have to touch too much :)
-# ------------------------------------------------
-# Except, perhaps the License and Trove Classifiers!
-# If you do change the License, remember to change the Trove Classifier for that!
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-# Import the README and use it as the long-description.
-# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
-try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-# Load the package's __version__.py module as a dictionary.
-about = {}
-if not VERSION:
-    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
-        exec(f.read(), about)
-else:
-    about['__version__'] = VERSION
-
-
-class UploadCommand(Command):
-    """Support setup.py upload."""
-
-    description = 'Build and publish the package.'
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
-        except OSError:
-            pass
-
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system(
-            '{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
-
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
-
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
-
-        sys.exit()
-
-
-# Where the magic happens:
-setup(
-    name=NAME,
-    version=about['__version__'],
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=URL,
-    packages=find_packages(
-        exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    package_data={"baseflow": ["example.csv"]},
-    # If your package is a single module, use this instead of 'packages':
-    # py_modules=['baseflow'],
-
-    # entry_points={
-    #     'console_scripts': ['mycli=mymodule:cli'],
-    # },
-    install_requires=REQUIRED,
-    extras_require=EXTRAS,
-    # include_package_data=True,
-    license='MIT',
-    classifiers=[
-        # Trove classifiers
-        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy'
-    ],
-    # $ setup.py publish support.
-    cmdclass={
-        'upload': UploadCommand,
-    },
-)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Note: To use the 'upload' functionality of this file, you must:
+#   $ pipenv install twine --dev
+
+import io
+import os
+import sys
+from shutil import rmtree
+
+from setuptools import find_packages, setup, Command
+
+# Package meta-data.
+NAME = 'baseflow'
+DESCRIPTION = 'A python package for baseflow separation'
+URL = 'https://github.com/xiejx5/baseflow'
+EMAIL = 'xiejx5@gmail.com'
+AUTHOR = 'Cody James'
+REQUIRES_PYTHON = '>=3.6.0'
+VERSION = '0.0.7'
+
+# What packages are required for this module to be executed?
+REQUIRED = [
+    'numpy', 'numba',
+]
+
+# What packages are optional?
+EXTRAS = {
+    'fancy feature': ['pandas', 'matplotlib', 'scipy'],
+}
+
+# The rest you shouldn't have to touch too much :)
+# ------------------------------------------------
+# Except, perhaps the License and Trove Classifiers!
+# If you do change the License, remember to change the Trove Classifier for that!
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+# Import the README and use it as the long-description.
+# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
+try:
+    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
+        long_description = '\n' + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+# Load the package's __version__.py module as a dictionary.
+about = {}
+if not VERSION:
+    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
+    with open(os.path.join(here, project_slug, '__version__.py')) as f:
+        exec(f.read(), about)
+else:
+    about['__version__'] = VERSION
+
+
+class UploadCommand(Command):
+    """Support setup.py upload."""
+
+    description = 'Build and publish the package.'
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print('\033[1m{0}\033[0m'.format(s))
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status('Removing previous builds…')
+            rmtree(os.path.join(here, 'dist'))
+        except OSError:
+            pass
+
+        self.status('Building Source and Wheel (universal) distribution…')
+        os.system(
+            '{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
+
+        self.status('Uploading the package to PyPI via Twine…')
+        os.system('twine upload dist/*')
+
+        self.status('Pushing git tags…')
+        os.system('git tag v{0}'.format(about['__version__']))
+        os.system('git push --tags')
+
+        sys.exit()
+
+
+# Where the magic happens:
+setup(
+    name=NAME,
+    version=about['__version__'],
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=URL,
+    packages=find_packages(
+        exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    package_data={"baseflow": ["example.csv"]},
+    # If your package is a single module, use this instead of 'packages':
+    # py_modules=['baseflow'],
+
+    # entry_points={
+    #     'console_scripts': ['mycli=mymodule:cli'],
+    # },
+    install_requires=REQUIRED,
+    extras_require=EXTRAS,
+    # include_package_data=True,
+    license='MIT',
+    classifiers=[
+        # Trove classifiers
+        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy'
+    ],
+    # $ setup.py publish support.
+    cmdclass={
+        'upload': UploadCommand,
+    },
+)
```

