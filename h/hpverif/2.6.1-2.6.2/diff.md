# Comparing `tmp/hpverif-2.6.1-py3-none-any.whl.zip` & `tmp/hpverif-2.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 12583 bytes, number of entries: 15
+Zip file size: 12578 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     3046 b- defN 23-May-08 14:15 hpverif/Calibraton.py
 -rw-r--r--  2.0 unx      449 b- defN 23-May-08 15:40 hpverif/Driver.py
 -rw-r--r--  2.0 unx     3961 b- defN 23-May-08 14:15 hpverif/FrameCapture.py
 -rw-r--r--  2.0 unx     2576 b- defN 23-May-08 14:15 hpverif/FrameCapturePLY.py
 -rw-r--r--  2.0 unx     3967 b- defN 23-May-08 14:15 hpverif/PointCloud.py
--rw-r--r--  2.0 unx     5597 b- defN 23-May-11 22:36 hpverif/Segmentation.py
+-rw-r--r--  2.0 unx     5584 b- defN 23-May-15 15:28 hpverif/Segmentation.py
 -rw-r--r--  2.0 unx     2443 b- defN 23-May-08 14:15 hpverif/ShowFiles.py
 -rw-r--r--  2.0 unx     4934 b- defN 23-May-08 14:15 hpverif/Theoretical_distance.py
 -rw-r--r--  2.0 unx     1876 b- defN 23-May-11 22:37 hpverif/Verification.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-08 14:15 hpverif/__init__.py
 -rw-r--r--  2.0 unx      389 b- defN 23-May-08 14:15 hpverif/driver.py
--rw-r--r--  2.0 unx      321 b- defN 23-May-11 22:58 hpverif-2.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 22:58 hpverif-2.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-May-11 22:58 hpverif-2.6.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1159 b- defN 23-May-11 22:58 hpverif-2.6.1.dist-info/RECORD
-15 files, 30818 bytes uncompressed, 10683 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx      321 b- defN 23-May-15 15:28 hpverif-2.6.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 15:28 hpverif-2.6.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-15 15:28 hpverif-2.6.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1159 b- defN 23-May-15 15:28 hpverif-2.6.2.dist-info/RECORD
+15 files, 30805 bytes uncompressed, 10678 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: hpverif/__init__.py
 Comment: 
 
 Filename: hpverif/driver.py
 Comment: 
 
-Filename: hpverif-2.6.1.dist-info/METADATA
+Filename: hpverif-2.6.2.dist-info/METADATA
 Comment: 
 
-Filename: hpverif-2.6.1.dist-info/WHEEL
+Filename: hpverif-2.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: hpverif-2.6.1.dist-info/top_level.txt
+Filename: hpverif-2.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: hpverif-2.6.1.dist-info/RECORD
+Filename: hpverif-2.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hpverif/Segmentation.py

```diff
@@ -53,15 +53,15 @@
 
         depth_values_obj= np.asarray(inlier_cloud.points)[:,2]
         varianza = np.var(depth_values_obj)
         print("Variance of second Detection: " +str(varianza))
 
         segment = 0
         depth_value_obj= ((np.mean(depth_values_obj)/self.fact)*self.max)+self.min
-        if(theta < 8 or varianza <100):
+        if(varianza <100):
             print("Distance to Object: " + str(depth_value_obj))
         else:
             segment=1
             print("DIstance to Floor " + str(depth_value_obj))
 
         return depth_value_plane,depth_value_obj, segment
```

## Comparing `hpverif-2.6.1.dist-info/RECORD` & `hpverif-2.6.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 hpverif/Calibraton.py,sha256=3_apH-bhEFaYuS4uhOipNU8I4CG_9ubnpSvyJvvmeXA,3046
 hpverif/Driver.py,sha256=Ra-CMqpmRVMUhNoB5H3lYtz7_u5kHI8_umIvbVjOrco,449
 hpverif/FrameCapture.py,sha256=TH7-3ZDrAwIEckOjmM6oeYtGcD0cfx_4GgG78qHeWhk,3961
 hpverif/FrameCapturePLY.py,sha256=PK6Ki_7RZrIizsvZXJL4ixMeVrMG6ESU7vKrMOafbKA,2576
 hpverif/PointCloud.py,sha256=TreRhzS2rbdM2SovJZz-gXDRSpSfxRdqrqNp7fRb04Y,3967
-hpverif/Segmentation.py,sha256=1zOubQBwhR3Qo3kxe6-D4YstON4rId6VXreMoaT1eqY,5597
+hpverif/Segmentation.py,sha256=eZFBV1NC5ALDI9fvfiyeRcSWdmDvcBM2KhMIJpXF9Ow,5584
 hpverif/ShowFiles.py,sha256=vofjelAT-1kIfQC6KB6B_Vu-NljtjvZeV-uidOOOslk,2443
 hpverif/Theoretical_distance.py,sha256=AZMGa1AavpwJ_Ilk20II-2Ac52dEbG33SGbDglhhbHE,4934
 hpverif/Verification.py,sha256=H6gtRaBNU239j56JVoWV3GxVjIAO7g3WOqljHnN-Bmk,1876
 hpverif/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hpverif/driver.py,sha256=-Y_3y4xh1Gtygx3AruRyzaBszP15mLxSS0toIuZ_qO8,389
-hpverif-2.6.1.dist-info/METADATA,sha256=c1Vd5ml9maH1XGIeZDkW36NnUe8ZkWOEwLo_MZGU1vc,321
-hpverif-2.6.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-hpverif-2.6.1.dist-info/top_level.txt,sha256=XZSD1QWULYM6ehhNqJ8z6ssxrXEfKSsM1Gk2hv4UMcw,8
-hpverif-2.6.1.dist-info/RECORD,,
+hpverif-2.6.2.dist-info/METADATA,sha256=xirPyg4SLslSv-iTXyFQXs3Ixbv8HBhj_jkk02C9p1M,321
+hpverif-2.6.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+hpverif-2.6.2.dist-info/top_level.txt,sha256=XZSD1QWULYM6ehhNqJ8z6ssxrXEfKSsM1Gk2hv4UMcw,8
+hpverif-2.6.2.dist-info/RECORD,,
```

