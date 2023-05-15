# Comparing `tmp/pedon-0.0.2.tar.gz` & `tmp/pedon-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedon-0.0.2.tar", last modified: Fri Mar 10 14:43:58 2023, max compression
+gzip compressed data, was "pedon-0.0.3.tar", last modified: Mon May 15 07:16:15 2023, max compression
```

## Comparing `pedon-0.0.2.tar` & `pedon-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:43:58.930760 pedon-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-10 14:43:40.000000 pedon-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-03-10 14:43:58.930760 pedon-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-10 14:43:40.000000 pedon-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-03-10 14:43:40.000000 pedon-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 14:43:58.930760 pedon-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:43:58.926760 pedon-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:43:58.926760 pedon-0.0.2/src/pedon/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-10 14:43:40.000000 pedon-0.0.2/src/pedon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-03-10 14:43:40.000000 pedon-0.0.2/src/pedon/_params.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-10 14:43:40.000000 pedon-0.0.2/src/pedon/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-10 14:43:40.000000 pedon-0.0.2/src/pedon/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:43:58.930760 pedon-0.0.2/src/pedon/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)    15232 2023-03-10 14:43:40.000000 pedon-0.0.2/src/pedon/datasets/Soil_Parameters.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    25888 2023-03-10 14:43:40.000000 pedon-0.0.2/src/pedon/datasets/Staring_2001.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-03-10 14:43:40.000000 pedon-0.0.2/src/pedon/datasets/Staring_2018.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    14725 2023-03-10 14:43:40.000000 pedon-0.0.2/src/pedon/soil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-03-10 14:43:40.000000 pedon-0.0.2/src/pedon/soilmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:43:58.930760 pedon-0.0.2/src/pedon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-03-10 14:43:58.000000 pedon-0.0.2/src/pedon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-10 14:43:58.000000 pedon-0.0.2/src/pedon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 14:43:58.000000 pedon-0.0.2/src/pedon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-10 14:43:58.000000 pedon-0.0.2/src/pedon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-10 14:43:58.000000 pedon-0.0.2/src/pedon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:43:58.930760 pedon-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-10 14:43:40.000000 pedon-0.0.2/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-10 14:43:40.000000 pedon-0.0.2/tests/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-10 14:43:40.000000 pedon-0.0.2/tests/test_ptf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-10 14:43:40.000000 pedon-0.0.2/tests/test_soilmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:16:15.764203 pedon-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-15 07:15:56.000000 pedon-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-15 07:16:15.764203 pedon-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-15 07:15:56.000000 pedon-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-15 07:15:56.000000 pedon-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 07:16:15.764203 pedon-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:16:15.760203 pedon-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:16:15.760203 pedon-0.0.3/src/pedon/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-15 07:15:56.000000 pedon-0.0.3/src/pedon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-15 07:15:56.000000 pedon-0.0.3/src/pedon/_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 07:15:56.000000 pedon-0.0.3/src/pedon/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 07:15:56.000000 pedon-0.0.3/src/pedon/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:16:15.764203 pedon-0.0.3/src/pedon/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)    15232 2023-05-15 07:15:56.000000 pedon-0.0.3/src/pedon/datasets/Soil_Parameters.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    25888 2023-05-15 07:15:56.000000 pedon-0.0.3/src/pedon/datasets/Staring_2001.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-05-15 07:15:56.000000 pedon-0.0.3/src/pedon/datasets/Staring_2018.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    16321 2023-05-15 07:15:56.000000 pedon-0.0.3/src/pedon/soil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-05-15 07:15:56.000000 pedon-0.0.3/src/pedon/soilmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:16:15.764203 pedon-0.0.3/src/pedon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-15 07:16:15.000000 pedon-0.0.3/src/pedon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-15 07:16:15.000000 pedon-0.0.3/src/pedon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:16:15.000000 pedon-0.0.3/src/pedon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-15 07:16:15.000000 pedon-0.0.3/src/pedon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 07:16:15.000000 pedon-0.0.3/src/pedon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:16:15.764203 pedon-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-15 07:15:56.000000 pedon-0.0.3/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-15 07:15:56.000000 pedon-0.0.3/tests/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-15 07:15:56.000000 pedon-0.0.3/tests/test_ptf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-15 07:15:56.000000 pedon-0.0.3/tests/test_soilmodel.py
```

### Comparing `pedon-0.0.2/LICENSE` & `pedon-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pedon-0.0.2/pyproject.toml` & `pedon-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pedon-0.0.2/src/pedon/_params.py` & `pedon-0.0.3/src/pedon/_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             "n": 1.000001,
             "l": -7,
         },
         "p_max": {
             "k_s": 100000.0,
             "theta_r": 0.2,
             "theta_s": 0.9,
-            "alpha": 0.15,
+            "alpha": 0.20,
             "n": 12,
             "l": 8,
         },
         "swrc": {
             "k_s": False,
             "theta_r": True,
             "theta_s": True,
@@ -70,31 +70,31 @@
     data={
         "p_ini": {
             "k_s": 50.0,
             "theta_r": 0.02,
             "theta_s": 0.4,
             "alpha": 0.02,
             "beta": 2.3,
-            "brook": 0.5,
+            "brook": 10.0,
         },
         "p_min": {
             "k_s": 0.001,
             "theta_r": 1e-5,
             "theta_s": 0.2,
             "alpha": 0.001,
             "beta": 1.0,
-            "brook": -7,
+            "brook": 1.0,
         },
         "p_max": {
             "k_s": 100000.0,
             "theta_r": 0.2,
             "theta_s": 0.5,
-            "alpha": 0.15,
+            "alpha": 0.30,
             "beta": 12,
-            "brook": 8,
+            "brook": 50.0,
         },
         "swrc": {
             "k_s": False,
             "theta_r": True,
             "theta_s": True,
             "alpha": True,
             "beta": True,
```

### Comparing `pedon-0.0.2/src/pedon/datasets/Soil_Parameters.xlsx` & `pedon-0.0.3/src/pedon/datasets/Soil_Parameters.xlsx`

 * *Files identical despite different names*

### Comparing `pedon-0.0.2/src/pedon/datasets/Staring_2001.xlsx` & `pedon-0.0.3/src/pedon/datasets/Staring_2001.xlsx`

 * *Files identical despite different names*

### Comparing `pedon-0.0.2/src/pedon/datasets/Staring_2018.xlsx` & `pedon-0.0.3/src/pedon/datasets/Staring_2018.xlsx`

 * *Files identical despite different names*

### Comparing `pedon-0.0.2/src/pedon/soil.py` & `pedon-0.0.3/src/pedon/soil.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from numpy import append, exp, log, ones
 from pandas import DataFrame, read_excel
 from scipy.optimize import least_squares
 
 from ._params import get_params
 from ._typing import FloatArray
-from .soilmodel import Brooks, Genuchten, SoilModel
+from .soilmodel import Brooks, Genuchten, SoilModel, get_soilmodel
 
 
 @dataclass
 class SoilSample:
     sand_p: float | None = None  # sand %
     silt_p: float | None = None  # silt %
     clay_p: float | None = None  # clay %
@@ -112,50 +112,63 @@
         self,
         sm: Type[SoilModel],
         pbounds: DataFrame | None = None,
         weights: FloatArray | None = None,
         W1: float | None = None,
         W2: float | None = None,
         return_res: bool = False,
+        k_s: float | None = None,
     ) -> SoilModel:
         """Same method as RETC"""
+
+        theta = self.theta
+        k = self.k
+
         if pbounds is None:
             pbounds = get_params(sm.__name__)
-            pbounds.loc["k_s", "p_ini"] = max(self.k)
-            pbounds.loc["k_s", "p_max"] = max(self.k) * 10
-            pbounds.loc["theta_s", "p_ini"] = max(self.theta)
-            pbounds.loc["theta_s", "p_max"] = max(self.theta) + 0.02
+            if k_s is not None:
+                pbounds = pbounds.drop("k_s")
+            else:
+                pbounds.loc["k_s", "p_ini"] = max(k)
+                pbounds.loc["k_s", "p_max"] = max(k) * 10
+            pbounds.loc["theta_s", "p_ini"] = max(theta)
+            pbounds.loc["theta_s", "p_max"] = max(theta) + 0.02
 
         if weights is None:
             weights = ones(self.h.shape)
 
         if W1 is None:
             W1 = 0.1
 
         if W2 is None:
-            M = len(self.k) + len(self.theta)
-            N = len(self.theta)
-            W2 = (M - N) * sum(weights * self.theta) / (N * sum(weights * self.k))
+            M = len(k) + len(theta)
+            N = len(theta)
+            W2 = (M - N) * sum(weights * theta) / (N * sum(weights * k))
 
         def fit_staring(p: FloatArray) -> FloatArray:
-            sml = sm(**dict(zip(pbounds.index, p)))
-            theta_diff = sml.theta(h=self.h) - self.theta
-            k_diff = log(sml.k(h=self.h)) - log(self.k)
+            est_pars = dict(zip(pbounds.index, p))
+            if k_s is not None:
+                est_pars["k_s"] = k_s
+            sml = sm(**est_pars)
+            theta_diff = sml.theta(h=self.h) - theta
+            k_diff = log(sml.k(h=self.h)) - log(k)
             diff = append(weights * theta_diff, weights * W1 * W2 * k_diff)
             return diff
 
         res = least_squares(
             fit_staring,
             x0=pbounds.loc[:, "p_ini"],
             bounds=(
                 pbounds.loc[:, "p_min"],
                 pbounds.loc[:, "p_max"],
             ),
         )
         opt_pars = dict(zip(pbounds.index, res.x))
+        if k_s is not None:
+            opt_pars["k_s"] = k_s
         opt_sm = sm(**opt_pars)
         if return_res:
             return opt_sm, {"res": res}
         return opt_sm
 
     def wosten(self, ts: bool = False) -> Genuchten:
         """Wosten et al (1999) - Development and use of a database of hydraulic
@@ -402,30 +415,66 @@
     name: str
     type: str | None = None
     model: SoilModel | None = None
     sample: SoilSample | None = None
     source: str | None = None
     description: str | None = None
 
-    def from_name(self, sm: Type[SoilModel]) -> "Soil":
+    def from_name(self, sm: Type[SoilModel] | SoilModel | str) -> "Soil":
+        if isinstance(sm, SoilModel):
+            if hasattr(sm, "__name__"):
+                smn = sm.__name__
+            else:
+                smn = sm.__class__.__name__
+                sm = type(sm)
+        elif isinstance(sm, str):
+            smn = sm
+            sm = get_soilmodel(smn)
+
+        else:
+            raise ValueError(
+                f"Argument must either be Type[SoilModel] | SoilModel | str,"
+                f"not {type(sm)}"
+            )
+
         path = Path(__file__).parent / "datasets/Soil_Parameters.xlsx"
-        ser = (
-            read_excel(path, sheet_name=sm.__name__, index_col=0)
-            .loc[self.name]
-            .to_dict()
-        )
+        ser = read_excel(path, sheet_name=smn, index_col=0).loc[self.name].to_dict()
         # path = Path(__file__).parent / f"datasets/{sm.__name__}.csv"
         # ser = read_csv(path, index_col=["name"]).loc[self.name].to_dict()
         self.__setattr__("type", ser.pop("soil type"))
         self.__setattr__("source", ser.pop("source"))
         self.__setattr__("description", ser.pop("description"))
         self.__setattr__("model", sm(**ser))
         return self
 
+    @staticmethod
+    def list_names(sm: Type[SoilModel] | SoilModel | str) -> list[str]:
+        if isinstance(sm, SoilModel):
+            if hasattr(sm, "__name__"):
+                smn = sm.__name__
+            else:
+                smn = sm.__class__.__name__
+                sm = type(sm)
+        elif isinstance(sm, str):
+            smn = sm
+            sm = get_soilmodel(smn)
+
+        else:
+            raise ValueError(
+                f"Argument must either be Type[SoilModel] | SoilModel | str,"
+                f"not {type(sm)}"
+            )
+
+        path = Path(__file__).parent / "datasets/Soil_Parameters.xlsx"
+        names = read_excel(path, sheet_name=smn).loc[:, "name"].to_list()
+        return names
+
     def from_staring(self, year: str = "2018") -> "Soil":
+        if year not in ("2001", 2001, "2018", 2018):
+            raise ValueError(f"Year must either be '2001' or '2018', not {year}")
         path = Path(__file__).parent / f"datasets/Staring_{year}.xlsx"
         parameters = read_excel(path, sheet_name="parameters", index_col=0)
         ser = parameters.loc[self.name].to_dict()
         self.__setattr__("type", ser.pop("soil type"))
         self.__setattr__("source", ser.pop("source"))
         self.__setattr__("description", ser.pop("description"))
         sm = Genuchten(**ser)
```

### Comparing `pedon-0.0.2/src/pedon.egg-info/SOURCES.txt` & `pedon-0.0.3/src/pedon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pedon-0.0.2/tests/test_fit.py` & `pedon-0.0.3/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `pedon-0.0.2/tests/test_soilmodel.py` & `pedon-0.0.3/tests/test_soilmodel.py`

 * *Files identical despite different names*

