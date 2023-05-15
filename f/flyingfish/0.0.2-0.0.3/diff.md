# Comparing `tmp/flyingfish-0.0.2.tar.gz` & `tmp/flyingfish-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flyingfish-0.0.2.tar", last modified: Thu Jan 12 08:21:11 2023, max compression
+gzip compressed data, was "flyingfish-0.0.3.tar", last modified: Mon May 15 17:28:30 2023, max compression
```

## Comparing `flyingfish-0.0.2.tar` & `flyingfish-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,29 @@
-drwxr-xr-x   0 lena      (1000) lena      (1000)        0 2023-01-12 08:21:11.910878 flyingfish-0.0.2/
--rw-r--r--   0 lena      (1000) lena      (1000)     1075 2022-11-18 15:56:05.000000 flyingfish-0.0.2/LICENSE
--rw-r--r--   0 lena      (1000) lena      (1000)     2244 2023-01-12 08:21:11.910878 flyingfish-0.0.2/PKG-INFO
--rw-r--r--   0 lena      (1000) lena      (1000)     1766 2023-01-11 19:15:25.000000 flyingfish-0.0.2/README.md
-drwxr-xr-x   0 lena      (1000) lena      (1000)        0 2023-01-12 08:21:11.910878 flyingfish-0.0.2/flyingfish/
--rw-r--r--   0 lena      (1000) lena      (1000)     5961 2023-01-11 20:50:49.000000 flyingfish-0.0.2/flyingfish/EDA.py
--rw-r--r--   0 lena      (1000) lena      (1000)        0 2023-01-10 15:10:56.000000 flyingfish-0.0.2/flyingfish/__init__.py
--rw-r--r--   0 lena      (1000) lena      (1000)     5823 2023-01-11 19:20:39.000000 flyingfish-0.0.2/flyingfish/timeseries.py
-drwxr-xr-x   0 lena      (1000) lena      (1000)        0 2023-01-12 08:21:11.910878 flyingfish-0.0.2/flyingfish.egg-info/
--rw-r--r--   0 lena      (1000) lena      (1000)     2244 2023-01-12 08:21:11.000000 flyingfish-0.0.2/flyingfish.egg-info/PKG-INFO
--rw-r--r--   0 lena      (1000) lena      (1000)      234 2023-01-12 08:21:11.000000 flyingfish-0.0.2/flyingfish.egg-info/SOURCES.txt
--rw-r--r--   0 lena      (1000) lena      (1000)        1 2023-01-12 08:21:11.000000 flyingfish-0.0.2/flyingfish.egg-info/dependency_links.txt
--rw-r--r--   0 lena      (1000) lena      (1000)       11 2023-01-12 08:21:11.000000 flyingfish-0.0.2/flyingfish.egg-info/top_level.txt
--rw-r--r--   0 lena      (1000) lena      (1000)      549 2023-01-12 08:21:04.000000 flyingfish-0.0.2/pyproject.toml
--rw-r--r--   0 lena      (1000) lena      (1000)       38 2023-01-12 08:21:11.910878 flyingfish-0.0.2/setup.cfg
+drwxr-xr-x   0 lena      (1000) lena      (1000)        0 2023-05-15 17:28:30.790674 flyingfish-0.0.3/
+-rw-r--r--   0 lena      (1000) lena      (1000)     1075 2022-11-18 15:56:05.000000 flyingfish-0.0.3/LICENSE
+-rw-r--r--   0 lena      (1000) lena      (1000)     3604 2023-05-15 17:28:30.790674 flyingfish-0.0.3/PKG-INFO
+-rw-r--r--   0 lena      (1000) lena      (1000)     3127 2023-05-15 17:08:31.000000 flyingfish-0.0.3/README.md
+drwxr-xr-x   0 lena      (1000) lena      (1000)        0 2023-05-15 17:28:30.790674 flyingfish-0.0.3/flyingfish/
+drwxr-xr-x   0 lena      (1000) lena      (1000)        0 2023-05-15 17:28:30.790674 flyingfish-0.0.3/flyingfish/EDA/
+-rw-r--r--   0 lena      (1000) lena      (1000)     1523 2023-05-15 17:08:46.000000 flyingfish-0.0.3/flyingfish/EDA/__init__.py
+-rw-r--r--   0 lena      (1000) lena      (1000)     3505 2023-02-27 15:34:31.000000 flyingfish-0.0.3/flyingfish/EDA/estimates_location.py
+-rw-r--r--   0 lena      (1000) lena      (1000)     1688 2023-02-27 15:34:31.000000 flyingfish-0.0.3/flyingfish/EDA/estimates_shape.py
+-rw-r--r--   0 lena      (1000) lena      (1000)     3789 2023-02-27 15:34:31.000000 flyingfish-0.0.3/flyingfish/EDA/estimates_variability.py
+-rw-r--r--   0 lena      (1000) lena      (1000)     2288 2023-05-15 17:01:49.000000 flyingfish-0.0.3/flyingfish/EDA/multivariate.py
+-rw-r--r--   0 lena      (1000) lena      (1000)     2593 2023-05-15 17:05:49.000000 flyingfish-0.0.3/flyingfish/EDA/outlier_analysis.py
+-rw-r--r--   0 lena      (1000) lena      (1000)     1087 2023-02-27 15:34:31.000000 flyingfish-0.0.3/flyingfish/EDA/plotting_positions.py
+-rw-r--r--   0 lena      (1000) lena      (1000)      883 2023-02-27 15:34:31.000000 flyingfish-0.0.3/flyingfish/EDA/quality_investigation.py
+drwxr-xr-x   0 lena      (1000) lena      (1000)        0 2023-05-15 17:28:30.790674 flyingfish-0.0.3/flyingfish/FDM/
+-rw-r--r--   0 lena      (1000) lena      (1000)     8646 2023-05-15 17:23:20.000000 flyingfish-0.0.3/flyingfish/FDM/Model.py
+-rw-r--r--   0 lena      (1000) lena      (1000)        0 2023-02-27 15:40:46.000000 flyingfish-0.0.3/flyingfish/FDM/__init__.py
+-rw-r--r--   0 lena      (1000) lena      (1000)        0 2023-02-27 14:51:59.000000 flyingfish-0.0.3/flyingfish/__init__.py
+-rw-r--r--   0 lena      (1000) lena      (1000)     6100 2023-01-21 15:18:56.000000 flyingfish-0.0.3/flyingfish/timeseries.py
+drwxr-xr-x   0 lena      (1000) lena      (1000)        0 2023-05-15 17:28:30.790674 flyingfish-0.0.3/flyingfish.egg-info/
+-rw-r--r--   0 lena      (1000) lena      (1000)     3604 2023-05-15 17:28:30.000000 flyingfish-0.0.3/flyingfish.egg-info/PKG-INFO
+-rw-r--r--   0 lena      (1000) lena      (1000)      591 2023-05-15 17:28:30.000000 flyingfish-0.0.3/flyingfish.egg-info/SOURCES.txt
+-rw-r--r--   0 lena      (1000) lena      (1000)        1 2023-05-15 17:28:30.000000 flyingfish-0.0.3/flyingfish.egg-info/dependency_links.txt
+-rw-r--r--   0 lena      (1000) lena      (1000)       11 2023-05-15 17:28:30.000000 flyingfish-0.0.3/flyingfish.egg-info/top_level.txt
+-rw-r--r--   0 lena      (1000) lena      (1000)      549 2023-05-15 17:27:54.000000 flyingfish-0.0.3/pyproject.toml
+-rw-r--r--   0 lena      (1000) lena      (1000)       38 2023-05-15 17:28:30.790674 flyingfish-0.0.3/setup.cfg
+drwxr-xr-x   0 lena      (1000) lena      (1000)        0 2023-05-15 17:28:30.790674 flyingfish-0.0.3/tests/
+-rw-r--r--   0 lena      (1000) lena      (1000)    15128 2023-05-15 17:26:15.000000 flyingfish-0.0.3/tests/test_EDA.py
+-rw-r--r--   0 lena      (1000) lena      (1000)     4203 2023-01-21 15:18:56.000000 flyingfish-0.0.3/tests/test_TimeSeries.py
```

### Comparing `flyingfish-0.0.2/LICENSE` & `flyingfish-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flyingfish-0.0.2/flyingfish/timeseries.py` & `flyingfish-0.0.3/flyingfish/timeseries.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,16 @@
         Args:
             date_start (datetime.datetime): first date
             date_end (datetime.datetime): last date
 
         Returns:
             pd.DataFrame: sub-DataFrame with "date" as index
         """
+        if self.df.empty:
+            raise ValueError("empty data")
         df_sub = self.df.loc[date_start:date_end]
         return TimeSeries(df_sub)
 
     def subset_period(
             self,
             months: list[int] = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]):
         """Returns a sub-DataFrame based on given months.
@@ -50,14 +52,16 @@
         Args:
             months (list[int]): month index (e.g. 1 for January).
                 Defaults to [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12].
 
         Returns:
             pd.DataFrame: sub-DataFrame with "date" as index
         """
+        if self.df.empty:
+            raise ValueError("empty data")
         df_sub = self.df.copy(deep=True)
         df_sub["month"] = df_sub.index
         df_sub["month"] = [int(x.month) for x in df_sub["month"].tolist()]
         df_sub = df_sub[df_sub["month"].isin(months)]
         df_sub = df_sub.drop(columns=["month"], axis=1)
         return TimeSeries(df_sub)
 
@@ -73,14 +77,17 @@
                 Defaults to 11.
             hyd_year_begin_day (int, optional): number of day of a month.
                 Defaults to 1.
 
         Returns:
             pd.DataFrame: given input DataFrame with new column "hyd_year"
         """
+        if self.df.empty:
+            raise ValueError("empty data")
+
         df_copy = self.df.copy(deep=True)
 
         # Initialize hydrological year with calendric year.
         df_copy['hyd_year'] = df_copy.index.year
 
         # Increment the hydrological year if it starts before 1st of January.
         for index, _ in df_copy.iterrows():
@@ -127,14 +134,16 @@
             aggr_col_name (str): column name for aggregation
                 (e.g. "hyd_year" derived from function hyd_year)
 
         Returns:
             float, float, float, float, float: values representing
                 HHX, HX, MX, NX, NNX
         """
+        if self.df.empty:
+            raise ValueError("empty data")
 
         # Create new TimeSeries instance
         df_copy = self.df.copy(deep=True)
         ts_new = TimeSeries(df=df_copy)
 
         # Derive highest and lowest value ever observed
         hhx = np.round(np.max(ts_new.df[varname]), 2)
```

### Comparing `flyingfish-0.0.2/pyproject.toml` & `flyingfish-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flyingfish"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Lena Marie Müller", email="lenamariemue@gmail.com" },
 ]
 description = "An open source library for common hydrological and meteorological issues"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

