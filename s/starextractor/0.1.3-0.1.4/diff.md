# Comparing `tmp/starextractor-0.1.3-py3-none-any.whl.zip` & `tmp/starextractor-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10151 bytes, number of entries: 10
--rw-r--r--  2.0 unx       31 b- defN 23-May-12 07:36 starextractor/__init__.py
--rw-r--r--  2.0 unx     5713 b- defN 23-May-12 07:03 starextractor/classes.py
+Zip file size: 10229 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       31 b- defN 23-May-12 07:32 starextractor/__init__.py
+-rw-r--r--  2.0 unx     5930 b- defN 23-May-15 01:45 starextractor/classes.py
 -rw-r--r--  2.0 unx     3814 b- defN 23-May-11 09:11 starextractor/image.py
 -rw-r--r--  2.0 unx     3077 b- defN 23-May-12 07:26 starextractor/invariantfeatures.py
 -rw-r--r--  2.0 unx     2937 b- defN 23-Apr-05 07:44 starextractor/plot.py
--rw-r--r--  2.0 unx     1068 b- defN 23-May-12 07:36 starextractor-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4740 b- defN 23-May-12 07:36 starextractor-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-12 07:36 starextractor-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-May-12 07:36 starextractor-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      825 b- defN 23-May-12 07:36 starextractor-0.1.3.dist-info/RECORD
-10 files, 22311 bytes uncompressed, 8739 bytes compressed:  60.8%
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-15 01:57 starextractor-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4743 b- defN 23-May-15 01:57 starextractor-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 01:57 starextractor-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-May-15 01:57 starextractor-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      825 b- defN 23-May-15 01:57 starextractor-0.1.4.dist-info/RECORD
+10 files, 22531 bytes uncompressed, 8817 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: starextractor/invariantfeatures.py
 Comment: 
 
 Filename: starextractor/plot.py
 Comment: 
 
-Filename: starextractor-0.1.3.dist-info/LICENSE
+Filename: starextractor-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: starextractor-0.1.3.dist-info/METADATA
+Filename: starextractor-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: starextractor-0.1.3.dist-info/WHEEL
+Filename: starextractor-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: starextractor-0.1.3.dist-info/top_level.txt
+Filename: starextractor-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: starextractor-0.1.3.dist-info/RECORD
+Filename: starextractor-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## starextractor/classes.py

```diff
@@ -1,8 +1,9 @@
 from photutils.aperture import CircularAperture,aperture_photometry
+from scipy.spatial import KDTree
 
 from .image import read_image,source_extract
 from .plot import show_image
 from .invariantfeatures import _generate_invariants
 
 class AstroImage(object):
     """
@@ -129,19 +130,19 @@
             plot_kwargs = {'mark':(self._apertures,'blue')}
         else:
             plot_kwargs = {'mark':(self._apertures,'blue'),'figname':fig_out}
         show_image(self.image_raw,origin='lower',mask_rectangle=self._mask_rectangle,**plot_kwargs)     
 
     def invariantfeatures(self):
         """
-        Calculate the unique invariants (L2/L1,L1/L0), where L2 >= L1 >= L0 are the three sides of the triangle composed of centroids.
-        At the same time, record an array of the indices of centroids that correspond to each invariant.
+        1. Calculate the unique invariants (L2/L1,L1/L0), where L2 >= L1 >= L0 are the three sides of the triangle composed of centroids.
+        2. Construct the 2D Tree from the the unique invariants.
+        3. Record an array of the indices of centroids that correspond to each invariant.
         """
         inv_uniq, triang_vrtx_uniq = _generate_invariants(self.xy)
-
-        info = self.info.copy()
-        info.update({'invariants':inv_uniq,'asterisms':triang_vrtx_uniq})
-
-        return Source(info)
+        inv_uniq_tree = KDTree(inv_uniq)
+        self.info.update({'invariants':inv_uniq,'asterisms':triang_vrtx_uniq,'invariants_2dtree':inv_uniq_tree})
+        self.invariants,self.asterisms,self.kdtree = inv_uniq,triang_vrtx_uniq,inv_uniq_tree
+        return self
```

## Comparing `starextractor-0.1.3.dist-info/LICENSE` & `starextractor-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `starextractor-0.1.3.dist-info/METADATA` & `starextractor-0.1.4.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starextractor
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package to extract stars from an astronomical image
 Home-page: https://github.com/lcx366/STAREXTRACTOR
 Author: Chunxiao Li
 Author-email: lcx366@126.com
 License: MIT
 Keywords: source extract,stars
 Classifier: Development Status :: 4 - Beta
@@ -77,19 +77,19 @@
 Estimate the centroids coordinates, brightness(sum of gray value within an aperture),  and SNR of star spots.
 
 ```python
 >>> sources = image.find_source(fwhm=12,mask=True)
 >>> print(sources.xy,sources.brightness,sources.snr,sources.offset)
 ```
 
-### Calculate the triangle invariants and the asterism indices of the star spots.
+### Calculate the triangle invariants and construct a 2D Tree; and record the asterism indices for each triangle.
 
 ```python
->>> sources = sources.invariantfeatures()
->>> print(sources.invariants,sources.asterisms)
+>>> sources.invariantfeatures()
+>>> print(sources.invariants,sources.asterisms,sources.kdtree)
 ```
 
 ### Show the extracted sources in image
 
 ```python
 >>> sources.show()
 >>> #sources.show('figs/sources.png') # save image to a file
@@ -97,21 +97,21 @@
 
 <p align="middle">
   <img src="readme_figs/centroids.png" width="500" />
 </p>
 
 ## Change log
 
-- **0.1.3 — May 12,  2023**
+- **0.1.4 — May 14,  2023**
   
   - The class `Centriod` is *deprecated*, and the class `Source` is used instead
-  - Add method `.invariantfeatures()` to class `Source`, which calculates the triangle invariants and the asterism indices of the star spots
+  - Add method `.invariantfeatures()` to class `Source`, which calculates the triangle invariants and construct a 2D Tree; and record the asterism indices for each triangle.
 
 - **0.1.0 — Apr 5,  2023**
   
   - The ***starextractor*** package was released.
 
 ## Reference
 
 - [photutils](https://photutils.readthedocs.io/en/stable/index.html)
 - [Photometry Methods](http://srmastro.uvacreate.virginia.edu/astr313/lectures/photometry/photometry_methods.html)
-- [Astroalign]([Astroalign documentation &mdash; astroalign 2.4.2 documentation](https://astroalign.quatrope.org/en/latest/))
+- [Astroalign](https://astroalign.quatrope.org/en/latest/)
```

## Comparing `starextractor-0.1.3.dist-info/RECORD` & `starextractor-0.1.4.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 starextractor/__init__.py,sha256=DGag1ir8yMtMV4xodLVjbr-PVPe1BCzZxzOx9mNelfg,31
-starextractor/classes.py,sha256=D3mUMrRBPUTntNi1p0HNnZgMb_Htb_v-BhjoL4oOqao,5713
+starextractor/classes.py,sha256=1srWvxCylsQZ-KoQnOPXTgvIha5M2ey9MzY_jyBtidg,5930
 starextractor/image.py,sha256=5WiKMycAwULNO44WOpJZs51IL6LogOb6n80R_G_HqTM,3814
 starextractor/invariantfeatures.py,sha256=XTqNIvRBBpropl5zb6h9EJHySQ5ued82NRM9yaVxKms,3077
 starextractor/plot.py,sha256=Dllpov4H72BOlZjhSLpwbmw9E2fKa5jXXFSNQNIKg-c,2937
-starextractor-0.1.3.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
-starextractor-0.1.3.dist-info/METADATA,sha256=1pnUynLM-7Zxx_W_FyLh4Ls8s3yrpLBDRodCFpsarO8,4740
-starextractor-0.1.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-starextractor-0.1.3.dist-info/top_level.txt,sha256=QBc6fvT33gTCfADa-aXjDX7yfBqb8twQR3BQjM5cwls,14
-starextractor-0.1.3.dist-info/RECORD,,
+starextractor-0.1.4.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
+starextractor-0.1.4.dist-info/METADATA,sha256=P3f7DpUEHr8C3Ej8NcUEc_kOGiGRtfe4bvE5LH6om78,4743
+starextractor-0.1.4.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+starextractor-0.1.4.dist-info/top_level.txt,sha256=QBc6fvT33gTCfADa-aXjDX7yfBqb8twQR3BQjM5cwls,14
+starextractor-0.1.4.dist-info/RECORD,,
```

