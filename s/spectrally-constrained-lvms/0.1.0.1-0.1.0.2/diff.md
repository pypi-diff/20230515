# Comparing `tmp/spectrally_constrained_lvms-0.1.0.1.tar.gz` & `tmp/spectrally_constrained_lvms-0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrally_constrained_lvms-0.1.0.1.tar", max compression
+gzip compressed data, was "spectrally_constrained_lvms-0.1.0.2.tar", max compression
```

## Comparing `spectrally_constrained_lvms-0.1.0.1.tar` & `spectrally_constrained_lvms-0.1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1090 2023-04-28 07:39:34.154025 spectrally_constrained_lvms-0.1.0.1/LICENSE
--rw-r--r--   0        0        0     1613 2023-05-12 14:09:19.441964 spectrally_constrained_lvms-0.1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1015 2023-05-12 14:09:14.966635 spectrally_constrained_lvms-0.1.0.1/README.md
--rw-r--r--   0        0        0     1113 2023-05-12 11:38:25.719388 spectrally_constrained_lvms-0.1.0.1/spectrally_constrained_LVMs/__init__.py
--rw-r--r--   0        0        0    16385 2023-05-12 11:16:37.818125 spectrally_constrained_lvms-0.1.0.1/spectrally_constrained_LVMs/constraint.py
--rw-r--r--   0        0        0    13400 2023-05-12 11:16:37.818626 spectrally_constrained_lvms-0.1.0.1/spectrally_constrained_LVMs/cost_functions.py
--rw-r--r--   0        0        0    21169 2023-05-12 11:16:37.819125 spectrally_constrained_lvms-0.1.0.1/spectrally_constrained_LVMs/helper.py
--rw-r--r--   0        0        0    14991 2023-05-12 11:16:37.820143 spectrally_constrained_lvms-0.1.0.1/spectrally_constrained_LVMs/negen_approx.py
--rw-r--r--   0        0        0    34652 2023-05-12 11:16:37.821162 spectrally_constrained_lvms-0.1.0.1/spectrally_constrained_LVMs/spectrally_constrained_linear_model.py
--rw-r--r--   0        0        0     1919 1970-01-01 00:00:00.000000 spectrally_constrained_lvms-0.1.0.1/setup.py
--rw-r--r--   0        0        0     2387 1970-01-01 00:00:00.000000 spectrally_constrained_lvms-0.1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-28 07:39:34.154025 spectrally_constrained_lvms-0.1.0.2/LICENSE
+-rw-r--r--   0        0        0     1616 2023-05-15 12:03:36.288103 spectrally_constrained_lvms-0.1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1289 2023-05-13 20:02:18.006810 spectrally_constrained_lvms-0.1.0.2/README.md
+-rw-r--r--   0        0        0     1214 2023-05-15 11:46:26.325532 spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/__init__.py
+-rw-r--r--   0        0        0    16039 2023-05-13 15:58:08.511125 spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/cost_functions.py
+-rw-r--r--   0        0        0    21547 2023-05-13 15:56:12.827004 spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/helper_methods.py
+-rw-r--r--   0        0        0    15121 2023-05-13 15:42:49.428404 spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/negen_approx.py
+-rw-r--r--   0        0        0    16446 2023-05-13 15:41:10.612996 spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/spectral_constraint.py
+-rw-r--r--   0        0        0    31798 2023-05-15 11:57:51.356604 spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/spectrally_constrained_model.py
+-rw-r--r--   0        0        0     2194 1970-01-01 00:00:00.000000 spectrally_constrained_lvms-0.1.0.2/setup.py
+-rw-r--r--   0        0        0     2559 1970-01-01 00:00:00.000000 spectrally_constrained_lvms-0.1.0.2/PKG-INFO
```

### Comparing `spectrally_constrained_lvms-0.1.0.1/LICENSE` & `spectrally_constrained_lvms-0.1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrally_constrained_lvms-0.1.0.1/pyproject.toml` & `spectrally_constrained_lvms-0.1.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrally-constrained-LVMs"
-version = "0.1.0.1"
+version = "0.1.0.2"
 description = "An optimisation implementation of linear transforms with a spectral constraint."
 authors = ["Ryan Balshaw <ryanbalshaw81@gmail.com>"]
 maintainers = ["Ryan Balshaw <ryanbalshaw81@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/RyanBalshaw/scICA"
 repository = "https://github.com/RyanBalshaw/scICA"
@@ -15,15 +15,15 @@
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: Implementation",
     "Topic :: Scientific/Engineering",
 ]
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 numpy = "^1.23.1"
 matplotlib = "^3.5.2"
 scipy = "^1.8.1"
 scikit-learn = "^1.1.2"
 tqdm = "^4.64.1"
 sympy = "^1.11.1"
 
@@ -33,15 +33,15 @@
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.2"
 black = "^23.3.0"
 isort = "^5.12.0"
 interrogate = {extras = ["png"], version = "^1.5.0"}
 pytest = "^7.3.1"
 ruff = "^0.0.263"
-cairosvg = "^2.7.0"
+jupyterlab = "^3.6.3"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
```

### Comparing `spectrally_constrained_lvms-0.1.0.1/README.md` & `spectrally_constrained_lvms-0.1.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-# Spectrally constrained linear transformations
+# Spectrally constrained LVMs
 
 ![GitHub](https://img.shields.io/github/license/RyanBalshaw/spectrally-constrained-LVMs)
 ![GitHub issues](https://img.shields.io/github/issues-raw/RyanBalshaw/spectrally-constrained-LVMs)
 ![PyPI](https://img.shields.io/pypi/v/spectrally-constrained-lvms)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/spectrally-constrained-lvms?color=blueviolet)
+![Read the Docs](https://img.shields.io/readthedocs/spectrally-constrained-lvms)
+![GitHub last commit](https://img.shields.io/github/last-commit/RyanBalshaw/spectrally-constrained-LVMs)
 
-A repository for all code for sICA. This is the first setup of this project.
+A repository for all code for the package. This is the first setup of this project.
 
 The package can be installed using [pip](https://pypi.org/project/pip/):
 
 # Documentation
 Please visit... for the documentation.
 
 ## Purpose
```

### Comparing `spectrally_constrained_lvms-0.1.0.1/spectrally_constrained_LVMs/__init__.py` & `spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # Copyright 2023-present Ryan Balshaw
 """Spectrally-constrained-LVMs. Train linear LVMs with the addition
  of a spectral constraint with minimal effort."""
-from .constraint import spectral_objective
-from .cost_functions import negentropy_cost, sympy_cost, user_cost
-from .helper import (
+from .cost_functions import negentropy_cost, sympy_cost, user_cost, variance_cost
+from .helper_methods import (
     Hankel_matrix,
     batch_sampler,
     data_processor,
     deflation_orthogonalisation,
     quasi_Newton,
 )
 from .negen_approx import cube_object, exp_object, logcosh_object, quad_object
-from .spectrally_constrained_linear_model import linear_model
+from .spectral_constraint import spectral_objective
+from .spectrally_constrained_model import linear_model
 
 __author__ = "Ryan Balshaw"
-__version__ = "0.1.0"
+__version__ = "0.1.0.1"
 __email__ = "ryanbalshaw81@gmail.com"
 __description__ = (
     "Train linear LVMs with the addition "
     "of a spectral constraint with minimal effort."
 )
-__uri__ = ""
+# __uri__ = "http://spectrally-constrained-lvms.readthedocs.io/"
 __all__ = [
     "spectral_objective",
     "negentropy_cost",
     "sympy_cost",
     "user_cost",
+    "variance_cost",
     "Hankel_matrix",
     "batch_sampler",
     "data_processor",
     "deflation_orthogonalisation",
     "quasi_Newton",
     "cube_object",
     "exp_object",
```

### Comparing `spectrally_constrained_lvms-0.1.0.1/spectrally_constrained_LVMs/constraint.py` & `spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/spectral_constraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+# Copyright 2023-present Ryan Balshaw
 """
-The spectral constraint method to be added to FastICA.
+The spectral constraint method to be added to negentropy-based ICA approach.
 """
 import numpy as np
 
 
 class spectral_objective(object):
     """
     An object that implements the spectral constraint objective.
```

### Comparing `spectrally_constrained_lvms-0.1.0.1/spectrally_constrained_LVMs/cost_functions.py` & `spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/cost_functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,116 +1,69 @@
+# Copyright 2023-present Ryan Balshaw
 """
 This set of methods that define general cost functions that
-one can use, and the FastICA cost function.
+one can use, and two specific methods (principal component analysis
+and independent component analysis).
 """
 import numpy as np
 import sympy as sp
 
 from .negen_approx import initialise_sources
 
 
-class user_cost(object):
+class costClass(object):
     """
-    An object that implements the a general user cost function
-     class. This allows the user to manually define their cost function
-     and associated gradient vector and hessian.
-
-     Assumed format for methods: func(X, w, y) where X is an ndarray
-      with shape (n_samples, n_features), w is an ndarray with shape (n_features, 1)
-      and y is the linear transformation X @ w with shape (n_samples, 1).
+    Base class for different formulations of the user
+    cost function.
 
+    Finish write up here!
     """
 
-    def __init__(self, use_hessian: bool):
-        """
-
-        Parameters
-        ----------
-        use_hessian : bool
-            A flag to control whether you use the Hessian or not.
-            This is useful in the solver, as you may wish to just
-            perform steepest descent instead of using Newton's method.
-        """
-        self.use_hessian = use_hessian
+    def __init__(self, verbose=True):
+        self.verbose = verbose
 
     def set_cost(self, cost_func):
         """
         This method allows one to set their cost function.
 
         Parameters
         ----------
         cost_func : function
             The users cost function.
             Example: cost_func = lambda X, w, y: -1 * np.mean(y ** 2, axis=0)
 
-        Raises
-        -------
-        AssertionError
-            Error is thrown when cost_func is not of type 'function'.
         """
-        try:
-            assert type(cost_func).__name__ == "function"
-
-        except AssertionError:
-            ("Please implement a cost function that accepts parameters " "(X, w, y).")
-            raise AssertionError
-
-        else:
-            self._cost = cost_func
+        self._cost = cost_func
 
     def set_gradient(self, cost_gradient):
         """
         This method allows one to set their gradient vector.
 
         Parameters
         ----------
         cost_gradient : function
             The users gradient vector of the cost function.
         Example:
             cost_gradient = lambda X, w, y: -2 * np.mean(y * X, axis=0, keepdims = True)
 
-        Raises
-        -------
-        AssertionError
-            Error is thrown when cost_gradient is not of type 'function'.
         """
-        try:
-            assert type(cost_gradient).__name__ == "function"
-
-        except AssertionError:
-            ("Please implement a gradient function that accepts parameters (X, w, y).")
-            raise AssertionError
-
-        else:
-            self._cost_gradient = cost_gradient
+        self._cost_gradient = cost_gradient
 
     def set_hessian(self, cost_hessian):
         """
         This method allows one to set their objective Hessian (optional).
 
         Parameters
         ----------
         cost_hessian : function
             The users gradient vector of the cost function.
             Example: cost_hessian = lambda X, w, y: -2 /X.shape[0] * (X.T @ X)
 
-        Raises
-        -------
-        AssertionError
-            Error is thrown when cost_hessian is not of type 'function'.
         """
-        try:
-            assert type(cost_hessian).__name__ == "function"
-
-        except AssertionError:
-            ("Please implement a hessian function that accepts parameters (X, w, y).")
-            raise AssertionError
-
-        else:
-            self._cost_hessian = cost_hessian
+        self._cost_hessian = cost_hessian
 
     def get_cost(self):
         """
         Method to return the cost function to the user.
 
         Returns
         -------
@@ -143,14 +96,102 @@
         cost_hessian if attribute exists, else None.
         """
         if hasattr(self, "_cost_hessian"):
             return self._cost_hessian
         else:
             return None
 
+    def check_gradient(self, X, w, y, step_size):
+        # Finite difference gradient approximation (central difference)
+        # Method cannot work without
+        # NB! - self._cost must be a primary function of X and w, not y
+
+        if self.verbose:
+            print("\nChecking the gradient using central difference approximation...")
+        w0 = w.copy().reshape(-1, 1)
+
+        grad_current = self.cost_gradient(X, w0, y).reshape(-1, 1)
+        grad_check = np.zeros_like(grad_current)
+
+        for i in range(grad_check.shape[0]):
+            e_i = np.zeros_like(w0)
+            e_i[i, 0] = step_size
+
+            f_f = self.cost(X, w0 + e_i, y)
+            f_b = self.cost(X, w0 - e_i, y)
+
+            grad_check[i, 0] = (f_f - f_b) / (2 * step_size)
+
+        grad_norm = np.linalg.norm(grad_current - grad_check)
+
+        if self.verbose:
+            print(f"Finished! The gradient norm (row-wise) is: {np.round(grad_norm)}")
+
+        return grad_current, grad_check, grad_norm
+
+    def check_hessian(self, X, w, y, step_size):
+        # Finite difference Hessian approximation (central difference)
+
+        if self.verbose:
+            print("\nChecking the hessian using central difference approximation...")
+
+        w0 = w.copy().reshape(-1, 1)
+        hess_current = self.cost_hessian(X, w0, y)
+        hess_check = np.zeros_like(hess_current)
+
+        r, c = hess_check.shape
+
+        for i in range(r):
+            e_i = np.zeros_like(w0)
+            e_i[i, 0] = step_size
+
+            for j in range(c):
+                e_j = np.zeros_like(w0)
+                e_j[j, 0] = step_size
+
+                f1 = self.cost(X, w0 + e_i + e_j, y)
+                f2 = self.cost(X, w0 + e_i - e_j, y)
+                f3 = self.cost(X, w0 - e_i + e_j, y)
+                f4 = self.cost(X, w0 - e_i - e_j, y)
+
+                hess_check[i, j] = (f1 - f2 - f3 + f4) / (4 * step_size**2)
+
+        hess_norm = np.mean(np.linalg.norm(hess_current - hess_check, axis=1))
+
+        if self.verbose:
+            print(f"Finished! The hessian norm (row-wise) is: {np.round(hess_norm)}")
+
+        return hess_current, hess_check, hess_norm
+
+
+class user_cost(costClass):
+    """
+    An object that implements the a general user cost function
+     class. This allows the user to manually define their cost function
+     and associated gradient vector and hessian.
+
+     Assumed format for methods: func(X, w, y) where X is an ndarray
+      with shape (n_samples, n_features), w is an ndarray with shape (n_features, 1)
+      and y is the linear transformation X @ w with shape (n_samples, 1).
+
+    """
+
+    def __init__(self, use_hessian: bool, verbose=True):
+        """
+
+        Parameters
+        ----------
+        use_hessian : bool
+            A flag to control whether you use the Hessian or not.
+            This is useful in the solver, as you may wish to just
+            perform steepest descent instead of using Newton's method.
+        """
+        super().__init__(verbose)
+        self.use_hessian = use_hessian
+
     def cost(self, X, w, y):
         """
         A method that returns the cost function for the inputs.
 
         Parameters
         ----------
         X : ndarray
@@ -208,74 +249,92 @@
         if self.use_hessian:
             return self._cost_hessian(X, w, y)
 
         else:
             return np.eye(w.shape[0])
 
 
-class sympy_cost(object):
-    def __init__(self, n_samples, n_features, use_hessian=False):
+class sympy_cost(costClass):
+    def __init__(self, n_samples, n_features, use_hessian=False, verbose=True):
+        super().__init__(verbose)
         self.n_samples = n_samples
         self.n_features = n_features
         self.use_hessian = use_hessian
 
-    def get_model_parameters(self):
-        i, j = sp.symbols("i j", cls=sp.Idx)
+    def set_cost(self, cost_func):
+        # overwrites the base method
+        """
+        This method allows one to set their cost function (overwrites default).
+
+        Parameters
+        ----------
+        cost_func : function
+            The users cost function.
+            Example: cost_func = lambda X, w, y: -1 * np.mean(y ** 2, axis=0)
 
-        w = sp.IndexedBase("w", shape=(self.n_features, 1))
-        X = sp.IndexedBase("X", shape=(self.n_samples, self.n_features))
+        """
+        self._sympy_cost = cost_func
 
-        return X, w, (i, j)
+    def get_model_parameters(self):
+        i, j = sp.symbols("i j", cls=sp.Idx)
 
-    def set_cost_sympy(self, cost_func_sympy, X, w):
-        self.X = X
-        self.w = w
-        self._cost_sympy = cost_func_sympy
+        self.w = sp.IndexedBase("w", shape=(self.n_features, 1))
+        self.X = sp.IndexedBase("X", shape=(self.n_samples, self.n_features))
+        self.y = sp.symbols("y")  # Placeholder variable
 
-    def get_cost_sympy(self):
-        return self._cost_sympy
+        return self.X, self.w, (i, j)
 
     def implement_cost(self):
-        self._cost = sp.lambdify((self.X, self.w), self._cost_sympy)
+        print("Lambdifying the sympy cost function...")
+
+        self._cost = sp.lambdify(
+            (self.X, self.w, self.y), self._sympy_cost
+        )  # Will overwrite the sympy variable
 
     def implement_first_derivative(self):
+        print("Deriving and lambdifying the sympy derivative function...")
+
         self._first_derivative_sympy = sp.Matrix(
-            [self._cost_sympy.diff(self.w[i, 0]) for i in range(self.n_features)]
+            [self._sympy_cost.diff(self.w[i, 0]) for i in range(self.n_features)]
         )
-        self._first_derivative = sp.lambdify(
-            (self.X, self.w), self._first_derivative_sympy
+        self._cost_gradient = sp.lambdify(
+            (self.X, self.w, self.y), self._first_derivative_sympy
         )
 
     def implement_second_derivative(self):
+        print("Deriving and lambdifying the sympy Hessian function...")
+
         if self.use_hessian:
             self._second_derivative_sympy = sp.BlockMatrix(
                 [
                     self._first_derivative_sympy.diff(self.w[i, 0])
                     for i in range(self.n_features)
                 ]
             )
-            self._second_derivative = sp.lambdify(
-                (self.X, self.w), self._second_derivative_sympy
+            self._cost_hessian = sp.lambdify(
+                (self.X, self.w, self.y), self._second_derivative_sympy
             )
 
         else:
-            self._second_derivative = lambda X, w: np.eye(w.shape[0])
+            self._cost_hessian = lambda X, w, y: np.eye(w.shape[0])
 
     def implement_methods(self):
-        if hasattr(self, "cost_sympy"):
+        if hasattr(self, "_sympy_cost"):
+            print("Calculating the sympy method components...")
+
             self.implement_cost()
             self.implement_first_derivative()
 
             if self.use_hessian:
                 self.implement_second_derivative()
 
         else:
             print(
                 "Please first initialise the sympy cost function "
-                "using set_cost_sympy()."
+                "using inst.set_cost()."
             )
             raise SystemExit
 
     def check_X(self, X):
         r, c = X.shape
         assert r == self.n_samples, print(
             f"Number of samples ({r}) in X  does not match the"
@@ -292,55 +351,57 @@
             f"Number of samples ({r}) in w  does not match the"
             f" expected value: {self.n_features}."
         )
         assert c == 1, print(
             f"Number of features ({c}) in w does not match the" f" expected value: {1}."
         )
 
-    def cost(self, X, w, *args):
+    def cost(self, X, w, y, *args):
         self.check_X(X)
         self.check_w(w)
 
-        return self._cost(X, w)
+        if not hasattr(self, "_cost"):
+            self.implement_methods()  # Ensure creation of _methods.
+
+        return self._cost(X, w, y)
 
-    def cost_gradient(self, X, w, *args):
-        return self._first_derivative(X, w)
+    def cost_gradient(self, X, w, y, *args):
+        return self._cost_gradient(X, w, y)
 
-    def cost_hessian(self, X, w, *args):
+    def cost_hessian(self, X, w, y, *args):
         if self.use_hessian:
-            return self._second_derivative(X, w)
+            return self._cost_hessian(X, w, y)
 
         else:
             return np.eye(w.shape[0])
 
 
-class negentropy_cost(object):
-    def __init__(self, source_name: str, source_params: dict):
+class negentropy_cost(costClass):
+    def __init__(self, source_name: str, source_params: dict, verbose=True):
+        super().__init__(verbose)
         self.source_name = source_name
         self.source_params = source_params  # dictionary of parameters
 
         # Initialise the source PDFs
         self.source_instance, self.source_expectation = initialise_sources(
             source_name, self.source_params
         )
 
-    def cost(self, X, w, y):  # Important to FastICA
+    def cost(self, X, w, y):  # Important to negentropy-based ICA
         # Negentropy-estimate calculation
 
         if y.shape[1] == 1:
             EG_y = np.mean(self.source_instance.function(y))
 
         else:
             EG_y = np.mean(self.source_instance.function(y), axis=0)
 
         return -1 * (EG_y - self.source_expectation) ** 2
 
-    def cost_gradient(self, X, w, y):  # Important to FastICA
-        # t0 = time.time()
-
+    def cost_gradient(self, X, w, y):  # Important to negentropy-based ICA
         N, m = X.shape
 
         g_y = self.source_instance.first_derivative(y)
 
         # Calculate the expectation
         expectation = np.mean(g_y * X, axis=0, keepdims=True).T
 
@@ -348,16 +409,17 @@
         r = np.mean(self.source_instance.function(y)) - self.source_expectation
 
         # Calculate the gradient vector
         grad_vector = -2 * r * expectation
 
         return grad_vector
 
-    def cost_hessian(self, X, w, y, approx_flag=True):  # Important to FastICA
-        # t0 = time.time()
+    def cost_hessian(
+        self, X, w, y, approx_flag=True
+    ):  # Important to negentropy-based ICA
         N, m = X.shape
 
         # Compute g'(y)
         g_prime_y = self.source_instance.second_derivative(y)
 
         # t0 = time.time()
         if approx_flag:
@@ -384,64 +446,71 @@
 
         # Calculate the Jacobian (Hessian)
         jacobian = -2 * (grad_outer + r * expectation)
 
         return jacobian
 
 
+class variance_cost(user_cost):
+    def __init__(self, use_hessian: bool, verbose=True):
+        super().__init__(use_hessian, verbose)
+
+        def loss(X, w, y):
+            return -1 * np.mean((X @ w) ** 2, axis=0)
+
+        def grad(X, w, y):
+            return -2 * np.mean(y * X, axis=0, keepdims=True).T
+
+        def hess(X, w, y):
+            return -2 * np.cov(X, rowvar=False)
+
+        self.set_cost(loss)
+        self.set_gradient(grad)
+        self.set_hessian(hess)
+
+
 # if __name__ == "__main__":
 #
-#     # Method 1
 #     n_samples = 10000
 #     n_features = 3
 #
-#     sympy_inst = sympy_cost(n_samples, n_features)
+#     # Method 1
+#     test_inst1 = sympy_cost(n_samples, n_features, use_hessian=True)
 #
-#     X, w, iter_params = sympy_inst.get_model_parameters()
+#     X, w, iter_params = test_inst1.get_model_parameters()
 #     i, j = iter_params
 #
 #     loss_i = sp.Sum(w[j, 0] * X[i, j], (j, 0, n_features - 1))
-#     loss = 1 / n_samples * sp.Sum(loss_i ** 2, (i, 0, n_samples - 1))
+#     loss = -1 / n_samples * sp.Sum(loss_i ** 2, (i, 0, n_samples - 1))
+#
+#     test_inst1.set_cost(loss)
+#     test_inst1.implement_methods()
+#
+#     # Method 2
+#     test_inst2 = user_cost(use_hessian=True)
+#
+#     loss = lambda X, w, y: -1 * np.mean((X @ w) ** 2, axis=0)
+#     grad = lambda X, w, y: -2 * np.mean(y * X, axis=0, keepdims=True).T
+#     hess = lambda X, w, y: -2 * np.cov(X, rowvar=False)
+#
+#     test_inst2.set_cost(loss)
+#     test_inst2.set_gradient(grad)
+#     test_inst2.set_hessian(hess)
 #
-#     sympy_inst.set_cost_sympy(loss, X, w)
+#     # Method 3
+#     test_inst3 = negentropy_cost(source_name = 'exp',
+#                                 source_params = {"alpha": 1})
 #
+#     #
 #     w_ = np.ones((n_features, 1))
 #     X_ = np.random.randn(n_samples, n_features)
 #     mu_ = np.mean(X_, axis=0, keepdims=True)
 #     std_ = np.std(X_, axis=0, keepdims=True)
 #
 #     X_ = (X_ - mu_) / std_
 #     y_ = X_ @ w_
 #
-#     print("\nResults for method 2")
-#     print("--------------------\n")
-#     print("Loss function:")
-#     print(sympy_inst.cost(X_, w_, y_))
-#
-#     print("\nDerivative:")
-#     print(sympy_inst.cost_gradient(X_, w_, y_))
-#
-#     print("\nHessian:")
-#     print(sympy_inst.cost_hessian(X_, w_, y_))
-#
-#     # Method 2
-#     user_inst = user_cost()
-#
-#     linear_model = lambda X, w: X @ w
-#     loss = lambda X, w, y: np.mean(y ** 2, axis = 0)
-#     grad = lambda X, w, y: np.mean(2 * y * X, axis=0, keepdims=True).T
-#     hess = lambda X, w, y: 2 / X.shape[0] * X.T @ X
-#
-#     user_inst.set_cost(loss)
-#     user_inst.set_gradient(grad)
-#     user_inst.set_hessian(hess)
-#
-#     print("\nResults for method 2")
-#     print("--------------------\n")
-#     print("Loss function:")
-#     print(user_inst.cost(X_, w_, y_))
-#
-#     print("\nDerivative:")
-#     print(user_inst.cost_gradient(X_, w_, y_))
-#
-#     print("\nHessian:")
-#     print(user_inst.cost_hessian(X_, w_, y_))
+#     # Check derivatives
+#     for cnt, test_inst in enumerate([test_inst1, test_inst2, test_inst3]):
+#         print(f"\n\nFor instance {cnt + 1}:")
+#         check_grad = test_inst3.check_gradient(X_, w_, y_, 1e-4)
+#         check_hess = test_inst3.check_hessian(X_, w_, y_, 1e-4)
```

### Comparing `spectrally_constrained_lvms-0.1.0.1/spectrally_constrained_LVMs/helper.py` & `spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/helper_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,26 @@
+# Copyright 2023-present Ryan Balshaw
 """
-The helper methods for the spectrally constrained FastICA solver.
+The helper methods for the solver.
 
-Method 1: ica_batch_sampler
+Method 1: data_processor
+    This method implements the pre-processing steps applied to X (standardisation
+    and/or whitening).
+
+Method 2: batch_sampler
     This is a simple batch sampler method for quicker solving.
 
-Method 2: quasi_Newton
+Method 3: quasi_Newton
     This is a method that implements different Hessian approximation strategies.
+
+Method 5: deflation_orthogonalisation
+    This method implements the Gram-Schmidt orthogonalisation process.
+
+Method 5: Hankel_matrix
+    This method implements the data hankelisation step.
 """
 
 import copy
 
 import numpy as np
 
 
@@ -603,15 +614,17 @@
         Returns
         -------
 
         """
 
         return u.T @ v / (u.T @ u) * u
 
-    def gram_schmidt_orthogonalisation(self, w, W, idx):  # Important to FastICA
+    def gram_schmidt_orthogonalisation(
+        self, w, W, idx
+    ):  # Important to negentropy-based ICA
         """
 
         Parameters
         ----------
         w: ndarray
             A Nx1 array that contains the vector we want to orthogonalise.
 
@@ -653,15 +666,15 @@
             w_orth = w_orth - self.projection_operator(W[[i], :].T, w_orth)
 
         # Normalise w_gorth
         w_orth /= np.linalg.norm(w_orth)
 
         return w_orth
 
-    def global_gso(self, W):  # Important to FastICA
+    def global_gso(self, W):  # Important to negentropy-based ICA
         """
         A method that orthogonalises a set of Nx1 vectors
         stores in some W matrix of shape MxN.
 
         Parameters
         ----------
         W: ndarray
```

### Comparing `spectrally_constrained_lvms-0.1.0.1/spectrally_constrained_LVMs/negen_approx.py` & `spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/negen_approx.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+# Copyright 2023-present Ryan Balshaw
 """
-The negentropy approximation functions for the FastICA methods.
+The negentropy approximation functions for the negentropy-based ICA methods.
 """
 import numpy as np
 
 
 class general_object(object):
     """
     An object that implements the first derivative, second derivative and
     gamma functions of the XXXX (fill in here) function. These functions are used in the
-    negentropy calculation for FastICA.
+    negentropy calculation for negentropy-based ICA.
 
     Methods
     -------
     function(u = float)
         Return the function form of G(u) for the XXXX function
 
     first_derivative(u = float)
@@ -87,15 +88,15 @@
         return None
 
 
 class logcosh_object(object):
     """
     An object that implements the first derivative, second derivative and
     gamma functions of the logcosh function. These functions are used in the
-    negentropy approximation calculation for FastICA.
+    negentropy approximation calculation for negentropy-based ICA.
 
     Methods
     -------
     function(u = float) -> 1/a1 * log((exp(a1 * u) + exp(-a1 * u)) / 2)
         Return the function form of G(u) for the logcosh function
 
     first_derivative(u = float) -> tanh
@@ -229,15 +230,15 @@
     #     return np.array([-1, 1]) * deriv.reshape(-1, 1)
 
 
 class exp_object(object):
     """
     An object that implements the first derivative, second derivative and
     gamma functions of the exp function. These functions are used in the
-    negentropy approximation calculation for FastICA.
+    negentropy approximation calculation for negentropy-based ICA.
 
     Methods
     -------
     function(u = float) -> -1/a2 * exp(-a2/2 * u^2)
         Return the function form of G(u) for the exp function
 
     first_derivative(u = float) -> u * exp(-a2/2 * u^2)
@@ -333,15 +334,15 @@
         return (1 - self.a2 * u * u) / u
 
 
 class quad_object(object):
     """
     An object that implements the first derivative, second derivative and
     gamma functions of the quad (u**4) function. These functions are used in the
-    negentropy approximation calculation for FastICA.
+    negentropy approximation calculation for negentropy-based ICA.
 
     Methods
     -------
     function(u = float) -> 1/4 u^4
         Return the function form of G(u) for the quartic function
 
     first_derivative(u = float) -> u^3
@@ -412,15 +413,15 @@
         return 3 / u
 
 
 class cube_object(object):
     """
     An object that implements the first derivative, second derivative and
     gamma functions of the quad (u**4) function. These functions are used in the
-    negentropy approximation calculation for FastICA.
+    negentropy approximation calculation for negentropy-based ICA.
 
     Methods
     -------
     function(u = float) -> u^3
         Return the function form of G(u) for the quartic function
 
     first_derivative(u = float) -> 3 u^2
@@ -525,14 +526,14 @@
     elif source_name.lower() == "cube":
         source_instance = cube_object()
 
     else:
         print("Source name ({}) is unknown. Exiting the function.".format(source_name))
         raise SystemExit
 
-    # Initialise expected value for G(nu) (for the FastICA objective)
+    # Initialise expected value for G(nu) (for the negentropy-based ICA objective)
 
     source_expectation = np.mean(
         source_instance.function(np.random.randn(100000))
     )  # 1 hundred thousand samples... hot damn
 
     return source_instance, source_expectation
```

### Comparing `spectrally_constrained_lvms-0.1.0.1/spectrally_constrained_LVMs/spectrally_constrained_linear_model.py` & `spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/spectrally_constrained_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,34 @@
+# Copyright 2023-present Ryan Balshaw
 """
 A complete implementation of the scICA method.
 """
 
 import os
 import time
+from typing import TypeVar
 
 import numpy as np
 import scipy.optimize as sciopt
 import scipy.stats as scistats
 from matplotlib import pyplot as plt
 from tqdm import tqdm
 
-from .constraint import spectral_objective
-from .helper import (
+from .cost_functions import costClass
+from .helper_methods import (
     batch_sampler,
     data_processor,
     deflation_orthogonalisation,
     quasi_Newton,
 )
+from .spectral_constraint import spectral_objective
 
 
 def initialise_W(n_sources, m, init_type):
+    """initialise_W docstring"""
     if init_type == "broadband":
         W = np.zeros((n_sources, m))
 
         # Set to one (impulse response)
         W[:, 0] = 1
 
     elif init_type == "random":
@@ -37,59 +41,62 @@
     # Normalise rows
     W /= np.linalg.norm(W, axis=1, keepdims=True)
 
     return W
 
 
 def initialise_lambda(n_sources):
+    """initialise_lambda docstring"""
     Lambda = np.ones((n_sources, 1))  # np.zeros((n_sources, 1)) #
 
     return Lambda
 
 
 class linear_model(object):
+    """Linear model docstring"""
+
     def __init__(
         self,
         n_sources: int,  # keep
-        cost_instance,  # keep
+        cost_instance: TypeVar("cost_inst", bound=costClass),  # keep
         whiten: bool = True,  # keep
         init_type: str = "broadband",  # broadband or random - keep
-        organise_by_kurtosis: bool = False,  # keep
+        organise_by_kurt: bool = False,  # keep
         perform_gso: bool = True,  # keep
-        batch_size: bool = None,  # keep
-        var_PCA: bool = None,  # keep
-        alpha_reg: float = 1,  # keep
+        batch_size: int | None = None,  # keep
+        var_PCA: bool | None = None,  # keep
+        alpha_reg: float = 1.0,  # keep
         sumt_flag: bool = False,  # keep
-        sumt_parameters: dict = {
+        sumt_parameters: dict[str, float] = {  # keep
             "alpha_init": 0.1,
             "alpha_end": 10,
             "alpha_multiplier": 10,
         },
-        jacobian_update_type: str = "full",  # full, SR1, DFP, BFGS
-        use_ls: bool = False,
-        use_hessian: bool = True,
-        save_dir: str | None = None,
-        verbose: bool = False,
+        hessian_update_type: str = "full",  # full, SR1, DFP, BFGS
+        use_ls: bool = True,  # keep
+        use_hessian: bool = True,  # Controls whether SGD or Newton
+        save_dir: bool | None = None,  # Not sure
+        verbose: bool = False,  # keep
     ):
         # Initialise instances
         self.n_sources = n_sources
         self.cost_instance = cost_instance  # ({'source_name':'exp', 'alpha':1})
         self.whiten = whiten
         self.var_PCA = var_PCA
         self.init_type = init_type.lower()
-        self.organise_by_kurtosis = (
-            organise_by_kurtosis  # A flag used to organise the ICA components
+        self.organise_by_kurt = (
+            organise_by_kurt  # A flag used to organise the ICA components
         )
         self.perform_gso = perform_gso
         self.batch_size = batch_size
         self.alpha_reg = alpha_reg
         self.sumt_flag = sumt_flag  # SUMT approach to alpha_reg
         self.sumt_parameters = sumt_parameters  # Parameters for SUMT updating
-        self.jacobian_update_type = (
-            jacobian_update_type.lower()
+        self.hessian_update_type = (
+            hessian_update_type.lower()
         )  # Type of jacobian update
         self.use_ls = use_ls
         self.use_hessian = use_hessian
         self.save_dir = save_dir
         self.verbose = verbose
 
         # Initialise the processor instance  (could be in base class except for var_PCA)
@@ -108,85 +115,34 @@
                 "alpha_end"
             ]  # Overrides the default value
             self.alpha_multiplier = self.sumt_parameters["alpha_multiplier"]
 
             self.alpha_cnt = 0
 
         # Quasi-Newton solvers
-        if self.jacobian_update_type != "full":
+        if self.hessian_update_type != "full":
             self.quasi_newton_inst = quasi_Newton(
-                self.jacobian_update_type, use_inverse=True
+                self.hessian_update_type, use_inverse=True
             )
             print("Using a quasi-Newton iteration scheme.")
 
-        if self.jacobian_update_type != "full" and self.use_hessian:
+        if self.hessian_update_type != "full" and self.use_hessian:
             print(
                 "Selected quasi-Newton scheme but opted to "
                 "not use hessian in update step."
                 "\nDefaulting to quasi-Newton scheme."
             )
 
         if type(self.n_sources) != int:
             print("Please enter in a valid number of sources.")
             raise SystemExit
 
         if not self.whiten:
             print("Non-whitened version is chosen.")
 
-    def check_gradient(self, step_size, X, w, y, W, idx, lambda_vector):
-        # Finite difference gradient approximation (central difference)
-
-        x0 = np.vstack((w, lambda_vector))
-
-        grad_current = self._gradient(x0, self, W, X, idx).reshape(-1, 1)
-        grad_check = np.zeros_like(grad_current)
-
-        for i in range(grad_check.shape[0]):
-            e_i = np.zeros_like(x0)
-            e_i[i, 0] = step_size
-
-            f_f = self._function(x0 + e_i, self, W, X, idx)
-            f_b = self._function(x0 - e_i, self, W, X, idx)
-
-            grad_check[i, 0] = (f_f - f_b) / (2 * step_size)
-
-        norm = np.linalg.norm(grad_current - grad_check)
-
-        return grad_current, grad_check, norm
-
-    def check_hessian(self, step_size, X, w, y, W, idx, lambda_vector):
-        # Finite difference Hessian approximation (central difference)
-
-        x0 = np.vstack((w.copy(), lambda_vector.copy()))
-        hess_current = self._hessian(x0, self, W, X, idx)
-        hess_check = np.zeros_like(hess_current)
-
-        r, c = hess_check.shape
-
-        for i in range(r):
-            e_i = np.zeros_like(x0)
-            e_i[i, 0] = step_size
-
-            for j in range(c):
-                x0 = np.vstack((w.copy(), lambda_vector.copy()))
-
-                e_j = np.zeros_like(x0)
-                e_j[j, 0] = step_size
-
-                f1 = self._function(x0 + e_i + e_j, self, W, X, idx)
-                f2 = self._function(x0 + e_i - e_j, self, W, X, idx)
-                f3 = self._function(x0 - e_i + e_j, self, W, X, idx)
-                f4 = self._function(x0 - e_i - e_j, self, W, X, idx)
-
-                hess_check[i, j] = (f1 - f2 - f3 + f4) / (4 * step_size**2)
-
-        norm = np.mean(np.linalg.norm(hess_current - hess_check, axis=1))
-
-        return hess_current, hess_check, norm
-
     def kurtosis(self, y):  # Important to FastICA
         if self.whiten:  # y is zero-mean unit-variance
             if y.shape[1] == 1:
                 return np.mean(y**4) - 3
 
             else:
                 return np.mean(y**4, axis=0) - 3
@@ -375,44 +331,22 @@
         jacobian = np.vstack((j_top, j_bot))
 
         return jacobian
 
     def Newton_update(self, X, w, y, W, idx, lambda_vector):
         if self.gradient_store is None:
             # t0 = time.time()
-
-            # if self.cnt_iter == 0:
-            #     grad_orig, grad_check, grad_norm = self.check_gradient(1e-3,
-            #                                               X,
-            #                                               w,
-            #                                               y,
-            #                                               W,
-            #                                               idx,
-            #                                               lambda_vector)
-            #     print(f"\nGradient norm: {grad_norm}")
-            #
-            #     hess_orig, hess_check, hess_norm = self.check_hessian(1e-3,
-            #                                                   X,
-            #                                                   w,
-            #                                                   y,
-            #                                                   W,
-            #                                                   idx,
-            #                                                   lambda_vector)
-            #     print(f"\nHessian norm: {hess_norm}")
-            #
-            #     print("Nothing")
-
             gradient = self.lagrange_gradient(X, w, y, W, idx, lambda_vector)
             # t1 = time.time()
             # print(f"Calculate derivative: {t1 - t0} seconds")
 
         else:
             gradient = self.gradient_store  # Use the new stored gradient
 
-        if self.jacobian_update_type == "full":
+        if self.hessian_update_type == "full":
             # t0 = time.time()
 
             if self.use_hessian:
                 jacobian = self.lagrange_hessian(X, w, y, W, idx, lambda_vector)
 
             else:
                 jacobian = np.eye(gradient.shape[0])
@@ -511,14 +445,15 @@
         #     print("Hit a break, check out why it is taking so long.")
 
         return delta_w, delta_lambda, gradient
 
     def spectral_trainer(self, X, W, n_iters, learning_rate, tol, Lambda, Fs):
         # Initialise training metrics
         self.kurtosis_ = []
+        self.variance_ = []
         self.grad_norm_ = []
         self.cost_ = []
         self.lagrange_cost_ = []
         self.w_similarity_ = []
         self.spectral_loss_ = []
 
         # Done to ensure that we do not update W (numpy memory pointing effect)
@@ -533,14 +468,15 @@
         for idx in range(0, W_.shape[0], 1):
             w_new = W_[[idx], :].T.copy()
 
             lambda_new = Lambda_[[idx], :].T.copy()  # Should just be a 1 x 1 vector
 
             grad_norm = np.zeros(n_iters)
             kurtosis = np.zeros(n_iters)
+            variance = np.zeros(n_iters)
             obj_cost = np.zeros(n_iters)
             lagrange_loss = np.zeros(n_iters)
             w_similarity = np.zeros(n_iters)
             spectral_loss = np.zeros(n_iters)
 
             if idx > 0:
                 # Make grid to extract from W_
@@ -549,15 +485,15 @@
                 # Compute the Hessian
                 self._hessian_constraint = np.sum(
                     self.spectral_obj.spectral_hessian(w_new, W_[ix_grid].copy()),
                     axis=0,
                 )
 
             # Update
-            if self.jacobian_update_type != "full":
+            if self.hessian_update_type != "full":
                 self.quasi_newton_inst.initialise_jacobian(self.n_sources + 1)
 
             self.cnt_iter = 0
             error = np.inf
 
             if self.verbose:
                 pbar = tqdm(total=n_iters)
@@ -588,43 +524,40 @@
 
                 w_prev = w_new.copy()
 
                 w_new, lambda_new = self.update_params(
                     w_new, lambda_new, delta_w, delta_lambda, W_, idx
                 )
 
-                # t1 = time.time()
-                # print(f"\nCalculate update: {t1 - t0} seconds")
-
-                # # Store metrics
-                # t0 = time.time()
-
+                # Generate stored metrics
                 y_new = np.dot(X, w_new)
                 grad_norm[self.cnt_iter] = np.linalg.norm(gradient)
                 kurtosis[self.cnt_iter] = self.kurtosis(y_new)
+                variance[self.cnt_iter] = np.std(y_new)
                 obj_cost[self.cnt_iter] = self.cost_instance.cost(X, w_new, y_new)
                 lagrange_loss[self.cnt_iter] = self.lagrange_function(
                     X, w_new, y_new, W_, idx, lambda_new
                 )
                 w_similarity[self.cnt_iter] = np.abs(w_new.T @ w_prev - 1)[0, 0]
+
                 # Compute spectral loss term
                 if idx > 0:
                     idx_grid = np.ix_(np.arange(0, idx, 1), np.arange(W_.shape[1]))
                     spectral_loss[self.cnt_iter] = self.alpha_reg * np.sum(
                         self.spectral_obj.spectral_loss(w_new, W_[idx_grid]), axis=0
                     )
 
                 else:
                     spectral_loss[self.cnt_iter] = 0
 
                 # t1 = time.time()
                 # print(f"Calculate metrics: {t1 - t0} seconds")
                 # t0 = time.time()
 
-                if self.cnt_iter > 1:
+                if self.cnt_iter > 5:
                     error = w_similarity[self.cnt_iter]
 
                 # Update the iterator
                 if self.verbose:
                     pbar.update(1)
                     pbar.set_description(
                         f"Component {idx + 1} - " f"Error: {np.round(error, 6)}"
@@ -648,31 +581,31 @@
                 # Plot
                 ax[0].set_title("Spectral content")
                 ax[0].plot(freq, vals, color="#003f5c")
 
                 ax[1].set_title(r"$\Delta x$ norm")
                 ax[1].semilogy(grad_norm[: self.cnt_iter], color="#444e86")
 
-                ax[2].set_title("Latent kurtosis")
-                ax[2].plot(kurtosis[: self.cnt_iter], color="#955196")
+                ax[2].set_title("Latent variance")
+                ax[2].plot(variance[: self.cnt_iter], color="#955196")
 
-                ax[3].set_title("Original loss")
-                ax[3].plot(obj_cost[: self.cnt_iter], color="#dd5182")
+                ax[3].set_title("Latent kurtosis")
+                ax[3].plot(kurtosis[: self.cnt_iter], color="#955196")
 
-                ax[4].set_title("Lagrange function loss")
-                ax[4].plot(lagrange_loss[: self.cnt_iter], color="#ff6e54")
+                ax[4].set_title("Original loss")
+                ax[4].plot(obj_cost[: self.cnt_iter], color="#dd5182")
 
-                ax[5].set_title("Update similarity")
-                ax[5].plot(w_similarity[: self.cnt_iter], color="#ffa600")
+                ax[5].set_title("Lagrange function loss")
+                ax[5].plot(lagrange_loss[: self.cnt_iter], color="#ff6e54")
 
-                ax[6].set_title("Spectral constraint")
-                ax[6].plot(spectral_loss[: self.cnt_iter], color="b")
+                ax[6].set_title("Update similarity")
+                ax[6].plot(w_similarity[: self.cnt_iter], color="#ffa600")
 
-                # ax[7].set_title("R term")
-                # ax[7].plot(self.r, color="b")
+                ax[7].set_title("Spectral constraint")
+                ax[7].plot(spectral_loss[: self.cnt_iter], color="b")
 
                 for axs in ax:
                     axs.grid()
 
                 for axs in ax[1:]:
                     axs.set_xlabel("Iteration index")
 
@@ -687,27 +620,24 @@
 
                 plt.savefig(os.path.join(self.save_dir, save_name))
 
                 plt.close("all")
 
             # Close the iterator
             if self.verbose:
-                pbar.set_description(
-                    f"\nCompleted solving for component {idx + 1} "
-                    f"in {self.cnt_iter} iterations."
-                )
                 pbar.close()
 
             # Store W and lambda
             W_[idx, :] = w_new[:, 0]
 
             Lambda_[idx, :] = lambda_new.copy()  # Should just be a 1 x 1 vector
 
             # t0 = time.time()
             self.kurtosis_.append(kurtosis[: self.cnt_iter])
+            self.variance_.append(variance[: self.cnt_iter])
             self.grad_norm_.append(grad_norm[: self.cnt_iter])
             self.cost_.append(obj_cost[: self.cnt_iter])
             self.lagrange_cost_.append(lagrange_loss[: self.cnt_iter])
             self.w_similarity_.append(w_similarity[: self.cnt_iter])
             self.spectral_loss_.append(spectral_loss[: self.cnt_iter])
 
             # t1 = time.time()
@@ -746,28 +676,27 @@
     def spectral_fit(
         self,
         X,
         W,
         n_iters=1,
         learning_rate=0.1,
         tol=1e-3,
-        approx_flag=False,
         Lambda=None,
         Fs: float | int = 25e3,
     ):
         # Call the spectral trainer
         W_update, Lambda_update = self.spectral_trainer(
             X, W, n_iters, learning_rate, tol, Lambda, Fs
         )
 
         # Calculate the excess kurtosis
         Y = np.dot(X, W_update.T)
         kurt = np.mean(Y**4, axis=0) - 3  # Excess kurtosis
 
-        if self.organise_by_kurtosis:
+        if self.organise_by_kurt:
             pos_idx = np.argsort(kurt)[::-1]
             kurt = kurt[pos_idx]
 
             W_update = W_update[pos_idx, :]
             if self.verbose:
                 print("\nOrganised W by source excess kurtosis.")
 
@@ -795,25 +724,24 @@
 
             if self.sumt_flag:
                 save_name = f"spectral_W_alpha={self.alpha_cnt}.png"
 
             else:
                 save_name = "spectral_W_final.png"
             plt.savefig(os.path.join(self.save_dir, save_name))
-            plt.show()
+            plt.close("all")
 
         return W_update, Lambda_update
 
     def fit(
         self,
         X,
-        n_iters=1,
-        learning_rate=0.1,
-        tol=1e-3,
-        approx_flag=False,
+        n_iters=100,
+        learning_rate=1,
+        tol=1e-4,
         Fs: int | float = 25e3,
     ):
         # Initialise pre-processing
         self.processor_inst.initialise_preprocessing(X)
 
         # Pre-process the data
         X_preprocess = self.processor_inst.preprocess_data(X)
@@ -852,23 +780,23 @@
             while self.alpha_reg <= self.alpha_end:
                 W_update, Lambda_update = self.spectral_fit(
                     X_preprocess,
                     W_iters[-1],
                     n_iters,
                     learning_rate,
                     tol,
-                    approx_flag,
                     lambda_iters[-1],
                     Fs,
                 )
 
                 # Store solution and parameters
                 param_iters.append(
                     (
                         self.kurtosis_,
+                        self.variance_,
                         self.grad_norm_,
                         self.cost_,
                         self.lagrange_cost_,
                         self.w_similarity_,
                         self.spectral_loss_,
                     )
                 )
@@ -906,14 +834,15 @@
                 self.alpha_reg = self.alpha_reg * self.alpha_multiplier
 
             # Store actual and value over iterations.
             pos_min = np.argmin(solution_error)
             self.solution_error = solution_error
             (
                 self.kurtosis_,
+                self.variance_,
                 self.grad_norm_,
                 self.cost_,
                 self.lagrange_cost_,
                 self.w_similarity_,
                 self.spectral_loss_,
             ) = param_iters[pos_min]
 
@@ -937,15 +866,14 @@
         else:
             W_update, Lambda_update = self.spectral_fit(
                 X_preprocess,
                 W,
                 n_iters,
                 learning_rate,
                 tol,
-                approx_flag,
                 Lambda,
                 Fs,
             )
 
             # Store the parameters
             self.W = W_update
             self.Lambda = Lambda_update
```

### Comparing `spectrally_constrained_lvms-0.1.0.1/setup.py` & `spectrally_constrained_lvms-0.1.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,78 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: spectrally-constrained-lvms
+Version: 0.1.0.2
+Summary: An optimisation implementation of linear transforms with a spectral constraint.
+Home-page: https://github.com/RyanBalshaw/scICA
+License: MIT
+Keywords: Linear transformation,spectral constraint,PCA,ICA
+Author: Ryan Balshaw
+Author-email: ryanbalshaw81@gmail.com
+Maintainer: Ryan Balshaw
+Maintainer-email: ryanbalshaw81@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation
+Classifier: Topic :: Scientific/Engineering
+Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
+Requires-Dist: numpy (>=1.23.1,<2.0.0)
+Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
+Requires-Dist: scipy (>=1.8.1,<2.0.0)
+Requires-Dist: sympy (>=1.11.1,<2.0.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Project-URL: Bug tracker, https://github.com/RyanBalshaw/scICA/issues
+Project-URL: Documentation, https://github.com/RyanBalshaw/scICA
+Project-URL: Repository, https://github.com/RyanBalshaw/scICA
+Description-Content-Type: text/markdown
+
+# Spectrally constrained LVMs
+
+![GitHub](https://img.shields.io/github/license/RyanBalshaw/spectrally-constrained-LVMs)
+![GitHub issues](https://img.shields.io/github/issues-raw/RyanBalshaw/spectrally-constrained-LVMs)
+![PyPI](https://img.shields.io/pypi/v/spectrally-constrained-lvms)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/spectrally-constrained-lvms?color=blueviolet)
+![Read the Docs](https://img.shields.io/readthedocs/spectrally-constrained-lvms)
+![GitHub last commit](https://img.shields.io/github/last-commit/RyanBalshaw/spectrally-constrained-LVMs)
+
+A repository for all code for the package. This is the first setup of this project.
+
+The package can be installed using [pip](https://pypi.org/project/pip/):
+
+# Documentation
+Please visit... for the documentation.
+
+## Purpose
+words words words
+
+# Installation
+
+```sh
+pip install package_name
+```
+
+*Current version:* 0.1.0
+
+# Requirements
+
+This package used Python >= 3.xxx or later to run. For other python dependencies, please check the `pyproject.toml`
+file included in this repository.
+
+Note that the following packages should be installed on your system:
+- Numpy
+
+# API usage
+
+A generic example is shown below:
+```shell
 
-packages = \
-['spectrally_constrained_lvms']
+```
 
-package_data = \
-{'': ['*']}
+# Contributing
+Words words words
 
-install_requires = \
-['matplotlib>=3.5.2,<4.0.0',
- 'numpy>=1.23.1,<2.0.0',
- 'scikit-learn>=1.1.2,<2.0.0',
- 'scipy>=1.8.1,<2.0.0',
- 'sympy>=1.11.1,<2.0.0',
- 'tqdm>=4.64.1,<5.0.0']
-
-setup_kwargs = {
-    'name': 'spectrally-constrained-lvms',
-    'version': '0.1.0.1',
-    'description': 'An optimisation implementation of linear transforms with a spectral constraint.',
-    'long_description': '# Spectrally constrained linear transformations\n\n![GitHub](https://img.shields.io/github/license/RyanBalshaw/spectrally-constrained-LVMs)\n![GitHub issues](https://img.shields.io/github/issues-raw/RyanBalshaw/spectrally-constrained-LVMs)\n![PyPI](https://img.shields.io/pypi/v/spectrally-constrained-lvms)\n\nA repository for all code for sICA. This is the first setup of this project.\n\nThe package can be installed using [pip](https://pypi.org/project/pip/):\n\n# Documentation\nPlease visit... for the documentation.\n\n## Purpose\nwords words words\n\n# Installation\n\n```sh\npip install package_name\n```\n\n*Current version:* 0.1.0\n\n# Requirements\n\nThis package used Python >= 3.xxx or later to run. For other python dependencies, please check the `pyproject.toml`\nfile included in this repository.\n\nNote that the following packages should be installed on your system:\n- Numpy\n\n# API usage\n\nA generic example is shown below:\n```shell\n\n```\n\n# Contributing\nWords words words\n\n# License\n',
-    'author': 'Ryan Balshaw',
-    'author_email': 'ryanbalshaw81@gmail.com',
-    'maintainer': 'Ryan Balshaw',
-    'maintainer_email': 'ryanbalshaw81@gmail.com',
-    'url': 'https://github.com/RyanBalshaw/scICA',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+# License
 
-
-setup(**setup_kwargs)
```

