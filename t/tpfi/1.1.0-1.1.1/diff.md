# Comparing `tmp/tpfi-1.1.0.tar.gz` & `tmp/tpfi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpfi-1.1.0.tar", max compression
+gzip compressed data, was "tpfi-1.1.1.tar", max compression
```

## Comparing `tpfi-1.1.0.tar` & `tpfi-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-05-14 08:17:57.313763 tpfi-1.1.0/LICENSE
--rw-r--r--   0        0        0     2367 2023-05-14 08:17:57.681764 tpfi-1.1.0/README.md
--rw-r--r--   0        0        0      563 2023-05-14 08:17:57.317763 tpfi-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      154 2023-05-14 08:17:57.317763 tpfi-1.1.0/src/tpfi/__init__.py
--rw-r--r--   0        0        0    15318 2023-05-14 08:17:57.317763 tpfi-1.1.0/src/tpfi/tpfi.py
--rw-r--r--   0        0        0     5333 2023-05-14 08:17:57.321763 tpfi-1.1.0/src/tpfi/utils.py
--rw-r--r--   0        0        0       22 2023-05-14 08:17:57.321763 tpfi-1.1.0/src/tpfi/version.py
--rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 tpfi-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-15 14:53:24.901009 tpfi-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2367 2023-05-15 14:53:25.189011 tpfi-1.1.1/README.md
+-rw-r--r--   0        0        0      563 2023-05-15 14:53:24.905009 tpfi-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-05-15 14:53:24.905009 tpfi-1.1.1/src/tpfi/__init__.py
+-rw-r--r--   0        0        0    15319 2023-05-15 14:53:24.905009 tpfi-1.1.1/src/tpfi/tpfi.py
+-rw-r--r--   0        0        0     5333 2023-05-15 14:53:24.905009 tpfi-1.1.1/src/tpfi/utils.py
+-rw-r--r--   0        0        0       22 2023-05-15 14:53:24.905009 tpfi-1.1.1/src/tpfi/version.py
+-rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 tpfi-1.1.1/PKG-INFO
```

### Comparing `tpfi-1.1.0/LICENSE` & `tpfi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tpfi-1.1.0/README.md` & `tpfi-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tpfi-1.1.0/pyproject.toml` & `tpfi-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tpfi"
-version = "1.1.0"
+version = "1.1.1"
 description = "Plot identification charts for Kepler, K2 and TESS."
 authors = ["Keyu Xing <kyxing@mail.bnu.edu.cn>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/keyuxing/tpfi"
 repository = "https://github.com/keyuxing/tpfi"
```

### Comparing `tpfi-1.1.0/src/tpfi/tpfi.py` & `tpfi-1.1.1/src/tpfi/tpfi.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,30 +198,31 @@
     ax_tpf.invert_xaxis()
 
     if r is None:
         at = AnchoredText("No Gaia DR3 Data", frameon=False, loc="upper left", prop=dict(size=13))
         ax_tpf.add_artist(at)
     else:
         target_gaia_id = r[0]["source_id"]
+        target_gaia_mag = r[0]["phot_g_mean_mag"]
+
         r.sort("phot_g_mean_mag")
         this = np.nonzero(r["source_id"] == target_gaia_id)[0][0]
-        magnitude_limit = max(r["phot_g_mean_mag"][0] + 3, mag_limit)
+        magnitude_limit = max(target_gaia_mag + 3, mag_limit)
         r = r[r["phot_g_mean_mag"] < magnitude_limit][: max(this + 50, 300)]
 
         qr = QTable([r["ra"].filled(), r["dec"].filled(), r["pmra"].filled(0), r["pmdec"].filled(0)])
         coords_gaia = SkyCoord(
             qr["ra"], qr["dec"], pm_ra_cosdec=qr["pmra"], pm_dec=qr["pmdec"], frame="icrs", obstime=REF_EPOCH
         )
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=ErfaWarning)
             coords_obs = coords_gaia.apply_space_motion(new_obstime=tpf.time[0])
 
         x, y = tpf.wcs.world_to_pixel(coords_obs)
         gaia_mags = np.asarray(r["phot_g_mean_mag"])
-        target_gaia_mag = gaia_mags[this]
 
         size_k = 1.2 * np.piecewise(
             target_gaia_mag,
             [target_gaia_mag < 12, 12 <= target_gaia_mag < mag_limit, target_gaia_mag > mag_limit],
             [70, lambda mag: 190 - mag * 10, 10],
         )
         if tpf.meta["TELESCOP"] != "TESS":
```

### Comparing `tpfi-1.1.0/src/tpfi/utils.py` & `tpfi-1.1.1/src/tpfi/utils.py`

 * *Files identical despite different names*

### Comparing `tpfi-1.1.0/PKG-INFO` & `tpfi-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpfi
-Version: 1.1.0
+Version: 1.1.1
 Summary: Plot identification charts for Kepler, K2 and TESS.
 Home-page: https://github.com/keyuxing/tpfi
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

