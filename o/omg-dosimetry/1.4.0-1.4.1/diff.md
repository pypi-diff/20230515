# Comparing `tmp/omg_dosimetry-1.4.0.tar.gz` & `tmp/omg_dosimetry-1.4.1.tar.gz`

## Comparing `omg_dosimetry-1.4.0.tar` & `omg_dosimetry-1.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10880 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/requirements.txt
--rw-r--r--   0        0        0    27306 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/src/omg_dosimetry/OMG_Logo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/src/omg_dosimetry/__init__.py
--rw-r--r--   0        0        0    44160 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/src/omg_dosimetry/analysis.py
--rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/src/omg_dosimetry/calibration.py
--rw-r--r--   0        0        0    41949 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/src/omg_dosimetry/imageRGB.py
--rw-r--r--   0        0        0    17012 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/src/omg_dosimetry/tiff2dose.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/LICENSE
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/README.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    10880 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.1/requirements.txt
+-rw-r--r--   0        0        0    27306 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.1/src/omg_dosimetry/OMG_Logo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.1/src/omg_dosimetry/__init__.py
+-rw-r--r--   0        0        0    43965 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.1/src/omg_dosimetry/analysis.py
+-rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.1/src/omg_dosimetry/calibration.py
+-rw-r--r--   0        0        0    41949 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.1/src/omg_dosimetry/imageRGB.py
+-rw-r--r--   0        0        0    17012 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.1/src/omg_dosimetry/tiff2dose.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.1/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.1/LICENSE
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.1/README.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.1/PKG-INFO
```

### Comparing `omg_dosimetry-1.4.0/requirements.txt` & `omg_dosimetry-1.4.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.4.0/src/omg_dosimetry/OMG_Logo.png` & `omg_dosimetry-1.4.1/src/omg_dosimetry/OMG_Logo.png`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.4.0/src/omg_dosimetry/analysis.py` & `omg_dosimetry-1.4.1/src/omg_dosimetry/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         
     def gamma_analysis(self, film_filt=0, doseTA=3.0, distTA=3.0, threshold=0.1, norm_val='max', local_gamma=False, max_gamma=None, random_subset=None):
         """ Perform Gamma analysis """
         self.doseTA, self.distTA = doseTA, distTA
         self.film_filt, self.threshold, self.norm_val = film_filt, threshold, norm_val        
         start_time = time.time()
         self.GammaMap = self.computeGamma(doseTA=doseTA, distTA=distTA, threshold=threshold, norm_val=norm_val, local_gamma=local_gamma, max_gamma=max_gamma, random_subset=random_subset)       
-        print("--- Calcul Gamma fait en %s seconds ---" % (time.time() - start_time))
+        print("--- Done! ({:.1f} seconds) ---".format((time.time() - start_time)))
         self.computeDiff()
     
     def computeHDmedianDiff(self, threshold=0.8, ref = 'max'):
         """ Compute median difference between film and reference doses in high dose region. """
         if ref == 'max': HDthreshold = threshold * self.ref_dose.array.max()
         else:  HDthreshold = threshold * ref
         film_HD = self.film_dose.array[self.ref_dose.array > HDthreshold]
@@ -446,24 +446,16 @@
         fig.tight_layout()
         axes = [ax1,ax2,ax3,ax4,ax5,ax6]
         max_dose_comp = np.percentile(self.ref_dose.array,[98])[0].round(decimals=-1)
         clim = [0, max_dose_comp]  
 
         self.film_dose.plotCB(ax1, clim=clim, title='Film dose')
         self.ref_dose.plotCB(ax2, clim=clim, title='Reference dose')
-        # gamma_map = ArrayImage(copy.copy(self.GammaMap.array))
-        # np.nan_to_num(gamma_map.array, copy=False, nan=1.0)
-        masked_array = np.ma.array(self.GammaMap.array, mask=np.isnan(self.GammaMap.array))
-        gamma_map = ArrayImage(masked_array)
-        cmap = matplotlib.cm.bwr
-        cmap.set_bad('k',1.)
-        gamma_map.plotCB(ax3, clim=[0,2], cmap='bwr', title='Gamma map ({:.2f}% pass; {:.2f} mean)'.format(self.GammaMap.passRate, self.GammaMap.mean))
-
-        # self.GammaMap.plotCB(ax3, clim=[0,2], cmap='bwr', title='Gamma map ({:.2f}% pass; {:.2f} mean)'.format(self.GammaMap.passRate, self.GammaMap.mean))
-        
+        self.GammaMap.plotCB(ax3, clim=[0,2], cmap='bwr', title='Gamma map ({:.2f}% pass; {:.2f} mean)'.format(self.GammaMap.passRate, self.GammaMap.mean))
+        ax3.set_facecolor('k')
         min_value = max(-20, np.percentile(self.DiffMap.array,[1])[0].round(decimals=0))
         max_value = min(20, np.percentile(self.DiffMap.array,[99])[0].round(decimals=0))
         clim = [min_value, max_value]    
         self.RelError.plotCB(ax4, cmap='jet', clim=clim, title='Relative Error (%) (RMSE={:.2f})'.format(self.DiffMap.RMSE))
         self.show_profiles(axes, x=x, y=y)
         
         fig.canvas.mpl_connect('button_press_event', lambda event: self.set_profile(event, axes))
@@ -696,14 +688,18 @@
         (self.film_dose, self.ref_dose) = equate_images(self.film_dose, self.ref_dose)
         self.film_dose.path = film_dose_path
         self.ref_dose.path = ref_dose_path
         print('Fine tune registration using keyboard if needed. Arrow keys = move; ctrl+left/right = rotate. Press enter when done.')
         self.fig = plt.figure()
         ax = plt.gca()
         self.cid = self.fig.canvas.mpl_connect('key_press_event', self.reg_ontype)
+        img_array = self.film_dose.array - self.ref_dose.array
+        min_max = [np.percentile(img_array,[1])[0].round(decimals=-1), np.percentile(img_array,[99])[0].round(decimals=-1)] 
+        lim = abs(max(min_max, key=abs))
+        self.clim = [-1.0*lim, lim]
         self.show_registration(ax=ax)
         
     def show_registration(self, ax=None, cmap='bwr'):
         if ax==None:
                 plt.plot()
                 ax = plt.gca()
         ax.clear()
@@ -717,16 +713,16 @@
             film_grad = np.hypot(film_x, film_y)
             img_array = film_grad - ref_grad
         else:
             img_array = self.film_dose.array - self.ref_dose.array
         img = load(img_array, dpi=self.film_dose.dpi) 
         RMSE =  (sum(sum(img.array**2)) / len(self.film_dose.array[(self.film_dose.array > 0)]))**0.5
         
-        clim = [np.percentile(img_array,[1])[0].round(decimals=-1), np.percentile(img_array,[99])[0].round(decimals=-1)]   
-        img.plot(ax=ax, clim=clim, cmap=cmap)     
+        #clim = [np.percentile(img_array,[1])[0].round(decimals=-1), np.percentile(img_array,[99])[0].round(decimals=-1)]   
+        img.plot(ax=ax, clim=self.clim, cmap=cmap)     
         ax.plot((0, img.shape[1]), (img.center.y, img.center.y),'k--')
         ax.plot((img.center.x, img.center.x), (0, img.shape[0]),'k--')
         ax.set_xlim(0, img.shape[1])
         ax.set_ylim(img.shape[0],0)
         ax.set_title('Fine tune registration. Arrow keys = move; ctrl+left/right = rotate. Press enter when done. RMSE = {}'.format(RMSE))
         
     def reg_ontype(self, event):
```

### Comparing `omg_dosimetry-1.4.0/src/omg_dosimetry/calibration.py` & `omg_dosimetry-1.4.1/src/omg_dosimetry/calibration.py`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.4.0/src/omg_dosimetry/imageRGB.py` & `omg_dosimetry-1.4.1/src/omg_dosimetry/imageRGB.py`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.4.0/src/omg_dosimetry/tiff2dose.py` & `omg_dosimetry-1.4.1/src/omg_dosimetry/tiff2dose.py`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.4.0/.gitignore` & `omg_dosimetry-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.4.0/LICENSE` & `omg_dosimetry-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.4.0/README.md` & `omg_dosimetry-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.4.0/pyproject.toml` & `omg_dosimetry-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "omg_dosimetry"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
   { name="JF Cabana", email="jean-francois.cabana.cisssca@ssss.gouv.qc.ca" },
 ]
 description = "Optimized Multichannel Gafchromic Dosimetry (OMG Dosimetry)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `omg_dosimetry-1.4.0/PKG-INFO` & `omg_dosimetry-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omg_dosimetry
-Version: 1.4.0
+Version: 1.4.1
 Summary: Optimized Multichannel Gafchromic Dosimetry (OMG Dosimetry)
 Project-URL: Homepage, https://bitbucket.org/cric_levis/omg-film-dosimetry
 Author-email: JF Cabana <jean-francois.cabana.cisssca@ssss.gouv.qc.ca>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

