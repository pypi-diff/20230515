# Comparing `tmp/colorsysx-0.2a1.tar.gz` & `tmp/colorsysx-0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorsysx-0.2a1.tar", last modified: Mon May 15 12:23:23 2023, max compression
+gzip compressed data, was "colorsysx-0.2a2.tar", last modified: Mon May 15 12:34:58 2023, max compression
```

## Comparing `colorsysx-0.2a1.tar` & `colorsysx-0.2a2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      506 2023-05-13 17:41:09.960408 colorsysx-0.2a1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       53 2023-05-11 22:49:25.520127 colorsysx-0.2a1/.gitignore
--rw-r--r--   0        0        0    32422 2023-05-11 09:15:26.337556 colorsysx-0.2a1/LICENSE
--rw-r--r--   0        0        0     3082 2023-05-15 12:22:59.382536 colorsysx-0.2a1/README.md
--rw-r--r--   0        0        0     1448 2023-05-13 19:38:00.135300 colorsysx-0.2a1/colorsysx/__init__.py
--rw-r--r--   0        0        0     5538 2023-05-15 12:22:59.386536 colorsysx-0.2a1/colorsysx/_glhs.py
--rw-r--r--   0        0        0     4279 2023-05-15 12:22:59.386536 colorsysx-0.2a1/colorsysx/_hcy.py
--rw-r--r--   0        0        0      379 2023-05-11 02:07:41.913560 colorsysx-0.2a1/colorsysx/_helpers.py
--rw-r--r--   0        0        0      741 2023-05-13 16:25:55.939388 colorsysx-0.2a1/colorsysx/_swizzle.py
--rw-r--r--   0        0        0     2760 2023-05-13 16:30:36.870102 colorsysx-0.2a1/colorsysx/_yuv.py
--rw-r--r--   0        0        0     1807 2023-05-13 00:51:20.967395 colorsysx-0.2a1/colorsysx/weights.py
--rw-r--r--   0        0        0      688 2023-05-13 18:47:24.806900 colorsysx-0.2a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-13 01:06:47.992623 colorsysx-0.2a1/tests/__init__.py
--rw-r--r--   0        0        0      319 2023-05-13 01:01:00.825464 colorsysx-0.2a1/tests/context.py
--rw-r--r--   0        0        0     3703 2023-05-15 12:22:59.386536 colorsysx-0.2a1/tests/test_glhs.py
--rw-r--r--   0        0        0     2749 2023-05-15 12:22:59.386536 colorsysx-0.2a1/tests/test_hcy.py
--rw-r--r--   0        0        0      592 2023-05-13 16:25:28.626827 colorsysx-0.2a1/tests/test_swizzle.py
--rw-r--r--   0        0        0      799 2023-05-13 01:05:35.215977 colorsysx-0.2a1/tests/test_weights.py
--rw-r--r--   0        0        0     1673 2023-05-13 01:06:48.008623 colorsysx-0.2a1/tests/test_yuv.py
--rw-r--r--   0        0        0      865 2023-05-13 19:25:52.937780 colorsysx-0.2a1/tox.ini
--rw-r--r--   0        0        0     3609 1970-01-01 00:00:00.000000 colorsysx-0.2a1/PKG-INFO
+-rw-r--r--   0        0        0      506 2023-05-13 17:41:09.960408 colorsysx-0.2a2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       53 2023-05-11 22:49:25.520127 colorsysx-0.2a2/.gitignore
+-rw-r--r--   0        0        0    32422 2023-05-15 12:34:48.810921 colorsysx-0.2a2/LICENSE
+-rw-r--r--   0        0        0     3191 2023-05-15 12:23:34.051206 colorsysx-0.2a2/README.md
+-rw-r--r--   0        0        0     1448 2023-05-15 12:25:11.137654 colorsysx-0.2a2/colorsysx/__init__.py
+-rw-r--r--   0        0        0     5553 2023-05-15 12:23:34.055206 colorsysx-0.2a2/colorsysx/_glhs.py
+-rw-r--r--   0        0        0     4471 2023-05-15 12:23:34.055206 colorsysx-0.2a2/colorsysx/_hcy.py
+-rw-r--r--   0        0        0      379 2023-05-11 02:07:41.913560 colorsysx-0.2a2/colorsysx/_helpers.py
+-rw-r--r--   0        0        0      741 2023-05-13 16:25:55.939388 colorsysx-0.2a2/colorsysx/_swizzle.py
+-rw-r--r--   0        0        0     2760 2023-05-13 16:30:36.870102 colorsysx-0.2a2/colorsysx/_yuv.py
+-rw-r--r--   0        0        0     1807 2023-05-13 00:51:20.967395 colorsysx-0.2a2/colorsysx/weights.py
+-rw-r--r--   0        0        0      688 2023-05-15 12:34:48.810921 colorsysx-0.2a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-13 01:06:47.992623 colorsysx-0.2a2/tests/__init__.py
+-rw-r--r--   0        0        0      319 2023-05-13 01:01:00.825464 colorsysx-0.2a2/tests/context.py
+-rw-r--r--   0        0        0     5702 2023-05-15 12:23:34.055206 colorsysx-0.2a2/tests/test_glhs.py
+-rw-r--r--   0        0        0     2677 2023-05-15 12:23:34.055206 colorsysx-0.2a2/tests/test_hcy.py
+-rw-r--r--   0        0        0      592 2023-05-13 16:25:28.626827 colorsysx-0.2a2/tests/test_swizzle.py
+-rw-r--r--   0        0        0      799 2023-05-13 01:05:35.215977 colorsysx-0.2a2/tests/test_weights.py
+-rw-r--r--   0        0        0     1673 2023-05-13 01:06:48.008623 colorsysx-0.2a2/tests/test_yuv.py
+-rw-r--r--   0        0        0      865 2023-05-13 19:25:52.937780 colorsysx-0.2a2/tox.ini
+-rw-r--r--   0        0        0     3718 1970-01-01 00:00:00.000000 colorsysx-0.2a2/PKG-INFO
```

### Comparing `colorsysx-0.2a1/LICENSE` & `colorsysx-0.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `colorsysx-0.2a1/README.md` & `colorsysx-0.2a2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 * **HCY**: a cylindrical hue, relative chroma, and luma model.
 * **GLHS**: a _generalized_ lightness/hue/saturation model.
 
 [YUV][1] has a perceptually relevant lightness term. It can preserve
 absolute chroma when manipulating luma.
 
 [HCY][2] is intuitive to use, and its lightness term is the same as
-YUV's. It's particularly useful when manipulating colours to meet WCAG
-2.2 or draft 3.0 WCAG contrast criteria.
+YUV's. It's particularly useful when manipulating colours to meet [WCAG
+2.2][9] or [draft 3.0 WCAG][10] contrast criteria.
 
 [GLHS][3] is a generalization of the cylindrical coordinate spaces
 provided in `colorsysx` and `colorsys`. It can be parameterised to
 provide any of the other similar models.
 
 # For developers
 
 ColorsysX is library code, with no bundled scripts. Other projects are
-free to depend on it inthe normal way.
+free to depend on it in the normal way.
 
 ## Installation
 
 To install the [latest version from PyPI][4], for example into your
 current Python virtual environment:
 
 ```sh
@@ -87,7 +87,9 @@
 [2]: https://chilliant.com/rgb2hsv.html
 [3]: https://doi.org/10.1006/cgip.1993.1019
 [4]: https://pypi.org/project/colorsysx/
 [5]: https://github.com/achadwick/python-colorsysx
 [6]: https://github.com/achadwick/python-colorsysx/issues
 [7]: https://tox.wiki/
 [8]: https://flit.pypa.io
+[9]: https://www.w3.org/TR/WCAG22/#dfn-contrast-ratio
+[10]: https://github.com/Myndex/SAPC-APCA/
```

### Comparing `colorsysx-0.2a1/colorsysx/__init__.py` & `colorsysx-0.2a2/colorsysx/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 See the corresponding module help texts for further details about each
 model. All of the colour spaces added by this package can be
 parameterized to tune them for different tasks. See the
 colorsysx.weights module for details.
 
 """
 
-__version__ = "0.2a1"
+__version__ = "0.2a2"
 
 # Imports::
 
 # Import just the functions,
 # people wanting weights can import .weights submodule.
 from ._yuv import rgb_to_yuv, yuv_to_rgb  # noqa: F401
 from ._hcy import rgb_to_hcy, hcy_to_rgb  # noqa: F401
```

### Comparing `colorsysx-0.2a1/colorsysx/_glhs.py` & `colorsysx-0.2a2/colorsysx/_glhs.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             = sorted(zip([r, g, b], w_rgb))
     else:
         w_min, w_mid, w_max = w_min2max
         c_min, c_mid, c_max = sorted([r, g, b])
 
     # Handle the achromatic case first to avoid a division by zero later.
     if c_max == c_min:
-        return (c_max, 0., 0.)
+        return (c_max, 0.0, 0.0)
 
     # Compute hue
     mid_minus_min = c_mid - c_min
     max_minus_min = c_max - c_min
     max_minus_mid = c_max - c_mid
     if r > g >= b:
         sector = 0
@@ -130,43 +130,43 @@
     # Pick a sector based on the hue angle.
     # This determines the order in which {r, g, b} are selected from
     # the {min, mid, max} components we're going to be calculating
     # later.
     sector = int((h % 1.0) * 6.0)
     f = ((h % 1.0) * 6.0) - sector
     if (sector % 2) == 0:
-        g = f
+        ff = f
     else:
-        g = 1.0 - f
+        ff = 1.0 - f
 
     # If the weights are in RGB order,
     # swizzle them back into min-to-max order now.
     if w_rgb is not None:
         mapping_indices = _swizzle.FROM_RGB_TO_MIN2MAX[sector]
         w_min2max = tuple(w_rgb[i] for i in mapping_indices)
     w_min, w_mid, w_max = w_min2max
 
     # Calculate the RGB components in min-to-max order
-    l_q = (w_mid * g) + w_max
+    l_q = (w_mid * ff) + w_max
     if l <= l_q:
         c_min = (1 - s) * l
         c_mid = (
-            ((g * l) + (c_min * ((1-g)*w_max - (g*w_min)))) /
-            (w_max + (g * w_mid))
+            ((ff * l) + (c_min * ((1-ff)*w_max - (ff*w_min)))) /
+            (w_max + (ff * w_mid))
         )
         c_max = (l - (w_mid * c_mid) - (w_min * c_min)) / w_max
     else:
         c_max = s + ((1 - s) * l)
         c_mid = (
-            (((1 - g)*l) - (c_max * (((1-g)*w_max) - (g*w_min)))) /
-            (((1-g)*w_mid) + w_min)
+            (((1 - ff)*l) - (c_max * (((1-ff)*w_max) - (ff*w_min)))) /
+            (((1-ff)*w_mid) + w_min)
         )
         if w_min > 0:
             c_min = (l - (w_max * c_max) - (w_mid * c_mid)) / w_min
         else:
-            c_min = (c_mid - (g * c_max)) / (1 - g)
+            c_min = (c_mid - (ff * c_max)) / (1 - ff)
 
     # Back to RGB order
     mapping_indices = _swizzle.FROM_MIN2MAX_TO_RGB[sector]
     c_min2max = (c_min, c_mid, c_max)
     c_rgb = tuple(c_min2max[i] for i in mapping_indices)
     return (clamp(c, 0.0, 1.0) for c in c_rgb)
```

### Comparing `colorsysx-0.2a1/colorsysx/_swizzle.py` & `colorsysx-0.2a2/colorsysx/_swizzle.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.2a1/colorsysx/_yuv.py` & `colorsysx-0.2a2/colorsysx/_yuv.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.2a1/colorsysx/weights.py` & `colorsysx-0.2a2/colorsysx/weights.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.2a1/pyproject.toml` & `colorsysx-0.2a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `colorsysx-0.2a1/tests/test_glhs.py` & `colorsysx-0.2a2/tests/test_glhs.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,39 +8,53 @@
 from sys import float_info
 import itertools
 
 
 # Module vars::
 
 EPSILON = float_info.epsilon
-WEIGHTS = (
+WEIGHTS_MIN2MAX = (
     colorsysx.weights.W_MIN2MAX_HSI,
     colorsysx.weights.W_MIN2MAX_HSV,
     colorsysx.weights.W_MIN2MAX_HLS,
 )
+WEIGHTS_RGB = (
+    colorsysx.weights.W_RGB_REC601,
+    colorsysx.weights.W_RGB_REC709,
+    colorsysx.weights.W_RGB_REC2020,
+)
 
 
 # Test funcs::
 
-def test_grey_is_grey():
+def test_grey_is_grey_min2max():
     """Neutral grey is always neutral grey."""
-    for w in WEIGHTS:
+    for w in WEIGHTS_MIN2MAX:
         l, h, s = colorsysx.rgb_to_glhs(0.5, 0.5, 0.5, w_min2max=w)
         assert abs(l - 0.5) <= EPSILON
         assert h <= EPSILON
         assert s <= EPSILON  # just a convention
 
 
-def test_ranges():
+def test_grey_is_grey_rgb():
+    """Neutral grey is always neutral grey."""
+    for w in WEIGHTS_RGB:
+        l, h, s = colorsysx.rgb_to_glhs(0.5, 0.5, 0.5, w_rgb=w)
+        assert abs(l - 0.5) <= EPSILON
+        assert h <= EPSILON
+        assert s <= EPSILON  # just a convention
+
+
+def test_ranges_min2max():
     """Output should lie within the stated bounds, and cover that range"""
     n = 16
     min_l, max_l = [1, 0]
     min_h, max_h = [1, 0]
     min_s, max_s = [1, 0]
-    for w in WEIGHTS:
+    for w in WEIGHTS_MIN2MAX:
         for rn, gn, bn in itertools.product(range(n+1), repeat=3):
             r0, g0, b0 = (rn/n, gn/n, bn/n)
             l, h, s = colorsysx.rgb_to_glhs(r0, g0, b0, w_min2max=w)
             assert 0-EPSILON <= l <= 1+EPSILON
             assert 0-EPSILON <= h <= 1+EPSILON
             assert 0-EPSILON <= s <= 1+EPSILON
             min_l, max_l = min(l, min_l), max(l, max_l)
@@ -50,43 +64,88 @@
     assert max_l > 1-EPSILON
     assert min_h < 1/12
     assert max_h > 1 - 1/12
     assert min_s < EPSILON
     assert max_s > 1-EPSILON
 
 
-def test_round_trips():
+def test_ranges_rgb():
+    """Output should lie within the stated bounds, and cover that range"""
+    n = 16
+    min_l, max_l = [1, 0]
+    min_h, max_h = [1, 0]
+    min_s, max_s = [1, 0]
+    for w in WEIGHTS_RGB:
+        for rn, gn, bn in itertools.product(range(n+1), repeat=3):
+            r0, g0, b0 = (rn/n, gn/n, bn/n)
+            l, h, s = colorsysx.rgb_to_glhs(r0, g0, b0, w_rgb=w)
+            assert 0-EPSILON <= l <= 1+EPSILON
+            assert 0-EPSILON <= h <= 1+EPSILON
+            assert 0-EPSILON <= s <= 1+EPSILON
+            min_l, max_l = min(l, min_l), max(l, max_l)
+            min_h, max_h = min(h, min_h), max(h, max_h)
+            min_s, max_s = min(s, min_s), max(s, max_s)
+    assert min_l < EPSILON
+    assert max_l > 1-EPSILON
+    assert min_h < 1/12
+    assert max_h > 1 - 1/12
+    assert min_s < EPSILON
+    assert max_s > 1-EPSILON
+
+
+def test_round_trips_min2max():
     """Should be able to convert to GHLS and back to RGB accurately."""
     n = 16
-    for w in WEIGHTS:
+
+    for w in WEIGHTS_MIN2MAX:
         for rn, gn, bn in itertools.product(range(n+1), repeat=3):
             r0, g0, b0 = (rn/n, gn/n, bn/n)
             l, h, s = colorsysx.rgb_to_glhs(r0, g0, b0, w_min2max=w)
             assert 0 <= l <= 1
             r1, g1, b1 = colorsysx.glhs_to_rgb(l, h, s, w_min2max=w)
             assert 0 <= r1 <= 1
             assert 0 <= g1 <= 1
             assert 0 <= b1 <= 1
 
-            # See note in test_hcy.test_round_trips()
             fudge = 4
             assert abs(r1 - r0) <= EPSILON*fudge
             assert abs(g1 - g0) <= EPSILON*fudge
             assert abs(b1 - b0) <= EPSILON*fudge
 
 
+def test_round_trips_rgb():
+    """Should be able to convert to GHLS and back to RGB accurately."""
+    n = 16
+
+    for w in WEIGHTS_RGB:
+        for rn, gn, bn in itertools.product(range(n+1), repeat=3):
+            r0, g0, b0 = (rn/n, gn/n, bn/n)
+            l, h, s = colorsysx.rgb_to_glhs(r0, g0, b0, w_rgb=w)
+            assert 0 <= l <= 1
+            r1, g1, b1 = colorsysx.glhs_to_rgb(l, h, s, w_rgb=w)
+            assert 0 <= r1 <= 1
+            assert 0 <= g1 <= 1
+            assert 0 <= b1 <= 1
+
+            # Fudge factor seems pretty high.
+            fudge = 20
+            # Perhaps I should just be testing that 16bpc linear colour
+            # and 8bpc gamma-encoded colour remain unchanged?
+            assert abs(r1 - r0) <= EPSILON*fudge
+            assert abs(g1 - g0) <= EPSILON*fudge
+            assert abs(b1 - b0) <= EPSILON*fudge
+
+
 def test_equivalences():
     """The GHLS funcs can reproduce other models with dedicated funcs."""
     n = 16
+    fudge = 1
     for rn, gn, bn in itertools.product(range(n+1), repeat=3):
         r, g, b = (rn/n, gn/n, bn/n)
 
-        # Don't need much fudge for colorsys funcs
-        fudge = 1   # wow!
-
         # "HLS" double hexcone model
         (gl1, gh1, gs1) = colorsysx.rgb_to_glhs(
             r, g, b,
             w_min2max=colorsysx.weights.W_MIN2MAX_HLS,
         )
         (h1, l1, s1) = colorsys.rgb_to_hls(r, g, b)
         assert abs(gl1 - l1) <= EPSILON*fudge
@@ -99,17 +158,14 @@
             w_min2max=colorsysx.weights.W_MIN2MAX_HSV,
         )
         (h2, s2, v2) = colorsys.rgb_to_hsv(r, g, b)
         assert abs(gl2 - v2) <= EPSILON*fudge
         assert abs(gs2 - s2) <= EPSILON*fudge
         assert abs(gh2 - h2) <= EPSILON*fudge
 
-        # Use more fudge for the standalone HCY stuff
-        fudge = 4
-
         # "HCY" luma-based model
         (gl3, gh3, gs3) = colorsysx.rgb_to_glhs(
             r, g, b,
             w_rgb=colorsysx.weights.W_RGB_REC709,
         )
         (h3, c3, y3) = colorsysx.rgb_to_hcy(
             r, g, b,
```

### Comparing `colorsysx-0.2a1/tests/test_hcy.py` & `colorsysx-0.2a2/tests/test_hcy.py`

 * *Files 16% similar despite different names*

```diff
@@ -74,15 +74,13 @@
             h, c, y = colorsysx.rgb_to_hcy(r0, g0, b0, w_rgb=w)
             assert 0 <= y <= 1
             r1, g1, b1 = colorsysx.hcy_to_rgb(h, c, y, w_rgb=w)
             assert 0 <= r1 <= 1
             assert 0 <= g1 <= 1
             assert 0 <= b1 <= 1
 
-            # Hey hey, big errors.
-            # Do some numeric analysis of the number of ops,
-            # figure out why it's so big.
-            # It's probably fine if it's <= 1/256 though...
-            fudge = 10
+            # Oddly, the current GLHS implementation is worse (20×Epsilon)
+            # for the same 3 sets of coefficients.
+            fudge = 9
             assert abs(r1 - r0) <= EPSILON*fudge
             assert abs(g1 - g0) <= EPSILON*fudge
             assert abs(b1 - b0) <= EPSILON*fudge
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `colorsysx-0.2a1/tests/test_swizzle.py` & `colorsysx-0.2a2/tests/test_swizzle.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.2a1/tests/test_weights.py` & `colorsysx-0.2a2/tests/test_weights.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.2a1/tests/test_yuv.py` & `colorsysx-0.2a2/tests/test_yuv.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.2a1/tox.ini` & `colorsysx-0.2a2/tox.ini`

 * *Files identical despite different names*

### Comparing `colorsysx-0.2a1/PKG-INFO` & `colorsysx-0.2a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorsysx
-Version: 0.2a1
+Version: 0.2a2
 Summary: Extra, human-relevant, colour spaces derived from RGB.
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Multimedia :: Graphics :: Presentation
 Classifier: Topic :: Software Development :: Libraries
@@ -31,25 +31,25 @@
 * **HCY**: a cylindrical hue, relative chroma, and luma model.
 * **GLHS**: a _generalized_ lightness/hue/saturation model.
 
 [YUV][1] has a perceptually relevant lightness term. It can preserve
 absolute chroma when manipulating luma.
 
 [HCY][2] is intuitive to use, and its lightness term is the same as
-YUV's. It's particularly useful when manipulating colours to meet WCAG
-2.2 or draft 3.0 WCAG contrast criteria.
+YUV's. It's particularly useful when manipulating colours to meet [WCAG
+2.2][9] or [draft 3.0 WCAG][10] contrast criteria.
 
 [GLHS][3] is a generalization of the cylindrical coordinate spaces
 provided in `colorsysx` and `colorsys`. It can be parameterised to
 provide any of the other similar models.
 
 # For developers
 
 ColorsysX is library code, with no bundled scripts. Other projects are
-free to depend on it inthe normal way.
+free to depend on it in the normal way.
 
 ## Installation
 
 To install the [latest version from PyPI][4], for example into your
 current Python virtual environment:
 
 ```sh
@@ -100,8 +100,10 @@
 [2]: https://chilliant.com/rgb2hsv.html
 [3]: https://doi.org/10.1006/cgip.1993.1019
 [4]: https://pypi.org/project/colorsysx/
 [5]: https://github.com/achadwick/python-colorsysx
 [6]: https://github.com/achadwick/python-colorsysx/issues
 [7]: https://tox.wiki/
 [8]: https://flit.pypa.io
+[9]: https://www.w3.org/TR/WCAG22/#dfn-contrast-ratio
+[10]: https://github.com/Myndex/SAPC-APCA/
```

