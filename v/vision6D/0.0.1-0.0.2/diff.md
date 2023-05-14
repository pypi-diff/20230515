# Comparing `tmp/vision6D-0.0.1.tar.gz` & `tmp/vision6D-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision6D-0.0.1.tar", last modified: Fri Nov  4 01:33:18 2022, max compression
+gzip compressed data, was "dist\vision6D-0.0.2.tar", last modified: Sun May 14 22:26:06 2023, max compression
```

## Comparing `vision6D-0.0.1.tar` & `vision6D-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-11-04 01:33:18.000000 vision6D-0.0.1/
--rw-rw-rw-   0        0        0     1086 2022-11-02 15:05:21.000000 vision6D-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      791 2022-11-04 01:33:18.457639 vision6D-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       84 2022-11-03 16:01:00.000000 vision6D-0.0.1/README.md
--rw-rw-rw-   0        0        0      412 2022-11-03 16:03:49.000000 vision6D-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1884 2022-11-04 01:33:18.469641 vision6D-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       64 2022-11-03 16:03:49.000000 vision6D-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-04 01:33:18.000000 vision6D-0.0.1/test/
--rw-rw-rw-   0        0        0     1307 2022-11-04 01:13:02.000000 vision6D-0.0.1/test/test_load_image.py
-drwxrwxrwx   0        0        0        0 2022-11-04 01:33:18.000000 vision6D-0.0.1/vision6D/
--rw-rw-rw-   0        0        0      803 2022-11-03 16:03:49.000000 vision6D-0.0.1/vision6D/__init__.py
--rw-rw-rw-   0        0        0     7498 2022-11-04 01:28:05.000000 vision6D-0.0.1/vision6D/app.py
--rw-rw-rw-   0        0        0     5425 2022-11-03 16:03:49.000000 vision6D-0.0.1/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-04 01:33:18.000000 vision6D-0.0.1/vision6D.egg-info/
--rw-rw-rw-   0        0        0      791 2022-11-04 01:33:18.000000 vision6D-0.0.1/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2022-11-04 01:33:18.000000 vision6D-0.0.1/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-04 01:33:18.000000 vision6D-0.0.1/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2022-11-04 01:33:18.000000 vision6D-0.0.1/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-04 01:33:18.000000 vision6D-0.0.1/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 22:26:06.185261 vision6D-0.0.2/
+-rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      793 2023-05-14 22:26:06.186261 vision6D-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      106 2023-05-11 21:10:38.000000 vision6D-0.0.2/README.md
+-rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1918 2023-05-14 22:26:06.207264 vision6D-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       65 2023-01-03 15:55:08.000000 vision6D-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 22:26:06.142265 vision6D-0.0.2/test/
+-rw-rw-rw-   0        0        0    21974 2023-05-11 22:16:59.000000 vision6D-0.0.2/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-04-21 21:41:53.000000 vision6D-0.0.2/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-05-14 22:26:06.162264 vision6D-0.0.2/vision6D/
+-rw-rw-rw-   0        0        0    45348 2023-05-14 22:21:14.000000 vision6D-0.0.2/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      935 2023-05-09 15:00:33.000000 vision6D-0.0.2/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-05 15:04:28.000000 vision6D-0.0.2/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-05-11 22:14:53.000000 vision6D-0.0.2/vision6D/config.py
+-rw-rw-rw-   0        0        0    22897 2023-05-08 19:47:11.000000 vision6D-0.0.2/vision6D/interface.py
+-rw-rw-rw-   0        0        0    28492 2023-05-14 22:15:55.000000 vision6D-0.0.2/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-08 19:54:14.000000 vision6D-0.0.2/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    14911 2023-05-08 18:27:06.000000 vision6D-0.0.2/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-14 22:26:06.182261 vision6D-0.0.2/vision6D.egg-info/
+-rw-rw-rw-   0        0        0      793 2023-05-14 22:26:05.000000 vision6D-0.0.2/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2023-05-14 22:26:06.000000 vision6D-0.0.2/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 22:26:05.000000 vision6D-0.0.2/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-05-14 22:26:05.000000 vision6D-0.0.2/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 22:26:05.000000 vision6D-0.0.2/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.0.1/LICENSE` & `vision6D-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.1/setup.cfg` & `vision6D-0.0.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e31 0d0a 7572  sion = 0.0.1..ur
+00000020: 7369 6f6e 203d 2030 2e30 2e32 0d0a 7572  sion = 0.0.2..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
@@ -49,70 +49,72 @@
 00000300: 0973 6574 7570 746f 6f6c 730d 0a69 6e73  .setuptools..ins
 00000310: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
 00000320: 0d0a 0970 7976 6973 7461 0d0a 096e 756d  ...pyvista...num
 00000330: 7079 0d0a 096d 6174 706c 6f74 6c69 620d  py...matplotlib.
 00000340: 0a09 7472 696d 6573 680d 0a09 6561 7379  ..trimesh...easy
 00000350: 6469 6374 0d0a 0970 696c 6c6f 770d 0a09  dict...pillow...
 00000360: 7363 6970 790d 0a09 7079 7465 7374 0d0a  scipy...pytest..
-00000370: 0970 7265 2d63 6f6d 6d69 740d 0a09 6f70  .pre-commit...op
-00000380: 656e 6376 2d70 7974 686f 6e0d 0a0d 0a5b  encv-python....[
-00000390: 6f70 7469 6f6e 732e 6578 7472 6173 5f72  options.extras_r
-000003a0: 6571 7569 7265 5d0d 0a74 6573 7420 3d20  equire]..test = 
-000003b0: 0d0a 0970 7974 6573 740d 0a0d 0a5b 6f70  ...pytest....[op
-000003c0: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
-000003d0: 7461 5d0d 0a2a 203d 202a 2e70 6e67 2c20  ta]..* = *.png, 
-000003e0: 2a2e 6a70 672c 202a 2e71 6d6c 0d0a 0d0a  *.jpg, *.qml....
-000003f0: 5b62 6469 7374 5f77 6865 656c 5d0d 0a75  [bdist_wheel]..u
-00000400: 6e69 7665 7273 616c 203d 2074 7275 650d  niversal = true.
-00000410: 0a0d 0a5b 7364 6973 745d 0d0a 666f 726d  ...[sdist]..form
-00000420: 6174 7320 3d20 7a69 702c 2067 7a74 6172  ats = zip, gztar
-00000430: 0d0a 0d0a 5b63 6f76 6572 6167 653a 7265  ....[coverage:re
-00000440: 706f 7274 5d0d 0a73 686f 775f 6d69 7373  port]..show_miss
-00000450: 696e 6720 3d20 7472 7565 0d0a 6578 636c  ing = true..excl
-00000460: 7564 655f 6c69 6e65 7320 3d20 0d0a 0970  ude_lines = ...p
-00000470: 7261 676d 613a 206e 6f20 636f 7665 720d  ragma: no cover.
-00000480: 0a09 6966 2046 616c 7365 0d0a 0d0a 5b67  ..if False....[g
-00000490: 7265 656e 5d0d 0a66 696c 652d 7061 7474  reen]..file-patt
-000004a0: 6572 6e20 3d20 7465 7374 5f2a 2e70 790d  ern = test_*.py.
-000004b0: 0a76 6572 626f 7365 203d 2032 0d0a 6e6f  .verbose = 2..no
-000004c0: 2d73 6b69 702d 7265 706f 7274 203d 2074  -skip-report = t
-000004d0: 7275 650d 0a71 7569 6574 2d73 7464 6f75  rue..quiet-stdou
-000004e0: 7420 3d20 7472 7565 0d0a 7275 6e2d 636f  t = true..run-co
-000004f0: 7665 7261 6765 203d 2074 7275 650d 0a0d  verage = true...
-00000500: 0a5b 7079 646f 6373 7479 6c65 5d0d 0a6d  .[pydocstyle]..m
-00000510: 6174 6368 2d64 6972 203d 2028 3f21 7465  atch-dir = (?!te
-00000520: 7374 7329 283f 2172 6573 6f75 7263 6573  sts)(?!resources
-00000530: 2928 3f21 646f 6373 295b 5e5c 2e5d 2e2a  )(?!docs)[^\.].*
-00000540: 0d0a 6d61 7463 6820 3d20 283f 2174 6573  ..match = (?!tes
-00000550: 7429 283f 2173 6574 7570 295b 5e5c 2e5f  t)(?!setup)[^\._
-00000560: 5d2e 2a5c 2e70 790d 0a69 6e68 6572 6974  ].*\.py..inherit
-00000570: 203d 2066 616c 7365 0d0a 6967 6e6f 7265   = false..ignore
-00000580: 203d 2044 3230 302c 2044 3230 332c 2044   = D200, D203, D
-00000590: 3231 332c 2044 3430 362c 2044 3430 370d  213, D406, D407.
-000005a0: 0a0d 0a5b 666c 616b 6538 5d0d 0a6d 6178  ...[flake8]..max
-000005b0: 2d6c 696e 652d 6c65 6e67 7468 203d 2039  -line-length = 9
-000005c0: 390d 0a64 6f63 7465 7374 7320 3d20 5472  9..doctests = Tr
-000005d0: 7565 0d0a 6578 636c 7564 6520 3d20 2e67  ue..exclude = .g
-000005e0: 6974 2c20 2e65 6767 732c 205f 5f70 7963  it, .eggs, __pyc
-000005f0: 6163 6865 5f5f 2c20 7465 7374 732f 2c20  ache__, tests/, 
-00000600: 646f 6373 2f2c 2062 7569 6c64 2f2c 2064  docs/, build/, d
-00000610: 6973 742f 0d0a 0d0a 5b6d 7970 795d 0d0a  ist/....[mypy]..
-00000620: 6469 7361 6c6c 6f77 5f61 6e79 5f64 6563  disallow_any_dec
-00000630: 6f72 6174 6564 203d 2074 7275 650d 0a64  orated = true..d
-00000640: 6973 616c 6c6f 775f 616e 795f 6765 6e65  isallow_any_gene
-00000650: 7269 6373 203d 2074 7275 650d 0a64 6973  rics = true..dis
-00000660: 616c 6c6f 775f 616e 795f 756e 696d 706f  allow_any_unimpo
-00000670: 7274 6564 203d 2066 616c 7365 0d0a 6469  rted = false..di
-00000680: 7361 6c6c 6f77 5f73 7562 636c 6173 7369  sallow_subclassi
-00000690: 6e67 5f61 6e79 203d 2066 616c 7365 0d0a  ng_any = false..
-000006a0: 6469 7361 6c6c 6f77 5f75 6e74 7970 6564  disallow_untyped
-000006b0: 5f63 616c 6c73 203d 2074 7275 650d 0a64  _calls = true..d
-000006c0: 6973 616c 6c6f 775f 756e 7479 7065 645f  isallow_untyped_
-000006d0: 6465 6673 203d 2074 7275 650d 0a69 676e  defs = true..ign
-000006e0: 6f72 655f 6d69 7373 696e 675f 696d 706f  ore_missing_impo
-000006f0: 7274 7320 3d20 7472 7565 0d0a 7761 726e  rts = true..warn
-00000700: 5f75 6e75 7365 645f 6967 6e6f 7265 7320  _unused_ignores 
-00000710: 3d20 7472 7565 0d0a 7761 726e 5f72 6574  = true..warn_ret
-00000720: 7572 6e5f 616e 7920 3d20 7472 7565 0d0a  urn_any = true..
-00000730: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000740: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000750: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000370: 0970 7974 6573 742d 6c61 7a79 2d66 6978  .pytest-lazy-fix
+00000380: 7475 7265 0d0a 0970 7265 2d63 6f6d 6d69  ture...pre-commi
+00000390: 740d 0a09 6f70 656e 6376 2d70 7974 686f  t...opencv-pytho
+000003a0: 6e0d 0a09 7363 696b 6974 2d69 6d61 6765  n...scikit-image
+000003b0: 0d0a 0963 6861 7264 6574 0d0a 0970 7967  ...chardet...pyg
+000003c0: 656f 6465 7369 630d 0a09 5079 5174 350d  eodesic...PyQt5.
+000003d0: 0a09 7079 7669 7374 6171 740d 0a0d 0a5b  ..pyvistaqt....[
+000003e0: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
+000003f0: 6461 7461 5d0d 0a2a 203d 202a 2e70 6e67  data]..* = *.png
+00000400: 2c20 2a2e 6a70 672c 202a 2e71 6d6c 0d0a  , *.jpg, *.qml..
+00000410: 0d0a 5b62 6469 7374 5f77 6865 656c 5d0d  ..[bdist_wheel].
+00000420: 0a75 6e69 7665 7273 616c 203d 2074 7275  .universal = tru
+00000430: 650d 0a0d 0a5b 7364 6973 745d 0d0a 666f  e....[sdist]..fo
+00000440: 726d 6174 7320 3d20 7a69 702c 2067 7a74  rmats = zip, gzt
+00000450: 6172 0d0a 0d0a 5b63 6f76 6572 6167 653a  ar....[coverage:
+00000460: 7265 706f 7274 5d0d 0a73 686f 775f 6d69  report]..show_mi
+00000470: 7373 696e 6720 3d20 7472 7565 0d0a 6578  ssing = true..ex
+00000480: 636c 7564 655f 6c69 6e65 7320 3d20 0d0a  clude_lines = ..
+00000490: 0970 7261 676d 613a 206e 6f20 636f 7665  .pragma: no cove
+000004a0: 720d 0a09 6966 2046 616c 7365 0d0a 0d0a  r...if False....
+000004b0: 5b67 7265 656e 5d0d 0a66 696c 652d 7061  [green]..file-pa
+000004c0: 7474 6572 6e20 3d20 7465 7374 5f2a 2e70  ttern = test_*.p
+000004d0: 790d 0a76 6572 626f 7365 203d 2032 0d0a  y..verbose = 2..
+000004e0: 6e6f 2d73 6b69 702d 7265 706f 7274 203d  no-skip-report =
+000004f0: 2074 7275 650d 0a71 7569 6574 2d73 7464   true..quiet-std
+00000500: 6f75 7420 3d20 7472 7565 0d0a 7275 6e2d  out = true..run-
+00000510: 636f 7665 7261 6765 203d 2074 7275 650d  coverage = true.
+00000520: 0a0d 0a5b 7079 646f 6373 7479 6c65 5d0d  ...[pydocstyle].
+00000530: 0a6d 6174 6368 2d64 6972 203d 2028 3f21  .match-dir = (?!
+00000540: 7465 7374 7329 283f 2172 6573 6f75 7263  tests)(?!resourc
+00000550: 6573 2928 3f21 646f 6373 295b 5e5c 2e5d  es)(?!docs)[^\.]
+00000560: 2e2a 0d0a 6d61 7463 6820 3d20 283f 2174  .*..match = (?!t
+00000570: 6573 7429 283f 2173 6574 7570 295b 5e5c  est)(?!setup)[^\
+00000580: 2e5f 5d2e 2a5c 2e70 790d 0a69 6e68 6572  ._].*\.py..inher
+00000590: 6974 203d 2066 616c 7365 0d0a 6967 6e6f  it = false..igno
+000005a0: 7265 203d 2044 3230 302c 2044 3230 332c  re = D200, D203,
+000005b0: 2044 3231 332c 2044 3430 362c 2044 3430   D213, D406, D40
+000005c0: 370d 0a0d 0a5b 666c 616b 6538 5d0d 0a6d  7....[flake8]..m
+000005d0: 6178 2d6c 696e 652d 6c65 6e67 7468 203d  ax-line-length =
+000005e0: 2039 390d 0a64 6f63 7465 7374 7320 3d20   99..doctests = 
+000005f0: 5472 7565 0d0a 6578 636c 7564 6520 3d20  True..exclude = 
+00000600: 2e67 6974 2c20 2e65 6767 732c 205f 5f70  .git, .eggs, __p
+00000610: 7963 6163 6865 5f5f 2c20 7465 7374 732f  ycache__, tests/
+00000620: 2c20 646f 6373 2f2c 2062 7569 6c64 2f2c  , docs/, build/,
+00000630: 2064 6973 742f 0d0a 0d0a 5b6d 7970 795d   dist/....[mypy]
+00000640: 0d0a 6469 7361 6c6c 6f77 5f61 6e79 5f64  ..disallow_any_d
+00000650: 6563 6f72 6174 6564 203d 2074 7275 650d  ecorated = true.
+00000660: 0a64 6973 616c 6c6f 775f 616e 795f 6765  .disallow_any_ge
+00000670: 6e65 7269 6373 203d 2074 7275 650d 0a64  nerics = true..d
+00000680: 6973 616c 6c6f 775f 616e 795f 756e 696d  isallow_any_unim
+00000690: 706f 7274 6564 203d 2066 616c 7365 0d0a  ported = false..
+000006a0: 6469 7361 6c6c 6f77 5f73 7562 636c 6173  disallow_subclas
+000006b0: 7369 6e67 5f61 6e79 203d 2066 616c 7365  sing_any = false
+000006c0: 0d0a 6469 7361 6c6c 6f77 5f75 6e74 7970  ..disallow_untyp
+000006d0: 6564 5f63 616c 6c73 203d 2074 7275 650d  ed_calls = true.
+000006e0: 0a64 6973 616c 6c6f 775f 756e 7479 7065  .disallow_untype
+000006f0: 645f 6465 6673 203d 2074 7275 650d 0a69  d_defs = true..i
+00000700: 676e 6f72 655f 6d69 7373 696e 675f 696d  gnore_missing_im
+00000710: 706f 7274 7320 3d20 7472 7565 0d0a 7761  ports = true..wa
+00000720: 726e 5f75 6e75 7365 645f 6967 6e6f 7265  rn_unused_ignore
+00000730: 7320 3d20 7472 7565 0d0a 7761 726e 5f72  s = true..warn_r
+00000740: 6574 7572 6e5f 616e 7920 3d20 7472 7565  eturn_any = true
+00000750: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000760: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000770: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

