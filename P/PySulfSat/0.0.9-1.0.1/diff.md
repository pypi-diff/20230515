# Comparing `tmp/PySulfSat-0.0.9.tar.gz` & `tmp/PySulfSat-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySulfSat-0.0.9.tar", last modified: Fri Jan 20 19:50:14 2023, max compression
+gzip compressed data, was "PySulfSat-1.0.1.tar", last modified: Mon May 15 20:23:31 2023, max compression
```

## Comparing `PySulfSat-0.0.9.tar` & `PySulfSat-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 19:50:14.565988 PySulfSat-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-20 19:50:14.565988 PySulfSat-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-20 19:50:14.569989 PySulfSat-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 19:50:14.565988 PySulfSat-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 19:50:14.565988 PySulfSat-0.0.9/src/PySulfSat/
--rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_BW2022.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    87168 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_Blanchard2021.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    35617 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_ChowDas22.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    45229 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_Fortin2015.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    27276 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_LiZhang22.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_Liu2021.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    19872 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_MK2015.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    41651 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_OM2022.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    75124 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_Smythe17.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    36905 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Cali_ZT2019.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    71594 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/Smythe17.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/cali_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    38417 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/core_calcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/import_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/mantle_melting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/s6_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/scas_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)    65506 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/scss_calcs2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-01-20 19:50:04.000000 PySulfSat-0.0.9/src/PySulfSat/sulf_mass_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 19:50:14.565988 PySulfSat-0.0.9/src/PySulfSat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-20 19:50:14.000000 PySulfSat-0.0.9/src/PySulfSat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-01-20 19:50:14.000000 PySulfSat-0.0.9/src/PySulfSat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 19:50:14.000000 PySulfSat-0.0.9/src/PySulfSat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-20 19:50:14.000000 PySulfSat-0.0.9/src/PySulfSat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-20 19:50:14.000000 PySulfSat-0.0.9/src/PySulfSat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:23:31.515687 PySulfSat-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-15 20:23:31.515687 PySulfSat-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 20:23:31.515687 PySulfSat-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:23:31.511686 PySulfSat-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:23:31.515687 PySulfSat-1.0.1/src/PySulfSat/
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/Cali_BW2022.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    87168 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/Cali_Blanchard2021.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    35617 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/Cali_ChowDas22.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    45229 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/Cali_Fortin2015.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    27276 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/Cali_LiZhang22.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/Cali_Liu2021.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    19872 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/Cali_MK2015.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    41651 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/Cali_OM2022.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    75124 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/Cali_Smythe17.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    36905 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/Cali_ZT2019.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    71594 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/Smythe17.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/cali_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39287 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/core_calcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/error_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/import_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/mantle_melting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/monte_carlo_s_in_sulf_recon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21606 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/s6_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/scas_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67361 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/scss_calcs2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-15 20:23:20.000000 PySulfSat-1.0.1/src/PySulfSat/sulf_mass_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:23:31.515687 PySulfSat-1.0.1/src/PySulfSat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-15 20:23:31.000000 PySulfSat-1.0.1/src/PySulfSat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-15 20:23:31.000000 PySulfSat-1.0.1/src/PySulfSat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:23:31.000000 PySulfSat-1.0.1/src/PySulfSat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 20:23:31.000000 PySulfSat-1.0.1/src/PySulfSat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 20:23:31.000000 PySulfSat-1.0.1/src/PySulfSat.egg-info/top_level.txt
```

### Comparing `PySulfSat-0.0.9/setup.py` & `PySulfSat-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.9/src/PySulfSat/Cali_BW2022.pkl` & `PySulfSat-1.0.1/src/PySulfSat/Cali_BW2022.pkl`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.9/src/PySulfSat/Cali_Blanchard2021.pkl` & `PySulfSat-1.0.1/src/PySulfSat/Cali_Blanchard2021.pkl`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.9/src/PySulfSat/Cali_ChowDas22.pkl` & `PySulfSat-1.0.1/src/PySulfSat/Cali_ChowDas22.pkl`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.9/src/PySulfSat/Cali_Fortin2015.pkl` & `PySulfSat-1.0.1/src/PySulfSat/Cali_Fortin2015.pkl`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.9/src/PySulfSat/Cali_LiZhang22.pkl` & `PySulfSat-1.0.1/src/PySulfSat/Cali_LiZhang22.pkl`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.9/src/PySulfSat/Cali_Liu2021.pkl` & `PySulfSat-1.0.1/src/PySulfSat/Cali_Liu2021.pkl`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.9/src/PySulfSat/Cali_MK2015.pkl` & `PySulfSat-1.0.1/src/PySulfSat/Cali_MK2015.pkl`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.9/src/PySulfSat/Cali_OM2022.pkl` & `PySulfSat-1.0.1/src/PySulfSat/Cali_OM2022.pkl`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.9/src/PySulfSat/Cali_Smythe17.pkl` & `PySulfSat-1.0.1/src/PySulfSat/Cali_Smythe17.pkl`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.9/src/PySulfSat/Cali_ZT2019.pkl` & `PySulfSat-1.0.1/src/PySulfSat/Cali_ZT2019.pkl`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.9/src/PySulfSat/Smythe17.pkl` & `PySulfSat-1.0.1/src/PySulfSat/Smythe17.pkl`

 * *Files identical despite different names*

### Comparing `PySulfSat-0.0.9/src/PySulfSat/__init__.py` & `PySulfSat-1.0.1/src/PySulfSat/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from PySulfSat.scss_calcs2 import *
 # This has stuff for performing s6+ corrections
 from PySulfSat.s6_corrections import *
 from PySulfSat.scas_calc import *
 from PySulfSat.sulf_mass_balance import *
 from PySulfSat.cali_plots import *
 from PySulfSat.mantle_melting import *
+from PySulfSat.monte_carlo_s_in_sulf_recon import *
+from PySulfSat.error_prop import *
 
 
 # version
 from ._version import __version__
```

### Comparing `PySulfSat-0.0.9/src/PySulfSat/cali_plots.py` & `PySulfSat-1.0.1/src/PySulfSat/cali_plots.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,20 @@
         MK_2015: Masotta and Keppler(2015)
 
 
         CS6:
         O2022_CS6:  ONeill and Mavrogenes (2022)
         BW2022_CS6: Boulliung and Wood (2022)
 
+    Returns
+    -------
+    pd.DataFrame
+        dataframe of the calibration dataset, with column headings MgO_Liq, SiO2_Liq etc.
+
+
     """
 
     #SCSS models
     if model=="S2017_SCSS":
         with open(PySulfSat_dir/'Cali_Smythe17.pkl', 'rb') as f:
             Cali_input=load(f)
```

### Comparing `PySulfSat-0.0.9/src/PySulfSat/core_calcs.py` & `PySulfSat-1.0.1/src/PySulfSat/core_calcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,15 @@
     cat_prop['sum'] = cat_prop.sum(axis='columns')
     cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
     cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
     cat_frac_anhyd.columns = [str(col).replace('prop', 'frac')
                               for col in cat_frac_anhyd.columns]
     cat_frac_anhyd = pd.concat([liq_comps, mol_prop, cat_frac_anhyd], axis=1)
 
+
     if "Fe3Fet_Liq" in cat_frac_anhyd:
         cat_frac_anhyd['Mg_Number_Liq_NoFe3'] = (cat_frac_anhyd['MgO_Liq'] / 40.3044) / (
             (cat_frac_anhyd['MgO_Liq'] / 40.3044) + (cat_frac_anhyd['FeOt_Liq'] / 71.844))
         cat_frac_anhyd['Mg_Number_Liq_Fe3'] = (cat_frac_anhyd['MgO_Liq'] / 40.3044) / (
             (cat_frac_anhyd['MgO_Liq'] / 40.3044) + (cat_frac_anhyd['FeOt_Liq'] * (1 - cat_frac_anhyd['Fe3Fet_Liq']) / 71.844))
     if "Fe3Fet_Liq" not in cat_frac_anhyd:
         cat_frac_anhyd['Mg_Number_Liq_Fe3'] = (cat_frac_anhyd['MgO_Liq'] / 40.3044) / (
@@ -859,17 +860,14 @@
         Temperature in Kelvin (buffer positions are very T-sensitive)
 
     P_kbar: int, flt, pandas.Series
         Pressure in Kbar (Buffer positions are slightly sensitive to pressure)
 
 
 
-
-
-
     model: str
         "Kress1991" - Uses Kress and Carmichael 1991 to calculate XFe2Fe3 from fo2
         "Put2016_eq6b" - Uses Putirka (2016) expression to calculate XFe2Fe3 from fo2
 
     renorm: bool
         Following excel code of K. Iacovino.
         If True, renormalizes other oxide concentrations
@@ -934,14 +932,24 @@
 mol_mass_SO3=mol_mass_S+mol_mass_O*3
 mol_mass_SO4=mol_mass_S+mol_mass_O*4
 mol_mass_SO2=mol_mass_S+mol_mass_O*2
 
 def convert_S_types(SO3_wt=None, SO3_ppm=None, S_wt=None, S_ppm=None, SO2_wt=None, SO2_ppm=None,
  SO4_wt=None, SO4_ppm=None):
     """ converts SO3 in wt% into S in ppm
+
+    Parameters
+    -------------------
+    SO3_wt, SO3_ppm, S_wt, S_ppm, SO2_wt, SO2_ppm, SO4_wt, SO4_ppm: int, float, pd.Series, np.array
+        S in various units and forms
+    Returns
+    -------------------
+    pd.DataFrame
+        S content in all forms listed.
+
     """
     params = {
         "a": SO3_wt,
         "ab": SO3_ppm,
         "b": S_wt,
         "c": S_ppm,
         "d": SO2_wt,
@@ -976,22 +984,33 @@
 
         S_wt2= moles_s*mol_mass_S
         S_ppm2=S_wt2*10**4
         SO2=moles_s*mol_mass_SO2
         SO3=moles_s*mol_mass_SO3
         SO4=moles_s*mol_mass_SO4
 
+        if isinstance(S_wt2, pd.Series) or isinstance(S_wt2, np.ndarray):
+            df=pd.DataFrame(data={
+                                    'S_wt': S_wt2,
+                                    'S_ppm': S_ppm2,
+                                    'SO2_wt': SO2,
+                                    'SO2_ppm': SO2*10**4,
+                                    'SO3_wt': SO3,
+                                    'SO3_ppm': SO3*10**4,
+                                    'SO4_wt': SO4,
+                                    'SO4_ppm': SO4*10**4})
+        else:
+            df=pd.DataFrame(data={
+                                    'S_wt': S_wt2,
+                                    'S_ppm': S_ppm2,
+                                    'SO2_wt': SO2,
+                                    'SO2_ppm': SO2*10**4,
+                                    'SO3_wt': SO3,
+                                    'SO3_ppm': SO3*10**4,
+                                    'SO4_wt': SO4,
+                                    'SO4_ppm': SO4*10**4}, index=[0])
 
-        df=pd.DataFrame(data={
-                                'S_wt': S_wt2,
-                                'S_ppm': S_ppm2,
-                                'SO2_wt': SO2,
-                                'SO2_ppm': SO2*10**4,
-                                'SO3_wt': SO3,
-                                'SO3_ppm': SO3*10**4,
-                                'SO4_wt': SO4,
-                                'SO4_ppm': SO4*10**4})
 
 
 
         return df
```

### Comparing `PySulfSat-0.0.9/src/PySulfSat/mantle_melting.py` & `PySulfSat-1.0.1/src/PySulfSat/mantle_melting.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,35 +4,64 @@
 import warnings as w
 
 ## Mantle melting, adapted from Lee et al. (2012) and Wieser et al. (2020)
 
 def Lee_Wieser_sulfide_melting(*,  M_Max=0.01, Modes, KDs,
                         N=3001, F=None,
                         S_Sulf=363636, elem_Per=30,
-                        S_Mantle=[300, 200, 100, 50, 0],
-                        S_Melt_SCSS_2=980.7872088,
-                        Prop_S6=0,
-                        KdCuSulf=800,
-                        KdBaSulf=0,
-                        Trace1_per=6.85,
+                        S_Mantle=200,
+                        S_Melt_SCSS_2_ppm=980.7872088,
+                        Prop_S6=0
                         ):
+
     """ Function for calculating trajectory of S during mantle melting,
     adapted from the Excel workbook of Lee et al. (2012) and the Python code
     of Wieser et al. (2020)
 
     Parameters
     -----------
     N: int
         Number of iterative steps for melting.
+
+    Either
+
     M_Max: float
         Amount of peridotite left at final step. E.g. M_Max=0.7
         calculates 0-30% melting (F=1-M)
+
+    F: np.array
+        F you want
+
     Modes: Pandas.Dataframe
         Dataframe of ol-opx-cpx-sp modes, with column headings 'ol',
         'opx', 'cpx', 'sp'
+        (can be 1 row or multiple for each step of melting, in which case N is adjusted to be length of this dataframe)
+
+    KDs: pandas.DataFrame
+        Dataframe of KD values. Can be 1 row or multiple for each step of melting
+
+    S_Sulf: float, int
+        S content of mantle sulfides in ppm
+
+    S_Mantle: float, int
+        S content of mantle in ppm
+
+    elem_Per: float, int
+        Content of element of interest in mantle prior to melting (in ppm).
+
+    S_Melt_SCSS_2_ppm: float, int, pd.Series
+        S2- content of mantle in ppm
+
+    Prop_S6: float, int, pd.Series
+        Proportion of S6, increases S_Melt_SCSS if S6+ is present
+
+
+    Returns
+    -------------
+    pd.DataFrame: dataframe with melt extents, instantaneous and aggregate melts, and residual mantle source composition.
 
 
     """
     elx=KDs['element'][0]
 
     # Mass of peridotite
 
@@ -50,94 +79,94 @@
                 M=M=np.linspace(1, M_Max, len(Modes))
             else:
                 M=M=np.linspace(1, M_Max, len(Modes))
 
 
 
 
-    if isinstance(S_Melt_SCSS_2, float) or isinstance(S_Melt_SCSS_2, int):
-        S_Melt_SCSS_2=np.repeat(S_Melt_SCSS_2, len(M))
+    if isinstance(S_Melt_SCSS_2_ppm, float) or isinstance(S_Melt_SCSS_2_ppm, int):
+        S_Melt_SCSS_2_ppm=np.repeat(S_Melt_SCSS_2_ppm, len(M))
 
-    S_Melt = S_Melt_SCSS_2/(1+Prop_S6)
+    S_Melt = S_Melt_SCSS_2_ppm/(1+Prop_S6)
 
     # Setting up variables to be filled in loop
     #These ones have only 1 dimension for different M steps, as they do not vary with different mantle S contents
     DeltaM= np.empty(len(M), dtype=float)
     X_FStep=np.empty(len(M), dtype=float)
     X_FStart=np.empty( len(M), dtype=float)
 
+    len_S_Mantle=1
+
 # These ones have 2 dimensions, one for different M steps, one for different mantle S contents
-    S_residue= np.empty( (len(S_Mantle), len(M)), dtype=float)
-    XSulf= np.empty( (len(S_Mantle), len(M)), dtype=float)
-    elem_residue= np.empty( (len(S_Mantle), len(M)), dtype=float)
-    elem_Melt_Inst= np.empty( (len(S_Mantle), len(M)), dtype=float)
-    elem_Melt_Agg= np.empty( (len(S_Mantle), len(M)), dtype=float)
-    S_Melt_Agg= np.empty( (len(S_Mantle), len(M)), dtype=float)
-    S_Melt_Inst= np.empty( (len(S_Mantle), len(M)), dtype=float)
-    DeltaXSulf=np.empty( (len(S_Mantle), len(M)), dtype=float)
-    DeltaXSil=np.empty( (len(S_Mantle), len(M)), dtype=float)
-    P=np.empty( (len(S_Mantle), len(M)), dtype=float)
-    Kd_Cu=np.empty( (len(S_Mantle), len(M)), dtype=float)
-    DeltaXMeltTot=np.empty( (len(S_Mantle), len(M)), dtype=float)
+    S_residue= np.empty((len_S_Mantle, len(M)), dtype=float)
+    XSulf= np.empty((len_S_Mantle, len(M)), dtype=float)
+    elem_residue= np.empty((len_S_Mantle, len(M)), dtype=float)
+    elem_Melt_Inst= np.empty((len_S_Mantle, len(M)), dtype=float)
+    elem_Melt_Agg= np.empty((len_S_Mantle, len(M)), dtype=float)
+    S_Melt_Agg= np.empty((len_S_Mantle, len(M)), dtype=float)
+    S_Melt_Inst= np.empty((len_S_Mantle, len(M)), dtype=float)
+    DeltaXSulf=np.empty((len_S_Mantle, len(M)), dtype=float)
+    DeltaXSil=np.empty((len_S_Mantle, len(M)), dtype=float)
+    P=np.empty((len_S_Mantle, len(M)), dtype=float)
+    Kd_el=np.empty((len_S_Mantle, len(M)), dtype=float)
+    DeltaXMeltTot=np.empty((len_S_Mantle, len(M)), dtype=float)
 
 
-    # Loop for Cu
-    for i in range(0, len(M)-1):
+    # Loop for element
+    for i in range(0, len(M)):
 
         # If length of KDs>1, need to extract right one for each loop
         #print(KDs)
         if len(KDs)>1:
             KDs_trim=KDs.iloc[i].to_frame().T.reset_index(drop=True)
         else:
             KDs_trim=KDs
-        KdCuSulf=KDs_trim['sulf']
+        KdelSulf=KDs_trim['sulf']
 
         # If length of Modes is >1, need to extract the right one for each loop
         if len(Modes)>1:
-            KdCuSil=Modes.iloc[i].mul(KDs_trim).sum(axis=1).iloc[0]
-            KdBaSil=Modes.iloc[i].mul(KDs_trim).sum(axis=1).iloc[0]
+            KdelSil=Modes.iloc[i].mul(KDs_trim).sum(axis=1).iloc[0]
         else:
-            KdCuSil=Modes.mul(KDs_trim).sum(axis=1)
-            KdBaSil=Modes.mul(KDs_trim).sum(axis=1)
+            KdelSil=Modes.mul(KDs_trim).sum(axis=1)
 
 
 
 
 
 
 
         if i==0: # Setting up the system before any melting takes place
             S_residue[:,i]=S_Mantle # Initial S contents of mantle before any melting set at those defined in S_Mantle
             XSulf[:,i]=S_residue[:,i]/S_Sulf # Proportion (by mass) of sulfides in the source
-            elem_residue[:,i]=elem_Per # Initial Cu content of peridotite mantle
-            elem_Melt_Inst[:,i]=0 # No melting, so no Cu in the instantaneous melt
-            elem_Melt_Agg[:,i]=0 # No melting, so no Cu in the aggregated melt
+            elem_residue[:,i]=elem_Per # Initial el content of peridotite mantle
+            elem_Melt_Inst[:,i]=0 # No melting, so no el in the instantaneous melt
+            elem_Melt_Agg[:,i]=0 # No melting, so no el in the aggregated melt
             DeltaM[i]=0 # No change in the amount of peridotite residue
             DeltaXSulf[:,i]=0 # No change in the proportion of sulfide
             DeltaXSil[:,i]=0  # No change in the proportion of silicate
             P[:,i]=0          # No melting, so no preferential melting of different minerals
-            Kd_Cu[:,i]=KdCuSil* (1- XSulf[:,i]) + KdCuSulf* (XSulf[:,i]) # Bulk Kd for the mantle before any melting occurs
+            Kd_el[:,i]=KdelSil* (1- XSulf[:,i]) + KdelSulf* (XSulf[:,i]) # Bulk Kd for the mantle before any melting occurs
             X_FStep[i]=0 # No melt, so no melt proportion made in this step
             X_FStart[i]=0 # as above
             DeltaXMeltTot[:,i]=0 # as above
             S_Melt_Inst[:, i]=S_Melt[i]
         else:
             DeltaM[i]=M[i-1]-M[i]  # Equation 1
             X_FStep[i]= DeltaM[i]/M[i-1] # Equation 2
             S_residue[:,i] = (S_residue[:,i-1] -S_Melt[i]* X_FStep[i])/(1-X_FStep[i]) # Equation 3
             S_residue[S_residue<0]=0 # To avoid negative numbers.
             XSulf[:,i] = S_residue[:,i]/S_Sulf # Equation 4
 
             DeltaXSulf[:,i]=(S_residue[:,i-1]-S_residue[:,i])/S_Sulf # Equation 5
             DeltaXSil[:,i]=DeltaM[i]- DeltaXSulf[:,i] # Equation 6
 
-            Kd_Cu[:,i]=KdCuSil* (1- XSulf[:,i]) + KdCuSulf* (XSulf[:,i]) # Equation 8
-            P[:,i] = KdCuSil* ( DeltaXSil[:,i]/DeltaM[i] ) + (KdCuSulf * (DeltaXSulf[:,i]/DeltaM[i])) # Equation 9
+            Kd_el[:,i]=KdelSil* (1- XSulf[:,i]) + KdelSulf* (XSulf[:,i]) # Equation 8
+            P[:,i] = KdelSil* ( DeltaXSil[:,i]/DeltaM[i] ) + (KdelSulf * (DeltaXSulf[:,i]/DeltaM[i])) # Equation 9
 
-            elem_Melt_Inst[:,i]=elem_residue[:,i-1]/ ( Kd_Cu[:,i-1] + (1-P[:,i])*X_FStep[i] ) # Equation 7
+            elem_Melt_Inst[:,i]=elem_residue[:,i-1]/ ( Kd_el[:,i-1] + (1-P[:,i])*X_FStep[i] ) # Equation 7
             elem_residue[:,i]=( elem_residue[:,i-1] - elem_Melt_Inst[:,i] * X_FStep[i] )/( 1- X_FStep[i] ) # Equation 10
             X_FStart[i]=DeltaM[i]/(1-M[i]) #Equation 13
             elem_Melt_Agg[:,i]=(elem_Melt_Agg[:,i-1]*(1-X_FStart[i])) + (elem_Melt_Inst[:,i]* X_FStart[i]) # Equation 12
 
             # Sulfur
             if S_residue[:, i]>0:
                 S_Melt_Inst[:, i]=S_Melt[i]
@@ -148,15 +177,15 @@
 
 
 
 
 
     df_out_S0=pd.DataFrame(data={'F': 1-M,
                         'M': M,
-                    '{}_KD'.format(elx): Kd_Cu[0,:],
+                    '{}_KD'.format(elx): Kd_el[0,:],
                     '{}_Melt_Agg'.format(elx): elem_Melt_Agg[0,:],
                 '{}_Melt_Inst'.format(elx): elem_Melt_Inst[0,:],
                 '{}_Residue'.format(elx): elem_residue[0,:],
                 'S_Residue': S_residue[0,:],
                 'S_Melt_Inst': S_Melt_Inst[0,:],
                 'S_Melt_Agg': S_Melt_Agg[0,:],
                   'S_Melt_input': S_Melt,
@@ -168,14 +197,23 @@
                 #
 
     return df_out_S0
 
 
 def calculate_inst_melts_Thermocalc(Thermocalc_df):
     """ Calculates instantaneous melts from Thermocalc aggregated melt outputs
+    Parameters
+    ----------------
+    Thermocalc_df: pd.DataFrame
+        Dataframe of thermocalc outputs (aggregated melts)
+
+    Returns
+    ----------------
+    pd.DataFrame: Instantaneous liquids.
+
     """
     SiO2_EJ=Thermocalc_df['SiO2']
     #TiO2_EJ=Thermocalc_df['TiO2'] - No Ti, ask Ellie
     Al2O3_EJ=Thermocalc_df['Al2O3']
     CaO_EJ=Thermocalc_df['CaO']
     MgO_EJ=Thermocalc_df['MgO']
     FeO_EJ=Thermocalc_df['FeO']
```

### Comparing `PySulfSat-0.0.9/src/PySulfSat/s6_corrections.py` & `PySulfSat-1.0.1/src/PySulfSat/s6_corrections.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import numpy as np
 import pandas as pd
 
 import scipy
 import scipy.optimize as optimize
 from scipy.special import erf
 
-#import warnings
-#warnings.simplefilter('error')
+# import warnings
+# warnings.simplefilter('error')
 
 
 
 from PySulfSat.core_calcs import *
 
 def calculate_SCSS_Total(SCSS, S6St_Liq):
     '''
     Calculates SCSS Total from the SCSS (2-)
-    See Wieser et al. (2019) for details
+    following Jugo et al. (2009, 2010)
 
     Parameters
     -----------
     SCSS: int, float, pandas.Series
         SCSS from different calculators (only uses S2-)
 
     S6St_Liq: int, float, pandas.Series
@@ -32,69 +32,74 @@
         SCSS total, i.e inputted SCSS (2-) scaled up to account for S present in the S6+ form.
 
     '''
     SCSS_Total=SCSS/(1-S6St_Liq)
     return SCSS_Total
 
 
-def calculate_SCAS_Total(SCAS, S2St_Liq):
+def calculate_SCAS_Total(SCAS, S2St_Liq=None, S6St_Liq=None):
     '''
     Calculates SCAS Total from the SCAS (6+)
-    See Wieser et al. (2019) for details
+    following Jugo et al. (2009, 2010)
 
     Parameters
     -----------
-    SCAS: int, float, pandas.Series
+    SCAS: int, float, pandas.Series, np.array
         SCAS from different calculators (only uses S6+)
 
-    S2St_Liq: int, float, pandas.Series
+    S2St_Liq: int, float, pandas.Series, np.array
         Proportion of S2- in the liquid
 
+    or
+    S6St_Liq: proportion of S6+ in the liquid
+
     Returns
     -----------
-    float, pandas.Series
+    float, pandas.Series, np.array
         SCAStotal, i.e inputted SCAS (6+) scaled up to account for S present in the S2- form.
 
     '''
+    if S6St_Liq is not None:
+        S2St_Liq=1-S6St_Liq
     SCAS_Total=SCAS/(1-S2St_Liq)
     return SCAS_Total
 
 def calculate_S6St_Jugo2010_eq10(deltaQFM):
     '''
     Calculates The S6/St ratio from deltaQFM using
     Jugo et al. (2010) eq10
 
     Parameters
     -----------
-    deltaQFM: int, float, pandas.Series
-        Offset from the QFM buffer in log units.
+    deltaQFM: int, float, pandas.Series, np.array
+        Offset from the QFM buffer in log units. Make sure relative to frost buffer
 
     Returns
     -----------
-    float, pandas.Series
+    float, pandas.Series, np.array
         Proportion of S6+ in the liquid
 
     '''
     S6St_Liq=1/(1+10**(2.1-2*deltaQFM))
 
     return S6St_Liq
 
 def calculate_S2St_Jugo2009_eq8(deltaQFM):
     '''
     Calculates The S2/St ratio from deltaQFM using
     Jugo (2009) eq8 (re-arranged).
 
     Parameters
     -----------
-    deltaQFM: int, float, pandas.Series
+    deltaQFM: int, float, pandas.Series, np.array
         Offset from the QFM buffer in log units.
 
     Returns
     -----------
-    float, pandas.Series
+    float, pandas.Series, np.array
         Proportion of S6+ in the liquid
 
     '''
     S2St_Liq=1/(1+np.exp(2.23*deltaQFM-2.89))
 
     return S2St_Liq
 
@@ -102,43 +107,66 @@
 def calculate_S6St_Nash2019(T_K, Fe3Fet_Liq):
     '''
     Calculates The S6/St ratio from the temperature and the proportion
     of Fe3+ in the liquid using Nash et al. (2019).
 
     Parameters
     -----------
-    T_K: int, float, pandas.Series
+    T_K: int, float, pandas.Series, np.array
         Temperature in Kelvin.
 
-    Fe3Fet_Liq: int, float, pandas.Series
+    Fe3Fet_Liq: int, float, pandas.Series, np.array
         Proportion of Fe3 in the liquid
     Returns
     -----------
-    float, pandas.Series
+    float, pandas.Series,  np.array
         Proportion of S6+ in the liquid
 
     '''
     # First, calculate Fe3/Fe2 from Fe3/Fet
     Fe3Fe2=Fe3Fet_Liq/(1-Fe3Fet_Liq)
-    log_Fe3Fe2=np.log10(Fe3Fe2)
+    #print(Fe3Fe2)
+    if isinstance(Fe3Fe2, float) or isinstance(Fe3Fe2, int): 
+        log_Fe3Fe2=np.log10(Fe3Fe2)
+
+    else:
+        log_Fe3Fe2=np.log10(Fe3Fe2.astype(float))
+
 
     log_S6S2=8*log_Fe3Fe2 + 8.7436*10**6/(T_K**2) - 27703/T_K + 20.273
     S6S2=10**(log_S6S2)
 
     S6=S6S2/(1+S6S2)
 
     S2=1/(1+S6S2)
     S6St=S6/(S6+S2)
 
     return S6St
 
 
 def calculate_S_Tot_Kleinsasser2022_dacite(*, SCSS2=None,  SCAS=None, deltaQFM=None):
     """ Calculates SCSS total as a function of S2- and S6+ in dacitic melts,
-    following Kleinsasser et al. 2022"""
+    following Kleinsasser et al. 2022
+
+    Parameters
+    -----------
+    SCSS2: int, float, pd.Series, np.array
+        SCSS in ppm
+
+    SCAS: int, float, pd.Series, np.array
+        SCAS in ppm
+
+    deltaQFM: int, float, pd.Series, np.array
+
+    Returns
+    --------
+    same format as inputs
+        Proportion of S6+ in the liquid
+
+    """
 
     if SCSS2 is not None:
         SCSS_Tot=SCSS2*(1+10**(2*deltaQFM-3.05))
         return SCSS_Tot
     if SCAS is not None:
         SCAS_Tot=SCAS*(1+np.exp(1.26-2*deltaQFM))
         return SCAS_Tot
@@ -165,15 +193,15 @@
         return SCSS_Tot
 
         SCAS_Tot=SCAS*(1+np.exp(2.89-2.23*deltaFMQ))
         return SCAS_Tot
 
 
 def calculate_S_Total_SCSS_SCAS(*, SCSS, SCAS, deltaQFM=None,  model=None, S6St_Liq=None,
-                                T_K=None, Fe3Fet_Liq=None):
+                                T_K=None, Fe3Fet_Liq=None, df=None, logfo2=None):
     """
     Calculates the total amount of S accounting for the SCSS and SCAS
 
     Parameters
     -----------
     SCSS: int, float, pandas.Series
         SCSS (2-) you have calculated from whatever model you want.
@@ -182,81 +210,129 @@
         SCAS (6+) you have calculated from whatever model you want.
 
     model: str
         Model used to calculate S6St_Liq, choice of:
         'Nash': Uses Nash et al. (2019) based on Fe3Fet_Liq and T_K
         'Jugo': Uses Jugo et al. (2010) Eq 10 based on DeltaQFM
         'Kleinsasser': Uses Kleinsasser et al. 2022 based on deltaQFM
+        'OM2022': Need to also enter your dataframe of liquid compositions.
 
     deltaQFM: int, float, panda.Series (for Jugo et al. 2010, or Kleinsasser et al. 2022)
 
+    logfo2: int, float, panda.Series (works for OM2022)
+
     Fe3Fet_Liq: int, float, panda.Series
         Proportion of Fe3Fet in the liquid, needed if model='Nash'
 
     T_K: int, float, panda.Series
         Temperature in Kelvin, needed if model='Nash'
 
+    df: panda.DataFrame
+        Option, needed for OM2022
+
+
+
 
     """
+
     if model =="Kleinsasser":
         SCSS_Tot=calculate_S_Tot_Kleinsasser2022_dacite(SCSS2=SCSS,
                                                            deltaQFM=deltaQFM)
         SCAS_Tot=calculate_S_Tot_Kleinsasser2022_dacite(SCAS=SCAS,
                                                            deltaQFM=deltaQFM)
-        S6_St=np.nan
+        S6St_Liq=np.nan
+
+
+
+
     else:
+
+        if model=='OM2022':
+            if T_K is None:
+                raise TypeError('You need to specify a temp')
+            if df is None:
+                raise TypeError('You need to input a liquid dataframe')
+            if Fe3Fet_Liq is None and logfo2 is None:
+                raise TypeError('you need to input either Fe3Fet_Liq or logfo2')
+            if Fe3Fet_Liq is not None:
+                calcS_OM2022_GivenFe3=calculate_OM2022_S6St(df=df, T_K=T_K,
+                            Fe3Fet_Liq=Fe3Fet_Liq)
+            if logfo2 is not None:
+                calcS_OM2022_GivenFe3=calculate_OM2022_S6St(df=df,
+                        T_K=T_K,
+                        logfo2=logfo2)
+            S6St_Liq=calcS_OM2022_GivenFe3['S6St_Liq']
+
         if model =="Jugo":
-            S6_St=calculate_S6St_Jugo2010_eq10(deltaQFM=deltaQFM)
+            S6St_Liq=calculate_S6St_Jugo2010_eq10(deltaQFM=deltaQFM)
 
         if model =="Nash":
             if T_K is None:
                 raise Exception('Need a T_K input to use Nash')
             if Fe3Fet_Liq is None:
                 raise Exception('Need a Fe3Fet_Liq input to use Nash')
-            S6_St=calculate_S6St_Nash2019(T_K=T_K, Fe3Fet_Liq=Fe3Fet_Liq)
+            S6St_Liq=calculate_S6St_Nash2019(T_K=T_K, Fe3Fet_Liq=Fe3Fet_Liq)
 
         if S6St_Liq is not None:
-            S6_St=S6St_Liq
+            S6St_Liq=S6St_Liq
 
 
-        SCSS_Tot=calculate_SCSS_Total(SCSS=SCSS, S6St_Liq=S6_St)
-        SCAS_Tot=calculate_SCAS_Total(SCAS=SCAS, S2St_Liq=1-S6_St)
+        SCSS_Tot=calculate_SCSS_Total(SCSS=SCSS, S6St_Liq=S6St_Liq)
+        SCAS_Tot=calculate_SCAS_Total(SCAS=SCAS, S2St_Liq=1-S6St_Liq)
 
 
 
     SCSS_S6_cont=SCSS_Tot-SCSS
     SCAS_S2_cont=SCAS_Tot-SCAS
 
-    df_Species=pd.DataFrame(data={'deltaQFM': deltaQFM,
-                                  'S6_St': S6_St,
-                                  'SCSS_2': SCSS,
-                              'SCAS_6': SCAS,
-                              'SCSS_Tot': SCSS_Tot,
-                              'SCAS_Tot': SCAS_Tot,
-                                 'S6 in SCSS_Tot': SCSS_S6_cont,
-                               'S2 in SCAS_Tot': SCAS_S2_cont
-                              })
+    if isinstance(SCSS_Tot, float):
+        df_Species=pd.DataFrame(data={'deltaQFM': deltaQFM,
+                                    'S6St_Liq': S6St_Liq,
+                                    'SCSS_2_ppm': SCSS,
+                                'SCAS_6_ppm': SCAS,
+                                'SCSS_Tot': SCSS_Tot,
+                                'SCAS_Tot': SCAS_Tot,
+                                    'S6 in SCSS_Tot': SCSS_S6_cont,
+                                'S2 in SCAS_Tot': SCAS_S2_cont
+                                }, index=[0])
+    else:
+
+        df_Species=pd.DataFrame(data={'deltaQFM': deltaQFM,
+                                    'S6St_Liq': S6St_Liq,
+                                    'SCSS_2_ppm': SCSS,
+                                'SCAS_6_ppm': SCAS,
+                                'SCSS_Tot': SCSS_Tot,
+                                'SCAS_Tot': SCAS_Tot,
+                                    'S6 in SCSS_Tot': SCSS_S6_cont,
+                                'S2 in SCAS_Tot': SCAS_S2_cont
+                                })
 
     # Cant have more S6 than the SCAS
-    toomuchS6=df_Species['S6 in SCSS_Tot']>df_Species['SCAS_6']
+
+
+    toomuchS6=df_Species['S6 in SCSS_Tot']>df_Species['SCAS_6_ppm']
     df_Species['SCSS_Tot_check']=df_Species['SCSS_Tot']
-    df_Species.loc[toomuchS6, 'SCSS_Tot_check']=df_Species['SCAS_6']+df_Species['SCSS_2']
+    df_Species.loc[toomuchS6, 'SCSS_Tot_check']=df_Species['SCAS_6_ppm']+df_Species['SCSS_2_ppm']
 
     # Cant have more S2- than the SCSS
-    toomuchS2=df_Species['S2 in SCAS_Tot']>df_Species['SCSS_2']
+    toomuchS2=df_Species['S2 in SCAS_Tot']>df_Species['SCSS_2_ppm']
     df_Species['SCAS_Tot_check']=df_Species['SCAS_Tot']
-    df_Species.loc[toomuchS2, 'SCAS_Tot_check']=df_Species['SCAS_6']+df_Species['SCSS_2']
+    # Ignore this error for now, seems a panda issue. wasted a lot of time on it.
+
+    df_Species['SCAS_6_ppm'] = pd.to_numeric(df_Species['SCAS_6_ppm'], errors='coerce')
+    df_Species['SCSS_2_ppm'] = pd.to_numeric(df_Species['SCSS_2_ppm'], errors='coerce')
+    df_Species.loc[toomuchS2, 'SCAS_Tot_check']=df_Species['SCAS_6_ppm']+df_Species['SCSS_2_ppm']
 
     #Set as the minimum one
-    df_Species.insert(0, 'Total_S',df_Species['SCAS_Tot_check'])
+    df_Species.insert(0, 'Total_S_ppm',df_Species['SCAS_Tot_check'])
     SCAS_higher=df_Species['SCAS_Tot_check']>df_Species['SCSS_Tot_check']
-    df_Species.loc[SCAS_higher, 'Total_S']=df_Species['SCSS_Tot_check']
+    df_Species.loc[SCAS_higher, 'Total_S_ppm']=df_Species['SCSS_Tot_check']
 
-    df_Species.insert(1, 'S2_Tot', df_Species['Total_S']*(1-df_Species['S6_St']))
-    df_Species.insert(2, 'S6_Tot', df_Species['Total_S']*(df_Species['S6_St']))
+    df_Species.insert(1, 'S2_Tot_ppm', df_Species['Total_S_ppm']*(1-df_Species['S6St_Liq']))
+    df_Species.insert(2, 'S6_Tot_ppm', df_Species['Total_S_ppm']*(df_Species['S6St_Liq']))
 
     df_Species2=df_Species.copy()
     df_Species2.drop(['SCAS_Tot_check', 'SCSS_Tot_check', 'SCSS_Tot_check'], axis=1, inplace=True)
     return df_Species2
 
 
 def calculate_BW2022_CS6(*, df, T_K):
@@ -268,14 +344,18 @@
     df: pandas Dataframe
         input dataframe of liquid compositions with _Liq after each oxide
 
 
     T_K: int, float, pd.series
         Temperature in Kelvin
 
+    Returns
+    --------------
+    pd.DataFrame:
+        includes columns for CS6 in BW22 and O22 format, and cat fractions
 
 
     """
 
     liqs=df.copy()
     liqs=calculate_anhydrous_cat_fractions_liquid(liq_comps=liqs)
 
@@ -301,14 +381,25 @@
     df: pandas Dataframe
         input dataframe of liquid compositions with _Liq after each oxide
 
 
     T_K: int, float, pd.series
         Temperature in Kelvin
 
+    Fe3Fet_Liq: float, pd.series
+        Fe3/Fet ratio in the liquid
+
+    logfo2: float, pd.series
+        logfo2 value
+
+
+    Returns
+    -----------
+    pd.DataFrame
+        input dataframe, with Cs6 calculated both Oneill and Bouilling way.
 
 
     """
     liqs=df.copy()
 
 
 
@@ -398,16 +489,16 @@
 
     if C5==1: # specify Fe3Fet not logfo2
         deltaQFM=(4*(np.log10(Fe3Fet_Liq/(1-Fe3Fet_Liq))+1.36-2*liqs['Na_Liq_cat_frac']
                     -3.7*liqs['K_Liq_cat_frac']-2.4*liqs['Ca_Liq_cat_frac']))
         logfo2_calc=deltaQFM-25050/T_K+8.58
         liqs['deltaQFM_calc']=deltaQFM
         liqs['logfo2_calc']=logfo2_calc
-    if C5==2: #If specify Fe3Fet
-        deltaQFM=logfo2-25050/T_K+8.58
+    if C5==2: #If specify logfo2
+        deltaQFM=logfo2-8.58+25050/T_K
         liqs['deltaQFM_calc']=deltaQFM
 
     if C5==2: # e.g. if Fe3Fet not given
         Fe2Fet_Liq=1/(1+10**(0.25*deltaQFM-1.36+2*liqs['Na_Liq_cat_frac']+2.4*liqs['Ca_Liq_cat_frac']+3.7*liqs['K_Liq_cat_frac']))
         liqs['Fe2Fet_Liq_calc']=Fe2Fet_Liq
     if C5==1: # IF Fe3Fet is given
         Fe2Fet_Liq=1-Fe3Fet_Liq
@@ -513,7 +604,80 @@
 
     cols_to_move = ['S6St_Liq', 'LnCS2_calc', 'LnCS6_calc', 'LnKSO2S2', 'LnS6S2',
                     'deltaQFM_calc']
     liqs = liqs[cols_to_move +
                                     [col for col in liqs.columns if col not in cols_to_move]]
     return liqs
 
+
+def calculate_fo2_QFM_buffers(logfo2=-8.52, T_K=1200, P_kbar=1):
+    """ Calculates fo2 values for Frost, Oneill, MELTS and Petrolog3/Myers 'QFM' buffer positions, and
+    the offset from each QFM bufer
+
+    Parameters
+    ----------------
+    logfo2: float, int, pd.Series, np.array
+        logfo2 value
+
+    T_K: float, int, pd.Series, np.array
+        Temperature in Kelvin
+
+    P_kbar: float, int, pd.Series, np.array
+        Presure in kbar
+
+    Returns
+    -------------------
+    pd.DataFrame
+        logfo2 positions for each buffer, and the delta QFM values for each reference point.
+    """
+    logfo2_QFM_Oneill=8.58-25050/T_K
+    # Frost depends on temperature
+
+    logfo2_QFM_highT=(-25096.3/T_K) + 8.735 + 0.11 * ((P_kbar*1000)-1)/T_K
+    T_Choice='HighT Beta Qtz'
+
+    logfo2_QFM_lowT=(-26455.3/T_K) +10.344 + 0.092 * ((P_kbar*1000)-1)/T_K
+    T_Choice='Low T alpha Qtz'
+
+    Cut_off_T=573+273.15+0.025*(P_kbar*1000)
+    if T_K<Cut_off_T:
+        logfo2_QFM_Frost= logfo2_QFM_lowT
+    if T_K>=Cut_off_T:
+        logfo2_QFM_Frost=logfo2_QFM_highT
+
+
+    logfo2_QFM_Petrolog=-24442/T_K+8.29 #This is actually Myers 1983
+    logfo2_QFM_MeltsExcel=-24442/T_K + 8.29 + 0.111*(P_kbar*1000-1)/T_K
+
+    DeltaQFM_Oneill=logfo2-logfo2_QFM_Oneill
+    DeltaQFM_Frost=logfo2-logfo2_QFM_Frost
+    DeltaQFM_Petrolog=logfo2-logfo2_QFM_Petrolog
+    DeltaQFM_MeltsExcel=logfo2-logfo2_QFM_MeltsExcel
+
+
+
+    if isinstance(DeltaQFM_Oneill, float):
+
+        df=pd.DataFrame(data={'logfo2_QFM_ONeill': logfo2_QFM_Oneill,
+    'logfo2_QFM_Frost': logfo2_QFM_Frost,
+    'logfo2_QFM_Petrolog3': logfo2_QFM_Petrolog,
+'DeltaQFM_ONeill': DeltaQFM_Oneill,
+    'DeltaQFM_Frost': DeltaQFM_Frost,
+    'DeltaQFM_Petrolog3': DeltaQFM_Petrolog,
+    'DeltaQFM_MeltsExcel': DeltaQFM_MeltsExcel,
+    },
+    index=[0])
+    else:
+        df=pd.DataFrame(data={'logfo2_QFM_ONeill': logfo2_QFM_Oneill,
+    'logfo2_QFM_Frost': logfo2_QFM_Frost,
+    'logfo2_QFM_Petrolog3': logfo2_QFM_Petrolog,
+'DeltaQFM_ONeill': DeltaQFM_Oneill,
+    'DeltaQFM_Frost': DeltaQFM_Frost,
+    'DeltaQFM_Petrolog3': DeltaQFM_Petrolog,
+    'DeltaQFM_MeltsExcel': DeltaQFM_MeltsExcel,
+    })
+
+    return df
+
+
+
+
```

### Comparing `PySulfSat-0.0.9/src/PySulfSat/scas_calc.py` & `PySulfSat-1.0.1/src/PySulfSat/scas_calc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,74 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scipy
 import scipy.optimize as optimize
 from scipy.special import erf
+import warnings as w
 
 
 
 from PySulfSat.core_calcs import *
 #SCAS (Li and Ripley, 2009;
 #Baker and Moretti, 2011; Masotta and Keppler, 2015;
 #Chowdhury and Dasgupta, 2019; Zajacz and Tsay, 2019)
 df_ideal_liq_Chow = pd.DataFrame(columns=['SiO2_Liq', 'TiO2_Liq', 'Al2O3_Liq',
 'FeOt_Liq', 'MnO_Liq', 'MgO_Liq', 'CaO_Liq', 'Na2O_Liq', 'K2O_Liq', 'H2O_Liq'])
 
 def norm_liqs_with_H2O(Liqs):
+    """ Normalizes liquids so hydrous sum is 100 (enter df of Liqs, returns normalized df)
+
+    """
     Liqs_c=Liqs.copy()
     Liqs_c=Liqs_c.fillna(0)
     Liqs2=Liqs_c.reindex(
         df_ideal_liq_Chow.columns, axis=1).fillna(0)
 
     sum_rows=Liqs2.sum(axis=1)
 
     Liqs_norm=Liqs2.divide(sum_rows/100, axis='rows')
     return Liqs_norm
 
 
-def calculate_CD2019_SCAS(*, df, T_K, H2O_Liq=None):
+def calculate_CD2019_SCAS(*, df, T_K, H2O_Liq=None, Fe3Fet_Liq=None, P_kbar=None):
     """" Calculates SCAS using the model of Chowdhury and Dasgupta, 2019
 
 
     Parameters
     -------
     df: pandas.DataFrame
         Dataframe of liquid compositions. Needs to have the headings "SiO2_Liq", "TiO2_Liq" etc, with
         compositions in oxide wt%. all FeO should be entered as FeOt_Liq
 
     T_K: int, float, pandas.Series
         Temperature in Kelvin.
 
+    Optional:
+
     H2O_Liq: int, float, pandas.Series
         Option input, overwrites H2O_Liq in input dataframe
 
-
+    Fe3Fet_Liq, P_kbar not required, here for consistency with other functions
 
 
     Returns
     -------
     df of input dataframe, with new column heading "Calc SCAS (ppm)"
 
     """
+    if P_kbar is not None:
+        w.warn('you entered a P_kbar, just be aware this function isnt actually pressure sensitive')
+    if Fe3Fet_Liq is not None:
+        w.warn('you entered a Fe3Fet_Liq, just be aware this function isnt actually redox sensitive')
 
 
     df_c=df.copy()
+    if H2O_Liq is not None:
+        df_c['H2O_Liq']=H2O_Liq
     df_norm=norm_liqs_with_H2O(Liqs=df_c)
     hyd_prop=calculate_hydrous_mol_proportions_liquid(liq_comps=df_norm)
     sum_hyd_prop=hyd_prop.sum(axis=1)
     hyd_frac=calculate_hydrous_mol_fractions_liquid(liq_comps=df_norm)
     sum_hydr_frac=hyd_frac.sum(axis=1)
 
     # Coefficients
@@ -81,44 +93,50 @@
     molesS=Xs*(sum_hyd_prop+Xs)
     SCAS=molesS*32.065
     SCASppm=SCAS*10000
     # print(SCASppm)
     # print(len(SCASppm))
     out=pd.concat([df_c, hyd_prop, hyd_frac], axis=1)
 
-    out.insert(0, 'Calc SCAS (ppm)', SCASppm)
+    out.insert(0, 'SCAS6_ppm', SCASppm)
     out.insert(1, 'lnXS', lnXS)
     out.insert(2, 'Xs', Xs)
     out.insert(3, 'molesS', molesS)
     return out
 
-def calculate_ZT2022_SCAS(*, df, T_K, H2O_Liq=None):
+def calculate_ZT2022_SCAS(*, df, T_K, H2O_Liq=None, Fe3Fet_Liq=None, P_kbar=None):
     """" Calculates SCAS using the model of Zajacz and Tsay, 2022
 
     Parameters
     -------
     df: pandas.DataFrame
         Dataframe of liquid compositions. Needs to have the headings "SiO2_Liq", "TiO2_Liq" etc, with
         compositions in oxide wt%. all FeO should be entered as FeOt_Liq
 
     T_K: int, float, pandas.Series
         Temperature in Kelvin.
 
+    Optional
+
     H2O_Liq: int, float, pandas.Series
         Option input, overwrites H2O_Liq in input dataframe
 
 
-
+    Fe3Fet_Liq, P_kbar not required, here for consistency with other functions
 
     Returns
     -------
     df of input dataframe, with new column heading "Calc SCAS (ppm)"
 
     """
 
+    if P_kbar is not None:
+        w.warn('you entered a P_kbar, just be aware this function isnt actually pressure sensitive')
+    if Fe3Fet_Liq is not None:
+        w.warn('you entered a Fe3Fet_Liq, just be aware this function isnt actually redox sensitive')
 
     df_c=df.copy()
     df_c['MnO_Liq']=0
     if H2O_Liq is not None:
         df_c['H2O_Liq']=H2O_Liq
 
     hyd_prop=calculate_hydrous_mol_proportions_liquid(liq_comps=df_c)
@@ -147,70 +165,86 @@
     P_H2O=hyd_frac['H2O_Liq_mol_frac']*(2.09-1.65*NBOT)+0.42*NBOT+0.23
 
     # Ksp
     Ksp=np.exp(1.226*np.log(P_c*P_T*P_H2O)+0.079)
     XSmelt=Ksp/hyd_frac['CaO_Liq_mol_frac']
     Smelt=XSmelt*sum_hyd_prop*32.07*10000
 
-    df_c.insert(0, 'Calc SCAS (ppm)', Smelt)
+    df_c.insert(0, 'SCAS6_ppm', Smelt)
 
     return df_c
 
 
 ## Masotta et al. (2013) calculations
-def calculate_MK2015_SCAS(liq_comps, T_K):
+def calculate_MK2015_SCAS(df, T_K, H2O_Liq=None, Fe3Fet_Liq=None, P_kbar=None):
     """ Calculates S6+ dissolved in the melt using Masotta and Kepler (2015)
     doi: https://doi.org/10.1016/j.gca.2015.02.033
 
     Parameters
     -------
 
-    liq_comps: pandas.DataFrame
+    df: pandas.DataFrame
                 Panda DataFrame of liquid compositions with column headings SiO2_Liq, TiO2_Liq etc.
 
     T_K: int, float, pandas.Series
         Temperature in Kelvin
 
 
+    Optional
+
+    H2O_Liq: int, float, pandas.Series
+        Option input, overwrites H2O_Liq in input dataframe
+
+
+    Fe3Fet_Liq, P_kbar not required, here for consistency with other functions
+
+
     Returns
     -------
     pandas dataframe with calculated S in wt% and ppm, other intermediate
     calculations, and input dataframe
     """
 
-    df=liq_comps.copy()
-    mol_prop=calculate_anhydrous_mol_proportions_liquid(liq_comps=df)
-    mol_frac=calculate_anhydrous_mol_fractions_liquid(liq_comps=df)
-    cat_frac=calculate_anhydrous_cat_fractions_liquid(liq_comps=df)
+    if P_kbar is not None:
+        w.warn('you entered a P_kbar, just be aware this function isnt actually pressure sensitive')
+    if Fe3Fet_Liq is not None:
+        w.warn('you entered a Fe3Fet_Liq, just be aware this function isnt actually redox sensitive')
+
+
+    df_c=df.copy()
+    if H2O_Liq is not None:
+        df['H2O_Liq']=H2O_Liq
+    mol_prop=calculate_anhydrous_mol_proportions_liquid(liq_comps=df_c)
+    mol_frac=calculate_anhydrous_mol_fractions_liquid(liq_comps=df_c)
+    cat_frac=calculate_anhydrous_cat_fractions_liquid(liq_comps=df_c)
 
     mol_prop_sum = mol_prop.sum(axis='columns')
 
     NBOT=((2*(2*cat_frac['Si_Liq_cat_frac']
     +2*cat_frac['Ti_Liq_cat_frac']+1.5*cat_frac['Al_Liq_cat_frac']
         +cat_frac['Fet_Liq_cat_frac']+cat_frac['Mg_Liq_cat_frac']
     +cat_frac['Ca_Liq_cat_frac']+0.5*cat_frac['Na_Liq_cat_frac']
     +0.5*cat_frac['K_Liq_cat_frac'])-4*(cat_frac['Si_Liq_cat_frac']
     +cat_frac['Ti_Liq_cat_frac']+cat_frac['Al_Liq_cat_frac']))
     /(cat_frac['Si_Liq_cat_frac']+cat_frac['Ti_Liq_cat_frac']
     +cat_frac['Al_Liq_cat_frac']))
 
     LnKps=(8.95+-146.5*NBOT+(-26960/(T_K))+197200*NBOT*(1/(T_K))
-           +0.409*liq_comps['H2O_Liq'])
+           +0.409*df_c['H2O_Liq'])
 
     # Wont match exactly as they include SO3 in their sum, which we dont know
-    CaO_MF=((liq_comps['CaO_Liq']/56.0774)/(mol_prop_sum-mol_prop['CaO_Liq_mol_prop']
-            +liq_comps['CaO_Liq']/56.0774))
+    CaO_MF=((df_c['CaO_Liq']/56.0774)/(mol_prop_sum-mol_prop['CaO_Liq_mol_prop']
+            +df_c['CaO_Liq']/56.0774))
     SO3_MF=np.exp(LnKps)/CaO_MF
     C_SO3_melt=SO3_MF*(mol_prop_sum-mol_prop['CaO_Liq_mol_prop']
-                +liq_comps['CaO_Liq']/56.0774)*80.066
+                +df_c['CaO_Liq']/56.0774)*80.066
     S_melt_wt=C_SO3_melt*0.40048
     S_melt_ppm=S_melt_wt*10000
 
-    new=pd.DataFrame(data={'S_melt_ppm': S_melt_ppm,
-                              'S_melt_wt': S_melt_wt,
+    new=pd.DataFrame(data={'SCAS6_ppm': S_melt_ppm,
                               'C_SO3_melt': C_SO3_melt,
                               'SO3_MF': SO3_MF,
                               'CaO_MF': CaO_MF,
                               'LnKps': LnKps,
                               'NBOT': NBOT})
     df_out=pd.concat([new, df], axis=1)
     return df_out
```

### Comparing `PySulfSat-0.0.9/src/PySulfSat/scss_calcs2.py` & `PySulfSat-1.0.1/src/PySulfSat/scss_calcs2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 ## Li and Zhang 2022
 df_ideal_liq_lizhang = pd.DataFrame(columns=['SiO2_Liq', 'TiO2_Liq', 'Al2O3_Liq',
 'FeOt_Liq', 'MnO_Liq', 'MgO_Liq', 'CaO_Liq', 'Na2O_Liq', 'K2O_Liq',
 'P2O5_Liq'])
 
 def norm_liqs_excl_H2O(Liqs):
+    """ Normalizes without H2O (anhydrous total = 100)
+    """
     Liqs_c=Liqs.copy()
     Liqs_c=Liqs_c.fillna(0)
     Liqs2=Liqs_c.reindex(
         df_ideal_liq_lizhang.columns, axis=1).fillna(0)
 
     sum_rows=Liqs2.sum(axis=1)
 
@@ -46,28 +48,41 @@
 
     T_K: int, float, pandas.Series
         Temperature in Kelvin.
 
     P_kbar: int, float, pandas.Series
         Pressure in kbar
 
-    logfo2: int, float, or pandas.Series
-        logfo2, used to convert to Fe3 following the method of Li and Zhang (2022)
+
 
     T_K_transition : bool
         The model shows a flip at 1200C. If T_K_transition is False, this doesnt happen. This generates more coherent results.
+        You then also need to specify whether you want to use the highT or lowT optoin (highT=True)
+
+
+    Optional
+
+    H2O_Liq: int, float, pandas.Series
+        Option input, overwrites H2O_Liq in input dataframe
+
+
+    logfo2: int, float, or pandas.Series
+        logfo2, used to convert to Fe3 following the method of Li and Zhang (2022)
+
 
     Fe3Fet_Liq: int, float, pandas.Series, or "Calc_ONeill"
         Proportion of Fe3+ in the liquid, as various parts of the calculation use only Fe2.
         If "Calc_ONeill" Calculates as a function of MgO content, using the MORB relationship.
 
-    Sulfide Composition: Options to calculate from the liquid composition, enter the comp in el wt%,
+
+
+    Various options for Sulfide Composition: calculate from the liquid composition, enter the comp in el wt%,
     or enter the Fe_FeNiCu_Sulf, Cu
 
-      if you want to calculate sulfide composition:
+        Calculate sulfide composition:
 
             Fe_FeNiCu_Sulf = "Calc_Smythe", also needs Ni_Sulf_init, and Cu_Sulf_init
             Calculates sulfide composition analagous to the Solver function in the Smythe et al. (2017) spreadsheet.
             Here, we use Scipy optimize to find the ideal Ni and Cu
             contents using Kds from Kiseeva et al. (2015) and the Ni and Cu content of the melt.
             Requires user to also enter Ni_Liq and Cu_Liq.
 
@@ -338,15 +353,15 @@
     df_out.insert(0, 'SCSS_Tot', Stot_calc_H2O)
     return df_out
 
 ## Blanchard et al. 2021 - SCSS calculations
 
 def calculate_B2021_SCSS(*, df, T_K, P_kbar, Fe_FeNiCu_Sulf=None,  Cu_FeNiCu_Sulf=None, Ni_FeNiCu_Sulf=None, H2O_Liq=None,
 Fe_Sulf=None, Ni_Sulf=None, Cu_Sulf=None,
-Ni_Liq=None, Cu_Liq=None):
+Ni_Liq=None, Cu_Liq=None, Fe3Fet_Liq=None):
     '''
     Calculates SCSS using the model of Blanchard et al. 2021
     doi: https://doi.org/10.2138/am-2021-7649
     designed for calculating sulfide saturation in peridotitic melt at upper         mantle conditions
 
 
     Parameters
@@ -361,15 +376,15 @@
         Temperature in Kelvin.
 
     P_kbar: int, float, pandas.Series
         Pressure in kbar
 
 
     H2O_Liq: int, float, pandas series (optional)
-        Overwrites H2O in the user entered dataframe
+        Overwrites H2O in the user entered dataframes
 
     Sulfide Composition: Options to calculate from the liquid composition, enter the comp in el wt%,
     or enter the FeFeNiCu, Cu
 
       if you want to calculate sulfide composition:
 
             Fe_FeNiCu_Sulf = "Calc_Smythe", also needs Ni_Sulf_init, and Cu_Sulf_init
@@ -432,15 +447,18 @@
     A_Mg_m2=-18258
     A_Fe_m2=-41706
     A_Ca_m2=-14668
     A_Na_m2=-19529
     A_K_m2=-34641
     A_H_m2=-22677
     A_SiFe_m2=120662
+
     Liqs=df.copy()
+    if H2O_Liq is not None:
+        Liqs['H2O_Liq']=H2O_Liq
 
     Liqs=calculate_sulfide_comp_generic(
     Fe_Sulf=Fe_Sulf, Ni_Sulf=Ni_Sulf, Cu_Sulf=Cu_Sulf, Fe_FeNiCu_Sulf=Fe_FeNiCu_Sulf,
     Cu_FeNiCu_Sulf=Cu_FeNiCu_Sulf, Ni_FeNiCu_Sulf=Ni_FeNiCu_Sulf,
     Ni_Liq=Ni_Liq, Cu_Liq=Cu_Liq, df_c=Liqs, T_K=T_K)
 
 
@@ -475,22 +493,22 @@
     SCSS_eq11=np.exp(lnSCSS_equation11)
     lnSCSS_equation12=(a_m2+B_m2/T_K + (C_m2 * P_GPa)/T_K +
                     catsum_term_m2/T_K +np.log(Liqs['Fe_FeNiCu_Sulf_calc'])
                     -np.log(calcs['Fet_Liq_cat_frac'])
                     )
     SCSS_eq12=np.exp(lnSCSS_equation12)
 
-    Liqs.insert(0, 'SCSS_eq11', SCSS_eq11)
-    Liqs.insert(1, 'SCSS_eq12', SCSS_eq12)
+    Liqs.insert(0, 'SCSS2_ppm_eq11', SCSS_eq11)
+    Liqs.insert(1, 'SCSS2_ppm_eq12', SCSS_eq12)
 
     return Liqs
 
 ## Fortin et al. (2015) SCSS Calculation
 
-def calculate_F2015_SCSS(df, T_K, P_kbar, H2O_Liq=None):
+def calculate_F2015_SCSS(df, T_K, P_kbar, H2O_Liq=None, Fe3Fet_Liq=None,Fe_FeNiCu_Sulf=None ):
     '''
     Calculates SCSS using the model of Fortin et al. (2015).
     doi: http://dx.doi.org/10.1016/j.gca.2015.03.0220
     Unlike the models of Symthe et al. (2017) or O'Neill (2021) this model doesn't
     require the sulfide composition, or the proportion of Fe3 in the liqiud.
 
     Parameters
@@ -503,20 +521,31 @@
 
     T_K: int, float, pandas.Series
         Temperature in Kelvin.
 
     P_kbar: int, float, pandas.Series
         Pressure in kbar
 
+    Optional
+
+    H2O_Liq: int, float, pandas.Series
+        Option input, overwrites H2O_Liq in input dataframe
+
+    Fe3Fet_Liq, Fe_FeNiCu_Sulf - Doesnt use these values. here for consistency with other functions
+
     Returns
     -----------
     pandas.DataFrame
         Calculated SCSS, mol fractions, and input compositions.
 
     '''
+    if Fe3Fet_Liq is not None:
+        w.warn('F2015 doesnt use your inputted Fe3Fet_Liq value')
+    if Fe_FeNiCu_Sulf is not None:
+        w.warn('F2015 doesnt use your inputted sulfide comp')
 
     df_c=df.copy()
     if H2O_Liq is not None:
         df_c['H2O_Liq']=H2O_Liq
     mol_fracs=calculate_hydrous_mol_fractions_liquid(df_c)
     Ln_SCSS_Calc=(34.7837+(1/T_K*-5772.322)+
 ((P_kbar/10)/T_K*-346.5377)+
@@ -529,15 +558,15 @@
 (mol_fracs['CaO_Liq_mol_frac']*-20.3778)+
 (mol_fracs['Na2O_Liq_mol_frac']*-18.9539)+
 (mol_fracs['K2O_Liq_mol_frac']*-32.1944)+
 (mol_fracs['P2O5_Liq_mol_frac']*0)+
 (mol_fracs['H2O_Liq_mol_frac']*-20.3934))
     SCSS_Calc=np.exp(Ln_SCSS_Calc)
     out=pd.concat([mol_fracs, df_c], axis=1)
-    out.insert(0, 'SCSS_ppm_Fortin2015', SCSS_Calc)
+    out.insert(0, 'SCSS2_ppm', SCSS_Calc)
     return out
 ## Liu et al. 2021 SCSS calculations
 def calculate_Liu2021_SCSS(df, T_K, P_kbar, Fe_FeNiCu_Sulf=None, H2O_Liq=None, Cu_FeNiCu_Sulf=None, Ni_FeNiCu_Sulf=None,
 Ni_Liq=None, Cu_Liq=None, Fe_Sulf=None, Cu_Sulf=None, Ni_Sulf=None, Ni_Sulf_init=5, Cu_Sulf_init=5, Fe3Fet_Liq=None):
     '''
     Calculates the SCSS using the model of Liu et al. (2021), doesnt depend on silicate melt composition apart from H2O_Liq.
     Doi - https://doi.org/10.1016/j.chemgeo.2020.119913
@@ -551,14 +580,19 @@
 
     T_K: int, float, pandas.Series
         Temperature in Kelvin.
 
     P_kbar: int, float, pandas.Series
         Pressure in kbar
 
+    Optional
+
+    H2O_Liq: int, float, pandas.Series
+        Option input, overwrites H2O_Liq in input dataframe
+
     Fe3Fet_Liq: int, float, pandas.Series, or "Calc_ONeill"
         Proportion of Fe3+ in the liquid, as various parts of the calculation use only Fe2.
         If "Calc_ONeill" Calculates as a function of MgO content, using the MORB relationship.
 
     Sulfide Composition: Options to calculate from the liquid composition, enter the comp in el wt%,
     or enter the FeFeNiCu, Cu
 
@@ -586,24 +620,33 @@
 
         if you want to input a measured sulfide composition in el wt%
             Fe_Sulf, Ni_Sulf, Cu_Sulf = int, float, pandas series
 
 
 
     '''
-    df_c=df.copy()
 
+
+    df_c=df.copy()
+    if H2O_Liq is not None:
+        df_c['H2O_Liq']=H2O_Liq
     Fe_FeNiCu_Sulf_calc=calculate_sulfide_comp_generic(
     Fe_Sulf=Fe_Sulf, Ni_Sulf=Ni_Sulf, Cu_Sulf=Cu_Sulf, Fe_FeNiCu_Sulf=Fe_FeNiCu_Sulf,
     Cu_FeNiCu_Sulf=Cu_FeNiCu_Sulf, Ni_FeNiCu_Sulf=Ni_FeNiCu_Sulf,
-    Ni_Liq=Ni_Liq, Cu_Liq=Cu_Liq, df_c=df_c)
+    Ni_Liq=Ni_Liq, Cu_Liq=Cu_Liq, df_c=df_c, T_K=T_K)
+
+    if isinstance(T_K, pd.Series):
+        T_K=T_K.astype(float)
+    if isinstance(P_kbar, pd.Series):
+        P_kbar=P_kbar.astype(float)
 
-    scss=Fe_FeNiCu_Sulf_calc*np.exp(13.88-9744/T_K-328*(P_kbar/10)/T_K)+104*H2O_Liq
 
-    df_c.insert(0, 'SCSS_calc', scss)
+    scss=Fe_FeNiCu_Sulf_calc['Fe_FeNiCu_Sulf_calc'].astype(float)*np.exp(13.88-9744/T_K-328*(P_kbar/10)/T_K)+104*df_c['H2O_Liq']
+
+    df_c.insert(0, 'SCSS2_ppm', scss)
     return df_c
 
 ## ONeill 2021 SCSS calculations
 
 def calculate_ONeill_sulf(FeOt_Liq, Ni_Liq, Cu_Liq, MgO_Liq=None, Fe3Fet_Liq=None):
     '''
     Calculating the Fe_FeNiCu ratio in the sulfide using the empirical
@@ -1007,15 +1050,15 @@
 
     P_kbar: int, float, pandas.Series
         Pressure in kbar
 
     Returns
     -----------
     pandas.DataFrame
-        Calculated Cu, Ni, O, S and Fe content of sulfide.
+        Calculated Cu, Ni, O, S and Fe content of sulfide, along with Ds from Kiseeva and Brenan
 
     '''
     if Fe3Fet_Liq is not None:
         FeO_Liq=FeOt_Liq*(1-Fe3Fet_Liq)
     else:
         FeO_Liq=FeOt_Liq
     OCalc_CellAG12=0.24*FeO_Liq
@@ -1417,15 +1460,15 @@
     Cu_moles=Cu_Sulf/63.546
     Fe_moles=Fe_Sulf/55.8457
     NiFeNiCu=Ni_moles/(Fe_moles+Cu_moles+Ni_moles)
     return NiFeNiCu
 ## Smythe Parameterization
 
 def calculate_S2017_SCSS(*, df, T_K, P_kbar, Fe3Fet_Liq=None, Fe_FeNiCu_Sulf=None, Cu_FeNiCu_Sulf=None, Ni_FeNiCu_Sulf=None,
-Fe_Sulf=None, Ni_Sulf=None, Cu_Sulf=None, Ni_Liq=None, Cu_Liq=None,
+Fe_Sulf=None, Ni_Sulf=None, Cu_Sulf=None, Ni_Liq=None, Cu_Liq=None, H2O_Liq=None,
 Ni_Sulf_init=5, Cu_Sulf_init=5):
     '''
     Calculates SCSS using the model of Smythe et al. (2017).
     doi: https://doi.org/10.2138/am-2017-5800CCBY
 
     Has with options for users to calculate sulfide composition from liquid composition, or input sulfide  composition.
 
@@ -1442,14 +1485,17 @@
     P_kbar: int, float, pandas.Series
         Pressure in kbar
 
     Fe3Fet_Liq: int, float, pandas.Series
         Proportion of Fe3+ in the liquid.
         Various parts of the calculation use only Fe2.
 
+    H2O_Liq: int, float, panda.Series
+        Overwrites H2O_Liq in the input dataframe.
+
     Sulfide Composition: Options to calculate from the liquid composition, enter the comp in el wt%,
     or enter the FeFeNiCu, Cu
 
       if you want to calculate sulfide composition:
 
             Fe_FeNiCu_Sulf = "Calc_Smythe", also needs Ni_Sulf_init, and Cu_Sulf_init
             Calculates sulfide composition analagous to the Solver function in the Smythe et al. (2017) spreadsheet.
@@ -1484,23 +1530,27 @@
     pandas.DataFrame:
         Contains column for SCSS ideal, 1 sigma, input T and P, and the various intermediate steps of the calculation.
 
     '''
     df_c=df.copy()
     if Fe3Fet_Liq is not None:
         df_c['Fe3Fet_Liq']=Fe3Fet_Liq
+    if H2O_Liq is not None:
+        df_c['H2O_Liq']=H2O_Liq
     # First, calculate silicate hydrous mole fractions, as true regardless of choice of sulfide composition
     Smythe_calcs=calculate_Smythe_silicate_mole_fractions(df_c, Fe3Fet_Liq)
 
 
     df_c=calculate_sulfide_comp_generic(
     Fe_Sulf=Fe_Sulf, Ni_Sulf=Ni_Sulf, Cu_Sulf=Cu_Sulf, Fe_FeNiCu_Sulf=Fe_FeNiCu_Sulf,
     Cu_FeNiCu_Sulf=Cu_FeNiCu_Sulf, Ni_FeNiCu_Sulf=Ni_FeNiCu_Sulf,
     Ni_Liq=Ni_Liq, Cu_Liq=Cu_Liq, df_c=df_c, T_K=T_K)
 
+    
+
 
     # Calculating the different liquid components
     Smythe_calcs['Si_XA_ideal']=Smythe_calcs['Si_wt_atom']*(-27561.044)
     Smythe_calcs['Ti_XA_ideal']=Smythe_calcs['Ti_wt_atom']*(-11220.488)
     Smythe_calcs['Al_XA_ideal']=Smythe_calcs['Al_wt_atom']*(-18450.292)
     Smythe_calcs['Mg_XA_ideal']=Smythe_calcs['Mg_wt_atom']*(-13969.67)
     Smythe_calcs['Fe2_XA_ideal']=Smythe_calcs['Fe2_wt_atom']*(-34274.174)
@@ -1518,82 +1568,69 @@
     Smythe_calcs['Fe2_XA_non_ideal']=Smythe_calcs['Fe2_wt_atom']*(-34895.294)
     Smythe_calcs['Ca_XA_non_ideal']=Smythe_calcs['Ca_wt_atom']*(-8831.616)
     Smythe_calcs['Na_XA_non_ideal']=Smythe_calcs['Na_wt_atom']*(-13712.715)
     Smythe_calcs['K_XA_non_ideal']=Smythe_calcs['K_wt_atom']*(-28583.983)
     Smythe_calcs['H_XA_non_ideal']=Smythe_calcs['H_wt_atom']*(-17766.114)
     Smythe_calcs['Si*Fe_non_ideal']=(Smythe_calcs['Si_wt_atom']*Smythe_calcs['Fe2_wt_atom'])*117815.515
 
+    if isinstance(T_K, pd.Series):
+        T_K=T_K.astype(float)
 
     Smythe_calcs['log_SCSS_ideal']=(
-
 (122175-80.28*T_K+8.474*T_K*np.log(T_K))/(8.314*T_K)+9.087+(Smythe_calcs['Si_XA_ideal']+Smythe_calcs['Ti_XA_ideal']
 +Smythe_calcs['Al_XA_ideal']+Smythe_calcs['Mg_XA_ideal']+Smythe_calcs['Fe2_XA_ideal']+Smythe_calcs['Ca_XA_ideal']
 +Smythe_calcs['Na_XA_ideal']+Smythe_calcs['K_XA_ideal']+Smythe_calcs['H_XA_ideal']+Smythe_calcs['Si*Fe_ideal'])/T_K
 +np.log(df_c['Fe_FeNiCu_Sulf_calc'])-np.log(Smythe_calcs['Fe2_wt_atom'])-269.4*0.1*P_kbar/T_K
 
 
     )
 
 
-    Smythe_calcs['SCSS_ideal_ppm_Smythe2017']=np.exp(Smythe_calcs['log_SCSS_ideal'])
-    Smythe_calcs['SCSS_ideal_ppm_Smythe2017_1sigma']=Smythe_calcs['SCSS_ideal_ppm_Smythe2017']*0.273169775211857
+    Smythe_calcs['SCSS2_ppm_ideal_Smythe2017']=np.exp(Smythe_calcs['log_SCSS_ideal'].astype(float))
+    Smythe_calcs['SCSS2_ppm_ideal_Smythe2017_1sigma']=Smythe_calcs['SCSS2_ppm_ideal_Smythe2017']*0.273169775211857
     Smythe_calcs['T_Input_K']=T_K
     Smythe_calcs['P_Input_kbar']=P_kbar
     Smythe_calcs['Fe_FeNiCu_Sulf']=df_c['Fe_FeNiCu_Sulf_calc']
     Smythe_calcs['Fe3Fet_Liq_input']=Fe3Fet_Liq
 
-    # if (isinstance(Fe_FeNiCu_Sulf, float) or isinstance(Fe_FeNiCu_Sulf, int)) or (isinstance(Fe_FeNiCu_Sulf, pd.Series)) and (Cu_FeNiCu_Sulf is None and Ni_FeNiCu_Sulf is None):
-    #     non_ideal=False
-    #     print('no non ideal SCSS as no Cu/CuFeNiCu')
-    # elif not (isinstance(Fe_FeNiCu_Sulf, pd.Series)):
-    #     if Fe_FeNiCu_Sulf == 'Calc_ONeill':
-    #         non_ideal=False
-    #     if Fe_FeNiCu_Sulf == 'Calc_Smythe':
-    #         non_ideal=True
-    #
-    #
-    # elif (isinstance(Fe_FeNiCu_Sulf, pd.Series)) and (Cu_FeNiCu_Sulf is not None and Ni_FeNiCu_Sulf is not None):
-    #     non_ideal=True
-    #
-    #
-    # if
+
     if 'Ni_FeNiCu_Sulf_calc' in df_c.columns and 'Cu_FeNiCu_Sulf_calc' in df_c.columns:
         Smythe_calcs['log_SCSS_non_ideal']=(
         (122175-80.28*T_K+8.474*T_K*np.log(T_K))/(8.314*T_K)+9.352+(Smythe_calcs['Si_XA_non_ideal']+Smythe_calcs['Ti_XA_non_ideal']
     +Smythe_calcs['Al_XA_non_ideal']+Smythe_calcs['Mg_XA_non_ideal']+Smythe_calcs['Fe2_XA_non_ideal']+Smythe_calcs['Ca_XA_non_ideal']
     +Smythe_calcs['Na_XA_non_ideal']+Smythe_calcs['K_XA_non_ideal']+Smythe_calcs['H_XA_non_ideal']+Smythe_calcs['Si*Fe_non_ideal'])
     /T_K+np.log(df_c['Fe_FeNiCu_Sulf_calc'])-np.log(Smythe_calcs['Fe2_wt_atom'])-264.85*0.1*P_kbar/T_K+546.362*((df_c['Cu_FeNiCu_Sulf_calc']**2 +df_c['Cu_FeNiCu_Sulf_calc']*df_c['Ni_FeNiCu_Sulf_calc'])/T_K)
         )
-        Smythe_calcs['SCSS_non_ideal_ppm_Smythe2017']=np.exp(Smythe_calcs['log_SCSS_non_ideal'])
-        Smythe_calcs['SCSS_non_ideal_ppm_Smythe2017_1sigma']=Smythe_calcs['SCSS_non_ideal_ppm_Smythe2017']*0.267299081373473
+        Smythe_calcs['SCSS2_ppm_non_ideal_Smythe2017']=np.exp(Smythe_calcs['log_SCSS_non_ideal'])
+        Smythe_calcs['SCSS2_ppm_non_ideal_Smythe2017_1sigma']=Smythe_calcs['SCSS2_ppm_non_ideal_Smythe2017']*0.267299081373473
 
-        cols_to_move = ['SCSS_ideal_ppm_Smythe2017', 'SCSS_ideal_ppm_Smythe2017_1sigma',
-        'SCSS_non_ideal_ppm_Smythe2017', 'SCSS_non_ideal_ppm_Smythe2017_1sigma',
+        cols_to_move = ['SCSS2_ppm_ideal_Smythe2017', 'SCSS2_ppm_ideal_Smythe2017_1sigma',
+        'SCSS2_ppm_non_ideal_Smythe2017', 'SCSS2_ppm_non_ideal_Smythe2017_1sigma',
         'T_Input_K', "P_Input_kbar",'Fe_FeNiCu_Sulf', 'Fe3Fet_Liq_input']
 
     else:
         print('no non ideal SCSS as no Cu/CuFeNiCu')
 
 
-        cols_to_move = ['SCSS_ideal_ppm_Smythe2017', 'SCSS_ideal_ppm_Smythe2017_1sigma',
+        cols_to_move = ['SCSS2_ppm_ideal_Smythe2017', 'SCSS2_ppm_ideal_Smythe2017_1sigma',
         'T_Input_K', "P_Input_kbar",'Fe_FeNiCu_Sulf', 'Fe3Fet_Liq_input']
 
     Smythe_calcs = Smythe_calcs[cols_to_move +
                                     [col for col in Smythe_calcs.columns if col not in cols_to_move]]
 
     Smythe_calcs['Fe_FeNiCu_Sulf_calc']=df_c['Fe_FeNiCu_Sulf_calc']
     Concat=pd.concat([Smythe_calcs, df_c], axis=1)
 
 
     return Concat
 
 
 ## Generic function for calculating sulfide composition
 
-def calculate_sulfide_comp_generic(*, T_K,
+def calculate_sulfide_comp_generic(*, T_K=None,
 Fe_Sulf=None, Ni_Sulf=None, Cu_Sulf=None, Fe_FeNiCu_Sulf=None, Cu_FeNiCu_Sulf=None, Ni_FeNiCu_Sulf=None,
 Ni_Liq=None, Cu_Liq=None, df_c=None, Ni_Sulf_init=5, Cu_Sulf_init=5 ):
     """ Generic function for calculating sulfide composition,
     either from input Fe-Ni-Cu contents in wt%, or using models of
     ONeill and Smythe
 
     Sulfide Composition: Options to calculate from the liquid composition, enter the comp in el wt%,
@@ -1622,15 +1659,30 @@
             values for Cu_FeNiCu_Sulf and Ni_FeNiCu_Sulf
 
         if you want to input a measured sulfide composition in el wt%
             Fe_Sulf, Ni_Sulf, Cu_Sulf = int, float, pandas series
 
 
     """
+    # Check they have entered enough info
+    if Fe_FeNiCu_Sulf is not None and not isinstance(Fe_FeNiCu_Sulf, str):
+        method='entered sulfide ratio'
+    elif Ni_Sulf is not None and Fe_Sulf is not None and Cu_Sulf is not None:
+        method='entered sulf comp'
+    elif isinstance(Fe_FeNiCu_Sulf, str):
+
+        if Fe_FeNiCu_Sulf != 'Calc_Smythe' and Fe_FeNiCu_Sulf != 'Calc_ONeill':
+            raise ValueError('Enter either Calc_Smythe or Calc_ONeill')
+        method='sulfide model'
+        if Ni_Liq is None or Cu_Liq is None:
+            raise ValueError('If you have choosen a sulfide model, you need to enter Ni_Liq and Cu_Liq ')
+    else:
+        raise ValueError('You need to enter some form of sulfide comp for this model, or choose a model and supply Ni and Cu in the liquid')
     # First, if the user entered an integer or float for Ni and Cu, turn into a panda series
+
     if isinstance(Ni_Liq, int) is True or isinstance(Ni_Liq, float) is True:
         Ni_Liq=pd.Series(Ni_Liq, index=range(len(df_c)))
     if isinstance(Cu_Liq, int) is True or isinstance(Cu_Liq, float) is True:
         Cu_Liq=pd.Series(Cu_Liq, index=range(len(df_c)))
 
     # Checking no contradictory intputs
     if Fe_Sulf is not None and Ni_Sulf is not None and Cu_Sulf is not None and Fe_FeNiCu_Sulf is not None:
@@ -1661,14 +1713,16 @@
     # Start with these none
     Cu_FeNiCu_Sulf_calc=None
     Ni_FeNiCu_Sulf_calc=None
 
     # If its a model, do this.
     if isinstance(Fe_FeNiCu_Sulf, str):
         if Fe_FeNiCu_Sulf=="Calc_Smythe":
+            if T_K is None:
+                raise ValueError('you need to enter a  temperature using the arguement T_K to use this model')
 
 
             # This does the Scipy minimisation of Cu and Ni contents using Kiseeva et al. (2015)
             calc_sulf=calculate_Symthe_sulf_minimisation(FeOt_Liq=df_c['FeOt_Liq'], Fe3Fet_Liq=df_c['Fe3Fet_Liq'],
                                             T_K=T_K, Ni_Liq=Ni_Liq, Cu_Liq=Cu_Liq, Ni_Sulf_init=Ni_Sulf_init, Cu_Sulf_init=Cu_Sulf_init)
 
             # This feeds those result back into a simpler function to get the Fe, S and O content of the sulfide
@@ -1681,14 +1735,16 @@
             Ni_FeNiCu_Sulf_calc=calculate_sulf_NiFeNiCu(Sulf_All['Ni_Sulf'], Sulf_All['Cu_Sulf'], Sulf_All['Fe_Sulf'])
 
             df_c['Ni_Sulf_Calc']=Sulf_All['Ni_Sulf']
             df_c['Cu_Sulf_Calc']=Sulf_All['Cu_Sulf']
             df_c['Fe_Sulf_Calc']=Sulf_All['Fe_Sulf']
             df_c['O_Sulf_Calc']=Sulf_All['O_Sulf']
             df_c['S_Sulf_Calc']=Sulf_All['S_Sulf']
+            df_c['DCu']=Sulf_All['DCu']
+            df_c['DNi']=Sulf_All['DNi']
 
         if Fe_FeNiCu_Sulf=="Calc_ONeill":
             Fe_FeNiCu_Sulf_calc=calculate_ONeill_sulf(FeOt_Liq=df_c['FeOt_Liq'],
             Ni_Liq=Ni_Liq, Cu_Liq=Cu_Liq, Fe3Fet_Liq=df_c['Fe3Fet_Liq'])
             Fe_FeNiCu_Sulf=Fe_FeNiCu_Sulf_calc
 
     # If they have given the sulfide chemistry
```

### Comparing `PySulfSat-0.0.9/src/PySulfSat.egg-info/SOURCES.txt` & `PySulfSat-1.0.1/src/PySulfSat.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 src/PySulfSat/Cali_Smythe17.pkl
 src/PySulfSat/Cali_ZT2019.pkl
 src/PySulfSat/Smythe17.pkl
 src/PySulfSat/__init__.py
 src/PySulfSat/_version.py
 src/PySulfSat/cali_plots.py
 src/PySulfSat/core_calcs.py
+src/PySulfSat/error_prop.py
 src/PySulfSat/import_data.py
 src/PySulfSat/mantle_melting.py
+src/PySulfSat/monte_carlo_s_in_sulf_recon.py
 src/PySulfSat/s6_corrections.py
 src/PySulfSat/scas_calc.py
 src/PySulfSat/scss_calcs2.py
 src/PySulfSat/sulf_mass_balance.py
 src/PySulfSat.egg-info/PKG-INFO
 src/PySulfSat.egg-info/SOURCES.txt
 src/PySulfSat.egg-info/dependency_links.txt
```

