# Comparing `tmp/SpectroscopicBinarySystem-1.2.2.tar.gz` & `tmp/SpectroscopicBinarySystem-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.2.2.tar", last modified: Thu May 11 13:59:03 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.3.0.tar", last modified: Mon May 15 21:54:54 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.2.2.tar` & `SpectroscopicBinarySystem-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 13:59:03.233869 SpectroscopicBinarySystem-1.2.2/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     4759 2023-05-11 13:59:03.233869 SpectroscopicBinarySystem-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4368 2023-05-11 13:58:28.000000 SpectroscopicBinarySystem-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 13:59:03.216873 SpectroscopicBinarySystem-1.2.2/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     4759 2023-05-11 13:59:03.000000 SpectroscopicBinarySystem-1.2.2/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-05-11 13:59:03.000000 SpectroscopicBinarySystem-1.2.2/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 13:59:03.000000 SpectroscopicBinarySystem-1.2.2/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-05-11 13:59:03.000000 SpectroscopicBinarySystem-1.2.2/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-11 13:59:03.000000 SpectroscopicBinarySystem-1.2.2/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0      724 2023-05-11 13:59:03.235878 SpectroscopicBinarySystem-1.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 13:59:03.229428 SpectroscopicBinarySystem-1.2.2/spectroscopicbinarysystem/
--rw-rw-rw-   0        0        0    31292 2023-05-11 13:58:14.000000 SpectroscopicBinarySystem-1.2.2/spectroscopicbinarysystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 21:54:54.816656 SpectroscopicBinarySystem-1.3.0/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4709 2023-05-15 21:54:54.816656 SpectroscopicBinarySystem-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4318 2023-05-15 21:54:48.000000 SpectroscopicBinarySystem-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 21:54:54.813646 SpectroscopicBinarySystem-1.3.0/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     4709 2023-05-15 21:54:54.000000 SpectroscopicBinarySystem-1.3.0/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-15 21:54:54.000000 SpectroscopicBinarySystem-1.3.0/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 21:54:54.000000 SpectroscopicBinarySystem-1.3.0/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-05-15 21:54:54.000000 SpectroscopicBinarySystem-1.3.0/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-15 21:54:54.000000 SpectroscopicBinarySystem-1.3.0/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      724 2023-05-15 21:54:54.818810 SpectroscopicBinarySystem-1.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 21:54:54.815652 SpectroscopicBinarySystem-1.3.0/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    32045 2023-05-15 21:51:06.000000 SpectroscopicBinarySystem-1.3.0/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.2.2/LICENSE` & `SpectroscopicBinarySystem-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.2.2/PKG-INFO` & `SpectroscopicBinarySystem-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.2.2
+Version: 1.3.0
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.2.2)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.3.0)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
@@ -75,21 +75,20 @@
 sbs = SpectroscopicBinarySystem(
     object_name='hd123299',
     spectra_path='./examples/alphadra/',
     t0=2451441.804,
     period_guess=51,
     conf={
         "LAMBDA_REF": 6562.82,
-        "LINE_FIT_MODEL": "voigt",
-        "LINE_FIT_WINDOW_WIDTH": 10,
-        "LINE_FIT_CONT_NORM_EXCLUDE_WIDTH": 1,
+        "LINE_FIT_MODEL": "gaussian",
+        "LINE_FIT_FWHM": 1.0,
         "RV_CORR_TYPE": "barycentric",
         "SB_TYPE": 1
     },
-    verbose=True
+    verbose=False,
     debug=False)
 
 # plot result with matplotlib and save the results
 sbs.plotRadialVelocityCurve(
     title="α Dra - HD123299 - Phased radial velocities",
     subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to may 2023\nhttps://alphadra.staros-projects.org/\n",
     savefig=True)
```

### Comparing `SpectroscopicBinarySystem-1.2.2/README.md` & `SpectroscopicBinarySystem-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.2.2)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.3.0)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
@@ -63,21 +63,20 @@
 sbs = SpectroscopicBinarySystem(
     object_name='hd123299',
     spectra_path='./examples/alphadra/',
     t0=2451441.804,
     period_guess=51,
     conf={
         "LAMBDA_REF": 6562.82,
-        "LINE_FIT_MODEL": "voigt",
-        "LINE_FIT_WINDOW_WIDTH": 10,
-        "LINE_FIT_CONT_NORM_EXCLUDE_WIDTH": 1,
+        "LINE_FIT_MODEL": "gaussian",
+        "LINE_FIT_FWHM": 1.0,
         "RV_CORR_TYPE": "barycentric",
         "SB_TYPE": 1
     },
-    verbose=True
+    verbose=False,
     debug=False)
 
 # plot result with matplotlib and save the results
 sbs.plotRadialVelocityCurve(
     title="α Dra - HD123299 - Phased radial velocities",
     subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to may 2023\nhttps://alphadra.staros-projects.org/\n",
     savefig=True)
```

### Comparing `SpectroscopicBinarySystem-1.2.2/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.3.0/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.2.2
+Version: 1.3.0
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.2.2)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.3.0)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
@@ -75,21 +75,20 @@
 sbs = SpectroscopicBinarySystem(
     object_name='hd123299',
     spectra_path='./examples/alphadra/',
     t0=2451441.804,
     period_guess=51,
     conf={
         "LAMBDA_REF": 6562.82,
-        "LINE_FIT_MODEL": "voigt",
-        "LINE_FIT_WINDOW_WIDTH": 10,
-        "LINE_FIT_CONT_NORM_EXCLUDE_WIDTH": 1,
+        "LINE_FIT_MODEL": "gaussian",
+        "LINE_FIT_FWHM": 1.0,
         "RV_CORR_TYPE": "barycentric",
         "SB_TYPE": 1
     },
-    verbose=True
+    verbose=False,
     debug=False)
 
 # plot result with matplotlib and save the results
 sbs.plotRadialVelocityCurve(
     title="α Dra - HD123299 - Phased radial velocities",
     subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to may 2023\nhttps://alphadra.staros-projects.org/\n",
     savefig=True)
```

### Comparing `SpectroscopicBinarySystem-1.2.2/setup.cfg` & `SpectroscopicBinarySystem-1.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 322e 320d 0a61  rsion = 1.2.2..a
+00000030: 7273 696f 6e20 3d20 312e 332e 300d 0a61  rsion = 1.3.0..a
 00000040: 7574 686f 7220 3d20 4775 696c 6c61 756d  uthor = Guillaum
 00000050: 6520 4265 7274 7261 6e64 0d0a 6175 7468  e Bertrand..auth
 00000060: 6f72 5f65 6d61 696c 203d 2067 6265 2e69  or_email = gbe.i
 00000070: 6f40 706d 2e6d 650d 0a64 6573 6372 6970  o@pm.me..descrip
 00000080: 7469 6f6e 203d 2050 7974 686f 6e20 6173  tion = Python as
 00000090: 7472 6f6e 6f6d 7920 746f 6f6c 7320 666f  tronomy tools fo
 000000a0: 7220 7370 6563 7472 6f73 636f 7069 6320  r spectroscopic
```

### Comparing `SpectroscopicBinarySystem-1.2.2/spectroscopicbinarysystem/__init__.py` & `SpectroscopicBinarySystem-1.3.0/spectroscopicbinarysystem/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # astropy
 from astropy.io import fits
 from astropy.time import Time
 import astropy.units as u
 import astropy.wcs as fitswcs
 from astropy.time import Time
 from astropy.coordinates import SkyCoord, EarthLocation, SpectralCoord
-from astropy.modeling import models
+from astropy.modeling import models, fitting
 from astropy import constants as const
 
 # astroquery
 from astroquery.simbad import Simbad
 
 # specutils
 from specutils import Spectrum1D, SpectralRegion
@@ -48,14 +48,16 @@
     """
 
     def __init__(self, filename, skycoord, conf):
         self._filename = filename
         self._basename = os.path.basename(filename)
         self._skycoord = skycoord
         self._conf = conf
+        self._snr = 0.0
+        self._line_fit_fwhm = 0.0
         self._phase = None
 
         spectrum_file = fits.open(filename)
 
         self._header = spectrum_file[0].header
         self._jd = self._header['JD-OBS']
         self._observer = self._header['OBSERVER']
@@ -94,14 +96,31 @@
         """
         Return the final computed radial velocity of the line (already corrected of heliocentric/barycentric velocity)
         :return: radial velocity
         :rtype: float
         """
         return self._rv.value
 
+    def getError(self):
+        """
+        Return the random error in km/s if CRDER1 (in Angstroms) is in fits header
+        :return: radial velocity
+        :rtype: float
+        """
+        c = const.c.to('km/s')
+        calibration_error = float(
+            self._header['CRDER1']) if 'CRDER1' in self._header else 0
+        calibration_error = abs(
+            c * (calibration_error / self._conf["LAMBDA_REF"])).value
+
+        return calibration_error
+
+    def getSNR(self):
+        return self._snr
+
     def getJD(self):
         """
         Return 'JD-OBS' header field
         :return: float corresponding to the julian date of the observation
         :rtype: float
         """
         return float(self._header['JD-OBS'])
@@ -156,81 +175,80 @@
         """
         Compute the radial velocity from a line position and a radial velocity correction
         Reference line rest position in Angstroms can be customize in conf["LAMBDA_REF"]
         :return: None
         """
         c = const.c.to('km/s')
         self._rv = (c * ((self._center_of_line -
-                    self._conf["LAMBDA_REF"]) / self._conf["LAMBDA_REF"])) + self._rv_corr
+                          self._conf["LAMBDA_REF"]) / self._conf["LAMBDA_REF"])) + self._rv_corr
 
     def getCenterOfLine(self):
         """
         Return the center of the line computed for the spectrum using a fit (non corrected from heliocentric/barycentric velocity)
         :return: Float
         """
         return self._center_of_line
 
     def getDebugLineFitting(self):
         return self._debug_line_fitting
 
     def findCenterOfLine(self):
         """
-        Find the center of the line in a spectrum using a fit (models available : Gaussian1D, Lorentz1D, Voigt1D)
+        Find the center of the line in a spectrum using a fit (models available : Gaussian1D, Lorentz1D)
         :return: None
         """
-        w1 = float(self._conf['LINE_FIT_WINDOW_WIDTH']) / 2
-        w2 = float(self._conf['LINE_FIT_CONT_NORM_EXCLUDE_WIDTH']) / 2
         fwhm = float(self._conf['LINE_FIT_FWHM'])
         gauss_smooth_std = float(self._conf['LINE_FIT_GAUSS_SMOOTH_STD'])
 
         # Smooth the spectrum to make a first approximation of the center of the main line in absorption.
         # Assume that the line to be measured is the broadest and deepest in the spectrum
         spec1_gsmooth = gaussian_smooth(Spectrum1D(
             flux=self.flux, wcs=self.wcs), stddev=gauss_smooth_std)
 
         ipeak = spec1_gsmooth.flux[50:-50].argmin()
         xpeak = spec1_gsmooth.spectral_axis[50:-50][ipeak].to(u.AA)
 
-        sr_w1 = SpectralRegion(xpeak - (w1 * u.AA), xpeak + (w1 * u.AA))
-        sr_w2 = SpectralRegion(xpeak - (w2 * u.AA), xpeak + (w2 * u.AA))
+        sr_w1 = SpectralRegion(xpeak - (fwhm * 2.5 * u.AA),
+                               xpeak + (fwhm * 2.5 * u.AA))
+        sr_w2 = SpectralRegion(xpeak - (fwhm * u.AA), xpeak + (fwhm * u.AA))
 
         spec1d_line = extract_region(Spectrum1D(
             flux=self.flux, wcs=self.wcs), sr_w1)
 
         # continuum normalization of the extracted spectral region
-        s_fit = fit_generic_continuum(spec1d_line, exclude_regions=[sr_w2])
+        s_fit = fit_generic_continuum(spec1d_line)
         spec1d_line = spec1d_line / s_fit(spec1d_line.spectral_axis)
         spec1d_line -= 1
 
         # line fitting
         match self._conf['LINE_FIT_MODEL']:
             case 'gaussian':
                 g_init = models.Gaussian1D(
                     mean=xpeak, amplitude=spec1d_line.flux.argmin())
-            case 'voigt':
-                g_init = models.Voigt1D(
-                    x_0=xpeak, amplitude_L=spec1d_line.flux.argmin())
             case 'lorentz':
                 g_init = models.Lorentz1D(x_0=xpeak, fwhm=fwhm)
 
         g_fit = fit_lines(spec1d_line, g_init, window=sr_w2)
         y_fit = g_fit(spec1d_line.spectral_axis)
 
         match self._conf['LINE_FIT_MODEL']:
             case 'gaussian':
                 center = g_fit.mean
-            case _:
+                fwhm = g_fit.fwhm
+            case 'lorentz':
                 center = g_fit.x_0
+                fwhm = g_fit.fwhm
 
         self._debug_line_fitting = (spec1d_line, y_fit, extract_region(Spectrum1D(
             flux=spec1_gsmooth.flux, wcs=self.wcs), sr_w1))
         self._center_of_line = center.value
+        self._line_fit_fwhm = fwhm.value
 
     def __str__(self):
-        return f"Spectrum : {self._basename}\n- obs: {self._observer}\n- jd: {self._jd}\n- center: {self._center_of_line} A\n- {self._conf['RV_CORR_TYPE']}: {self._rv_corr}\n- rv: {self._rv}\n "
+        return f"Spectrum : {self._basename}\n- obs: {self._observer}\n- jd: {self._jd}\n- snr: {self._snr}\n- center: {self._center_of_line} A\n- {self._conf['RV_CORR_TYPE']}: {self._rv_corr}\n- rv: {self._rv}\n- error: {self.getError()}\n"
 
 #
 
 
 class SpectroscopicBinarySystem:
     """
     Class allowing to dynamically load spectra in fit(s) format and to
@@ -315,16 +333,18 @@
                     10, 7), sharex=True, sharey=True)
                 for i, s in enumerate(spectra):
                     ax = axs.flat[i]
                     extracted_profil, line_fitting, gauss_smooth = s.getDebugLineFitting()
                     ax.set_title(
                         f'{s.getBaseName()}\n{s.getObserver()} JD={s.getJD()}', fontsize="6")
                     ax.grid(True)
-                    ax.tick_params(axis='both', which='major', labelsize=6)
-                    ax.tick_params(axis='both', which='minor', labelsize=6)
+                    ax.tick_params(
+                        axis='both', which='major', labelsize=6)
+                    ax.tick_params(
+                        axis='both', which='minor', labelsize=6)
                     ax.plot(extracted_profil.spectral_axis.to(
                         u.AA), extracted_profil.flux, color="k")
                     ax.plot(gauss_smooth.spectral_axis.to(
                         u.AA), gauss_smooth.flux-1*u.Jy, "b--")
                     ax.plot(extracted_profil.spectral_axis.to(
                         u.AA), line_fitting, color="r")
                     ax.axvline(x=s.getCenterOfLine(),
@@ -375,15 +395,16 @@
     def __solveSystem(self):
         """
         Compute the orbital solution with BinaryStarSolver
         """
         # write result file for BinaryStarSolver
         with open(f'{self._spectra_path}/sbs_results.txt', 'w') as f:
             for s in self._sb_spectra:
-                output = f"{float(s.getJD()) - 2400000.0} {round(s.getRV(), 3)}"
+                error = 1 / s.getError() if s.getError() else 1
+                output = f"{float(s.getJD()) - 2400000.0} {round(s.getRV(), 3)} {error}"
                 f.write(output + '\n')
 
         # [γ, K, ω, e, T0, P, a, f(M)]
         try:
             params, err, cov = StarSolve(
                 data_file=f"{self._spectra_path}/sbs_results.txt",
                 star="primary",
@@ -426,14 +447,15 @@
             f'- K = {params[1]} ± {err[1]}',
             f'- ω = {params[2]} ± {err[2]}',
             f'- e = {params[3]} ± {err[3]}',
             f'- T0 = {params[4]} ± {err[4]}',
             f'- P = {params[5]} ± {err[5]}',
             f'- a = {params[6]} ± {err[6]}',
             f'- f(M) = {params[7]} ± {err[7]}',
+            f'- Error sums = {sum(err)}',
             sep='\n')
 
     def getOrbitalSolution(self):
         self.__solveSystem()
         return self._orbital_solution
 
     def __findNearest(self, array, value):
@@ -498,28 +520,30 @@
                     axs[0].errorbar(s.getPhase(), s.getRV(), yerr=0,
                                     fmt=instruments[label], ecolor='k', capsize=0, color=color, lw=.7, markersize=5)
 
             xindex = self.__findNearest(self._model_x, s.getPhase())
             delta = s.getRV() - self._model_y[xindex]
             self._residuals.append(delta)
             fmt = instruments[label] if group_by_instruments else 'o'
+            error = s.getError()
+            capsize = 3 if error else 0
             axs[1].errorbar(s.getPhase(), delta,
-                            yerr=0, fmt=fmt, ecolor='k', capsize=0, color=color, lw=.7, markersize=5)
+                            yerr=s.getError(), fmt=fmt, ecolor='k', capsize=capsize, color=color, lw=.7, markersize=5)
 
         print(
             f'- Residual standard deviation : {np.std(self._residuals)}')
 
     def plotRadialVelocityCurve(self, title="", subtitle="", rv_y_multiple=10, residual_y_multiple=None, savefig=False, dpi=150, font_family='monospace', font_size=9, group_by_instruments=False):
         if not self._orbital_solution:
             self.__solveSystem()
 
         plt.rcParams['font.size'] = font_size
         plt.rcParams['font.family'] = font_family
-        fig, axs = plt.subplots(2, 1, figsize=(11, 7), gridspec_kw={
-                                'height_ratios': [4, 1]}, sharex=True)
+        fig, axs = plt.subplots(2, 1, figsize=(12, 7), gridspec_kw={
+            'height_ratios': [4, 1]}, sharex=True)
         axs[1].set_xlabel('Phase', fontdict=None,
                           labelpad=None, fontname='monospace', size=8)
         axs[0].set_ylabel(
             'Radial velocity [km $s^{-1}$]', fontdict=None, labelpad=None, fontname='monospace', size=8)
         axs[1].set_ylabel('RV residual', fontdict=None,
                           labelpad=None, fontname='monospace', size=8)
         axs[0].grid(color='grey', alpha=0.2, linestyle='-',
```

