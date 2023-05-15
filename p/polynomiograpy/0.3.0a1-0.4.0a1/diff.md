# Comparing `tmp/polynomiograpy-0.3.0a1.tar.gz` & `tmp/polynomiograpy-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polynomiograpy-0.3.0a1.tar", max compression
+gzip compressed data, was "polynomiograpy-0.4.0a1.tar", max compression
```

## Comparing `polynomiograpy-0.3.0a1.tar` & `polynomiograpy-0.4.0a1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-05-02 09:33:04.682513 polynomiograpy-0.3.0a1/LICENSE
--rw-r--r--   0        0        0       68 2023-05-02 09:33:04.683048 polynomiograpy-0.3.0a1/README.md
--rw-r--r--   0        0        0      414 2023-05-09 09:31:09.276312 polynomiograpy-0.3.0a1/polynomiograpy/__init__.py
--rw-r--r--   0        0        0     4797 2023-05-02 09:33:04.685799 polynomiograpy-0.3.0a1/polynomiograpy/cli/__init__.py
--rw-r--r--   0        0        0      970 2023-05-02 09:33:04.686106 polynomiograpy-0.3.0a1/polynomiograpy/common/finite_field.py
--rw-r--r--   0        0        0     1458 2023-05-08 09:49:29.117520 polynomiograpy-0.3.0a1/polynomiograpy/common/polynomial.py
--rw-r--r--   0        0        0     2302 2023-05-08 09:50:57.025154 polynomiograpy-0.3.0a1/polynomiograpy/iterations/__init__.py
--rw-r--r--   0        0        0     1266 2023-05-08 09:31:50.010724 polynomiograpy-0.3.0a1/polynomiograpy/iterations/helpers.py
--rw-r--r--   0        0        0     3146 2023-05-08 09:49:20.206774 polynomiograpy-0.3.0a1/polynomiograpy/iterations/methods.py
--rw-r--r--   0        0        0      915 2023-05-02 09:33:04.687769 polynomiograpy-0.3.0a1/polynomiograpy/roots/__init__.py
--rw-r--r--   0        0        0      931 2023-05-02 09:33:04.688126 polynomiograpy-0.3.0a1/polynomiograpy/roots/helpers.py
--rw-r--r--   0        0        0      737 2023-05-09 09:30:55.687964 polynomiograpy-0.3.0a1/pyproject.toml
--rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 polynomiograpy-0.3.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-02 09:33:04.682513 polynomiograpy-0.4.0a1/LICENSE
+-rw-r--r--   0        0        0       68 2023-05-02 09:33:04.683048 polynomiograpy-0.4.0a1/README.md
+-rw-r--r--   0        0        0      533 2023-05-15 10:04:57.052043 polynomiograpy-0.4.0a1/polynomiograpy/__init__.py
+-rw-r--r--   0        0        0     5528 2023-05-15 10:03:47.370593 polynomiograpy-0.4.0a1/polynomiograpy/cli/__init__.py
+-rw-r--r--   0        0        0      970 2023-05-02 09:33:04.686106 polynomiograpy-0.4.0a1/polynomiograpy/common/finite_field.py
+-rw-r--r--   0        0        0     1458 2023-05-08 09:49:29.117520 polynomiograpy-0.4.0a1/polynomiograpy/common/polynomial.py
+-rw-r--r--   0        0        0     3071 2023-05-09 10:59:36.896531 polynomiograpy-0.4.0a1/polynomiograpy/iterations/__init__.py
+-rw-r--r--   0        0        0     1266 2023-05-08 09:31:50.010724 polynomiograpy-0.4.0a1/polynomiograpy/iterations/helpers.py
+-rw-r--r--   0        0        0     5757 2023-05-09 14:28:28.887254 polynomiograpy-0.4.0a1/polynomiograpy/iterations/methods.py
+-rw-r--r--   0        0        0     2186 2023-05-09 11:22:48.376339 polynomiograpy-0.4.0a1/polynomiograpy/roots/__init__.py
+-rw-r--r--   0        0        0     2001 2023-05-09 10:22:56.186800 polynomiograpy-0.4.0a1/polynomiograpy/roots/helpers.py
+-rw-r--r--   0        0        0      737 2023-05-15 10:04:27.096137 polynomiograpy-0.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 polynomiograpy-0.4.0a1/PKG-INFO
```

### Comparing `polynomiograpy-0.3.0a1/LICENSE` & `polynomiograpy-0.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.3.0a1/polynomiograpy/cli/__init__.py` & `polynomiograpy-0.4.0a1/polynomiograpy/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import numpy as np
 from PIL import Image
 from polynomiograpy.common.finite_field import FiniteField
 from polynomiograpy.common.polynomial import Polynomial
 from polynomiograpy.iterations.methods import available_methods
 from polynomiograpy.iterations import compute_screen_for_single_poly
-from polynomiograpy.roots import compute_screen_for_finite_field_poly
+from polynomiograpy.roots import (
+    compute_screen_for_finite_field_poly,
+    compute_screen_for_finite_field_poly_multi_color,
+)
 
 __all__ = ["run"]
 
 
 def input_with_default(prompt, default):
     res = input(prompt)
     if len(res) < 1:
@@ -29,68 +32,91 @@
             return
         else:
             print("Wrong usage")
 
 
 def run_root():
     print("** Complex Plane Setup **")
-    min_real = int(input_with_default("Min Real (-3): ", "-3"))
-    max_real = int(input_with_default("Max Real (3): ", "3"))
-    min_imag = int(input_with_default("Min Imag (-3): ", "-3"))
-    max_imag = int(input_with_default("Max Imag (3): ", "3"))
+    min_real = float(input_with_default("Min Real (-3): ", "-3"))
+    max_real = float(input_with_default("Max Real (3): ", "3"))
+    min_imag = float(input_with_default("Min Imag (-3): ", "-3"))
+    max_imag = float(input_with_default("Max Imag (3): ", "3"))
     print("** Finite Field **")
     finite_field_elements: str = input_with_default(
         "Finite field elements (1,0): ", "1,0"
     )
     parsed_elements = [int(e) for e in finite_field_elements.split(",")]
     finite_field = FiniteField(elements=parsed_elements)
     min_degree = int(input_with_default("Min degree (1): ", "1"))
     max_degree = int(input_with_default("Max degree (5): ", "5"))
     print("** Output Setup **")
     width = int(input_with_default("Width (1000): ", "1000"))
     height = int(input_with_default("Height (1000): ", "1000"))
+    multi_color = (
+        input_with_default(
+            "Use different color for each degree? (Deg diff must be at most 7) (y/N): ",
+            "n",
+        )
+        == "y"
+    )
     color_range = int(input_with_default("Color range (8): ", "8"))
     output_filename = input_with_default("Output (out.png): ", "out.png")
 
     print(
         f"Generating the output for all polynomials over {finite_field} "
         f"from degree {min_degree} to degree {max_degree}"
     )
     screen = np.zeros([height, width, 3], dtype=np.uint8)
     screen_buffer = np.zeros([height, width, 3], dtype=np.int64)
 
     scale_x = (max_real - min_real) / width
     scale_y = (max_imag - min_imag) / height
     shift_x = (max_real + min_real) / 2
     shift_y = (max_imag + min_imag) / 2
-    compute_screen_for_finite_field_poly(
-        finite_field,
-        min_degree,
-        max_degree,
-        width,
-        height,
-        screen,
-        screen_buffer,
-        scale_x=scale_x,
-        scale_y=scale_y,
-        shift_x=shift_x,
-        shift_y=shift_y,
-        color_range=color_range,
-    )
+    if multi_color:
+        compute_screen_for_finite_field_poly_multi_color(
+            finite_field,
+            min_degree,
+            max_degree,
+            width,
+            height,
+            screen,
+            screen_buffer,
+            scale_x=scale_x,
+            scale_y=scale_y,
+            shift_x=shift_x,
+            shift_y=shift_y,
+            color_range=color_range,
+        )
+    else:
+        compute_screen_for_finite_field_poly(
+            finite_field,
+            min_degree,
+            max_degree,
+            width,
+            height,
+            screen,
+            screen_buffer,
+            scale_x=scale_x,
+            scale_y=scale_y,
+            shift_x=shift_x,
+            shift_y=shift_y,
+            color_range=color_range,
+        )
     im = Image.fromarray(screen, mode="RGB")
     im.save(output_filename, format="PNG")
     print(f"Saved to {output_filename}")
 
 
 def run_iter():
     print("** Complex Plane Setup **")
-    min_real = int(input_with_default("Min Real (-3): ", "-3"))
-    max_real = int(input_with_default("Max Real (3): ", "3"))
-    min_imag = int(input_with_default("Min Imag (-3): ", "-3"))
-    max_imag = int(input_with_default("Max Imag (3): ", "3"))
+    min_real = float(input_with_default("Min Real (-3): ", "-3"))
+    max_real = float(input_with_default("Max Real (3): ", "3"))
+    min_imag = float(input_with_default("Min Imag (-3): ", "-3"))
+    max_imag = float(input_with_default("Max Imag (3): ", "3"))
     print("** Polynomial **")
     coeffs: str = input_with_default(
         "Coefficients from degree d to 0 (1,0,0,1): ", "1,0,0,1"
     )
     parsed_coeffs = [int(e) for e in coeffs.split(",")]
     parsed_coeffs.reverse()
     poly = Polynomial(coeffs=parsed_coeffs)
```

### Comparing `polynomiograpy-0.3.0a1/polynomiograpy/common/finite_field.py` & `polynomiograpy-0.4.0a1/polynomiograpy/common/finite_field.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.3.0a1/polynomiograpy/common/polynomial.py` & `polynomiograpy-0.4.0a1/polynomiograpy/common/polynomial.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.3.0a1/polynomiograpy/iterations/__init__.py` & `polynomiograpy-0.4.0a1/polynomiograpy/iterations/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,22 @@
 __all__ = [
     "compute_screen_for_single_poly",
     "available_methods",
 ]
 
 
 def compute_screen_for_single_poly(
-    method: Literal["newton", "halley", "secant", "steffensen"],
+    method: Literal[
+        "newton",
+        "halley",
+        "inverse_interpolation",
+        "mullers",
+        "secant",
+        "steffensen",
+    ],
     poly: Polynomial,
     delta: float,
     width: int,
     height: int,
     screen: np.ndarray,
     screen_buffer: np.ndarray,
     *,
@@ -48,14 +55,40 @@
                 poly,
                 val,
                 delta,
                 max_iter_count=max_value,
             )
             return iter_count
 
+    elif method == "inverse_interpolation":
+
+        def func(val: complex) -> int:
+            new_val, iter_count = methods.inverse_interpolation_method(
+                poly,
+                val,
+                None,
+                None,
+                delta,
+                max_iter_count=max_value,
+            )
+            return iter_count
+
+    elif method == "mullers":
+
+        def func(val: complex) -> int:
+            new_val, iter_count = methods.mullers_method(
+                poly,
+                val,
+                None,
+                None,
+                delta,
+                max_iter_count=max_value,
+            )
+            return iter_count
+
     elif method == "secant":
 
         def func(val: complex) -> int:
             new_val, iter_count = methods.secant_method(
                 poly,
                 val,
                 None,
```

### Comparing `polynomiograpy-0.3.0a1/polynomiograpy/iterations/helpers.py` & `polynomiograpy-0.4.0a1/polynomiograpy/iterations/helpers.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.3.0a1/polynomiograpy/roots/helpers.py` & `polynomiograpy-0.4.0a1/polynomiograpy/roots/helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -26,7 +26,42 @@
             pass
         else:
             screen_buffer[j, i, channel] += color_intensity_per_root
             if screen_buffer[j, i, channel] > 255:
                 screen_buffer[j, i, channel] = 255
     screen[:, :, channel] = screen_buffer[:, :, channel]
     return np.flipud(screen)
+
+
+def compute_screen_for_roots_multi_color(
+    roots: list[list[int]],
+    width: int,
+    height: int,
+    screen: np.ndarray,
+    screen_buffer: np.ndarray,
+    *,
+    scale_x: float = 1,
+    scale_y: float = 1,
+    shift_x: float = 0,
+    shift_y: float = 0,
+    color_range: int = 8,
+    colors: list[np.ndarray],
+):
+    screen_buffer.fill(0)
+    origin_x = width / 2
+    origin_y = height / 2
+    for deg, roots_ in enumerate(roots):
+        print("Deg:", deg)
+        color = colors[deg]
+        color_resolved = color // color_range
+        for root in roots_:
+            i = int((root.real - shift_x) / scale_x + origin_x)
+            j = int(((root.imag - shift_y) / scale_y + origin_y))
+            if i < 0 or j < 0 or i >= width or j >= height:
+                pass
+            else:
+                screen_buffer[j, i, :] += color_resolved
+                for c in range(3):
+                    if screen_buffer[j, i, c] > 255:
+                        screen_buffer[j, i, c] = 255
+    screen[:, :, :] = screen_buffer[:, :, :]
+    return np.flipud(screen)
```

### Comparing `polynomiograpy-0.3.0a1/pyproject.toml` & `polynomiograpy-0.4.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polynomiograpy"
-version = "0.3.0.a1"
+version = "0.4.0.a1"
 description = ""
 authors = ["İsmail Tapan <ismltpn@gmail.com>"]
 maintainers = ["İsmail Tapan <ismltpn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = ""
 repository = "https://github.com/ismltpn/polynomiograpy/"
```

### Comparing `polynomiograpy-0.3.0a1/PKG-INFO` & `polynomiograpy-0.4.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polynomiograpy
-Version: 0.3.0a1
+Version: 0.4.0a1
 Summary: 
 Home-page: https://github.com/ismltpn/polynomiograpy/
 License: MIT
 Keywords: Polynomiography,Polynomials,Visual Art
 Author: İsmail Tapan
 Author-email: ismltpn@gmail.com
 Maintainer: İsmail Tapan
```

