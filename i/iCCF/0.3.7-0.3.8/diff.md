# Comparing `tmp/iCCF-0.3.7.tar.gz` & `tmp/iCCF-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iCCF-0.3.7.tar", last modified: Fri Apr 10 17:05:43 2020, max compression
+gzip compressed data, was "dist/iCCF-0.3.8.tar", last modified: Thu Aug  6 15:15:36 2020, max compression
```

## Comparing `iCCF-0.3.7.tar` & `iCCF-0.3.8.tar`

### file list

```diff
@@ -1,31 +1,46 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-10 17:05:43.000000 iCCF-0.3.7/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-10 17:05:43.000000 iCCF-0.3.7/iCCF.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2933 2020-04-10 17:05:43.000000 iCCF-0.3.7/iCCF.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-10 17:05:43.000000 iCCF-0.3.7/iCCF.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2020-04-10 17:05:43.000000 iCCF-0.3.7/iCCF.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-10 17:05:43.000000 iCCF-0.3.7/iCCF.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      491 2020-04-10 17:05:43.000000 iCCF-0.3.7/iCCF.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2020-04-10 17:05:43.000000 iCCF-0.3.7/iCCF.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      101 2020-04-10 17:05:43.000000 iCCF-0.3.7/iCCF.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2933 2020-04-10 17:05:43.000000 iCCF-0.3.7/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-10 17:05:43.000000 iCCF-0.3.7/iCCF/
--rw-rw-r--   0 travis    (2000) travis    (2000)      642 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/bigaussian.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10785 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/iCCF.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10776 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/bisector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/writers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3410 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/keywords.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4495 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/gaussian.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12250 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/chromatic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2330 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      143 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16239 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/meta_ESPRESSO.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1041 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/wspan.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7692 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/meta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4673 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/scripts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      483 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2424 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/ssh_files.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1637 2020-04-10 17:05:16.000000 iCCF-0.3.7/iCCF/vspan.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2080 2020-04-10 17:05:16.000000 iCCF-0.3.7/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-04-10 17:05:43.000000 iCCF-0.3.7/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1363 2020-04-10 17:05:16.000000 iCCF-0.3.7/setup.py
+drwxrwxr-x   0 jfaria    (1000) jfaria    (1000)        0 2020-08-06 15:15:36.000000 iCCF-0.3.8/
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     1045 2020-08-06 13:23:07.000000 iCCF-0.3.8/.gitignore
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)      917 2020-08-06 15:13:54.000000 iCCF-0.3.8/.travis.yml
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     1083 2020-08-06 13:23:07.000000 iCCF-0.3.8/LICENSE
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     2933 2020-08-06 15:15:36.000000 iCCF-0.3.8/PKG-INFO
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     2080 2020-08-06 13:23:07.000000 iCCF-0.3.8/README.md
+drwxrwxr-x   0 jfaria    (1000) jfaria    (1000)        0 2020-08-06 15:15:36.000000 iCCF-0.3.8/data/
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     3303 2020-08-06 13:23:07.000000 iCCF-0.3.8/data/spectral_format_blue.dat
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     2962 2020-08-06 13:23:07.000000 iCCF-0.3.8/data/spectral_format_red.dat
+drwxrwxr-x   0 jfaria    (1000) jfaria    (1000)        0 2020-08-06 15:15:36.000000 iCCF-0.3.8/iCCF/
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)      519 2020-08-06 14:04:25.000000 iCCF-0.3.8/iCCF/__init__.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)      642 2020-08-06 13:23:07.000000 iCCF-0.3.8/iCCF/bigaussian.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)    10776 2020-08-06 13:23:07.000000 iCCF-0.3.8/iCCF/bisector.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)    14619 2020-08-06 14:11:56.000000 iCCF-0.3.8/iCCF/chromatic.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     1080 2020-08-06 13:23:07.000000 iCCF-0.3.8/iCCF/config.py
+drwxrwxr-x   0 jfaria    (1000) jfaria    (1000)        0 2020-08-06 15:15:36.000000 iCCF-0.3.8/iCCF/example_data/
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     2704 2020-08-06 13:23:07.000000 iCCF-0.3.8/iCCF/example_data/CCF1.npy
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     4790 2020-08-06 13:23:07.000000 iCCF-0.3.8/iCCF/gaussian.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)    14653 2020-08-06 14:02:12.000000 iCCF-0.3.8/iCCF/iCCF.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     7290 2020-08-06 13:23:07.000000 iCCF-0.3.8/iCCF/keywords.py
+drwxrwxr-x   0 jfaria    (1000) jfaria    (1000)        0 2020-08-06 15:15:36.000000 iCCF-0.3.8/iCCF/logo/
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     9715 2020-08-06 13:23:07.000000 iCCF-0.3.8/iCCF/logo/logo.png
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)      645 2020-08-06 13:23:07.000000 iCCF-0.3.8/iCCF/logo/logo.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     7692 2020-08-06 13:23:07.000000 iCCF-0.3.8/iCCF/meta.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)    17710 2020-08-06 13:23:10.000000 iCCF-0.3.8/iCCF/meta_ESPRESSO.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     5126 2020-08-06 13:23:10.000000 iCCF-0.3.8/iCCF/scripts.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     2424 2020-08-06 13:23:07.000000 iCCF-0.3.8/iCCF/ssh_files.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     2722 2020-08-06 13:40:41.000000 iCCF-0.3.8/iCCF/utils.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)      143 2020-08-06 15:04:52.000000 iCCF-0.3.8/iCCF/version.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     1637 2020-08-06 13:23:07.000000 iCCF-0.3.8/iCCF/vspan.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     2100 2020-08-06 13:23:07.000000 iCCF-0.3.8/iCCF/writers.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     1041 2020-08-06 13:23:07.000000 iCCF-0.3.8/iCCF/wspan.py
+drwxrwxr-x   0 jfaria    (1000) jfaria    (1000)        0 2020-08-06 15:15:36.000000 iCCF-0.3.8/iCCF.egg-info/
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     2933 2020-08-06 15:15:36.000000 iCCF-0.3.8/iCCF.egg-info/PKG-INFO
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)      708 2020-08-06 15:15:36.000000 iCCF-0.3.8/iCCF.egg-info/SOURCES.txt
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)        1 2020-08-06 15:15:36.000000 iCCF-0.3.8/iCCF.egg-info/dependency_links.txt
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)      101 2020-08-06 15:15:36.000000 iCCF-0.3.8/iCCF.egg-info/entry_points.txt
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)        1 2020-08-06 15:15:36.000000 iCCF-0.3.8/iCCF.egg-info/not-zip-safe
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)       56 2020-08-06 15:15:36.000000 iCCF-0.3.8/iCCF.egg-info/requires.txt
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)        5 2020-08-06 15:15:36.000000 iCCF-0.3.8/iCCF.egg-info/top_level.txt
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)       38 2020-08-06 15:15:36.000000 iCCF-0.3.8/setup.cfg
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)     1337 2020-08-06 13:23:07.000000 iCCF-0.3.8/setup.py
+drwxrwxr-x   0 jfaria    (1000) jfaria    (1000)        0 2020-08-06 15:15:36.000000 iCCF-0.3.8/tests/
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)      362 2020-08-06 13:23:07.000000 iCCF-0.3.8/tests/test_gaussian.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)      332 2020-08-06 13:23:07.000000 iCCF-0.3.8/tests/test_iCCF.py
+-rw-rw-r--   0 jfaria    (1000) jfaria    (1000)       87 2020-08-06 13:23:07.000000 iCCF-0.3.8/tests/test_import.py
```

### Comparing `iCCF-0.3.7/iCCF.egg-info/PKG-INFO` & `iCCF-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iCCF
-Version: 0.3.7
+Version: 0.3.8
 Summary: Analysis of CCF profiles and activity indicators
 Home-page: https://github.com/j-faria/iCCF
 Author: João Faria
 Author-email: joao.faria@astro.up.pt
 License: UNKNOWN
 Description: <p align="center">
           <img width = "450" src="https://github.com/j-faria/iCCF/blob/master/iCCF/logo/logo.png?raw=true"/>
```

### Comparing `iCCF-0.3.7/PKG-INFO` & `iCCF-0.3.8/iCCF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iCCF
-Version: 0.3.7
+Version: 0.3.8
 Summary: Analysis of CCF profiles and activity indicators
 Home-page: https://github.com/j-faria/iCCF
 Author: João Faria
 Author-email: joao.faria@astro.up.pt
 License: UNKNOWN
 Description: <p align="center">
           <img width = "450" src="https://github.com/j-faria/iCCF/blob/master/iCCF/logo/logo.png?raw=true"/>
```

### Comparing `iCCF-0.3.7/iCCF/bigaussian.py` & `iCCF-0.3.8/iCCF/bigaussian.py`

 * *Files identical despite different names*

### Comparing `iCCF-0.3.7/iCCF/iCCF.py` & `iCCF-0.3.8/iCCF/iCCF.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 from astropy.io import fits
 from cached_property import cached_property
 
 from .gaussian import gauss, gaussfit, FWHM as FWHMcalc, RV, RVerror, contrast
 from .bisector import BIS, BIS_HARPS as BIS_HARPS_calc, bisector
 from .vspan import vspan
 from .wspan import wspan
-from .keywords import getRVarray, getBJD, getRV, getFWHM
+from .keywords import *
 from . import writers
 from .ssh_files import ssh_fits_open
-from .utils import no_stack_warning
+from .utils import no_stack_warning, _get_hdul
 
-
-EPS = 1e-5 # all indicators are accurate up to this epsilon
-nEPS = abs(math.floor(math.log(EPS, 10))) # number of decimals for output
+EPS = 1e-5  # all indicators are accurate up to this epsilon
+nEPS = abs(math.floor(math.log(EPS, 10)))  # number of decimals for output
 
 
 def rdb_names(names):
     """ Return the usual .rdb format names. """
     r = []
     for name in names:
         # print(name)
@@ -84,123 +83,174 @@
         else:
             r = f'CCFindicators(CCF from {basename(self.filename)})'
         return r
 
     def __len__(self):
         return 1
 
-
     @classmethod
     def from_file(cls, file, hdu_number=1, data_index=-1, sort_bjd=True,
-                  **kwargs):
+                  guess_instrument=True, **kwargs):
         """ 
         Create an `Indicators` object from one or more fits files.
         
         Parameters
         ----------
         file : str or list of str
             The name(s) of the fits file(s)
         hdu_number : int, default = 1
             The index of the HDU list which contains the CCF
         data_index : int, default = -1
             The index of the .data array which contains the CCF. The data will 
             be accessed as ccf = HDU[hdu_number].data[data_index,:]
-        sort_bjd : bool
-            If True (default) and filename is a list of files, sort them by BJD
-            before reading
+        sort_bjd : bool (default True)
+            If True and filename is a list of files, sort them by BJD before 
+            reading
+        guess_instrument : bool (default False)
+            If True, try to guess the instrument and adjust both hdu_number
+            and data_index accordingly
         """
 
         if '*' in file or '?' in file:
             file = glob(file)
 
         # list of files
         if isinstance(file, Iterable) and not isinstance(file, str):
-            #! it's faster to do this after
-            # if sort_bjd:
-            #     file = sorted(file, key=getBJD)
-
-            indicators = [cls.from_file(f) for f in file]
+            indicators = []
+            for f in file:
+                indicators.append(
+                    cls.from_file(f, hdu_number, data_index, sort_bjd,
+                                  guess_instrument, **kwargs))
 
             if sort_bjd:
                 return sorted(indicators, key=lambda i: i.bjd)
             else:
                 return indicators
 
-            # N = len(file)
-            # rv, ccf = [], []
-            # for i in range(N):
-            #     f = file[i]
-            #     rv.append(getRVarray(f))
-            #     hdul = fits.open(f)
-            #     ccf.append(hdul[hdu_number].data[data_index, :])
-
         # just one file
         elif isinstance(file, str):
+            if 'S1D' in file:
+                no_stack_warning(
+                    f"filename {file} contains 'S1D', are you sure it's a CCF?"
+                )
+
             user, host = kwargs.pop('USER', None), kwargs.pop('HOST', None)
-            rv, hdul = getRVarray(file, return_hdul=True, USER=user, HOST=host)
+            if guess_instrument:
+                # find the instrument and adjust hdu_number / data_index
+                hdul = _get_hdul(file, USER=user, HOST=host)
+                try:
+                    inst = getINSTRUMENT(file, hdul)
+
+                    if inst == 'ESPRESSO':
+                        hdu_number, data_index = 1, -1
+
+                    if inst == 'HARPS':
+                        hdu_number, data_index = 0, -1
+
+                except KeyError:
+                    print('Cannot find instrument in {file}')
+
+                rv, hdul = getRVarray(file, hdul=hdul, return_hdul=True,
+                                      USER=user, HOST=host)
+
+            else:
+                # just try reading it
+                rv, hdul = getRVarray(file, return_hdul=True, USER=user,
+                                      HOST=host)
+
             ccf = hdul[hdu_number].data[data_index, :]
+
             I = cls(rv, ccf, **kwargs)
 
             # save attributes
             I.filename = file
             I.HDU = hdul
             I._hdu_number = hdu_number
             I._data_index = data_index
 
             return I
 
         else:
             raise ValueError(
                 'Input to `from_file` should be a string or list of strings.')
 
-
     @cached_property
     def bjd(self):
         """ Barycentric Julian Day when the observation was made """
         return getBJD(self.filename, hdul=self.HDU, mjd=False)
 
+    @property
+    def mask(self):
+        """ Mask used for the CCF calculation """
+        return getMASK(self.filename, hdul=self.HDU)
+
+    @property
+    def instrument(self):
+        return getINSTRUMENT(self.filename, hdul=self.HDU)
 
     @property
     def RV(self):
         """ The measured radial velocity, from a Gaussian fit to the CCF """
         return RV(self.rv, self.ccf)
 
     @property
     def RVerror(self):
         """ Photon-noise uncertainty on the measured radial velocity """
-        if self.eccf is not None: # CCF uncertainties were provided
+        if self.eccf is not None:  # CCF uncertainties were provided
             if self.eccf.size != self.ccf.size:
                 raise ValueError('CCF and CCF errors not of the same size')
             eccf = self.eccf
-        else: # try reading it from the HDU
+        else:  # try reading it from the HDU
             try:
-                eccf = self.HDU[2].data[-1,:] # for ESPRESSO
-            except Exception as e:
-                warnings.warn(e)
-                warnings.warn('Cannot access CCF uncertainties, using 1.0.')
-                eccf = np.ones_like(self.rv)
+                eccf = self.HDU[2].data[-1, :]  # for ESPRESSO
+            except Exception:
+                # warnings.warn('Cannot access CCF uncertainties, looking for value in header')
+                try:
+                    rve = getRVerror(None, hdul=self.HDU)
+                    return rve
+                except ValueError:
+                    # warnings.warn('Cannot access CCF uncertainties, using 1.0')
+                    eccf = np.ones_like(self.rv)
 
         return RVerror(self.rv, self.ccf, eccf)
 
-    @property
+    @cached_property
     def individual_RV(self):
-        """ Individual radial velocities calculated for each spectral order """
+        """ Individual radial velocities for each spectral order """
         if not hasattr(self, 'HDU'):
             raise ValueError(
                 'Cannot access individual CCFs (no HDU attribute)')
 
         RVs = []
         for ccf in self.HDU[self._hdu_number].data[:-1]:
             if np.nonzero(ccf)[0].size == 0:
                 RVs.append(np.nan)
             else:
-                RVs.append(RV(self.rv, ccf))
+                p0 = [-ccf.ptp(), self.RV, self.FWHM, ccf.mean()]
+                RVs.append(RV(self.rv, ccf, p0=p0))
 
         return np.array(RVs)
 
+    @cached_property
+    def individual_RVerror(self):
+        """ Individual radial velocity errors for each spectral order """
+        if not hasattr(self, 'HDU'):
+            raise ValueError(
+                'Cannot access individual CCFs (no HDU attribute)')
+
+        RVes = []
+        CCFs, eCCFs = self.HDU[self._hdu_number].data, self.HDU[2].data
+        for ccf, eccf in zip(CCFs[:-1], eCCFs[:-1]):
+            if np.nonzero(ccf)[0].size == 0:
+                RVes.append(np.nan)
+            else:
+                RVes.append(RVerror(self.rv, ccf, eccf))
+
+        return np.array(RVes)
+
     @property
     def FWHM(self):
         """ The full width at half maximum of the CCF """
         return FWHMcalc(self.rv, self.ccf)
 
     @cached_property
     def BIS(self):
@@ -245,41 +295,69 @@
         The FWHM as derived by the pipeline and stored in CCF fits file
         """
         if not hasattr(self, 'HDU'):
             raise ValueError('Cannot access header (no HDU attribute)')
 
         return getFWHM(None, hdul=self.HDU)
 
+    @property
+    def pipeline_RVerror(self):
+        """ 
+        The RV error as derived by the pipeline and stored in CCF fits file
+        """
+        if not hasattr(self, 'HDU'):
+            raise ValueError('Cannot access header (no HDU attribute)')
+
+        return getRVerror(None, hdul=self.HDU)
+
     def check(self, verbose=False):
         """ Check if calculated RV and FWHM match the pipeline values """
-        val1, val2 = self.RV, self.pipeline_RV
-        if verbose:
-            print('comparing RV calculated/pipeline')
-        np.testing.assert_almost_equal(val1, val2, self._nEPS, err_msg='')
-
-        val1, val2 = self.FWHM, self.pipeline_FWHM
-        if verbose:
-            print('comparing FWHM calculated/pipeline')
-            no_stack_warning(
-                'As of now, FWHM is only compared to 2 decimal places')
-        np.testing.assert_almost_equal(val1, val2, 2, err_msg='')
+        try:
+            val1, val2 = self.RV, self.pipeline_RV
+            if verbose:
+                print('comparing RV calculated/pipeline:', end=' ')
+                print(f'{val1:.{self._nEPS}f} / {val2:.{self._nEPS}f}')
+            np.testing.assert_almost_equal(val1, val2, self._nEPS, err_msg='')
+        except ValueError as e:
+            no_stack_warning(str(e))
+
+        try:
+            val1, val2 = self.RVerror, self.pipeline_RVerror
+            if verbose:
+                print('comparing RVerror calculated/pipeline:', end=' ')
+                print(f'{val1:.{self._nEPS}f} / {val2:.{self._nEPS}f}')
+            np.testing.assert_almost_equal(val1, val2, self._nEPS, err_msg='')
+        except ValueError as e:
+            no_stack_warning(str(e))
+
+        try:
+            val1, val2 = self.FWHM, self.pipeline_FWHM
+            if verbose:
+                print('comparing FWHM calculated/pipeline:', end=' ')
+                print(f'{val1:.{2}f} / {val2:.{2}f}')
+                no_stack_warning(
+                    'As of now, FWHM is only compared to 2 decimal places')
+            np.testing.assert_almost_equal(val1, val2, 2, err_msg='')
+        except ValueError as e:
+            no_stack_warning(str(e))
 
         return True  # all checks passed!
 
     def to_dict(self):
         return writers.to_dict(self)
 
     def to_rdb(self, filename='stdout', clobber=False):
         return writers.to_rdb(self, filename, clobber)
 
-    def plot(self, show_fit=True, show_bisector=False):
+    def plot(self, ax=None, show_fit=True, show_bisector=False):
         """ Plot the CCF, together with the Gaussian fit and the bisector """
-        fig, ax = plt.subplots(constrained_layout=True)
+        if ax is None:
+            _, ax = plt.subplots(constrained_layout=True)
 
-        ax.plot(self.rv, self.ccf, 's-', ms=3)
+        ax.plot(self.rv, self.ccf, 's-', ms=3, label='observed CCF')
 
         if show_fit:
             vv = np.linspace(self.rv.min(), self.rv.max(), 1000)
             pfit = gaussfit(self.rv, self.ccf)
             ax.plot(vv, gauss(vv, pfit), 'k', label='Gaussian fit')
 
         if show_bisector:
@@ -288,17 +366,37 @@
             #    (bottom_limit1, bottom_limit2), (top_limit1, top_limit2), \
             #    fl1, fl2, bisf
             bisf = out[-1]
             top_limit = out[-4][1]
             bot_limit = out[-5][0]
             yy = np.linspace(bot_limit, top_limit, 100)
             ax.plot(bisf(yy), yy, 'k')
+
+        ax.legend()
         ax.set(xlabel='RV [km/s]', ylabel='CCF')
         plt.show()
 
+    def plot_individual_RV(self, ax=None):
+        """ Plot the RV for individual orders """
+        if ax is None:
+            _, ax = plt.subplots(constrained_layout=True)
+
+        n = self.individual_RV.size
+        orders = np.arange(1, n + 1)
+        ax.errorbar(orders, self.individual_RV,
+                    self.individual_RVerror, fmt='o', label='individual RV')
+        ax.axhline(self.RV, color='darkgreen', ls='--', label='final RV')
+
+        m = np.full_like(orders, self.RV, dtype=np.float)
+        e = np.full_like(orders, self.RVerror, dtype=np.float)
+        ax.fill_between(orders, m-e, m+e, color='g', alpha=0.3)
+
+        ax.legend()
+        ax.set(xlabel='spectral order', ylabel='RV', xlim=(-5, n+5))
+
 
 def indicators_from_files(files, rdb_format=True, show=True, show_bjd=True,
                           sort_bjd=True, **kwargs):
 
     if sort_bjd:
         files = sorted(files, key=getBJD)
 
@@ -316,11 +414,11 @@
             else:
                 if show_bjd:
                     print(['jdb'] + I.on_indicators)
                 else:
                     print(I.on_indicators)
 
         if rdb_format:
-            print(
-                '\t'.join([f'{bjd:<.6f}'] + [f'{ind:<.5f}' for ind in I.all]))
+            print('\t'.join([f'{bjd:<.6f}'] + [f'{ind:<.5f}'
+                                               for ind in I.all]))
         else:
             print((bjd, ) + I.all)
```

### Comparing `iCCF-0.3.7/iCCF/bisector.py` & `iCCF-0.3.8/iCCF/bisector.py`

 * *Files identical despite different names*

### Comparing `iCCF-0.3.7/iCCF/writers.py` & `iCCF-0.3.8/iCCF/writers.py`

 * *Files identical despite different names*

### Comparing `iCCF-0.3.7/iCCF/gaussian.py` & `iCCF-0.3.8/iCCF/gaussian.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 import numpy as np 
 from numpy import exp, log, sqrt, inf
 from scipy import optimize
 
 from .utils import numerical_gradient
 
 def gauss(x, p):
@@ -18,25 +19,35 @@
     dgdsig = g * ((x-x0)**2/sig**3)
     dgdoffset = np.ones_like(x)
     return np.c_[dgdA, dgdx0, dgdsig, dgdoffset]
 
 
 def _gauss_initial_guess(x, y):
     """ Educated guess (from the data) for Gaussian parameters. """
+    # these guesses tend to work better for narrow-ish gaussians
     p0 = []
-    p0.append(y.mean() - y.max())  # guess the amplitude
+    # guess the amplitude
+    p0.append(y.ptp())
     # guess the center, but maybe the CCF is upside down?
-    if y[x.size // 2] > y[0]:  # seems like it
+    m = y.mean()
+    ups_down = np.sign(np.percentile(y, 50) - m) != np.sign(y.max() - m)
+    if ups_down:  # seems like it
+        # warnings.warn('It seems the CCF might be upside-down?')
         p0.append(x[y.argmax()])
     else:
+        p0[0] *= -1
         p0.append(x[y.argmin()])
-    p0.append(1)  # guess the sigma
-    p0.append(y.mean())  # guess the offset 
+    # guess the width
+    p0.append(np.percentile(x, 68))
+    # guess the offset
+    p0.append(0.5 * (y[0] + y[-1]))
+
     return p0
 
+
 def gaussfit(x, y, p0=None, return_errors=False, use_deriv=True):
     """ 
     Fit a Gaussian function to `x`,`y` using least-squares, with initial guess
     `p0` = [A, x0, σ, offset]. If p0 is not provided, the function tries an
     educated guess, which might lead to bad results.
 
     Parameters
@@ -52,15 +63,14 @@
     use_deriv : bool
         Whether to use partial derivatives of the Gaussian (wrt the parameters)
         as Jacobian in the fit. If False, the Jacobian will be estimated.
     """
     if (y == 0).all():
         return np.nan * np.ones(4)
 
-    # f = lambda x, A, x0, sig, offset: gauss(x, [A, x0, sig, offset])
     f = lambda p, x, y: gauss(x, p) - y
     if use_deriv:
         df = lambda p, x, y: _gauss_partial_deriv(x, p)
     else:
         df = None
     
     if p0 is None:
@@ -88,26 +98,28 @@
 
 
 def fwhm2sig(fwhm):
     """ Convert full width at half maximum to standard deviation. """
     return fwhm / (2 * sqrt(2 * log(2)))
 
 
-def RV(rv, ccf):
+def RV(rv, ccf, **kwargs):
     """
     Calculate the radial velocity as the center of a Gaussian fit the CCF.
     
     Parameters
     ----------
     rv : array
         The velocity values where the CCF is defined.
     ccf : array
         The values of the CCF profile.
+    kwargs : dict
+        Keyword arguments passed directly to gaussfit
     """
-    _, rv, _, _ = gaussfit(rv, ccf)
+    _, rv, _, _ = gaussfit(rv, ccf, **kwargs)
     return rv
 
 
 def RVerror(rv, ccf, eccf):
     """
     Calculate the uncertainty on the radial velocity, following the same steps
     as the ESPRESSO DRS pipeline.
```

### Comparing `iCCF-0.3.7/iCCF/chromatic.py` & `iCCF-0.3.8/iCCF/chromatic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import bisect
 import warnings
-from pkg_resources import resource_stream
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 from astropy.io import fits
 from cached_property import cached_property
 
@@ -13,19 +12,19 @@
 from .gaussian import gaussfit, RV, RVerror
 from .keywords import getRV, getRVarray
 from .utils import find_myself
 # from .utils import get_orders_mean_wavelength
 
 
 def read_spectral_format():
-
-    sf_red_stream = resource_stream(__name__, 'data/spectral_format_red.dat')
-    red = np.loadtxt(sf_red_stream)
-    sf_blue_stream = resource_stream(__name__, 'data/spectral_format_blue.dat')
-    blue = np.loadtxt(sf_blue_stream)
+    here = os.path.dirname(__file__)
+    sf_red_file = os.path.join(here, '..', 'data', 'spectral_format_red.dat')
+    red = np.loadtxt(sf_red_file)
+    sf_blue_file = os.path.join(here, '..', 'data', 'spectral_format_blue.dat')
+    blue = np.loadtxt(sf_blue_file)
 
     col_start_wave = 7
     col_end_wave = 8
 
     order_wave_range = {}
 
     for i, order in enumerate(blue[::-1]):
@@ -68,20 +67,22 @@
         self._redRVerror = None
 
         self.n = len(indicators)
         if self.n == 1:
             indicators = [indicators, ]
         self.I = self.indicators = indicators
         # store all but the last CCF for each of the Indicators instances
-        self.ccfs = [i.HDU[1].data[:-1] for i in self.I]
+        self.ccfs = [i.HDU[i._hdu_number].data[:-1] for i in self.I]
         # try storing the CCF uncertainties as well
-        try:
-            self.eccfs = [i.HDU[2].data[:-1] for i in self.I]
-        except IndexError:
-            self.eccfs = self.n * [None]
+        self.eccfs = []
+        for i in self.I:
+            try:
+                self.eccfs.append(i.HDU[2].data[:-1])
+            except IndexError:
+                self.eccfs.append(None)
 
 
     def __repr__(self):
         bands = ', '.join(map(repr, self.bands))
         nb = len(self.bands)
         return f'chromaticRV({self.n} CCFs; {nb} bands: {bands} nm)'
 
@@ -182,21 +183,23 @@
             ccf = full_ccf[orders].sum(axis=0)
             rv.append(RV(i.rv, ccf))
 
             if full_eccf is not None:
                 eccf = np.sqrt(np.square(full_eccf[orders]).sum(axis=0))
                 rve.append(RVerror(i.rv, ccf, eccf))
                 has_errors = True
+            else:
+                rve.append(np.nan)
 
-        if not has_errors:
-            warnings.warn(
-                'Cannot access CCF uncertainties to calculate RV error')
-            return np.array(rv), None
-        else:
-            return np.array(rv), np.array(rve)
+        # if not has_errors:
+        #     warnings.warn(
+        #         'Cannot access CCF uncertainties to calculate RV error')
+        #     return np.array(rv), None
+        # else:
+        return np.array(rv), np.array(rve)
 
 
     @property
     def bands(self):
         """ Wavelength limits of blue, mid, and red bands """
         b = self.blue_wave_limits, self.mid_wave_limits, self.red_wave_limits
         return b
@@ -223,42 +226,94 @@
         if self._redRV is None:
             self._redRV, self._redRVerror = self.get_rv(self.red_orders)
         return self._redRV
 
     @property
     def fullRV(self):
         return np.fromiter((i.RV for i in self.I), np.float, self.n)
-    
+
     @property
     def fullRVerror(self):
         return np.fromiter((i.RVerror for i in self.I), np.float, self.n)
 
-    def plot(self):
-        _, axs = plt.subplots(3+1, 1, sharex=True, sharey=False)
+    def plot(self, periodogram=False):
+        ncols = 2 if periodogram else 1
 
-        axs[0].errorbar(self.time, self.fullRV, self.fullRVerror, fmt='o')
+        fig, axs = plt.subplots(3 + 1, ncols,) #sharex=False, sharey=False,
+        # constrained_layout=True)
 
-        axs[1].errorbar(self.time, self.blueRV, self._blueRVerror, fmt='o')
-        axs[2].errorbar(self.time, self.midRV, self._midRVerror, fmt='o')
-        axs[3].errorbar(self.time, self.redRV, self._redRVerror, fmt='o')
+        axs = axs.ravel()
 
-        plt.show()
-        
+        if periodogram:
+            indices_plots = np.arange(0, 8, 2)
+        else:
+            indices_plots = np.arange(0, 4)
 
-    def plot_ccfs(self, orders=None):
+        kw = dict(fmt='o', ms=3)
+
+        axs[indices_plots[0]].errorbar(self.time,
+                                       self.fullRV - self.fullRV.mean(),
+                                       self.fullRVerror, color='k', **kw)
+
+        axs[indices_plots[1]].errorbar(self.time,
+                                       self.blueRV - self.blueRV.mean(),
+                                       self._blueRVerror, color='b', **kw)
+        axs[indices_plots[2]].errorbar(self.time,
+                                       self.midRV - self.midRV.mean(),
+                                       self._midRVerror, color='g', **kw)
+        axs[indices_plots[3]].errorbar(self.time,
+                                       self.redRV - self.redRV.mean(),
+                                       self._redRVerror, color='r', **kw)
+
+        if periodogram:
+            from astropy.timeseries import LombScargle
+
+            model = LombScargle(self.time, self.fullRV, self.fullRVerror)
+            f, p = model.autopower()
+            axs[1].semilogx(1 / f, p, color='k')
+            axs[1].hlines(model.false_alarm_level([0.1, 0.01]),
+                          *axs[1].get_xlim(), alpha=0.2, ls='--')
+
+            model = LombScargle(self.time, self.blueRV, self._blueRVerror)
+            f, p = model.autopower()
+            axs[3].semilogx(1 / f, p, color='b')
+            axs[3].hlines(model.false_alarm_level([0.1, 0.01]),
+                          *axs[3].get_xlim(), alpha=0.2, ls='--')
+
+            model = LombScargle(self.time, self.midRV, self._midRVerror)
+            f, p = model.autopower()
+            axs[5].semilogx(1 / f, p, color='g')
+            axs[5].hlines(model.false_alarm_level([0.1, 0.01]),
+                          *axs[5].get_xlim(), alpha=0.2, ls='--')
+
+            model = LombScargle(self.time, self.redRV, self._redRVerror)
+            f, p = model.autopower()
+            axs[7].semilogx(1 / f, p, color='r')
+            axs[7].hlines(model.false_alarm_level([0.1, 0.01]),
+                          *axs[7].get_xlim(), alpha=0.2, ls='--')
+
+        return fig, axs
+
+
+    def plot_ccfs(self, orders=None, show_filenames=False):
         if orders is None:
             orders = slice(None, None)
         elif isinstance(orders, int):
             orders = slice(orders, orders + 1)
         elif isinstance(orders, tuple):
             orders = slice(*orders)
 
+        fig, ax = plt.subplots(1, 1)  #, constrained_layout=True)
         for i in self.I:
-            fig, ax = plt.subplots(1, 1, constrained_layout=True)
-            ax.plot(i.ccf[orders].T)
+            line = ax.plot(i.rv, i.ccf[orders].T)
+            if show_filenames:
+                color = line[0].get_color()
+                ax.text(i.rv[0], i.ccf[0], i.filename, fontsize=8, color=color)
+        
+        ax.set(xlabel='RV', ylabel='CCF')
 
 
 
 
 def each_order_rv(rv, ccfs, exclude_last=True):
     """
     Calculate RVs for each spectral order by fitting Gaussians to individual CCFs
```

### Comparing `iCCF-0.3.7/iCCF/utils.py` & `iCCF-0.3.8/iCCF/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import os
 import re
 import warnings
 from copy import copy
 import numpy as np
+from astropy.io import fits
+
+from .ssh_files import ssh_fits_open
 
 _c = 299792.458
 
+
 def no_stack_warning(message):
     old_show = copy(warnings.showwarning)
     def new_show(message, category, filename, lineno, file, line):
         print(category.__name__ + ':', message)
     warnings.showwarning = new_show
     warnings.warn(message)
     warnings.showwarning = old_show
@@ -82,7 +86,18 @@
 
 
 def load_example_data():
     """ Load the example CCF stored in iCCF/example_data """
     from pkg_resources import resource_stream
     data = np.load(resource_stream(__name__, 'example_data/CCF1.npy'))
     return data
+
+
+def _get_hdul(fitsfile, **kwargs):
+    """ Dispatch opening of fits files to fits.open in normal cases, or to
+    `ssh_fits_open` for filenames starting with "ssh:"
+    """
+    if fitsfile.startswith('ssh:'):
+        hdul = ssh_fits_open(fitsfile[4:], **kwargs)
+    else:
+        hdul = fits.open(fitsfile)
+    return hdul
```

### Comparing `iCCF-0.3.7/iCCF/config.py` & `iCCF-0.3.8/iCCF/config.py`

 * *Files identical despite different names*

### Comparing `iCCF-0.3.7/iCCF/meta_ESPRESSO.py` & `iCCF-0.3.8/iCCF/meta_ESPRESSO.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,80 +130,94 @@
     return rvarray, ccfarray
 
 
 def espdr_compute_CCF_fast(ll, dll, flux, error, blaze, quality, RV_table,
                            mask, berv, bervmax, mask_width=0.5):
     c = 299792.458
 
-    # nx_s2d = len(flux)
-    n_mask = mask['lambda'].size #len(mask)
-    # n_mask = len(mask)
+    nx_s2d = flux.size
+    # ny_s2d = 1  #! since this function computes only one order
+    n_mask = mask.size
     nx_ccf = len(RV_table)
 
     ccf_flux = np.zeros_like(RV_table)
     ccf_error = np.zeros_like(RV_table)
     ccf_quality = np.zeros_like(RV_table)
 
     dll2 = dll / 2.0  # cpl_image_divide_scalar_create(dll,2.);
     ll2 = ll - dll2  # cpl_image_subtract_create(ll,dll2);
 
-    imin = np.where(quality == 0)[0][0]
-    imax = len(quality) - np.where(quality[::-1] == 0)[0][0] - 1
+    #? this mimics the pipeline (note that cpl_image_get indexes starting at 1)
+    imin = 1; imax = nx_s2d
+    while(imin < nx_s2d and quality[imin-1] != 0): imin += 1
+    while(imax > 1 and quality[imax-1] != 0): imax -= 1
+    # my tests to speed things up
+    # imin = np.where(quality == 0)[0][0]
+    # imax = len(quality) - np.where(quality[::-1] == 0)[0][0] - 1
     # print(imin, imax)
 
     if imin >= imax:
         return
-
-    llmin = ll[imin + 1] / (1. + berv / c) * (1. + bervmax / c) / (1. + RV_table[0] / c)
-    llmax = ll[imax - 1] / (1. + berv / c) * (1. - bervmax / c) / (1. + RV_table[nx_ccf - 1] / c)
-    # print(llmin, llmax)
-
-    imin = 0
-    imax = n_mask - 1
-
-    while (imin < n_mask
-           and mask['lambda'][imin] < (llmin + 0.5 * mask_width / c * llmin)):
-        imin += 1
-    while (imax >= 0
-           and mask['lambda'][imax] > (llmax - 0.5 * mask_width / c * llmax)):
-        imax -= 1
+    #? note that cpl_image_get indexes starting at 1, hence the "-1"s
+    llmin = ll[imin + 1 - 1] / (1. + berv / c) * (1. + bervmax / c) / (1. + RV_table[0] / c)
+    llmax = ll[imax - 1 - 1] / (1. + berv / c) * (1. - bervmax / c) / (1. + RV_table[nx_ccf - 1] / c)
+
+    imin = 0; imax = n_mask - 1
+
+    #? turns out cpl_table_get indexes stating at 0...
+    while (imin < n_mask and mask['lambda'][imin] < (llmin + 0.5 * mask_width / c * llmin)): imin += 1
+    while (imax >= 0     and mask['lambda'][imax] > (llmax - 0.5 * mask_width / c * llmax)): imax -= 1
     # print(imin, imax)
 
+    # for (i = imin; i <= imax; i++)
     for i in range(imin, imax + 1):
+        #? cpl_array_get also indexes starting at 0
         llcenter = mask['lambda'][i] * (1. + RV_table[nx_ccf // 2] / c)
 
-        index_center = np.where(ll < llcenter)[0][-1] + 1
+        # index_center = 1
+        # while(ll[index_center-1] < llcenter): index_center += 1
+        # my attempt to speed it up
+        index_center = np.where(ll < llcenter)[0][-1] +1
 
         contrast = mask['contrast'][i]
         w = contrast * contrast
+        # print(i, w)
 
         for j in range(0, nx_ccf):
             llcenter = mask['lambda'][i] * (1. + RV_table[j] / c)
             llstart = llcenter - 0.5 * mask_width / c * llcenter
             llstop = llcenter + 0.5 * mask_width / c * llcenter
-
-            index1 = np.where(ll2 < llstart)[0][-1] + 1
+            
+            # print(llstart, llcenter, llstop)
+            # index1 = 1
+            # while(ll2[index1-1] < llstart): index1 += 1
+            index1 = np.where(ll2 < llstart)[0][-1] +1
+            
             # index2 = index1
-
-            index2 = np.where(ll2 < llcenter)[0][-1] + 1
+            # while (ll2[index2-1] < llcenter): index2 += 1
+            index2 = np.where(ll2 < llcenter)[0][-1] +1
+            
             # index3 = index2
-
-            index3 = np.where(ll2 < llstop)[0][-1] + 1
+            # while (ll2[index3-1] < llstop): index3 += 1;
+            index3 = np.where(ll2 < llstop)[0][-1] +1
+            
+            # print(index1, index2, index3)
+            # sys.exit(0)
 
             k = j
 
             for index in range(index1, index3):
-                ccf_flux[k] += w * flux[index] / blaze[index] * blaze[index_center]
+                ccf_flux[k] += w * flux[index-1] / blaze[index-1] * blaze[index_center-1]
 
-            ccf_flux[k] += w * flux[index1 - 1] * (ll2[index1] - llstart) / dll[index1 - 1] / blaze[index1 - 1] * blaze[index_center]
-            ccf_flux[k] -= w * flux[index3 - 1] * (ll2[index3] - llstop) / dll[index3 - 1] / blaze[index3 - 1] * blaze[index_center]
+            ccf_flux[k] += w * flux[index1 - 1 - 1] * (ll2[index1-1] - llstart) / dll[index1 - 1 - 1] / blaze[index1 - 1 - 1] * blaze[index_center - 1]
+            ccf_flux[k] -= w * flux[index3 - 1 - 1] * (ll2[index3-1] - llstop) / dll[index3 - 1 - 1] / blaze[index3 - 1 - 1] * blaze[index_center - 1]
 
-            ccf_error[k] += w * w * error[index2 - 1] * error[index2 - 1]
+            ccf_error[k] += w * w * error[index2 - 1 - 1] * error[index2 - 1 - 1]
 
-            ccf_quality[k] += quality[index2 - 1]
+            ccf_quality[k] += quality[index2 - 1 - 1]
 
     # my_error = cpl_image_power(*CCF_error_RE,0.5);
     ccf_error = np.sqrt(ccf_error)
 
     return ccf_flux, ccf_error, ccf_quality
 
 
@@ -215,19 +229,23 @@
     elif len(glob(dllfile + '*')) > 1:
         return glob(dllfile + '*')[0]
     else:
         date = hdu[0].header['DATE-OBS']
 
 
 def calculate_s2d_ccf(s2dfile, rvarray, order='all',
-                      maskfile='ESPRESSO_G2.fits', mask=None, mask_width=0.5):
+                      maskfile='ESPRESSO_G2.fits', mask=None, mask_width=0.5,
+                      debug=False):
 
     hdu = fits.open(s2dfile)
 
     if order == 'all':
+        if debug:
+            print('can only debug one order at a time...')
+            return
         orders = range(hdu[1].data.shape[0])
         return_sum = True
     else:
         assert isinstance(order, int), 'order should be integer'
         orders = (order, )
         return_sum = False
 
@@ -275,14 +293,17 @@
 
         blaze = fits.open(blazefile)[1].data[order, :]
 
         y = flux * blaze / corr_model[order]
         # y = np.loadtxt('flux_in_pipeline_order0.txt')
         ye = error * blaze / corr_model[order]
 
+        if debug:
+            return ll, dll, y, ye, blaze, quality, rvarray, mask, BERV, BERVMAX
+
         print('calculating ccf (order %d)...' % order)
         ccf, ccfe, _ = espdr_compute_CCF_fast(ll, dll, y, ye, blaze, quality,
                                               rvarray, mask, BERV, BERVMAX,
                                               mask_width=mask_width)
         ccfs.append(ccf)
         ccfes.append(ccfe)
 
@@ -307,15 +328,15 @@
         found = found.decode().split()
         print('\tfound file:', found[-1])
         return found[-1]
     except:
         raise FileNotFoundError(file)
 
 
-def dowork(args):
+def dowork(args, debug=False):
     order, kwargs = args
     data = kwargs['data']
     dllfile = kwargs['dllfile']
     blazefile = kwargs['blazefile']
     flux_corr = kwargs['flux_corr']
     rvarray = kwargs['rvarray']
     mask = kwargs['mask']
@@ -353,14 +374,15 @@
 def calculate_s2d_ccf_parallel(s2dfile, rvarray, order='all',
                                maskfile='ESPRESSO_G2.fits', mask_width=0.5,
                                ncores=None, verbose=True, full_output=False):
     hdu = fits.open(s2dfile)
 
     if ncores is None:
         ncores = get_ncores()
+    print(f'Using {ncores} CPU cores for the calculation')
 
     if order == 'all':
         orders = range(hdu[1].data.shape[0])
         return_sum = True
     else:
         assert isinstance(order, int), 'order should be integer'
         orders = (order, )
@@ -390,23 +412,27 @@
     kwargs['rvarray'] = rvarray
     kwargs['mask'] = mask
     kwargs['BERV'] = BERV
     kwargs['BERVMAX'] = BERVMAX
     kwargs['mask_width'] = mask_width
     # kwargs['verbose'] = verbose
 
-    # return kwargs
     # print(list(product(orders, [kwargs,])))
     # return
 
     pool = multiprocessing.Pool(ncores)
     if verbose:
-        ccfs, ccfes = zip(*tqdm.tqdm(pool.imap_unordered(dowork, product(orders, [kwargs,])), total=len(orders)))
+        ccfs, ccfes = zip(*tqdm.tqdm(
+            pool.imap_unordered(dowork, product(orders, [
+                kwargs,
+            ])), total=len(orders)))
     else:
-        ccfs, ccfes = zip(*pool.map(dowork, product(orders, [kwargs,])))
+        ccfs, ccfes = zip(*pool.map(dowork, product(orders, [
+            kwargs,
+        ])))
     pool.close()
 
     if return_sum:
         ccf = np.concatenate([ccfs, np.array(ccfs).sum(axis=0, keepdims=True)])
         ccfe = np.concatenate([ccfes, np.zeros(len(rvarray)).reshape(1, -1)])
         # what to do with the errors?
         if full_output:
@@ -424,14 +450,18 @@
     mask = kwargs.pop('mask')
     maskfile = f"ESPRESSO_{mask}.fits"
     kwargs['maskfile'] = maskfile
 
     ccf, ccfe, kw = calculate_s2d_ccf_parallel(s2dfile, full_output=True,
                                                **kwargs)
 
+    # in the pipeline, data are saved as floats
+    ccf = ccf.astype(np.float32)
+    ccfe = ccfe.astype(np.float32)
+
     # read original S2D file
     s2dhdu = fits.open(s2dfile)
 
 
     s2dfile = os.path.basename(s2dfile)
     ccf_file = s2dfile[:s2dfile.index('_')] + f'_CCF_{mask}_iCCF.fits'
     rvarray = kwargs['rvarray']
```

### Comparing `iCCF-0.3.7/iCCF/wspan.py` & `iCCF-0.3.8/iCCF/wspan.py`

 * *Files identical despite different names*

### Comparing `iCCF-0.3.7/iCCF/meta.py` & `iCCF-0.3.8/iCCF/meta.py`

 * *Files identical despite different names*

### Comparing `iCCF-0.3.7/iCCF/scripts.py` & `iCCF-0.3.8/iCCF/scripts.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 import os
 import sys
 import argparse
+import re
 
 from . import iCCF
 from . import meta_ESPRESSO
 from .utils import get_ncores
 # from .meta_ESPRESSO import calculate_ccf as calculate_ccf_ESPRESSO
 from astropy.io import fits
 
@@ -62,21 +63,21 @@
 def _parse_args_make_CCF():
     desc = """
     This script takes a list of S2D fits files and calculates the CCF for a 
     given RV array and a given mask. If no mask is provided, it uses the same as
     specified in the S2D file.
     """
     parser = argparse.ArgumentParser(description=desc, prog='iccf-make-ccf')
-    
+
     parser.add_argument('-m', '--mask', type=str,
                         help='Mask (G2, G9, K6, M2, ...)')
-    
+
     parser.add_argument('-rv', type=str,
                         help='RV array, in the form start:end:step [km/s]')
-    
+
     default_ncores = get_ncores()
     help_ncores = 'Number of cores to distribute calculation; '\
                   f'default is all available ({default_ncores})'
     parser.add_argument('--ncores', type=int, help=help_ncores)
 
     args = parser.parse_args()
     return args, parser
@@ -111,15 +112,25 @@
                     sys.exit(1)
             else:
                 start, end, step = map(float, args.rv.split(':'))
                 rvarray = np.arange(start, end + step, step)
 
             mask = args.mask
             if mask is None:
-                mask = header['HIERARCH ESO QC CCF MASK']
+                try:
+                    mask = header['HIERARCH ESO QC CCF MASK']
+                except KeyError:
+                    try:
+                        mask = header['HIERARCH ESO PRO REC1 CAL25 NAME']
+                        if 'ESPRESSO_' in mask:
+                            mask = mask[9:11]
+                    except KeyError:
+                        print('Could not find CCF mask in S2D file.',
+                              'Please use the -m argument.')
+                        sys.exit(1)
                 print('using mask from S2D file:', mask)
 
             inst = header['INSTRUME']
 
             if inst == 'ESPRESSO':
                 meta_ESPRESSO.calculate_ccf(file, mask=mask, rvarray=rvarray,
                                             ncores=args.ncores)
```

### Comparing `iCCF-0.3.7/iCCF/ssh_files.py` & `iCCF-0.3.8/iCCF/ssh_files.py`

 * *Files identical despite different names*

### Comparing `iCCF-0.3.7/iCCF/vspan.py` & `iCCF-0.3.8/iCCF/vspan.py`

 * *Files identical despite different names*

### Comparing `iCCF-0.3.7/README.md` & `iCCF-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `iCCF-0.3.7/setup.py` & `iCCF-0.3.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 # Get the version from iCCF/version.py
 version = {}
 with open("iCCF/version.py") as fp:
     exec(fp.read(), version)
     __version__ = version['__version__']
 
-
 setup(
     name='iCCF',
     version=__version__,
     description='Analysis of CCF profiles and activity indicators',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/j-faria/iCCF',
@@ -33,15 +32,15 @@
     entry_points={
         'console_scripts': [
             'iccf-fits-to-rdb = iCCF.scripts:fits_to_rdb',
             'iccf-make-ccf = iCCF.scripts:make_CCF',
         ]
     },
     packages=find_packages(),
-    package_data={
-        '': ['example_data/*.npy', 'data/*'],
-    },
+    package_data={'': ['example_data/*.npy']},
     include_package_data=True,
     zip_safe=False,
-    install_requires=['numpy', 'scipy', 'matplotlib',
-                      'astropy', 'cached_property', 'paramiko'],
+    install_requires=[
+        'numpy', 'scipy', 'matplotlib', 'astropy', 'cached_property',
+        'paramiko'
+    ],
 )
```

