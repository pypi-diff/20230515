# Comparing `tmp/omniplate-0.9.82.tar.gz` & `tmp/omniplate-0.9.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniplate-0.9.82.tar", max compression
+gzip compressed data, was "omniplate-0.9.84.tar", max compression
```

## Comparing `omniplate-0.9.82.tar` & `omniplate-0.9.84.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0      244 2022-05-26 16:08:15.786293 omniplate-0.9.82/README.md
--rw-r--r--   0        0        0     2972 2023-05-09 11:28:17.764069 omniplate-0.9.82/om_code/admin.py
--rw-r--r--   0        0        0     2577 2023-04-24 14:56:03.000000 omniplate-0.9.82/om_code/analyseOldTecan.py
--rw-r--r--   0        0        0     1771 2023-01-30 16:21:37.000000 omniplate-0.9.82/om_code/analyseSunrise.py
--rw-r--r--   0        0        0     2609 2023-04-24 14:56:03.000000 omniplate-0.9.82/om_code/analyseTecan.py
--rw-r--r--   0        0        0     1289 2023-04-24 14:56:03.000000 omniplate-0.9.82/om_code/clogger.py
--rw-r--r--   0        0        0    24158 2023-05-09 11:28:17.764548 omniplate-0.9.82/om_code/corrections.py
--rw-r--r--   0        0        0     1380 2023-01-30 16:21:38.000000 omniplate-0.9.82/om_code/dilution_data_lucia.tsv
--rw-r--r--   0        0        0     1893 2023-01-30 16:21:38.000000 omniplate-0.9.82/om_code/dilution_data_xiao.tsv
--rw-r--r--   0        0        0     6965 2023-04-24 14:56:03.000000 omniplate-0.9.82/om_code/getfitnesspenalty.py
--rw-r--r--   0        0        0     3666 2023-01-30 16:21:38.000000 omniplate-0.9.82/om_code/loadplatedata.py
--rw-r--r--   0        0        0     3905 2023-05-09 11:28:17.764767 omniplate-0.9.82/om_code/midlog.py
--rw-r--r--   0        0        0      435 2022-05-26 16:08:15.904220 omniplate-0.9.82/om_code/omerrors.py
--rw-r--r--   0        0        0    17184 2023-05-09 11:28:17.765933 omniplate-0.9.82/om_code/omfitderiv.py
--rw-r--r--   0        0        0     4179 2023-05-09 11:28:17.774527 omniplate-0.9.82/om_code/omgenutils.py
--rw-r--r--   0        0        0    11514 2023-05-09 11:28:17.775566 omniplate-0.9.82/om_code/omplot.py
--rw-r--r--   0        0        0     6473 2023-05-09 11:28:17.776522 omniplate-0.9.82/om_code/omstats.py
--rw-r--r--   0        0        0     6472 2023-05-09 11:28:17.820114 omniplate-0.9.82/om_code/sunder.py
--rw-r--r--   0        0        0    95311 2023-05-09 11:28:17.820960 omniplate-0.9.82/omniplate/Omniplate.py
--rw-r--r--   0        0        0       44 2022-05-26 16:08:15.902667 omniplate-0.9.82/omniplate/__init__.py
--rw-r--r--   0        0        0     1116 2023-05-09 11:28:17.821366 omniplate-0.9.82/pyproject.toml
--rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 omniplate-0.9.82/PKG-INFO
+-rw-r--r--   0        0        0      244 2022-05-26 16:08:15.000000 omniplate-0.9.84/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 08:36:42.000000 omniplate-0.9.84/om_code/__init__.py
+-rw-r--r--   0        0        0     2972 2023-05-09 11:28:17.000000 omniplate-0.9.84/om_code/admin.py
+-rw-r--r--   0        0        0     2577 2023-04-24 14:56:03.906492 omniplate-0.9.84/om_code/analyseOldTecan.py
+-rw-r--r--   0        0        0     1771 2023-01-30 16:21:37.981212 omniplate-0.9.84/om_code/analyseSunrise.py
+-rw-r--r--   0        0        0     2609 2023-04-24 14:56:03.906801 omniplate-0.9.84/om_code/analyseTecan.py
+-rw-r--r--   0        0        0     1289 2023-04-24 14:56:03.907067 omniplate-0.9.84/om_code/clogger.py
+-rw-r--r--   0        0        0    24158 2023-05-09 11:28:17.000000 omniplate-0.9.84/om_code/corrections.py
+-rw-r--r--   0        0        0     1380 2023-01-30 16:21:38.087062 omniplate-0.9.84/om_code/dilution_data_lucia.tsv
+-rw-r--r--   0        0        0     1893 2023-01-30 16:21:38.122549 omniplate-0.9.84/om_code/dilution_data_xiao.tsv
+-rw-r--r--   0        0        0     6965 2023-04-24 14:56:03.907876 omniplate-0.9.84/om_code/getfitnesspenalty.py
+-rw-r--r--   0        0        0     3666 2023-01-30 16:21:38.140112 omniplate-0.9.84/om_code/loadplatedata.py
+-rw-r--r--   0        0        0     3905 2023-05-09 11:28:17.000000 omniplate-0.9.84/om_code/midlog.py
+-rw-r--r--   0        0        0      435 2022-05-26 16:08:15.000000 omniplate-0.9.84/om_code/omerrors.py
+-rw-r--r--   0        0        0    17865 2023-05-12 16:40:15.463890 omniplate-0.9.84/om_code/omfitderiv.py
+-rw-r--r--   0        0        0     4179 2023-05-09 11:28:17.000000 omniplate-0.9.84/om_code/omgenutils.py
+-rw-r--r--   0        0        0    11514 2023-05-09 11:28:17.000000 omniplate-0.9.84/om_code/omplot.py
+-rw-r--r--   0        0        0     6473 2023-05-09 11:28:17.000000 omniplate-0.9.84/om_code/omstats.py
+-rw-r--r--   0        0        0     6472 2023-05-09 11:28:17.000000 omniplate-0.9.84/om_code/sunder.py
+-rw-r--r--   0        0        0    95590 2023-05-15 09:46:12.940528 omniplate-0.9.84/omniplate/Omniplate.py
+-rw-r--r--   0        0        0       44 2022-05-26 16:08:15.000000 omniplate-0.9.84/omniplate/__init__.py
+-rw-r--r--   0        0        0     1116 2023-05-15 09:47:53.560320 omniplate-0.9.84/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 omniplate-0.9.84/setup.py
+-rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 omniplate-0.9.84/PKG-INFO
```

### Comparing `omniplate-0.9.82/om_code/admin.py` & `omniplate-0.9.84/om_code/admin.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/om_code/analyseOldTecan.py` & `omniplate-0.9.84/om_code/analyseOldTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/om_code/analyseSunrise.py` & `omniplate-0.9.84/om_code/analyseSunrise.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/om_code/analyseTecan.py` & `omniplate-0.9.84/om_code/analyseTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/om_code/clogger.py` & `omniplate-0.9.84/om_code/clogger.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/om_code/corrections.py` & `omniplate-0.9.84/om_code/corrections.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/om_code/dilution_data_lucia.tsv` & `omniplate-0.9.84/om_code/dilution_data_lucia.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/om_code/dilution_data_xiao.tsv` & `omniplate-0.9.84/om_code/dilution_data_xiao.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/om_code/getfitnesspenalty.py` & `omniplate-0.9.84/om_code/getfitnesspenalty.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/om_code/loadplatedata.py` & `omniplate-0.9.84/om_code/loadplatedata.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/om_code/midlog.py` & `omniplate-0.9.84/om_code/midlog.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/om_code/omfitderiv.py` & `omniplate-0.9.84/om_code/omfitderiv.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         exitearly=False,
         bd=False,
         empirical_errors=False,
         optmethod="L-BFGS-B",
         nosamples=100,
         stats=True,
         statnames=False,
+        printstats=True,
         showstaterrors=True,
         warn=False,
         linalgmax=3,
         iskip=False,
     ):
         """
         Smooth data and estimate time derivatives with a Gaussian process.
@@ -147,16 +148,18 @@
             maximal time
             derivative;
             'max f' for the maximal value of the smoothed data;
             'lag time' for the lag time defined as the time when the
             tangent from the point with the maximal time derivative
             crosses a line parallel to the time-axis that passes
             through the first data point.
+        printstats: boolean, optional
+            If True, print the summary statistics calculated.
         showstaterrors: boolean, optional
-            If True, display estimated errors for the statistics.
+            If True, display estimated errors for the statistics when printing.
         warn: boolean, optional
             If False, warnings created by covariance matrices that are not
             positive semi-definite are suppressed.
         linalgmax: integer, optional
             The number of times errors generated by underlying linear algebra
             modules during the optimisation by poor choices of the
             hyperparameters should be ignored.
@@ -263,14 +266,15 @@
                 noinits,
                 exitearly,
                 optmethod,
                 stats,
                 nosamples,
                 statnames,
                 showstaterrors,
+                printstats,
             )
 
     def run(
         self,
         cvfn,
         ta,
         da,
@@ -279,14 +283,15 @@
         noinits,
         exitearly,
         optmethod,
         stats,
         nosamples,
         statnames,
         showstaterrors,
+        printstats,
     ):
         """Instantiate and run a Gaussian process."""
         try:
             # instantiate GP
             g = getattr(gp, cvfn + "GP")(self.bds, ta, da, merrors=ma)
             print("Using a " + g.description + ".")
             g.info
@@ -318,15 +323,17 @@
         self.f = g.f
         self.df = g.df
         self.ddf = g.ddf
         self.fvar = g.fvar
         self.dfvar = g.dfvar
         self.ddfvar = g.ddfvar
         if stats:
-            self.calculatestats(nosamples, statnames, showstaterrors)
+            self.calculatestats(
+                nosamples, statnames, showstaterrors, printstats
+            )
 
     def fitderivsample(self, nosamples, newt=None):
         """
         Generate samples from the latent function.
 
         Both values for the latent function and its first two
         derivatives are returned, as a tuple.
@@ -356,45 +363,55 @@
             gps = copy.deepcopy(self.g)
             gps.predict(newt, derivs=2, addnoise=True)
         else:
             gps = self.g
         samples = gps.sample(nosamples, derivs=2)
         return samples
 
-    def calculatestats(self, nosamples=100, statnames=None, showerrors=True):
+    def calculatestats(self, nosamples, statnames, showerrors, printstats):
         """
         Calculate statistics from the smoothed data.
 
         The default names are 'max df', 'time of max df', 'inverse max grad',
         'max f', and 'lag time'.
 
         Parameters
         ----------
         nosamples: integer
             The number of bootstrap samples used to estimate errors.
         statnames: list of strings, optional
             A list of alternative names for the statistics.
         showerrors: boolean, optional
             If True, display the estimated errors.
+        printstats: boolean, optional
+            If True, print the summary stats calculated.
         """
         print(f"\nCalculating statistics with {nosamples} samples.")
-        if showerrors:
-            print("\t(displaying median +/- half interquartile range)\n")
         if statnames:
             self.stats = statnames
         else:
             self.stats = [
+                "min_f",
+                "max_f",
                 "max_df",
                 "time_of_max_df",
                 "doubling_time_from_max_df",
                 "lag_time",
             ]
         t = self.t
         fs, gs, hs = self.fitderivsample(nosamples)
-        # calculate stats
+        # min f
+        min_od = fs[np.argmin(fs, 0), np.arange(nosamples)]
+        if self.logs:
+            min_od = np.exp(min_od)
+        # max f
+        max_od = fs[np.argmax(fs, 0), np.arange(nosamples)]
+        if self.logs:
+            max_od = np.exp(max_od)
+        # calculate df stats
         im = np.argmax(gs, 0)
         # max df
         mgr = gs[im, np.arange(nosamples)]
         # time of max df
         tmgr = np.array([t[i] for i in im])
         # inverse max df
         dt = np.log(2) / mgr
@@ -402,47 +419,51 @@
         lagtime = (
             tmgr
             + (fs[0, np.arange(nosamples)] - fs[im, np.arange(nosamples)])
             / mgr
         )
         # store stats
         ds = {}
-        for stname, st in zip(self.stats, [mgr, tmgr, dt, lagtime]):
+        for stname, st in zip(
+            self.stats, [min_od, max_od, mgr, tmgr, dt, lagtime]
+        ):
             ds[stname] = np.median(st)
             ds[stname + "_err"] = omstats.statserr(st) / 2
         self.ds = ds
         self.nosamples = nosamples
-        self.printstats(showerrors=showerrors)
+        self.stats2dict(showerrors, printstats)
 
-    def printstats(self, showerrors=True, performprint=True):
+    def stats2dict(self, showerrors, printstats):
         """
         Create and print a dictionary of statistics.
 
         The statistics are calculated from the smoothed data and its
         inferred time-derivatives.
 
         Parameters
         ----------
         showerrors: boolean, optional
             If True, display the errors.
-        performprint: boolean optional
+        printstats: boolean optional
             If True, display the statistics.
 
         Returns
         -------
         statd: dictionary
             The statistics and their errors.
         """
+        if showerrors and printstats:
+            print("\t(displaying median +/- half interquartile range)\n")
         ds = self.ds
         statd = {}
         lenstr = np.max([len(s) for s in self.stats])
         for s in self.stats:
             statd[s] = ds[s]
             statd[s + "_err"] = ds[s + "_err"]
-            if performprint:
+            if printstats:
                 stname = s.rjust(lenstr + 1)
                 if showerrors:
                     print(
                         "{:s}= {:6e} +/- {:6e}".format(
                             stname, statd[s], ds[s + "_err"]
                         )
                     )
```

### Comparing `omniplate-0.9.82/om_code/omgenutils.py` & `omniplate-0.9.84/om_code/omgenutils.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/om_code/omplot.py` & `omniplate-0.9.84/om_code/omplot.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/om_code/omstats.py` & `omniplate-0.9.84/om_code/omstats.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/om_code/sunder.py` & `omniplate-0.9.84/om_code/sunder.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.82/omniplate/Omniplate.py` & `omniplate-0.9.84/omniplate/Omniplate.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import om_code.omstats as omstats
 import om_code.sunder as sunder
 import om_code.midlog as midlog
 import pandas as pd
 import seaborn as sns
 from om_code.omfitderiv import fitderiv
 
-version = "0.9.82"
+version = "0.9.84"
 
 plt.rcParams["figure.max_open_warning"] = 0
 sns.set()
 
 
 class platereader:
     """
@@ -1828,14 +1828,15 @@
         noruns=10,
         exitearly=True,
         noinits=100,
         nosamples=100,
         logs=True,
         iskip=False,
         stats=True,
+        printstats=False,
         figs=True,
         findareas=False,
         plotlocalmax=True,
         showpeakproperties=False,
         experiments="all",
         experimentincludes=False,
         experimentexcludes=False,
@@ -1895,15 +1896,17 @@
             bootstrapping.
         logs: boolean, optional
             If True, find the derivative of the log of the data and should be
             True to determine the specific growth rate when dtype= 'OD'.
         iskip: integer, optional
             Use only every iskip'th data point to increase speed.
         stats: boolean, optional
-            If False, do not calculate statistics.
+            If True, calculate summary statistics.
+        printstats: boolean, optional
+            If True, print summary statistics.
         figs: boolean, optional
             If True, plot both the fits and inferred derivative.
         findareas: boolean, optional
             If True, find the area under the plot of gr vs OD and the area
             under the plot of OD vs time. Setting to True can make getstats
             slow.
         plotlocalmax: boolean, optional
@@ -1961,14 +1964,16 @@
         linalgmax = 5
         warnings = ""
         if dtype == "OD" and logs:
             derivname = "gr"
         else:
             derivname = "d/dt_" + dtype
         snames = [
+            "min_" + dtype,
+            "max_" + dtype,
             "max_" + derivname,
             "time_of_max_" + derivname,
         ]
         if dtype == "OD" and logs:
             # special names with estimating specific growth rate
             snames += ["doubling_time", "lag_time"]
         else:
@@ -2043,14 +2048,15 @@
                         t,
                         d,
                         cvfn=cvfn,
                         logs=logs,
                         bd=bd,
                         empirical_errors=empirical_errors,
                         statnames=snames,
+                        printstats=printstats,
                         noruns=noruns,
                         noinits=noinits,
                         exitearly=exitearly,
                         linalgmax=linalgmax,
                         nosamples=nosamples,
                         iskip=iskip,
                     )
@@ -2097,14 +2103,15 @@
                                 + str(j)
                                 + "_for_"
                                 + derivname
                             ] = val
                         # add time series to s dataframe
                         admin.add_to_s(self, derivname, outdf)
                         if stats:
+                            # add stats calculated by omfitderiv
                             for sname in f.ds.keys():
                                 statsdict[sname] = f.ds[sname]
                         # create or add summary stats to sc dataframe
                         statsdf = pd.DataFrame(
                             statsdict, index=pd.RangeIndex(0, 1, 1)
                         )
                         admin.add_to_sc(self, statsdf)
```

### Comparing `omniplate-0.9.82/pyproject.toml` & `omniplate-0.9.84/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omniplate"
-version = "0.9.82"
+version = "0.9.84"
 description = "For analysing and meta-analysing plate-reader data"
 authors = ["Peter Swain <peter.swain@ed.ac.uk>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://swainlab.bio.ed.ac.uk/software/omniplate"
 repository = "https://git.ecdf.ed.ac.uk/pswain/omniplate"
```

### Comparing `omniplate-0.9.82/PKG-INFO` & `omniplate-0.9.84/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplate
-Version: 0.9.82
+Version: 0.9.84
 Summary: For analysing and meta-analysing plate-reader data
 Home-page: https://swainlab.bio.ed.ac.uk/software/omniplate
 License: MIT
 Keywords: omniplate,systems biology,bioinformatics,plate readers
 Author: Peter Swain
 Author-email: peter.swain@ed.ac.uk
 Requires-Python: >=3.8,<3.11
```

