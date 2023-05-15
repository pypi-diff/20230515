# Comparing `tmp/starcatalogquery-0.1.3-py3-none-any.whl.zip` & `tmp/starcatalogquery-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 26764 bytes, number of entries: 17
+Zip file size: 27158 bytes, number of entries: 17
 -rw-r--r--  2.0 unx       33 b- defN 23-May-08 07:01 starcatalogquery/__init__.py
 -rw-r--r--  2.0 unx     6048 b- defN 23-May-09 01:27 starcatalogquery/catalog_check.py
 -rw-r--r--  2.0 unx     6716 b- defN 23-May-09 01:26 starcatalogquery/catalog_download.py
 -rw-r--r--  2.0 unx    15124 b- defN 23-May-08 13:32 starcatalogquery/catalog_query.py
--rw-r--r--  2.0 unx    50907 b- defN 23-May-11 15:16 starcatalogquery/classes.py
--rw-r--r--  2.0 unx     3091 b- defN 23-May-11 15:15 starcatalogquery/invariantfeatures.py
+-rw-r--r--  2.0 unx    51653 b- defN 23-May-15 02:03 starcatalogquery/classes.py
+-rw-r--r--  2.0 unx     3078 b- defN 23-May-12 08:00 starcatalogquery/invariantfeatures.py
 -rw-r--r--  2.0 unx     5624 b- defN 23-May-10 03:48 starcatalogquery/tiles_draw.py
 -rw-r--r--  2.0 unx     1937 b- defN 23-May-09 08:46 starcatalogquery/wcs.py
 -rw-r--r--  2.0 unx        1 b- defN 23-May-11 04:20 starcatalogquery/utils/__init__.py
 -rw-r--r--  2.0 unx      612 b- defN 23-May-09 08:08 starcatalogquery/utils/df2info.py
 -rw-r--r--  2.0 unx     4272 b- defN 23-May-09 08:33 starcatalogquery/utils/starcatalog_statistic.py
 -rw-r--r--  2.0 unx      477 b- defN 23-May-09 08:06 starcatalogquery/utils/try_download.py
--rw-r--r--  2.0 unx     1068 b- defN 23-May-11 15:26 starcatalogquery-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    11946 b- defN 23-May-11 15:26 starcatalogquery-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 15:26 starcatalogquery-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-11 15:26 starcatalogquery-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1510 b- defN 23-May-11 15:26 starcatalogquery-0.1.3.dist-info/RECORD
-17 files, 109475 bytes uncompressed, 24244 bytes compressed:  77.9%
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-15 02:08 starcatalogquery-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12383 b- defN 23-May-15 02:08 starcatalogquery-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 02:08 starcatalogquery-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-15 02:08 starcatalogquery-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1510 b- defN 23-May-15 02:08 starcatalogquery-0.1.4.dist-info/RECORD
+17 files, 110645 bytes uncompressed, 24638 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: starcatalogquery/utils/starcatalog_statistic.py
 Comment: 
 
 Filename: starcatalogquery/utils/try_download.py
 Comment: 
 
-Filename: starcatalogquery-0.1.3.dist-info/LICENSE
+Filename: starcatalogquery-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: starcatalogquery-0.1.3.dist-info/METADATA
+Filename: starcatalogquery-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: starcatalogquery-0.1.3.dist-info/WHEEL
+Filename: starcatalogquery-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: starcatalogquery-0.1.3.dist-info/top_level.txt
+Filename: starcatalogquery-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: starcatalogquery-0.1.3.dist-info/RECORD
+Filename: starcatalogquery-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## starcatalogquery/classes.py

```diff
@@ -3,14 +3,15 @@
 import pandas as pd
 import numpy as np
 from pathlib import Path
 from astropy.time import Time
 from astropy.coordinates import SkyCoord
 from colorama import Fore
 import healpy as hp
+from scipy.spatial import KDTree
 
 from .catalog_download import catalog_download,hygv3_download
 from .catalog_check import catalog_check
 from .utils.starcatalog_statistic import tiles_statistic,starcatalog_info
 from .utils.df2info import df2info
 from .catalog_query import search_box,search_cone,search_box_magpm,search_cone_magpm,box2seqs,cone2seqs,_load_files
 from .tiles_draw import search_draw
@@ -907,74 +908,74 @@
 
         Outputs:
             An image that shows the scope of the search area and the coverage of the corresponding tiles.          
         """
         width = int(self.tile_size.split()[0]) 
         search_draw(width,kwargs)   
 
-    def h5_incices(self,fov,pixel_width,max_control_points=40):
+    def h5_incices(self,fov,pixel_width,max_control_points=60):
         """
         Generate a h5-formatted star catalog file, which records the center pointing of each sky area, the pixel coordinates of the stars, the triangle invariants and the asterism indices.
 
         Usage:
             >>> from starcatalogquery import StarCatalogSimplified
             >>> # load the simplified star catalog GAIADR3
             >>> dir_from_simplified = '/Volumes/TOSHIBA/starcatalog/simplified/gaiadr3/res2/'
             >>> gaiadr3_simplified = StarCatalogSimplified.load('simplified','gaiadr3',2,dir_from_simplified)
             >>> outh5 = gaiadr3_simplified.h5_incices(20,0.01)
 
         Inputs:
             fov -> [float] FOV of camera
             pixel_width -> [float] Pixel width in [deg]
-            max_control_points -> [int,optional,default=None] Number of brightest stars in the search area. If None, it is the number of all stars in the search area by deault.
+            max_control_points -> [int,optional,default=60] Number of brightest stars in the search area.
 
         Outputs:
             h5-formatted star catalog file    
         """ 
         dir_h5 = 'starcatalogs/indices/{:s}/'.format(self.sc_name)
         Path(dir_h5).mkdir(parents=True, exist_ok=True)  
 
-        outh5 = dir_h5 + 'fov{:d}_mag{:d}_mcp{:d}_{:.1f}.h5'.format(fov,self.mag_cutoff,max_control_points,self.epoch)
+        outh5 = dir_h5 + 'fov{:d}_mag{:.1f}_mcp{:d}_{:.1f}.h5'.format(fov,self.mag_cutoff,max_control_points,self.epoch)
 
         if os.path.exists(outh5): return outh5 
 
         # write to h5 file
         fout = h5py.File(outh5,'w')
         # create group 
         stars_xy_grp = fout.create_group("stars_xy")
         stars_invariants_grp = fout.create_group("stars_invariants")
         stars_asterisms_grp = fout.create_group("stars_asterisms")
 
-        if fov > 30: 
+        if fov > 43: 
             nside = 1
-            search_radius = 60
-        elif fov > 10:
+            search_radius = 34
+        elif fov > 22:
             nside = 2
-            search_radius = 30
+            search_radius = 17
         else:
             nside = 4
-            search_radius = 15
+            search_radius = 9
 
         npix = hp.nside2npix(nside)
         fp_radecs = []
         for seq in range(npix):
 
             desc = 'Generating starcatalog sky area index {:s}{:d}{:s} of {:d}'.format(Fore.BLUE,seq+1,Fore.RESET,npix)
             print(desc,end='\r')
 
             fp_radec = hp.pix2ang(nside,seq,lonlat=True)
             fp_radecs.append(fp_radec)
 
             stars = self.search_cone(fp_radec,search_radius,max_control_points)
-            pixels = stars.pixel_xy(pixel_width)
+            stars = stars.pixel_xy(pixel_width)
+            stars = stars.invariantfeatures()
 
-            stars_xy_grp.create_dataset(str(seq), data=pixels.xy)
-            stars_invariants, stars_asterisms = _generate_invariants(pixels.xy)
-            stars_invariants_grp.create_dataset(str(seq), data=stars_invariants)
-            stars_asterisms_grp.create_dataset(str(seq), data=stars_asterisms)  
+            stars_xy_grp.create_dataset(str(seq), data=stars.xy)
+            stars_invariants_grp.create_dataset(str(seq), data=stars.invariants)
+            stars_asterisms_grp.create_dataset(str(seq), data=stars.asterisms)  
 
         fout.create_dataset("fp_radecs", data=np.array(fp_radecs))
         fout.close() # close file
         return outh5
             
 class Stars(object):
     """
@@ -1025,8 +1026,21 @@
         x,y = xy_catalog(self.center,self.radec,pixel_width)
 
         info = copy.deepcopy(self.info)
         df = info['df']
         df['pixelx'],df['pixely'] = x,y
         info['xy'] = np.stack([x,y]).T
 
-        return Stars(info)
+        return Stars(info)
+
+    def invariantfeatures(self):
+        """
+        1. Calculate the unique invariants (L2/L1,L1/L0), where L2 >= L1 >= L0 are the three sides of the triangle composed of stars.
+        2. Construct the 2D Tree from the the unique invariants.
+        3. Record an array of the indices of stars that correspond to each invariant.
+        """
+        if not hasattr(self,'xy'): raise Exception("The pixel coordinates of stars should be caiculated first by `.pixel_xy(pixel_width`)")
+        inv_uniq, triang_vrtx_uniq = _generate_invariants(self.xy)
+        inv_uniq_tree = KDTree(inv_uniq)
+        self.info.update({'invariants':inv_uniq,'asterisms':triang_vrtx_uniq,'invariants_2dtree':inv_uniq_tree})
+        self.invariants,self.asterisms,self.kdtree = inv_uniq,triang_vrtx_uniq,inv_uniq_tree
+        return self
```

## starcatalogquery/invariantfeatures.py

```diff
@@ -1,12 +1,15 @@
 """
 Some slightly modified subroutines of package ASTROALIGN from Martin Beroiz.
 """
 
 import numpy as _np
+from scipy.spatial import KDTree
+from itertools import combinations
+from functools import partial
 
 # The number of nearest neighbors of a given star(including itself) to construct the triangle invariants.
 NUM_NEAREST_NEIGHBORS = 6
 
 def _invariantfeatures(x1, x2, x3):
     """
     Given 3 points x1, x2, x3, return the invariant features for the set.
@@ -49,29 +52,25 @@
 
 def _generate_invariants(sources):
     """
     Return an array of (unique) invariants derived from the array `sources`.
     Return an array of the indices of `sources` that correspond to each
     invariant, arranged as described in _arrangetriplet.
     """
-    from scipy.spatial import KDTree
-    from itertools import combinations
-    from functools import partial
-
     arrange = partial(_arrangetriplet, sources=sources)
 
     inv = []
     triang_vrtx = []
     coordtree = KDTree(sources)
     # The number of nearest neighbors to request (to work with few sources)
     knn = min(len(sources), NUM_NEAREST_NEIGHBORS)
     for asrc in sources:
         __, indx = coordtree.query(asrc, knn)
 
-        # Generate all possible triangles with the 5 indx provided, and store
+        # Generate all possible triangles with the 6 indx provided, and store
         # them with the order (a, b, c) defined in _arrangetriplet
         all_asterism_triang = [
             arrange(vertex_indices=list(cmb)) for cmb in combinations(indx, 3)
         ]
         triang_vrtx.extend(all_asterism_triang)
 
         inv.extend(
```

## Comparing `starcatalogquery-0.1.3.dist-info/LICENSE` & `starcatalogquery-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `starcatalogquery-0.1.3.dist-info/METADATA` & `starcatalogquery-0.1.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: starcatalogquery
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package to establish an offline star catalog query database
 Home-page: https://github.com/lcx366/STARQUERY
 Author: Chunxiao Li
 Author-email: lcx366@126.com
 License: MIT
-Keywords: Star Catalog
+Keywords: StarCatalog
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scipy
 Requires-Dist: pyshtools
 Requires-Dist: astropy (>=4.3.1)
 Requires-Dist: pandas
 Requires-Dist: colorama
 Requires-Dist: healpy
 Requires-Dist: cartopy
 Requires-Dist: wget
@@ -158,14 +159,21 @@
 
 ```python
 >>> pixel_width = 0.01 # pixel width in [deg]
 >>> stars = gaiadr3_simplified_stars.pixel_xy(0.01)
 >>> print(stars.xy)
 ```
 
+### Calculate the triangle invariants and the asterism indices of the filtered stars
+
+```python
+>>> stars.invariantfeatures()
+>>> print(stars.invariants,stars.asterisms,stars.kdtree)
+```
+
 ### Visualization
 
 Visualize the scope of the search area and the coverage of the corresponding catalog tiles.
 
 ```python
 >>> kwargs_box = {'box':[5,15,35,45]} # {'box':[ra_min,dec_min,ra_max,dec_max]}
 >>> kwargs_cone = {'cone':[20,30,15]} # {'cone':[ra_c,dec_c,radius]}
@@ -192,24 +200,24 @@
 
 <p align="middle">
   <img src="readme_figs/healpix_table.png" width="400" />
 </p>
 
 By default, we adopt the following strategy to divide the sky area:
 
-- For FOV > 30, k = 0; 
+- For FOV > 43, k = 0; 
 
-- For FOV > 10, k = 1;
+- For FOV > 22, k = 1;
 
 - Else, k = 2
 
 ```python
 >>> fov,pixel_width = 20,0.01 # in [deg]
 >>> # Set the maximum number of brightest stars in earch sky area
->>> max_control_points = 40 # optional, default = 40
+>>> max_control_points = 40 # optional, default = 60
 >>> outh5 = gaiadr3_simplified.h5_incices(fov,pixel_width,max_control_points)
 ```
 
 A h5-formatted star catalog file `outh5`is generated, which records the center pointing of each sky area, the pixel coordinates, the triangle invariants and the asterism indices of the stars.
 
 ### Read in h5-formatted star catalog file
 
@@ -217,39 +225,43 @@
 >>> from starcatalogquery import StarCatalog
 >>> infile_h5 = 'starcatalogs/indices/hygv3/fov20_mag8_mcp40_2023.0.h5'
 >>> fp_radecs,stars_xy,stars_invariants,stars_asterisms = StarCatalog.read_h5_indices(infile_h5)
 ```
 
 ### Load the local offline star catalog database
 
-Load the raw star catalog
+#### Load the raw or reduced star catalog
 
 ```python
 >>> from starcatalogquery import StarCatalog
 >>> sc_name = 'hygv3' # Name of the star catalog
 >>> tile_size = 2 # Size of the tile in [deg]
 >>> dir_from_raw = '/Volumes/TOSHIBA/starcatalogs/raw/hygv3/res2/' # Path of the raw starcatalog
 >>> hygv3_raw = StarCatalog.load('raw','sc_name',tile_size,dir_from_raw)
 >>> # dir_from_reduced = '/Volumes/TOSHIBA/starcatalogs/reduced/hygv3/res2/' # Path of the reduced starcatalog
 >>> # hygv3_reduced = StarCatalog.load('reduced','sc_name',tile_size,dir_from_reduced)
 ```
 
-Load the simplified star catalog
+#### Load the simplified star catalog
 
 ```python
 >>> from starcatalogquery import StarCatalog
 >>> sc_name = 'hygv3' # Name of the star catalog
 >>> tile_size = 5 # Size of the tile in [deg]
 >>> dir_from_simplified = '/Volumes/TOSHIBA/starcatalogs/raw/hygv3/res5/mag8.0/epoch2023.0/' # Path of the starcatalog
 >>> kwargs = {'mag_cutoff':8,'epoch':2023.0}
 >>> hygv3_raw = StarCatalog.load('simplified','sc_name',tile_size,dir_from_simplified,**kwargs)
 ```
 
 ## Change log
 
+- **0.1.4 — May 13, 2023**
+  
+  - Add method `.invariantfeatures()` to class `Stars`, which calculates the triangle invariants and constructs a 2D Tree; and records the asterism indices for each triangle.
+
 - **0.1.0 — May 10,  2023**
   
   - The ***starcatalogquery*** package was released.
 
 ## Reference
 
 - [MIKULSKI ARCHIVE&SPACE TELESCOPES](https://archive.stsci.edu)
```

## Comparing `starcatalogquery-0.1.3.dist-info/RECORD` & `starcatalogquery-0.1.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 starcatalogquery/__init__.py,sha256=F5XhiD_gjaRsVVK_KfSD9ZkmgQnoNiJQqIMoMsceHRY,33
 starcatalogquery/catalog_check.py,sha256=r6B-MtO3bq3NVRHkyq0xnZxBvTRf8Epmn-thBD53gHo,6048
 starcatalogquery/catalog_download.py,sha256=gDFjQEtwKX56Sdwv7L53YIZKLrLy_3CtbvE3tfyxrvQ,6716
 starcatalogquery/catalog_query.py,sha256=kBY8F25jt_WiLLY_SNJWseHCx0XWVti-b7ToL17csV4,15124
-starcatalogquery/classes.py,sha256=0VQQcu4XWqDY6M_n_eg67fQLOGNt-NurlcofahUhL-o,50907
-starcatalogquery/invariantfeatures.py,sha256=jEqRc1GFN691eWOcSPPH4-mumyemFzytyitBioPk8A8,3091
+starcatalogquery/classes.py,sha256=sHu6NCFNcxyEzA1uva8hqKLZHdRbYdtPpJJjEJKrxnw,51653
+starcatalogquery/invariantfeatures.py,sha256=iJG2K3R4BcbAqkX0I-P0nQYR4Xeo2UpPaQuEqx4CP58,3078
 starcatalogquery/tiles_draw.py,sha256=zsL2lOnfOrb-fWXDSSmdGwdfYWNIL08D84Kvk8Lvc0E,5624
 starcatalogquery/wcs.py,sha256=SMhSDUNat1755eyzwY9A56DZzDBqhz2XVVMBx8SYFQw,1937
 starcatalogquery/utils/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 starcatalogquery/utils/df2info.py,sha256=_eQENb_DxX5Q5EGxbanJuo9nQKBm-A6Tz8pEsLFinxI,612
 starcatalogquery/utils/starcatalog_statistic.py,sha256=xnyKAJFuduuXo3dKkO0B1YoeTlvu-j-BtNtgrRMvZIY,4272
 starcatalogquery/utils/try_download.py,sha256=cTfNaevU_ELwKP3R9SpYQsiGtEvoBETnsi__EdkLSVE,477
-starcatalogquery-0.1.3.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
-starcatalogquery-0.1.3.dist-info/METADATA,sha256=xEyLbwscGxcSyyaRiSsRPdnmqOzFKCggF5I4Ni1ksfc,11946
-starcatalogquery-0.1.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-starcatalogquery-0.1.3.dist-info/top_level.txt,sha256=xZmWsZTK993L9eaiWI9PM0exXZiKw-64leh_79J2M9U,17
-starcatalogquery-0.1.3.dist-info/RECORD,,
+starcatalogquery-0.1.4.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
+starcatalogquery-0.1.4.dist-info/METADATA,sha256=pmLAVRRYr2vJKXFb_Fk2k7rOSsHHr0EZ_Z0Ibrs7deU,12383
+starcatalogquery-0.1.4.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+starcatalogquery-0.1.4.dist-info/top_level.txt,sha256=xZmWsZTK993L9eaiWI9PM0exXZiKw-64leh_79J2M9U,17
+starcatalogquery-0.1.4.dist-info/RECORD,,
```

