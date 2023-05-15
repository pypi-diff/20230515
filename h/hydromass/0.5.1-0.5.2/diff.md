# Comparing `tmp/hydromass-0.5.1.tar.gz` & `tmp/hydromass-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydromass-0.5.1.tar", last modified: Tue May  9 09:07:05 2023, max compression
+gzip compressed data, was "hydromass-0.5.2.tar", last modified: Mon May 15 13:16:42 2023, max compression
```

## Comparing `hydromass-0.5.1.tar` & `hydromass-0.5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-09 09:07:05.677058 hydromass-0.5.1/
--rwxr-xr-x   0 deckert    (501) staff       (20)       24 2023-02-08 13:10:51.000000 hydromass-0.5.1/MANIFEST.in
--rw-r--r--   0 deckert    (501) staff       (20)      242 2023-05-09 09:07:05.676886 hydromass-0.5.1/PKG-INFO
--rwxr-xr-x   0 deckert    (501) staff       (20)     1590 2023-02-08 13:10:51.000000 hydromass-0.5.1/README.md
-drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-09 09:07:05.674429 hydromass-0.5.1/hydromass/
--rwxr-xr-x   0 deckert    (501) staff       (20)      316 2023-02-08 13:10:51.000000 hydromass-0.5.1/hydromass/__init__.py
--rwxr-xr-x   0 deckert    (501) staff       (20)      306 2023-05-04 12:45:19.000000 hydromass-0.5.1/hydromass/constants.py
--rw-r--r--   0 deckert    (501) staff       (20)    10052 2023-02-08 13:10:51.000000 hydromass-0.5.1/hydromass/contour.py
-drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-09 09:07:05.676625 hydromass-0.5.1/hydromass/data/
--rwxr-xr-x   0 deckert    (501) staff       (20)    95040 2023-02-08 13:10:51.000000 hydromass-0.5.1/hydromass/data/coolfunc_table.fits
--rwxr-xr-x   0 deckert    (501) staff       (20)      229 2023-02-08 13:10:51.000000 hydromass-0.5.1/hydromass/data/pnt_covmat.dat
--rwxr-xr-x   0 deckert    (501) staff       (20)       75 2023-02-08 13:10:51.000000 hydromass-0.5.1/hydromass/data/pnt_mean.dat
--rwxr-xr-x   0 deckert    (501) staff       (20)    26380 2023-02-08 13:10:51.000000 hydromass-0.5.1/hydromass/delta.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    15073 2023-02-08 13:10:51.000000 hydromass-0.5.1/hydromass/deproject.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    12085 2023-05-04 13:22:24.000000 hydromass-0.5.1/hydromass/emissivity.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    29819 2023-05-09 09:05:56.000000 hydromass-0.5.1/hydromass/forward.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    25184 2023-02-08 13:10:51.000000 hydromass-0.5.1/hydromass/functions.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    48893 2023-05-09 08:59:48.000000 hydromass-0.5.1/hydromass/mhyd.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    42623 2023-05-09 09:04:27.000000 hydromass-0.5.1/hydromass/nonparametric.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    28645 2023-05-09 09:04:10.000000 hydromass-0.5.1/hydromass/plots.py
--rwxr-xr-x   0 deckert    (501) staff       (20)     2777 2023-02-08 13:10:51.000000 hydromass-0.5.1/hydromass/pnt.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    36097 2023-05-09 09:04:55.000000 hydromass-0.5.1/hydromass/polytropic.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    25837 2023-05-04 13:46:01.000000 hydromass-0.5.1/hydromass/save.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    24071 2023-05-04 12:45:19.000000 hydromass-0.5.1/hydromass/tpdata.py
--rw-r--r--   0 deckert    (501) staff       (20)     3903 2023-05-04 12:56:59.000000 hydromass-0.5.1/hydromass/wl.py
-drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-09 09:07:05.675719 hydromass-0.5.1/hydromass.egg-info/
--rw-r--r--   0 deckert    (501) staff       (20)      242 2023-05-09 09:07:05.000000 hydromass-0.5.1/hydromass.egg-info/PKG-INFO
--rw-r--r--   0 deckert    (501) staff       (20)      622 2023-05-09 09:07:05.000000 hydromass-0.5.1/hydromass.egg-info/SOURCES.txt
--rw-r--r--   0 deckert    (501) staff       (20)        1 2023-05-09 09:07:05.000000 hydromass-0.5.1/hydromass.egg-info/dependency_links.txt
--rw-r--r--   0 deckert    (501) staff       (20)       68 2023-05-09 09:07:05.000000 hydromass-0.5.1/hydromass.egg-info/requires.txt
--rw-r--r--   0 deckert    (501) staff       (20)       10 2023-05-09 09:07:05.000000 hydromass-0.5.1/hydromass.egg-info/top_level.txt
--rw-r--r--   0 deckert    (501) staff       (20)       38 2023-05-09 09:07:05.677105 hydromass-0.5.1/setup.cfg
--rwxr-xr-x   0 deckert    (501) staff       (20)      546 2023-05-09 09:06:53.000000 hydromass-0.5.1/setup.py
+drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-15 13:16:42.960866 hydromass-0.5.2/
+-rwxr-xr-x   0 deckert    (501) staff       (20)       24 2023-02-08 13:10:51.000000 hydromass-0.5.2/MANIFEST.in
+-rw-r--r--   0 deckert    (501) staff       (20)      242 2023-05-15 13:16:42.960699 hydromass-0.5.2/PKG-INFO
+-rwxr-xr-x   0 deckert    (501) staff       (20)     1590 2023-02-08 13:10:51.000000 hydromass-0.5.2/README.md
+drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-15 13:16:42.958796 hydromass-0.5.2/hydromass/
+-rwxr-xr-x   0 deckert    (501) staff       (20)      316 2023-02-08 13:10:51.000000 hydromass-0.5.2/hydromass/__init__.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)      306 2023-05-04 12:45:19.000000 hydromass-0.5.2/hydromass/constants.py
+-rw-r--r--   0 deckert    (501) staff       (20)    10052 2023-02-08 13:10:51.000000 hydromass-0.5.2/hydromass/contour.py
+drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-15 13:16:42.960469 hydromass-0.5.2/hydromass/data/
+-rwxr-xr-x   0 deckert    (501) staff       (20)    95040 2023-02-08 13:10:51.000000 hydromass-0.5.2/hydromass/data/coolfunc_table.fits
+-rwxr-xr-x   0 deckert    (501) staff       (20)      229 2023-02-08 13:10:51.000000 hydromass-0.5.2/hydromass/data/pnt_covmat.dat
+-rwxr-xr-x   0 deckert    (501) staff       (20)       75 2023-02-08 13:10:51.000000 hydromass-0.5.2/hydromass/data/pnt_mean.dat
+-rwxr-xr-x   0 deckert    (501) staff       (20)    26380 2023-02-08 13:10:51.000000 hydromass-0.5.2/hydromass/delta.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    15073 2023-02-08 13:10:51.000000 hydromass-0.5.2/hydromass/deproject.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    13713 2023-05-10 13:12:30.000000 hydromass-0.5.2/hydromass/emissivity.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    29806 2023-05-15 13:08:35.000000 hydromass-0.5.2/hydromass/forward.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    25184 2023-02-08 13:10:51.000000 hydromass-0.5.2/hydromass/functions.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    49807 2023-05-10 13:05:23.000000 hydromass-0.5.2/hydromass/mhyd.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    42623 2023-05-09 09:04:27.000000 hydromass-0.5.2/hydromass/nonparametric.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    28645 2023-05-09 09:04:10.000000 hydromass-0.5.2/hydromass/plots.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)     2777 2023-02-08 13:10:51.000000 hydromass-0.5.2/hydromass/pnt.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    36097 2023-05-09 09:04:55.000000 hydromass-0.5.2/hydromass/polytropic.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    25837 2023-05-04 13:46:01.000000 hydromass-0.5.2/hydromass/save.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    24071 2023-05-04 12:45:19.000000 hydromass-0.5.2/hydromass/tpdata.py
+-rw-r--r--   0 deckert    (501) staff       (20)     3903 2023-05-04 12:56:59.000000 hydromass-0.5.2/hydromass/wl.py
+drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-15 13:16:42.959549 hydromass-0.5.2/hydromass.egg-info/
+-rw-r--r--   0 deckert    (501) staff       (20)      242 2023-05-15 13:16:42.000000 hydromass-0.5.2/hydromass.egg-info/PKG-INFO
+-rw-r--r--   0 deckert    (501) staff       (20)      622 2023-05-15 13:16:42.000000 hydromass-0.5.2/hydromass.egg-info/SOURCES.txt
+-rw-r--r--   0 deckert    (501) staff       (20)        1 2023-05-15 13:16:42.000000 hydromass-0.5.2/hydromass.egg-info/dependency_links.txt
+-rw-r--r--   0 deckert    (501) staff       (20)       68 2023-05-15 13:16:42.000000 hydromass-0.5.2/hydromass.egg-info/requires.txt
+-rw-r--r--   0 deckert    (501) staff       (20)       10 2023-05-15 13:16:42.000000 hydromass-0.5.2/hydromass.egg-info/top_level.txt
+-rw-r--r--   0 deckert    (501) staff       (20)       38 2023-05-15 13:16:42.960914 hydromass-0.5.2/setup.cfg
+-rwxr-xr-x   0 deckert    (501) staff       (20)      546 2023-05-15 13:09:08.000000 hydromass-0.5.2/setup.py
```

### Comparing `hydromass-0.5.1/README.md` & `hydromass-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hydromass-0.5.1/hydromass/contour.py` & `hydromass-0.5.2/hydromass/contour.py`

 * *Files identical despite different names*

### Comparing `hydromass-0.5.1/hydromass/data/coolfunc_table.fits` & `hydromass-0.5.2/hydromass/data/coolfunc_table.fits`

 * *Files identical despite different names*

### Comparing `hydromass-0.5.1/hydromass/delta.py` & `hydromass-0.5.2/hydromass/delta.py`

 * *Files identical despite different names*

### Comparing `hydromass-0.5.1/hydromass/deproject.py` & `hydromass-0.5.2/hydromass/deproject.py`

 * *Files identical despite different names*

### Comparing `hydromass-0.5.1/hydromass/emissivity.py` & `hydromass-0.5.2/hydromass/emissivity.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """Check whether `name` is on PATH."""
 
     from distutils.spawn import find_executable
 
     return find_executable(name) is not None
 
 
-def calc_emissivity(cosmo, z, nh, kt, rmf, abund='angr', Z=0.3, elow=0.5, ehigh=2.0, arf=None):
+def calc_emissivity(cosmo, z, nh, kt, rmf, abund='aspl', Z=0.3, elow=0.5, ehigh=2.0, unit='cr', lum_elow=0.5, lum_ehigh=2.0, arf=None):
     """
 
     Function calc_emissivity, computes scaling factor between count rate and APEC/MEKAL norm using XSPEC. The tool performs an XSPEC simulation of an absorbed APEC model with parameters set by the user, and computes the expected count rate in the band of interest corresponding to an APEC normalization of unity. The corresponding number is then used as conversion between count rate and emission measure for the hydrostatic mass reconstruction step. Note that since the computed count rates are corrected for vignetting through the exposure map, the provided ARF should correspond to the on-axis (unvignetted) effective area.
     Requires that XSPEC be in path
 
     :param cosmo: Astropy cosmology object containing the definition of the used cosmology.
     :type cosmo: class:`astropy.cosmology`
@@ -25,28 +25,39 @@
     :type z: float
     :param nh: Source NH in units of 1e22 cm**(-2)
     :type nh: float
     :param kt: Source temperature in keV
     :type kt: float
     :param rmf: Path to response file (RMF/RSP)
     :type rmf: str
-    :param abund: Solar abundance table in XSPEC format. Defaults to "angr"
+    :param abund: Solar abundance table in XSPEC format. Defaults to "aspl" (Asplund et al. 2009)
     :type abund: str
     :param Z: Metallicity with respect to solar. Defaults to 0.3
     :type Z: float
     :param elow: Low-energy bound of the input image in keV. Defaults to 0.5
     :type elow: float
     :param ehigh: High-energy bound of the input image in keV. Defaults to 2.0
     :type ehigh: float
     :param arf: Path to on-axis ARF (optional, in case response file is RMF)
     :type arf: str
+    :param unit: Specify whether the exposure map is in units of sec (unit='cr') or photon flux (unit='photon'). By default unit='cr'.
+    :type unit: str
+    :param lum_elow: Low energy bound (rest frame) for luminosity calculation. Defaults to 0.5
+    :type lum_elow: float
+    :param lum_ehigh: High energy bound (rest frame) for luminosity calculation. Defaults to 2.0
+    :type lum_ehigh: float
     :return: Conversion factor
     :rtype: float
     """
 
+    if unit!='cr' and unit!='photon':
+
+        print('Unknown unit %s, aborting' % (unit))
+        return
+
     check_xspec = is_tool('xspec')
 
     if not check_xspec:
 
         print('Error: XSPEC cannot be found in path')
 
         return
@@ -97,15 +108,29 @@
 
     fsim.write('ign **-%1.2lf\n' % (elow))
 
     fsim.write('ign %1.2lf-**\n' % (ehigh))
 
     fsim.write('log sim.txt\n')
 
-    fsim.write('show rates\n')
+    if unit == 'cr':
+
+        fsim.write('show rates\n')
+
+    elif unit == 'photon':
+
+        fsim.write('flux %1.2lf %1.2lf\n' % (elow, ehigh))
+
+    fsim.write('log none\n')
+
+    fsim.write('delcomp 1\n')
+
+    fsim.write('log lumin.txt\n')
+
+    fsim.write('lumin %1.2lf %1.2lf %g\n' % (lum_elow, lum_ehigh, z))
 
     fsim.write('log none\n')
 
     fsim.write('quit\n')
 
     fsim.close()
 
@@ -121,23 +146,39 @@
 
     if os.path.exists('%s.fak' % (nrmf)):
 
         os.system('rm %s.fak' % (nrmf))
 
     os.system('xspec < commands.xcm')
 
-    ssim = os.popen('grep cts/s sim.txt','r')
+    if unit == 'cr':
+
+        ssim = os.popen('grep cts/s sim.txt', 'r')
+
+        lsim = ssim.readline()
+
+        cr = float(lsim.split()[6])
+
+    else:
+
+        ssim = os.popen('grep photons sim.txt', 'r')
+
+        lsim = ssim.readline()
+
+        cr = float(lsim.split()[3])
+
+    slum = os.popen('grep Luminosity lumin.txt', 'r')
 
-    lsim = ssim.readline()
+    llum = slum.readline()
 
-    cr = float(lsim.split()[6])
+    lumtot = float(llum.split()[2])
 
-    #ccf = 1. / cr
+    lumfact = lumtot / cr
 
-    return cr
+    return cr, lumfact
 
 
 def medsmooth(prof):
     """
     Smooth a given profile by taking the median value of surrounding points instead of the initial value
 
     :param prof: Input profile to be smoothed
@@ -172,30 +213,31 @@
     rt=pars[4]
     c=pars[5]
     numer=Tmin/T0+np.power(x/rcool,acool)
     denom=1.+np.power(x/rcool,acool)
     t2=np.power(1.+(x/rt)**2,-c/2)
     return T0*numer/denom*t2
 
-def variable_ccf(Mhyd, cosmo, z, nh, rmf, method='interp', abund='angr', elow=0.5, ehigh=2.0, arf=None, outz=None, outkt=None):
+def variable_ccf(Mhyd, cosmo, z, nh, rmf, method='interp', abund='aspl', elow=0.5, ehigh=2.0,
+                 unit='cr', lum_elow=0.5, lum_ehigh=2.0, arf=None, outz=None, outkt=None):
     '''
 
     :param Mhyd: Hydromass object
     :type Mhyd: :class:`hydromass.mhyd.Mhyd`
     :param cosmo: Astropy cosmology object containing the definition of the used cosmology.
     :type cosmo: class:`astropy.cosmology`
     :param z: Source redshift
     :type z: float
     :param nh: Source NH in units of 1e22 cm**(-2)
     :type nh: float
     :param rmf: Path to response file (RMF/RSP)
     :type rmf: str
     :param method: Choose whether the temperature profile will be interpolated (method='interp') or fitted with a parametric function (method='fit'). Defaults to 'interp'.
     :type method: str
-    :param abund: Solar abundance table in XSPEC format. Defaults to "angr"
+    :param abund: Solar abundance table in XSPEC format. "aspl" (Asplund et al. 2009)
     :type abund: str
     :param elow: Low-energy bound of the input image in keV. Defaults to 0.5
     :type elow: float
     :param ehigh: High-energy bound of the input image in keV. Defaults to 2.0
     :type ehigh: float
     :param arf: Path to on-axis ARF (optional, in case response file is RMF)
     :type arf: str
@@ -215,15 +257,15 @@
 
     spec_data = Mhyd.spec_data
 
     bins = Mhyd.sbprof.bins
 
     nbin = Mhyd.sbprof.nbin
 
-    cf_prof = np.empty(nbin)
+    cf_prof, lf_prof = np.empty(nbin), np.empty(nbin)
 
     nkt = len(spec_data.temp_x)
 
     if method=='fit':
 
         pars_temp = np.array([1.2, 0.52 * 1.20, np.exp(-2.90), 1.06, 0.36, 0.28 * 2.0])
 
@@ -296,24 +338,27 @@
 
         print('No abundance value loaded, assuming 0.3 everywhere')
 
         for i in range(nbin):
 
 
 
-            cf_prof[i] = calc_emissivity(cosmo=cosmo,
+            cf_prof[i], lf_prof[i] = calc_emissivity(cosmo=cosmo,
                                          z=z,
                                          nh=nh,
                                          kt=ktprof[i],
                                          Z=0.3,
                                          elow=elow,
                                          ehigh=ehigh,
                                          rmf=rmf,
                                          abund=abund,
-                                         arf=arf)
+                                         arf=arf,
+                                         unit=unit,
+                                         lum_elow=lum_elow,
+                                         lum_ehigh=lum_ehigh)
 
     else:
 
         print('Modeling abundance profile...')
 
         active = np.where(spec_data.zfe_lo > 0.)
 
@@ -343,24 +388,27 @@
 
         med_norm = np.median(trace_z.posterior['norm'])
 
         zfe_prof = med_floor + med_norm * (1. + (bins*Mhyd.amin2kpc/med_rc)**2) ** (-beta_fe)
 
         for i in range(nbin):
 
-            cf_prof[i] = calc_emissivity(cosmo=cosmo,
+            cf_prof[i], lf_prof[i] = calc_emissivity(cosmo=cosmo,
                                          z=z,
                                          nh=nh,
                                          kt=ktprof[i],
                                          Z=zfe_prof[i],
                                          elow=elow,
                                          ehigh=ehigh,
                                          rmf=rmf,
                                          abund=abund,
-                                         arf=arf)
+                                         arf=arf,
+                                         unit=unit,
+                                         lum_elow=lum_elow,
+                                         lum_ehigh=lum_ehigh)
 
         if outz is not None:
 
             plt.clf()
 
             fig = plt.figure(figsize=(13, 10))
 
@@ -405,8 +453,8 @@
             plt.xlabel('Radius [kpc]', fontsize=28)
 
             plt.ylabel('$Z/Z_{\odot}$', fontsize=28)
 
             plt.savefig(outz)
 
 
-    return cf_prof
+    return cf_prof, lf_prof
```

### Comparing `hydromass-0.5.1/hydromass/forward.py` & `hydromass-0.5.2/hydromass/forward.py`

 * *Files 0% similar despite different names*

```diff
@@ -868,15 +868,15 @@
 
             if not isjax:
 
                 trace = pm.sample(nmcmc, init='ADVI', initvals=start, tune=tune, target_accept=0.9)
 
             else:
 
-                trace = pmjax.sample_numpyro_nuts(nmcmc, init='ADVI', initvals=start, tune=tune, target_accept=0.9)
+                trace = pmjax.sample_numpyro_nuts(nmcmc, initvals=start, tune=tune, target_accept=0.9)
 
         else:
 
             if not isjax:
 
                 trace = pm.sample(nmcmc, tune=tune, init='ADVI', target_accept=0.9)
```

### Comparing `hydromass-0.5.1/hydromass/functions.py` & `hydromass-0.5.2/hydromass/functions.py`

 * *Files identical despite different names*

### Comparing `hydromass-0.5.1/hydromass/mhyd.py` & `hydromass-0.5.2/hydromass/mhyd.py`

 * *Files 2% similar despite different names*

```diff
@@ -752,29 +752,29 @@
     :type sz_data: class:`hydromass.tpdata.SZData`
     :param directory: Name of output file directory. Defaults to 'mhyd'
     :type directory: str
     :param redshift: Source redshift
     :type redshift: float
     :param cosmo: Astropy cosmological model
     :type cosmo: class:`astropy.cosmology`
-    :param f_abund: Solar abundance table. Available are 'angr', 'aspl', and 'grsa'. Defaults to 'angr'
-    :type f_abund: str
+    :param abund: Solar abundance table. Available are 'angr' (Anders & Grevesse 1987), 'aspl' (Asplund et al. 2009), and 'grsa' (Grevesse & Sauval 2005). Defaults to 'aspl'
+    :type abund: str
     """
 
-    def __init__(self, sbprofile=None, spec_data=None, sz_data=None, wl_data=None, directory=None, redshift=None, cosmo=None, f_abund = 'angr'):
+    def __init__(self, sbprofile=None, spec_data=None, sz_data=None, wl_data=None, directory=None, redshift=None, cosmo=None, abund = 'aspl'):
 
-        if f_abund == 'angr':
+        if abund == 'angr':
             nhc = 1 / 0.8337
             mup = 0.6125
             mu_e = 1.1738
-        elif f_abund == 'aspl':
+        elif abund == 'aspl':
             nhc = 1 / 0.8527
             mup = 0.5994
             mu_e = 1.1548
-        elif f_abund == 'grsa':
+        elif abund == 'grsa':
             nhc = 1 / 0.8520
             mup = 0.6000
             mu_e = 1.1555
         else:  # aspl default
             nhc = 1 / 0.8527
             mup = 0.5994
             mu_e = 1.1548
@@ -847,37 +847,44 @@
 
         self.mfact0 = kev2erg * cgskpc / (cgsG * cgsamu * self.mup) / Msun / 1e13
 
         self.mgas_fact = cgsamu * self.mu_e / Msun
 
         self.transf = 4. * (1. + redshift) ** 2 * (180. * 60.) ** 2 / np.pi / 1e-14 * self.nhc / cgsMpc * 1e3
 
+        self.abund = abund
 
-    def emissivity(self, nh, rmf, type='single', kt=None, abund='angr', Z=0.3, elow=0.5, ehigh=2.0, arf=None, outz=None, method='interp', outkt=None):
+
+    def emissivity(self, nh, rmf, type='single', kt=None, Z=0.3, elow=0.5, ehigh=2.0,
+                   arf=None, unit='cr', lum_elow=0.5, lum_ehigh=2.0, outz=None, method='interp', outkt=None):
         '''
         Compute the conversion between count rate and emissivity using XSPEC by run the :func:`hydromass.emissivity.calc_emissivity` function. Requires XSPEC to be available in PATH.
 
         :param nh: Source NH in units of 1e22 cm**(-2)
         :type nh: float
         :param kt: Source temperature in keV. If None, the code will search for a loaded spectroscopic temperature profile and use the weighted mean temperature. Defaults to None
         :type kt: float
         :param rmf: Path to response file (RMF/RSP)
         :type rmf: str
         :param type: Set whether we will assume a constant conversion factor across the range (type="single") or if we will attempt to model the radial variations of the emissivity conversion factor (type="variable). Defaults to "single".
         :type type: str
-        :param abund: Solar abundance table in XSPEC format. Defaults to "angr"
-        :type abund: str
-        :param Z: Metallicity with respect to solar. Defaults to 0.3
+        :param Z: Metallicity with respect to solar. If type='variable' and an abundance profile is loaded, this parameter is ignored. Defaults to 0.3
         :type Z: float
         :param elow: Low-energy bound of the input image in keV. Defaults to 0.5
         :type elow: float
         :param ehigh: High-energy bound of the input image in keV. Defaults to 2.0
         :type ehigh: float
         :param arf: Path to on-axis ARF (optional, in case response file is RMF)
         :type arf: str
+        :param unit: Specify whether the exposure map is in units of sec (unit='cr') or photon flux (unit='photon'). By default unit='cr'.
+        :type unit: str
+        :param lum_elow: Low energy bound (rest frame) for luminosity calculation. Defaults to 0.5
+        :type lum_elow: float
+        :param lum_ehigh: High energy bound (rest frame) for luminosity calculation. Defaults to 2.0
+        :type lum_ehigh: float
         :param outz: If type='variable', name of output file including the fit to the metal abundance profile. If None, it is ignored. Defaults to None.
         :type outz: str
         :param method: If type='variable', choose whether the temperature profile will be interpolated (method='interp') or fitted with a parametric function (method='fit'). Defaults to 'interp'.
         :type method: str
         :param outkt: If type='variable', name of output file including the fit to the temperature profile. If None, it is ignored. Defaults to None.
         :type outkt: str
         '''
@@ -894,37 +901,43 @@
 
                 return
 
         if type == 'single':
 
             print('Mean cluster temperature:', kt, ' keV')
 
-            self.ccf = calc_emissivity(cosmo=self.cosmo,
+            self.ccf, self.lumfact = calc_emissivity(cosmo=self.cosmo,
                                             z=self.redshift,
                                             nh=nh,
                                             kt=kt,
                                             rmf=rmf,
-                                            abund=abund,
+                                            abund=self.abund,
                                             Z=Z,
                                             elow=elow,
                                             ehigh=ehigh,
-                                            arf=arf)
+                                            arf=arf,
+                                            unit=unit,
+                                            lum_elow=lum_elow,
+                                            lum_ehigh=lum_ehigh)
 
         elif type == 'variable':
 
-            self.ccf = variable_ccf(self,
+            self.ccf, self.lumfact = variable_ccf(self,
                                     cosmo=self.cosmo,
                                     z=self.redshift,
                                     nh=nh,
                                     rmf=rmf,
                                     method=method,
-                                    abund=abund,
+                                    abund=self.abund,
                                     elow=elow,
                                     ehigh=ehigh,
                                     arf=arf,
+                                    unit=unit,
+                                    lum_elow=lum_elow,
+                                    lum_ehigh=lum_ehigh,
                                     outz=outz,
                                     outkt=outkt)
 
 
     def run(self, model=None, bkglim=None, nmcmc=1000, fit_bkg=False, back=None,
             samplefile=None, nrc=None, nbetas=6, min_beta=0.6, nmore=5,
             p0_prior=None, tune=500, dmonly=False, mstar=None, find_map=True, pnt=False,
```

### Comparing `hydromass-0.5.1/hydromass/nonparametric.py` & `hydromass-0.5.2/hydromass/nonparametric.py`

 * *Files identical despite different names*

### Comparing `hydromass-0.5.1/hydromass/plots.py` & `hydromass-0.5.2/hydromass/plots.py`

 * *Files identical despite different names*

### Comparing `hydromass-0.5.1/hydromass/pnt.py` & `hydromass-0.5.2/hydromass/pnt.py`

 * *Files identical despite different names*

### Comparing `hydromass-0.5.1/hydromass/polytropic.py` & `hydromass-0.5.2/hydromass/polytropic.py`

 * *Files identical despite different names*

### Comparing `hydromass-0.5.1/hydromass/save.py` & `hydromass-0.5.2/hydromass/save.py`

 * *Files identical despite different names*

### Comparing `hydromass-0.5.1/hydromass/tpdata.py` & `hydromass-0.5.2/hydromass/tpdata.py`

 * *Files identical despite different names*

### Comparing `hydromass-0.5.1/hydromass/wl.py` & `hydromass-0.5.2/hydromass/wl.py`

 * *Files identical despite different names*

### Comparing `hydromass-0.5.1/hydromass.egg-info/SOURCES.txt` & `hydromass-0.5.2/hydromass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydromass-0.5.1/setup.py` & `hydromass-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
       name='hydromass',    # This is the name of your PyPI-package.
-      version='0.5.1',
+      version='0.5.2',
       description='Hydrostatic mass calculator',
       author='Dominique Eckert, Vittorio Ghirardini, Stefano Ettori',
       author_email='Dominique.Eckert@unige.ch',
       url="https://github.com/domeckert/hydromass",
       packages=['hydromass'],
       install_requires=[
             'numpy','scipy','astropy','matplotlib','pymc','aesara','pyproffit','numpyro','corner'
```

