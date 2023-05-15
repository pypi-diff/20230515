# Comparing `tmp/morecantile-3.3.0.tar.gz` & `tmp/morecantile-4.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morecantile-3.3.0.tar", last modified: Thu Mar  9 22:23:30 2023, max compression
+gzip compressed data, was "morecantile-4.0.0a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `morecantile-3.3.0.tar` & `morecantile-4.0.0a0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0      215 2023-03-09 22:23:19.930589 morecantile-3.3.0/.bumpversion.cfg
--rw-r--r--   0        0        0     1817 2023-03-09 22:23:19.930589 morecantile-3.3.0/.gitignore
--rw-r--r--   0        0        0      822 2023-03-09 22:23:19.930589 morecantile-3.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-03-09 22:23:19.930589 morecantile-3.3.0/LICENSE
--rw-r--r--   0        0        0     4239 2023-03-09 22:23:19.930589 morecantile-3.3.0/README.md
--rw-r--r--   0        0        0      436 2023-03-09 22:23:19.930589 morecantile-3.3.0/morecantile/__init__.py
--rw-r--r--   0        0        0     1015 2023-03-09 22:23:19.930589 morecantile-3.3.0/morecantile/commons.py
--rw-r--r--   0        0        0    10093 2023-03-09 22:23:19.930589 morecantile-3.3.0/morecantile/data/CanadianNAD83_LCC.json
--rwxr-xr-x   0        0        0     8530 2023-03-09 22:23:19.930589 morecantile-3.3.0/morecantile/data/EuropeanETRS89_LAEAQuad.json
--rw-r--r--   0        0        0     5204 2023-03-09 22:23:19.930589 morecantile-3.3.0/morecantile/data/LINZAntarticaMapTilegrid.json
--rw-r--r--   0        0        0     6576 2023-03-09 22:23:19.930589 morecantile-3.3.0/morecantile/data/NZTM2000.json
--rw-r--r--   0        0        0     7020 2023-03-09 22:23:19.930589 morecantile-3.3.0/morecantile/data/NZTM2000Quad.json
--rw-r--r--   0        0        0      242 2023-03-09 22:23:19.930589 morecantile-3.3.0/morecantile/data/README.md
--rw-r--r--   0        0        0     9893 2023-03-09 22:23:19.930589 morecantile-3.3.0/morecantile/data/UPSAntarcticWGS84Quad.json
--rw-r--r--   0        0        0     9887 2023-03-09 22:23:19.930589 morecantile-3.3.0/morecantile/data/UPSArcticWGS84Quad.json
--rw-r--r--   0        0        0     9679 2023-03-09 22:23:19.930589 morecantile-3.3.0/morecantile/data/UTM31WGS84Quad.json
--rw-r--r--   0        0        0     6866 2023-03-09 22:23:19.930589 morecantile-3.3.0/morecantile/data/WGS1984Quad.json
--rwxr-xr-x   0        0        0    10276 2023-03-09 22:23:19.934589 morecantile-3.3.0/morecantile/data/WebMercatorQuad.json
--rw-r--r--   0        0        0     6865 2023-03-09 22:23:19.934589 morecantile-3.3.0/morecantile/data/WorldCRS84Quad.json
--rwxr-xr-x   0        0        0    10138 2023-03-09 22:23:19.934589 morecantile-3.3.0/morecantile/data/WorldMercatorWGS84Quad.json
--rw-r--r--   0        0        0     1865 2023-03-09 22:23:19.934589 morecantile-3.3.0/morecantile/defaults.py
--rw-r--r--   0        0        0      818 2023-03-09 22:23:19.934589 morecantile-3.3.0/morecantile/errors.py
--rw-r--r--   0        0        0    34209 2023-03-09 22:23:19.934589 morecantile-3.3.0/morecantile/models.py
--rw-r--r--   0        0        0        0 2023-03-09 22:23:19.934589 morecantile-3.3.0/morecantile/py.typed
--rw-r--r--   0        0        0       23 2023-03-09 22:23:19.934589 morecantile-3.3.0/morecantile/scripts/__init__.py
--rw-r--r--   0        0        0    16665 2023-03-09 22:23:19.934589 morecantile-3.3.0/morecantile/scripts/cli.py
--rw-r--r--   0        0        0     3007 2023-03-09 22:23:19.934589 morecantile-3.3.0/morecantile/utils.py
--rw-r--r--   0        0        0     2235 2023-03-09 22:23:19.934589 morecantile-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     5591 1970-01-01 00:00:00.000000 morecantile-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0      217 2023-05-15 15:52:57.079291 morecantile-4.0.0a0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1817 2023-05-15 15:52:57.079291 morecantile-4.0.0a0/.gitignore
+-rw-r--r--   0        0        0      822 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/LICENSE
+-rw-r--r--   0        0        0     5305 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/README.md
+-rw-r--r--   0        0        0      438 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/__init__.py
+-rw-r--r--   0        0        0     1015 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/commons.py
+-rw-r--r--   0        0        0     7267 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/CanadianNAD83_LCC.json
+-rw-r--r--   0        0        0     4679 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/EuropeanETRS89_LAEAQuad.json
+-rw-r--r--   0        0        0     5176 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/LINZAntarticaMapTilegrid.json
+-rw-r--r--   0        0        0     8457 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/NZTM2000Quad.json
+-rw-r--r--   0        0        0      242 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/README.md
+-rw-r--r--   0        0        0     7374 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/UPSAntarcticWGS84Quad.json
+-rw-r--r--   0        0        0     7365 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/UPSArcticWGS84Quad.json
+-rw-r--r--   0        0        0     7367 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/UTM31WGS84Quad.json
+-rw-r--r--   0        0        0     6932 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/WGS1984Quad.json
+-rw-r--r--   0        0        0     7843 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/WebMercatorQuad.json
+-rw-r--r--   0        0        0     7072 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/WorldCRS84Quad.json
+-rw-r--r--   0        0        0     7001 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/WorldMercatorWGS84Quad.json
+-rw-r--r--   0        0        0     1748 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/defaults.py
+-rw-r--r--   0        0        0      907 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/errors.py
+-rw-r--r--   0        0        0    39247 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/models.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/py.typed
+-rw-r--r--   0        0        0       23 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/scripts/__init__.py
+-rw-r--r--   0        0        0    16657 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/scripts/cli.py
+-rw-r--r--   0        0        0     3364 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/utils.py
+-rw-r--r--   0        0        0     2295 2023-05-15 15:52:57.087291 morecantile-4.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     6734 1970-01-01 00:00:00.000000 morecantile-4.0.0a0/PKG-INFO
```

### Comparing `morecantile-3.3.0/.gitignore` & `morecantile-4.0.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `morecantile-3.3.0/.pre-commit-config.yaml` & `morecantile-4.0.0a0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `morecantile-3.3.0/LICENSE` & `morecantile-4.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `morecantile-3.3.0/morecantile/commons.py` & `morecantile-4.0.0a0/morecantile/commons.py`

 * *Files identical despite different names*

### Comparing `morecantile-3.3.0/morecantile/data/CanadianNAD83_LCC.json` & `morecantile-4.0.0a0/morecantile/data/WorldCRS84Quad.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.041666666666666664%*

 * *Differences: {"'crs'": "'http://www.opengis.net/def/crs/OGC/1.3/CRS84'",*

 * * "'id'": "'WorldCRS84Quad'",*

 * * "'orderedAxes'": "['Lon', 'Lat']",*

 * * "'tileMatrices'": "[OrderedDict([('id', '0'), ('scaleDenominator', 279541132.014358), "*

 * *                   "('cellSize', 0.703125), ('pointOfOrigin', [-180, 90]), ('tileWidth', 256), "*

 * *                   "('tileHeight', 256), ('matrixWidth', 2), ('matrixHeight', 1)]), "*

 * *                   "OrderedDict([('id', '1'), ('scaleDenominator', 139770566.007179), ('cellSize', "*

 * *               […]*

```diff
@@ -1,358 +1,325 @@
 {
-    "boundingBox": {
-        "crs": "urn:ogc:def:crs:EPSG::3978",
-        "lowerCorner": [
-            -7786476.885838887,
-            -5153821.09213678
-        ],
-        "type": "BoundingBoxType",
-        "upperCorner": [
-            7148753.233541353,
-            7928343.534071138
-        ]
-    },
-    "identifier": "CanadianNAD83_LCC",
-    "supportedCRS": "urn:ogc:def:crs:EPSG::3978",
-    "tileMatrix": [
+    "crs": "http://www.opengis.net/def/crs/OGC/1.3/CRS84",
+    "id": "WorldCRS84Quad",
+    "orderedAxes": [
+        "Lon",
+        "Lat"
+    ],
+    "tileMatrices": [
         {
-            "identifier": "0",
-            "matrixHeight": 5,
-            "matrixWidth": 5,
-            "scaleDenominator": 137016643.08090523,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 0.703125,
+            "id": "0",
+            "matrixHeight": 1,
+            "matrixWidth": 2,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
-        },
-        {
-            "identifier": "1",
-            "matrixHeight": 9,
-            "matrixWidth": 9,
-            "scaleDenominator": 80320101.11639273,
+            "scaleDenominator": 279541132.014358,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "2",
-            "matrixHeight": 15,
-            "matrixWidth": 15,
-            "scaleDenominator": 47247118.303760424,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 0.3515625,
+            "id": "1",
+            "matrixHeight": 2,
+            "matrixWidth": 4,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
-        },
-        {
-            "identifier": "3",
-            "matrixHeight": 25,
-            "matrixWidth": 25,
-            "scaleDenominator": 28348270.982256256,
+            "scaleDenominator": 139770566.007179,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "4",
-            "matrixHeight": 42,
-            "matrixWidth": 42,
-            "scaleDenominator": 16536491.40631615,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 0.17578125,
+            "id": "2",
+            "matrixHeight": 4,
+            "matrixWidth": 8,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 69885283.0035897,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "5",
-            "matrixHeight": 73,
-            "matrixWidth": 73,
-            "scaleDenominator": 9449423.660752086,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 0.087890625,
+            "id": "3",
+            "matrixHeight": 8,
+            "matrixWidth": 16,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 34942641.5017948,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "6",
-            "matrixHeight": 121,
-            "matrixWidth": 121,
-            "scaleDenominator": 5669654.196451251,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 0.0439453125,
+            "id": "4",
+            "matrixHeight": 16,
+            "matrixWidth": 32,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 17471320.7508974,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "7",
-            "matrixHeight": 208,
-            "matrixWidth": 208,
-            "scaleDenominator": 3307298.28126323,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 0.02197265625,
+            "id": "5",
+            "matrixHeight": 32,
+            "matrixWidth": 64,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 8735660.37544871,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "8",
-            "matrixHeight": 363,
-            "matrixWidth": 363,
-            "scaleDenominator": 1889884.732150417,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 0.010986328125,
+            "id": "6",
+            "matrixHeight": 64,
+            "matrixWidth": 128,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 4367830.18772435,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "9",
-            "matrixHeight": 605,
-            "matrixWidth": 605,
-            "scaleDenominator": 1133930.8392902503,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 0.0054931640625,
+            "id": "7",
+            "matrixHeight": 128,
+            "matrixWidth": 256,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 2183915.09386217,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "10",
-            "matrixHeight": 1036,
-            "matrixWidth": 1036,
-            "scaleDenominator": 661459.656252646,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 0.00274658203125,
+            "id": "8",
+            "matrixHeight": 256,
+            "matrixWidth": 512,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 1091957.54693108,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "11",
-            "matrixHeight": 1727,
-            "matrixWidth": 1727,
-            "scaleDenominator": 396875.79375158757,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 0.001373291015625,
+            "id": "9",
+            "matrixHeight": 512,
+            "matrixWidth": 1024,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 545978.773465544,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "12",
-            "matrixHeight": 2900,
-            "matrixWidth": 2900,
-            "scaleDenominator": 236235.59151880213,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 0.0006866455078125,
+            "id": "10",
+            "matrixHeight": 1024,
+            "matrixWidth": 2048,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 272989.386732772,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "13",
-            "matrixHeight": 5000,
-            "matrixWidth": 5000,
-            "scaleDenominator": 137016.64308090523,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 0.00034332275390625,
+            "id": "11",
+            "matrixHeight": 2048,
+            "matrixWidth": 4096,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 136494.693366386,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "14",
-            "matrixHeight": 8530,
-            "matrixWidth": 8530,
-            "scaleDenominator": 80320.10111639272,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 0.000171661376953125,
+            "id": "12",
+            "matrixHeight": 4096,
+            "matrixWidth": 8192,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 68247.346683193,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "15",
-            "matrixHeight": 14501,
-            "matrixWidth": 14501,
-            "scaleDenominator": 47247.11830376043,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 8.58306884765625e-05,
+            "id": "13",
+            "matrixHeight": 8192,
+            "matrixWidth": 16384,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 34123.6733415964,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "16",
-            "matrixHeight": 24167,
-            "matrixWidth": 24167,
-            "scaleDenominator": 28348.270982256254,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 4.29153442382812e-05,
+            "id": "14",
+            "matrixHeight": 16384,
+            "matrixWidth": 32768,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 17061.8366707982,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "17",
-            "matrixHeight": 41429,
-            "matrixWidth": 41429,
-            "scaleDenominator": 16536.49140631615,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 2.14576721191406e-05,
+            "id": "15",
+            "matrixHeight": 32768,
+            "matrixWidth": 65536,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 8530.91833539913,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "18",
-            "matrixHeight": 72500,
-            "matrixWidth": 72500,
-            "scaleDenominator": 9449.423660752085,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 1.07288360595703e-05,
+            "id": "16",
+            "matrixHeight": 65536,
+            "matrixWidth": 131072,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 4265.45916769956,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "19",
-            "matrixHeight": 120834,
-            "matrixWidth": 120834,
-            "scaleDenominator": 5669.654196451251,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 5.36441802978515e-06,
+            "id": "17",
+            "matrixHeight": 131072,
+            "matrixWidth": 262144,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 2132.72958384978,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "20",
-            "matrixHeight": 207143,
-            "matrixWidth": 207143,
-            "scaleDenominator": 3307.29828126323,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 2.68220901489258e-06,
+            "id": "18",
+            "matrixHeight": 262144,
+            "matrixWidth": 524288,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 1066.36479192489,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "21",
-            "matrixHeight": 362501,
-            "matrixWidth": 362501,
-            "scaleDenominator": 1889.884732150417,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 1.34110450744629e-06,
+            "id": "19",
+            "matrixHeight": 524288,
+            "matrixWidth": 1048576,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 533.182395962445,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "22",
-            "matrixHeight": 604167,
-            "matrixWidth": 604167,
-            "scaleDenominator": 1133.93083929025,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 6.7055225372314e-07,
+            "id": "20",
+            "matrixHeight": 1048576,
+            "matrixWidth": 2097152,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 266.591197981222,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "23",
-            "matrixHeight": 1035715,
-            "matrixWidth": 1035715,
-            "scaleDenominator": 661.4596562526459,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 3.3527612686157e-07,
+            "id": "21",
+            "matrixHeight": 2097152,
+            "matrixWidth": 4194304,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 133.295598990611,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "24",
-            "matrixHeight": 1726191,
-            "matrixWidth": 1726191,
-            "scaleDenominator": 396.87579375158754,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 1.6763806343079e-07,
+            "id": "22",
+            "matrixHeight": 4194304,
+            "matrixWidth": 8388608,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 66.6477994953056,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "25",
-            "matrixHeight": 2900001,
-            "matrixWidth": 2900001,
-            "scaleDenominator": 236.23559151880212,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -34655800,
-                39310000
+            "cellSize": 8.381903171539e-08,
+            "id": "23",
+            "matrixHeight": 8388608,
+            "matrixWidth": 16777216,
+            "pointOfOrigin": [
+                -180,
+                90
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 33.3238997476528,
+            "tileHeight": 256,
+            "tileWidth": 256
         }
     ],
-    "title": "Lambert conformal conic NAD83 for Canada",
-    "type": "TileMatrixSetType"
+    "title": "CRS84 for the World",
+    "uri": "http://www.opengis.net/def/tilematrixset/OGC/1.0/WorldCRS84Quad",
+    "wellKnownScaleSet": "http://www.opengis.net/def/wkss/OGC/1.0/GoogleCRS84Quad"
 }
```

### Comparing `morecantile-3.3.0/morecantile/data/LINZAntarticaMapTilegrid.json` & `morecantile-4.0.0a0/morecantile/data/LINZAntarticaMapTilegrid.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.1111111111111111%*

 * *Differences: {"'crs'": "'urn:ogc:def:crs:EPSG::5482'",*

 * * "'id'": "'LINZAntarticaMapTilegrid'",*

 * * "'orderedAxes'": "['Y', 'X']",*

 * * "'tileMatrices'": "[OrderedDict([('id', '0'), ('scaleDenominator', 409600000), ('pointOfOrigin', "*

 * *                   "[6918457.73, -918457.73]), ('tileWidth', 256), ('tileHeight', 256), "*

 * *                   "('matrixWidth', 1), ('matrixHeight', 1), ('cellSize', 114687.99999999999)]), "*

 * *                   "OrderedDict([('id', '1'), ('scaleDenominator', 204800000), ('pointOfOrigin', "*

 * *            […]*

```diff
@@ -1,190 +1,193 @@
 {
-    "identifier": "LINZAntarticaMapTilegrid",
-    "supportedCRS": "urn:ogc:def:crs:EPSG::5482",
-    "tileMatrix": [
+    "crs": "urn:ogc:def:crs:EPSG::5482",
+    "id": "LINZAntarticaMapTilegrid",
+    "orderedAxes": [
+        "Y",
+        "X"
+    ],
+    "tileMatrices": [
         {
-            "identifier": "0",
+            "cellSize": 114687.99999999999,
+            "id": "0",
             "matrixHeight": 1,
             "matrixWidth": 1,
-            "scaleDenominator": 409600000,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 6918457.73,
                 -918457.73
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 409600000,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "1",
+            "cellSize": 57343.99999999999,
+            "id": "1",
             "matrixHeight": 1,
             "matrixWidth": 1,
-            "scaleDenominator": 204800000,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 6918457.73,
                 -918457.73
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 204800000,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "2",
+            "cellSize": 28671.999999999996,
+            "id": "2",
             "matrixHeight": 2,
             "matrixWidth": 2,
-            "scaleDenominator": 102400000,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 6918457.73,
                 -918457.73
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 102400000,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "3",
+            "cellSize": 14335.999999999998,
+            "id": "3",
             "matrixHeight": 4,
             "matrixWidth": 4,
-            "scaleDenominator": 51200000,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 6918457.73,
                 -918457.73
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 51200000,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "4",
+            "cellSize": 7167.999999999999,
+            "id": "4",
             "matrixHeight": 7,
             "matrixWidth": 7,
-            "scaleDenominator": 25600000,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 6918457.73,
                 -918457.73
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 25600000,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "5",
+            "cellSize": 3583.9999999999995,
+            "id": "5",
             "matrixHeight": 13,
             "matrixWidth": 13,
-            "scaleDenominator": 12800000,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 6918457.73,
                 -918457.73
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 12800000,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "6",
+            "cellSize": 1791.9999999999998,
+            "id": "6",
             "matrixHeight": 26,
             "matrixWidth": 26,
-            "scaleDenominator": 6400000,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 6918457.73,
                 -918457.73
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 6400000,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "7",
+            "cellSize": 895.9999999999999,
+            "id": "7",
             "matrixHeight": 52,
             "matrixWidth": 52,
-            "scaleDenominator": 3200000,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 6918457.73,
                 -918457.73
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 3200000,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "8",
+            "cellSize": 447.99999999999994,
+            "id": "8",
             "matrixHeight": 104,
             "matrixWidth": 104,
-            "scaleDenominator": 1600000,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 6918457.73,
                 -918457.73
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 1600000,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "9",
+            "cellSize": 223.99999999999997,
+            "id": "9",
             "matrixHeight": 207,
             "matrixWidth": 207,
-            "scaleDenominator": 800000,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 6918457.73,
                 -918457.73
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 800000,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "10",
+            "cellSize": 111.99999999999999,
+            "id": "10",
             "matrixHeight": 413,
             "matrixWidth": 413,
-            "scaleDenominator": 400000,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 6918457.73,
                 -918457.73
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 400000,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "11",
+            "cellSize": 55.99999999999999,
+            "id": "11",
             "matrixHeight": 826,
             "matrixWidth": 826,
-            "scaleDenominator": 200000,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 6918457.73,
                 -918457.73
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 200000,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "12",
+            "cellSize": 27.999999999999996,
+            "id": "12",
             "matrixHeight": 1652,
             "matrixWidth": 1652,
-            "scaleDenominator": 100000,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 6918457.73,
                 -918457.73
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 100000,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "13",
+            "cellSize": 13.999999999999998,
+            "id": "13",
             "matrixHeight": 3303,
             "matrixWidth": 3303,
-            "scaleDenominator": 50000,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 6918457.73,
                 -918457.73
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 50000,
+            "tileHeight": 256,
+            "tileWidth": 256
         }
     ],
-    "title": "LINZ Antarctic Map Tile Grid (Ross Sea Region)",
-    "type": "TileMatrixSetType"
+    "title": "LINZ Antarctic Map Tile Grid (Ross Sea Region)"
 }
```

### Comparing `morecantile-3.3.0/morecantile/data/NZTM2000Quad.json` & `morecantile-4.0.0a0/morecantile/data/NZTM2000Quad.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.18181818181818182%*

 * *Differences: {"'crs'": "'urn:ogc:def:crs:EPSG::2193'",*

 * * "'id'": "'NZTM2000Quad'",*

 * * "'orderedAxes'": "['Y', 'X']",*

 * * "'tileMatrices'": "[OrderedDict([('id', '0'), ('scaleDenominator', 139770566.007179), "*

 * *                   "('pointOfOrigin', [10438190.1652, -3260586.7284]), ('tileWidth', 256), "*

 * *                   "('tileHeight', 256), ('matrixWidth', 1), ('matrixHeight', 1), ('cellSize', "*

 * *                   "39135.75848201011)]), OrderedDict([('id', '1'), ('scaleDenominator', "*

 * *                   "69885283.0035895), (' […]*

```diff
@@ -1,307 +1,298 @@
 {
     "abstract": "See https://github.com/linz/NZTM2000TileMatrixSet",
-    "boundingBox": {
-        "crs": "urn:ogc:def:crs:EPSG::2193",
-        "lowerCorner": [
-            419435.9938,
-            -3260586.7284
-        ],
-        "type": "BoundingBoxType",
-        "upperCorner": [
-            10438190.1652,
-            6758167.443
-        ]
-    },
-    "identifier": "NZTM2000Quad",
-    "supportedCRS": "urn:ogc:def:crs:EPSG::2193",
-    "tileMatrix": [
+    "crs": "urn:ogc:def:crs:EPSG::2193",
+    "id": "NZTM2000Quad",
+    "orderedAxes": [
+        "Y",
+        "X"
+    ],
+    "tileMatrices": [
         {
-            "identifier": "0",
+            "cellSize": 39135.75848201011,
+            "id": "0",
             "matrixHeight": 1,
             "matrixWidth": 1,
-            "scaleDenominator": 139770566.007179,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 139770566.007179,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "1",
+            "cellSize": 19567.879241005056,
+            "id": "1",
             "matrixHeight": 2,
             "matrixWidth": 2,
-            "scaleDenominator": 69885283.0035895,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 69885283.0035895,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "2",
+            "cellSize": 9783.939620502528,
+            "id": "2",
             "matrixHeight": 4,
             "matrixWidth": 4,
-            "scaleDenominator": 34942641.50179475,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 34942641.50179475,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "3",
+            "cellSize": 4891.969810251264,
+            "id": "3",
             "matrixHeight": 8,
             "matrixWidth": 8,
-            "scaleDenominator": 17471320.750897374,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 17471320.750897374,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "4",
+            "cellSize": 2445.984905125632,
+            "id": "4",
             "matrixHeight": 16,
             "matrixWidth": 16,
-            "scaleDenominator": 8735660.375448687,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 8735660.375448687,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "5",
+            "cellSize": 1222.992452562816,
+            "id": "5",
             "matrixHeight": 32,
             "matrixWidth": 32,
-            "scaleDenominator": 4367830.1877243435,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 4367830.1877243435,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "6",
+            "cellSize": 611.496226281408,
+            "id": "6",
             "matrixHeight": 64,
             "matrixWidth": 64,
-            "scaleDenominator": 2183915.0938621718,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 2183915.0938621718,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "7",
+            "cellSize": 305.748113140704,
+            "id": "7",
             "matrixHeight": 128,
             "matrixWidth": 128,
-            "scaleDenominator": 1091957.5469310859,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 1091957.5469310859,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "8",
+            "cellSize": 152.874056570352,
+            "id": "8",
             "matrixHeight": 256,
             "matrixWidth": 256,
-            "scaleDenominator": 545978.7734655429,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 545978.7734655429,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "9",
+            "cellSize": 76.437028285176,
+            "id": "9",
             "matrixHeight": 512,
             "matrixWidth": 512,
-            "scaleDenominator": 272989.38673277147,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 272989.38673277147,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "10",
+            "cellSize": 38.218514142588,
+            "id": "10",
             "matrixHeight": 1024,
             "matrixWidth": 1024,
-            "scaleDenominator": 136494.69336638573,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 136494.69336638573,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "11",
+            "cellSize": 19.109257071294,
+            "id": "11",
             "matrixHeight": 2048,
             "matrixWidth": 2048,
-            "scaleDenominator": 68247.34668319287,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 68247.34668319287,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "12",
+            "cellSize": 9.554628535647,
+            "id": "12",
             "matrixHeight": 4096,
             "matrixWidth": 4096,
-            "scaleDenominator": 34123.67334159643,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 34123.67334159643,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "13",
+            "cellSize": 4.7773142678235,
+            "id": "13",
             "matrixHeight": 8192,
             "matrixWidth": 8192,
-            "scaleDenominator": 17061.836670798217,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 17061.836670798217,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "14",
+            "cellSize": 2.38865713391175,
+            "id": "14",
             "matrixHeight": 16384,
             "matrixWidth": 16384,
-            "scaleDenominator": 8530.918335399108,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 8530.918335399108,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "15",
+            "cellSize": 1.194328566955875,
+            "id": "15",
             "matrixHeight": 32768,
             "matrixWidth": 32768,
-            "scaleDenominator": 4265.459167699554,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 4265.459167699554,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "16",
+            "cellSize": 0.5971642834779375,
+            "id": "16",
             "matrixHeight": 65536,
             "matrixWidth": 65536,
-            "scaleDenominator": 2132.729583849777,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 2132.729583849777,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "17",
+            "cellSize": 0.29858214173896874,
+            "id": "17",
             "matrixHeight": 131072,
             "matrixWidth": 131072,
-            "scaleDenominator": 1066.3647919248886,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 1066.3647919248886,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "18",
+            "cellSize": 0.14929107086948437,
+            "id": "18",
             "matrixHeight": 262144,
             "matrixWidth": 262144,
-            "scaleDenominator": 533.1823959624443,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 533.1823959624443,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "19",
+            "cellSize": 0.07464553543474219,
+            "id": "19",
             "matrixHeight": 524288,
             "matrixWidth": 524288,
-            "scaleDenominator": 266.59119798122214,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 266.59119798122214,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "20",
+            "cellSize": 0.03732276771737109,
+            "id": "20",
             "matrixHeight": 1048576,
             "matrixWidth": 1048576,
-            "scaleDenominator": 133.29559899061107,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 133.29559899061107,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "21",
+            "cellSize": 0.018661383858685546,
+            "id": "21",
             "matrixHeight": 2097152,
             "matrixWidth": 2097152,
-            "scaleDenominator": 66.64779949530553,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
+            "pointOfOrigin": [
                 10438190.1652,
                 -3260586.7284
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 66.64779949530553,
+            "tileHeight": 256,
+            "tileWidth": 256
         }
     ],
-    "title": "LINZ NZTM2000Quad Map Tile Grid",
-    "type": "TileMatrixSetType"
+    "title": "LINZ NZTM2000Quad Map Tile Grid"
 }
```

### Comparing `morecantile-3.3.0/morecantile/data/UTM31WGS84Quad.json` & `morecantile-4.0.0a0/morecantile/data/WebMercatorQuad.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.041666666666666664%*

 * *Differences: {"'crs'": "'http://www.opengis.net/def/crs/EPSG/0/3857'",*

 * * "'id'": "'WebMercatorQuad'",*

 * * "'orderedAxes'": "['X', 'Y']",*

 * * "'tileMatrices'": "[OrderedDict([('id', '0'), ('scaleDenominator', 559082264.028717), "*

 * *                   "('cellSize', 156543.033928041), ('pointOfOrigin', [-20037508.342789244, "*

 * *                   "20037508.342789244]), ('tileWidth', 256), ('tileHeight', 256), ('matrixWidth', "*

 * *                   "1), ('matrixHeight', 1)]), OrderedDict([('id', '1'), ('scaleDenominator', "*

 * *             […]*

```diff
@@ -1,332 +1,338 @@
 {
-    "boundingBox": {
-        "crs": "urn:ogc:def:crs:EPSG::32631",
-        "lowerCorner": [
-            -9501965.72931276,
-            -20003931.4586255
-        ],
-        "type": "BoundingBoxType",
-        "upperCorner": [
-            10501965.7293128,
-            20003931.4586255
-        ]
-    },
-    "identifier": "UTM31WGS84Quad",
-    "supportedCRS": "urn:ogc:def:crs:EPSG::32631",
-    "tileMatrix": [
+    "crs": "http://www.opengis.net/def/crs/EPSG/0/3857",
+    "id": "WebMercatorQuad",
+    "orderedAxes": [
+        "X",
+        "Y"
+    ],
+    "tileMatrices": [
         {
-            "identifier": "1",
-            "matrixHeight": 2,
+            "cellSize": 156543.033928041,
+            "id": "0",
+            "matrixHeight": 1,
             "matrixWidth": 1,
-            "scaleDenominator": 279072704.500914,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 559082264.028717,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "2",
-            "matrixHeight": 4,
+            "cellSize": 78271.5169640204,
+            "id": "1",
+            "matrixHeight": 2,
             "matrixWidth": 2,
-            "scaleDenominator": 139536352.250457,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 279541132.014358,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "3",
-            "matrixHeight": 8,
+            "cellSize": 39135.7584820102,
+            "id": "2",
+            "matrixHeight": 4,
             "matrixWidth": 4,
-            "scaleDenominator": 69768176.1252285,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 139770566.007179,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "4",
-            "matrixHeight": 16,
+            "cellSize": 19567.8792410051,
+            "id": "3",
+            "matrixHeight": 8,
             "matrixWidth": 8,
-            "scaleDenominator": 34884088.0626143,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 69885283.0035897,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "5",
-            "matrixHeight": 32,
+            "cellSize": 9783.93962050256,
+            "id": "4",
+            "matrixHeight": 16,
             "matrixWidth": 16,
-            "scaleDenominator": 17442044.0313071,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 34942641.5017948,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "6",
-            "matrixHeight": 64,
+            "cellSize": 4891.96981025128,
+            "id": "5",
+            "matrixHeight": 32,
             "matrixWidth": 32,
-            "scaleDenominator": 8721022.01565356,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 17471320.7508974,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "7",
-            "matrixHeight": 128,
+            "cellSize": 2445.98490512564,
+            "id": "6",
+            "matrixHeight": 64,
             "matrixWidth": 64,
-            "scaleDenominator": 4360511.00782678,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 8735660.37544871,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "8",
-            "matrixHeight": 256,
+            "cellSize": 1222.99245256282,
+            "id": "7",
+            "matrixHeight": 128,
             "matrixWidth": 128,
-            "scaleDenominator": 2180255.50391339,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 4367830.18772435,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "9",
-            "matrixHeight": 512,
+            "cellSize": 611.49622628141,
+            "id": "8",
+            "matrixHeight": 256,
             "matrixWidth": 256,
-            "scaleDenominator": 1090127.7519567,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 2183915.09386217,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "10",
-            "matrixHeight": 1024,
+            "cellSize": 305.748113140704,
+            "id": "9",
+            "matrixHeight": 512,
             "matrixWidth": 512,
-            "scaleDenominator": 545063.875978348,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 1091957.54693108,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "11",
-            "matrixHeight": 2048,
+            "cellSize": 152.874056570352,
+            "id": "10",
+            "matrixHeight": 1024,
             "matrixWidth": 1024,
-            "scaleDenominator": 272531.937989174,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 545978.773465544,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "12",
-            "matrixHeight": 4096,
+            "cellSize": 76.4370282851762,
+            "id": "11",
+            "matrixHeight": 2048,
             "matrixWidth": 2048,
-            "scaleDenominator": 136265.968994587,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 272989.386732772,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "13",
-            "matrixHeight": 8192,
+            "cellSize": 38.2185141425881,
+            "id": "12",
+            "matrixHeight": 4096,
             "matrixWidth": 4096,
-            "scaleDenominator": 68132.9844972935,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 136494.693366386,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "14",
-            "matrixHeight": 16384,
+            "cellSize": 19.109257071294,
+            "id": "13",
+            "matrixHeight": 8192,
             "matrixWidth": 8192,
-            "scaleDenominator": 34066.4922486467,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 68247.346683193,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "15",
-            "matrixHeight": 32768,
+            "cellSize": 9.55462853564703,
+            "id": "14",
+            "matrixHeight": 16384,
             "matrixWidth": 16384,
-            "scaleDenominator": 17033.2461243234,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 34123.6733415964,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "16",
-            "matrixHeight": 65536,
+            "cellSize": 4.77731426782351,
+            "id": "15",
+            "matrixHeight": 32768,
             "matrixWidth": 32768,
-            "scaleDenominator": 8516.62306216168,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 17061.8366707982,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "17",
-            "matrixHeight": 131072,
+            "cellSize": 2.38865713391175,
+            "id": "16",
+            "matrixHeight": 65536,
             "matrixWidth": 65536,
-            "scaleDenominator": 4258.31153108084,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 8530.91833539913,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "18",
-            "matrixHeight": 262144,
+            "cellSize": 1.19432856695587,
+            "id": "17",
+            "matrixHeight": 131072,
             "matrixWidth": 131072,
-            "scaleDenominator": 2129.15576554042,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 4265.45916769956,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "19",
-            "matrixHeight": 524288,
+            "cellSize": 0.597164283477939,
+            "id": "18",
+            "matrixHeight": 262144,
             "matrixWidth": 262144,
-            "scaleDenominator": 1064.57788277021,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 2132.72958384978,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "20",
-            "matrixHeight": 1048576,
+            "cellSize": 0.29858214173897,
+            "id": "19",
+            "matrixHeight": 524288,
             "matrixWidth": 524288,
-            "scaleDenominator": 532.288941385105,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 1066.36479192489,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "21",
-            "matrixHeight": 2097152,
+            "cellSize": 0.149291070869485,
+            "id": "20",
+            "matrixHeight": 1048576,
             "matrixWidth": 1048576,
-            "scaleDenominator": 266.144470692553,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 533.182395962445,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "22",
-            "matrixHeight": 4194304,
+            "cellSize": 0.0746455354347424,
+            "id": "21",
+            "matrixHeight": 2097152,
             "matrixWidth": 2097152,
-            "scaleDenominator": 133.072235346276,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 266.591197981222,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "23",
-            "matrixHeight": 8388608,
+            "cellSize": 0.0373227677173712,
+            "id": "22",
+            "matrixHeight": 4194304,
             "matrixWidth": 4194304,
-            "scaleDenominator": 66.5361176731382,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 133.295598990611,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "24",
-            "matrixHeight": 16777216,
+            "cellSize": 0.0186613838586856,
+            "id": "23",
+            "matrixHeight": 8388608,
             "matrixWidth": 8388608,
-            "scaleDenominator": 33.2680588365691,
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
+            ],
+            "scaleDenominator": 66.6477994953056,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -9501965.72931276,
-                20003931.4586255
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 0.0093306919293428,
+            "id": "24",
+            "matrixHeight": 16777216,
+            "matrixWidth": 16777216,
+            "pointOfOrigin": [
+                -20037508.342789244,
+                20037508.342789244
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 33.3238997476528,
+            "tileHeight": 256,
+            "tileWidth": 256
         }
     ],
-    "title": "Universal Transverse Mercator Zone 31 WGS84 Quad",
-    "type": "TileMatrixSetType"
+    "title": "Google Maps Compatible for the World",
+    "uri": "http://www.opengis.net/def/tilematrixset/OGC/1.0/WebMercatorQuad",
+    "wellKnownScaleSet": "http://www.opengis.net/def/wkss/OGC/1.0/GoogleMapsCompatible"
 }
```

### Comparing `morecantile-3.3.0/morecantile/data/WGS1984Quad.json` & `morecantile-4.0.0a0/morecantile/data/UPSArcticWGS84Quad.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.041666666666666664%*

 * *Differences: {"'crs'": "'http://www.opengis.net/def/crs/EPSG/0/5041'",*

 * * "'id'": "'UPSArcticWGS84Quad'",*

 * * "'orderedAxes'": "['E', 'N']",*

 * * "'tileMatrices'": "[OrderedDict([('id', '0'), ('scaleDenominator', 458726544.4), ('cellSize', "*

 * *                   "128443.4324), ('pointOfOrigin', [-14440759.350252, 18440759.350252]), "*

 * *                   "('tileWidth', 256), ('tileHeight', 256), ('matrixWidth', 1), ('matrixHeight', "*

 * *                   "1)]), OrderedDict([('id', '1'), ('scaleDenominator', 229363272.2), "*

 * *            […]*

```diff
@@ -1,255 +1,337 @@
 {
-    "boundingBox": {
-        "crs": "urn:ogc:def:crs:EPSG::4326",
-        "lowerCorner": [
-            -90,
-            -180
-        ],
-        "type": "BoundingBoxType",
-        "upperCorner": [
-            90,
-            180
-        ]
-    },
-    "identifier": "WGS1984Quad",
-    "supportedCRS": "urn:ogc:def:crs:EPSG::4326",
-    "tileMatrix": [
+    "crs": "http://www.opengis.net/def/crs/EPSG/0/5041",
+    "id": "UPSArcticWGS84Quad",
+    "orderedAxes": [
+        "E",
+        "N"
+    ],
+    "tileMatrices": [
         {
-            "identifier": "0",
+            "cellSize": 128443.4324,
+            "id": "0",
             "matrixHeight": 1,
-            "matrixWidth": 2,
-            "scaleDenominator": 279541132.014358,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 1,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 458726544.4,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "1",
+            "cellSize": 64221.71621,
+            "id": "1",
             "matrixHeight": 2,
-            "matrixWidth": 4,
-            "scaleDenominator": 139770566.007179,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 2,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 229363272.2,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "2",
+            "cellSize": 32110.85811,
+            "id": "2",
             "matrixHeight": 4,
-            "matrixWidth": 8,
-            "scaleDenominator": 69885283.0035897,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 4,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 114681636.1,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "3",
+            "cellSize": 16055.42905,
+            "id": "3",
             "matrixHeight": 8,
-            "matrixWidth": 16,
-            "scaleDenominator": 34942641.5017948,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 8,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 57340818.05,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "4",
+            "cellSize": 8027.714526,
+            "id": "4",
             "matrixHeight": 16,
-            "matrixWidth": 32,
-            "scaleDenominator": 17471320.7508974,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 16,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 28670409.02,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "5",
+            "cellSize": 4013.857263,
+            "id": "5",
             "matrixHeight": 32,
-            "matrixWidth": 64,
-            "scaleDenominator": 8735660.37544871,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 32,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 14335204.51,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "6",
+            "cellSize": 2006.928632,
+            "id": "6",
             "matrixHeight": 64,
-            "matrixWidth": 128,
-            "scaleDenominator": 4367830.18772435,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 64,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 7167602.256,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "7",
+            "cellSize": 1003.464316,
+            "id": "7",
             "matrixHeight": 128,
-            "matrixWidth": 256,
-            "scaleDenominator": 2183915.09386217,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 128,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 3583801.128,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "8",
+            "cellSize": 501.7321579,
+            "id": "8",
             "matrixHeight": 256,
-            "matrixWidth": 512,
-            "scaleDenominator": 1091957.54693108,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 256,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 1791900.564,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "9",
+            "cellSize": 250.866079,
+            "id": "9",
             "matrixHeight": 512,
-            "matrixWidth": 1024,
-            "scaleDenominator": 545978.773465544,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 512,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 895950.282,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "10",
+            "cellSize": 125.4330395,
+            "id": "10",
             "matrixHeight": 1024,
-            "matrixWidth": 2048,
-            "scaleDenominator": 272989.386732772,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 1024,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 447975.141,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "11",
+            "cellSize": 62.71651974,
+            "id": "11",
             "matrixHeight": 2048,
-            "matrixWidth": 4096,
-            "scaleDenominator": 136494.693366386,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 2048,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 223987.5705,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "12",
+            "cellSize": 31.35825987,
+            "id": "12",
             "matrixHeight": 4096,
-            "matrixWidth": 8192,
-            "scaleDenominator": 68247.346683193,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 4096,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 111993.7852,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "13",
+            "cellSize": 15.67912993,
+            "id": "13",
             "matrixHeight": 8192,
-            "matrixWidth": 16384,
-            "scaleDenominator": 34123.6733415964,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 8192,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 55996.89262,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "14",
+            "cellSize": 7.839564967,
+            "id": "14",
             "matrixHeight": 16384,
-            "matrixWidth": 32768,
-            "scaleDenominator": 17061.8366707982,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 16384,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 27998.44631,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "15",
+            "cellSize": 3.919782484,
+            "id": "15",
             "matrixHeight": 32768,
-            "matrixWidth": 65536,
-            "scaleDenominator": 8530.91833539913,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 32768,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 13999.22316,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "16",
+            "cellSize": 1.959891242,
+            "id": "16",
             "matrixHeight": 65536,
-            "matrixWidth": 131072,
-            "scaleDenominator": 4265.45916769956,
-            "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "matrixWidth": 65536,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 6999.611578,
+            "tileHeight": 256,
+            "tileWidth": 256
         },
         {
-            "identifier": "17",
+            "cellSize": 0.979945621,
+            "id": "17",
             "matrixHeight": 131072,
+            "matrixWidth": 131072,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
+            ],
+            "scaleDenominator": 3499.805789,
+            "tileHeight": 256,
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 0.48997281,
+            "id": "18",
+            "matrixHeight": 262144,
             "matrixWidth": 262144,
-            "scaleDenominator": 2132.72958384978,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
+            ],
+            "scaleDenominator": 1749.902894,
+            "tileHeight": 256,
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 0.244986405,
+            "id": "19",
+            "matrixHeight": 524288,
+            "matrixWidth": 524288,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
+            ],
+            "scaleDenominator": 874.9514472,
+            "tileHeight": 256,
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 0.122493203,
+            "id": "20",
+            "matrixHeight": 1048576,
+            "matrixWidth": 1048576,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
+            ],
+            "scaleDenominator": 437.4757236,
+            "tileHeight": 256,
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 0.061246601,
+            "id": "21",
+            "matrixHeight": 2097152,
+            "matrixWidth": 2097152,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
+            ],
+            "scaleDenominator": 218.7378618,
+            "tileHeight": 256,
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 0.030623301,
+            "id": "22",
+            "matrixHeight": 4194304,
+            "matrixWidth": 4194304,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
+            ],
+            "scaleDenominator": 109.3689309,
+            "tileHeight": 256,
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 0.01531165,
+            "id": "23",
+            "matrixHeight": 8388608,
+            "matrixWidth": 8388608,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
+            ],
+            "scaleDenominator": 54.68446545,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                90,
-                -180
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 0.007655825,
+            "id": "24",
+            "matrixHeight": 16777216,
+            "matrixWidth": 16777216,
+            "pointOfOrigin": [
+                -14440759.350252,
+                18440759.350252
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 27.34223273,
+            "tileHeight": 256,
+            "tileWidth": 256
         }
     ],
-    "title": "EPSG:4326 for the World",
-    "type": "TileMatrixSetType",
-    "wellKnownScaleSet": "http://www.opengis.net/def/wkss/OGC/1.0/GoogleCRS84Quad"
+    "title": "Universal Polar Stereographic WGS 84 Quad for Arctic",
+    "uri": "http://www.opengis.net/def/tilematrixset/OGC/1.0/UPSArcticWGS84Quad"
 }
```

### Comparing `morecantile-3.3.0/morecantile/data/WorldCRS84Quad.json` & `morecantile-4.0.0a0/morecantile/data/WorldMercatorWGS84Quad.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.08333333333333333%*

 * *Differences: {"'crs'": "'http://www.opengis.net/def/crs/EPSG/0/3395'",*

 * * "'id'": "'WorldMercatorWGS84Quad'",*

 * * "'orderedAxes'": "['E', 'N']",*

 * * "'tileMatrices'": "[OrderedDict([('id', '0'), ('scaleDenominator', 559082264.028717), "*

 * *                   "('cellSize', 156543.033928041), ('pointOfOrigin', [-20037508.3427892, "*

 * *                   "20037508.3427892]), ('tileWidth', 256), ('tileHeight', 256), ('matrixWidth', "*

 * *                   "1), ('matrixHeight', 1)]), OrderedDict([('id', '1'), ('scaleDenominator', "*

 * *          […]*

```diff
@@ -1,255 +1,338 @@
 {
-    "boundingBox": {
-        "crs": "urn:ogc:def:crs:OGC::CRS84",
-        "lowerCorner": [
-            -180,
-            -90
-        ],
-        "type": "BoundingBoxType",
-        "upperCorner": [
-            180,
-            90
-        ]
-    },
-    "identifier": "WorldCRS84Quad",
-    "supportedCRS": "urn:ogc:def:crs:OGC::CRS84",
-    "tileMatrix": [
+    "crs": "http://www.opengis.net/def/crs/EPSG/0/3395",
+    "id": "WorldMercatorWGS84Quad",
+    "orderedAxes": [
+        "E",
+        "N"
+    ],
+    "tileMatrices": [
         {
-            "identifier": "0",
+            "cellSize": 156543.033928041,
+            "id": "0",
             "matrixHeight": 1,
+            "matrixWidth": 1,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
+            "scaleDenominator": 559082264.028717,
+            "tileHeight": 256,
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 78271.5169640204,
+            "id": "1",
+            "matrixHeight": 2,
             "matrixWidth": 2,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 279541132.014358,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "1",
-            "matrixHeight": 2,
+            "cellSize": 39135.7584820102,
+            "id": "2",
+            "matrixHeight": 4,
             "matrixWidth": 4,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 139770566.007179,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "2",
-            "matrixHeight": 4,
+            "cellSize": 19567.8792410051,
+            "id": "3",
+            "matrixHeight": 8,
             "matrixWidth": 8,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 69885283.0035897,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "3",
-            "matrixHeight": 8,
+            "cellSize": 9783.93962050256,
+            "id": "4",
+            "matrixHeight": 16,
             "matrixWidth": 16,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 34942641.5017948,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "4",
-            "matrixHeight": 16,
+            "cellSize": 4891.96981025128,
+            "id": "5",
+            "matrixHeight": 32,
             "matrixWidth": 32,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 17471320.7508974,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "5",
-            "matrixHeight": 32,
+            "cellSize": 2445.98490512564,
+            "id": "6",
+            "matrixHeight": 64,
             "matrixWidth": 64,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 8735660.37544871,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "6",
-            "matrixHeight": 64,
+            "cellSize": 1222.99245256282,
+            "id": "7",
+            "matrixHeight": 128,
             "matrixWidth": 128,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 4367830.18772435,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "7",
-            "matrixHeight": 128,
+            "cellSize": 611.49622628141,
+            "id": "8",
+            "matrixHeight": 256,
             "matrixWidth": 256,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 2183915.09386217,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "8",
-            "matrixHeight": 256,
+            "cellSize": 305.748113140704,
+            "id": "9",
+            "matrixHeight": 512,
             "matrixWidth": 512,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 1091957.54693108,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "9",
-            "matrixHeight": 512,
+            "cellSize": 152.874056570352,
+            "id": "10",
+            "matrixHeight": 1024,
             "matrixWidth": 1024,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 545978.773465544,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "10",
-            "matrixHeight": 1024,
+            "cellSize": 76.4370282851762,
+            "id": "11",
+            "matrixHeight": 2048,
             "matrixWidth": 2048,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 272989.386732772,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "11",
-            "matrixHeight": 2048,
+            "cellSize": 38.2185141425881,
+            "id": "12",
+            "matrixHeight": 4096,
             "matrixWidth": 4096,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 136494.693366386,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "12",
-            "matrixHeight": 4096,
+            "cellSize": 19.109257071294,
+            "id": "13",
+            "matrixHeight": 8192,
             "matrixWidth": 8192,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 68247.346683193,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "13",
-            "matrixHeight": 8192,
+            "cellSize": 9.55462853564703,
+            "id": "14",
+            "matrixHeight": 16384,
             "matrixWidth": 16384,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 34123.6733415964,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "14",
-            "matrixHeight": 16384,
+            "cellSize": 4.77731426782351,
+            "id": "15",
+            "matrixHeight": 32768,
             "matrixWidth": 32768,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 17061.8366707982,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "15",
-            "matrixHeight": 32768,
+            "cellSize": 2.38865713391175,
+            "id": "16",
+            "matrixHeight": 65536,
             "matrixWidth": 65536,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 8530.91833539913,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "16",
-            "matrixHeight": 65536,
+            "cellSize": 1.19432856695587,
+            "id": "17",
+            "matrixHeight": 131072,
             "matrixWidth": 131072,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 4265.45916769956,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
-            ],
-            "type": "TileMatrixType"
+            "tileWidth": 256
         },
         {
-            "identifier": "17",
-            "matrixHeight": 131072,
+            "cellSize": 0.597164283477939,
+            "id": "18",
+            "matrixHeight": 262144,
             "matrixWidth": 262144,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
             "scaleDenominator": 2132.72958384978,
             "tileHeight": 256,
-            "tileWidth": 256,
-            "topLeftCorner": [
-                -180,
-                90
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 0.29858214173897,
+            "id": "19",
+            "matrixHeight": 524288,
+            "matrixWidth": 524288,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
+            "scaleDenominator": 1066.36479192489,
+            "tileHeight": 256,
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 0.149291070869485,
+            "id": "20",
+            "matrixHeight": 1048576,
+            "matrixWidth": 1048576,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
+            "scaleDenominator": 533.182395962445,
+            "tileHeight": 256,
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 0.0746455354347424,
+            "id": "21",
+            "matrixHeight": 2097152,
+            "matrixWidth": 2097152,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
+            "scaleDenominator": 266.591197981222,
+            "tileHeight": 256,
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 0.0373227677173712,
+            "id": "22",
+            "matrixHeight": 4194304,
+            "matrixWidth": 4194304,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
+            "scaleDenominator": 133.295598990611,
+            "tileHeight": 256,
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 0.0186613838586856,
+            "id": "23",
+            "matrixHeight": 8388608,
+            "matrixWidth": 8388608,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
+            ],
+            "scaleDenominator": 66.6477994953056,
+            "tileHeight": 256,
+            "tileWidth": 256
+        },
+        {
+            "cellSize": 0.0093306919293428,
+            "id": "24",
+            "matrixHeight": 16777216,
+            "matrixWidth": 16777216,
+            "pointOfOrigin": [
+                -20037508.3427892,
+                20037508.3427892
             ],
-            "type": "TileMatrixType"
+            "scaleDenominator": 33.3238997476528,
+            "tileHeight": 256,
+            "tileWidth": 256
         }
     ],
-    "title": "CRS84 for the World",
-    "type": "TileMatrixSetType",
-    "wellKnownScaleSet": "http://www.opengis.net/def/wkss/OGC/1.0/GoogleCRS84Quad"
+    "title": "World Mercator WGS84 (ellipsoid)",
+    "uri": "http://www.opengis.net/def/tilematrixset/OGC/1.0/WorldMercatorWGS84Quad",
+    "wellKnownScaleSet": "http://www.opengis.net/def/wkss/OGC/1.0/WorldMercatorWGS84"
 }
```

### Comparing `morecantile-3.3.0/morecantile/defaults.py` & `morecantile-4.0.0a0/morecantile/defaults.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Default Morecantile TMS."""
 
 import os
 import pathlib
 from copy import copy
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Union
 
 import attr
 
 from morecantile.errors import InvalidIdentifier
 from morecantile.models import TileMatrixSet
 
 morecantile_tms_dir = pathlib.Path(__file__).parent.joinpath("data")
@@ -30,35 +30,33 @@
 
     def get(self, identifier: str) -> TileMatrixSet:
         """Fetch a TMS."""
         if identifier not in self.tms:
             raise InvalidIdentifier(f"Invalid identifier: {identifier}")
 
         tms = self.tms[identifier]
+
+        # We lazyload the TMS document only when called
         if isinstance(tms, pathlib.Path):
             tms = TileMatrixSet.parse_file(tms)
             self.tms[identifier] = tms
 
         return tms
 
     def list(self) -> List[str]:
         """List registered TMS."""
         return list(self.tms.keys())
 
     def register(
         self,
-        custom_tms: Union[TileMatrixSet, Sequence[TileMatrixSet]],
+        custom_tms: Dict[str, TileMatrixSet],
         overwrite: bool = False,
     ) -> "TileMatrixSets":
         """Register TileMatrixSet(s)."""
-        if isinstance(custom_tms, TileMatrixSet):
-            custom_tms = (custom_tms,)
-
-        for tms in custom_tms:
-            if tms.identifier in self.tms and not overwrite:
-                raise Exception(f"{tms.identifier} is already a registered TMS.")
+        for identifier in custom_tms.keys():
+            if identifier in self.tms and not overwrite:
+                raise Exception(f"{identifier} is already a registered TMS.")
 
-        new_tms = {tms.identifier: tms for tms in custom_tms}
-        return TileMatrixSets({**self.tms, **new_tms})
+        return TileMatrixSets({**self.tms, **custom_tms})
 
 
 tms = TileMatrixSets(copy(default_tms))  # noqa
```

### Comparing `morecantile-3.3.0/morecantile/errors.py` & `morecantile-4.0.0a0/morecantile/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,7 +27,11 @@
 
 class QuadKeyError(MorecantileError):
     """Raised when errors occur in computing or parsing quad keys"""
 
 
 class InvalidZoomError(MorecantileError):
     """Raised when input zoom is invalid."""
+
+
+class DeprecationError(MorecantileError):
+    """Raised when TMS version is not 2.0"""
```

### Comparing `morecantile-3.3.0/morecantile/models.py` & `morecantile-4.0.0a0/morecantile/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """Pydantic modules for OGC TileMatrixSets (https://www.ogc.org/standards/tms)"""
 
 import math
 import warnings
-from typing import Any, Dict, Iterator, List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, Iterator, List, Literal, Optional, Sequence, Tuple, Union
 
+from cachetools import LRUCache, cached
+from cachetools.keys import hashkey
 from pydantic import AnyHttpUrl, BaseModel, Field, PrivateAttr, validator
 from pyproj import CRS, Transformer
-from pyproj.enums import WktVersion
 from pyproj.exceptions import ProjError
 
 from morecantile.commons import BoundingBox, Coords, Tile
 from morecantile.errors import (
+    DeprecationError,
     InvalidZoomError,
-    MorecantileError,
     NoQuadkeySupport,
     PointOutsideTMSBounds,
     QuadKeyError,
 )
 from morecantile.utils import (
     _parse_tile_arg,
     bbox_to_feature,
     check_quadkey_support,
     meters_per_unit,
     point_in_bbox,
+    to_rasterio_crs,
 )
 
 NumType = Union[float, int]
 BoundsType = Tuple[NumType, NumType]
 LL_EPSILON = 1e-11
 WGS84_CRS = CRS.from_epsg(4326)
 
@@ -40,15 +42,16 @@
     def __get_validators__(cls):
         """validator for the type."""
         yield cls.validate
 
     @classmethod
     def validate(cls, value: Union[CRS, str]) -> CRS:
         """Validate CRS."""
-        # If input is a string we tranlate it to CRS
+        # If input is a string we translate it to CRS
+        # TODO: add NotImplementedError for ISO 19115
         if not isinstance(value, CRS):
             return CRS.from_user_input(value)
 
         return value
 
     @classmethod
     def __modify_schema__(cls, field_schema):
@@ -86,14 +89,19 @@
 
 
 def crs_axis_inverted(crs: CRS) -> bool:
     """Check if CRS has inverted AXIS (lat,lon) instead of (lon,lat)."""
     return crs.axis_info[0].abbrev.upper() in ["Y", "LAT", "N"]
 
 
+def ordered_axis_inverted(ordered_axes: List[str]) -> bool:
+    """Check if ordered axes have inverted AXIS (lat,lon) instead of (lon,lat)."""
+    return ordered_axes[0].upper() in ["Y", "LAT", "N"]
+
+
 class TMSBoundingBox(BaseModel):
     """Bounding box"""
 
     type: str = Field("BoundingBoxType", const=True)
     crs: CRSType
     lowerCorner: BoundsType
     upperCorner: BoundsType
@@ -101,146 +109,285 @@
     class Config:
         """Configure TMSBoundingBox."""
 
         arbitrary_types_allowed = True
         json_encoders = {CRS: lambda v: CRS_to_uri(v)}
 
 
+# class variableMatrixWidth(BaseModel):
+#     """Variable Matrix Width Definition
+
+
+#     ref: https://github.com/opengeospatial/2D-Tile-Matrix-Set/blob/master/schemas/tms/2.0/json/variableMatrixWidth.json
+#     """
+
+#     coalesce: int = Field(..., ge=2, multiple_of=1, description="Number of tiles in width that coalesce in a single tile for these rows")
+#     minTileRow: int = Field(..., ge=0, multiple_of=1, description="First tile row where the coalescence factor applies for this tilematrix")
+#     maxTileRow: int = Field(..., ge=0, multiple_of=1, description="Last tile row where the coalescence factor applies for this tilematrix")
+
+
 class TileMatrix(BaseModel):
-    """Tile matrix"""
+    """Tile Matrix Definition
 
-    type: str = Field("TileMatrixType", const=True)
-    title: Optional[str]
-    abstract: Optional[str]
-    keywords: Optional[List[str]]
-    identifier: str = Field(..., regex=r"^[0-9]+$")
-    scaleDenominator: float
-    topLeftCorner: BoundsType
-    tileWidth: int
-    tileHeight: int
-    matrixWidth: int
-    matrixHeight: int
+    A tile matrix, usually corresponding to a particular zoom level of a TileMatrixSet.
+
+    ref: https://github.com/opengeospatial/2D-Tile-Matrix-Set/blob/master/schemas/tms/2.0/json/tileMatrix.json
+    """
+
+    title: Optional[str] = Field(
+        description="Title of this tile matrix, normally used for display to a human"
+    )
+    description: Optional[str] = Field(
+        description="Brief narrative description of this tile matrix set, normally available for display to a human"
+    )
+    keywords: Optional[List[str]] = Field(
+        description="Unordered list of one or more commonly used or formalized word(s) or phrase(s) used to describe this dataset"
+    )
+    id: str = Field(
+        ...,
+        regex=r"^[0-9]+$",
+        description="Identifier selecting one of the scales defined in the TileMatrixSet and representing the scaleDenominator the tile. Implementation of 'identifier'",
+    )
+    scaleDenominator: float = Field(
+        ..., description="Scale denominator of this tile matrix"
+    )
+    cellSize: float = Field(..., description="Cell size of this tile matrix")
+    cornerOfOrigin: Optional[Literal["topLeft", "bottomLeft"]] = Field(
+        description="The corner of the tile matrix (_topLeft_ or _bottomLeft_) used as the origin for numbering tile rows and columns. This corner is also a corner of the (0, 0) tile."
+    )
+    pointOfOrigin: BoundsType = Field(
+        ...,
+        description="Precise position in CRS coordinates of the corner of origin (e.g. the top-left corner) for this tile matrix. This position is also a corner of the (0, 0) tile. In previous version, this was 'topLeftCorner' and 'cornerOfOrigin' did not exist.",
+    )
+    tileWidth: int = Field(
+        ...,
+        ge=1,
+        multiple_of=1,
+        description="Width of each tile of this tile matrix in pixels",
+    )
+    tileHeight: int = Field(
+        ...,
+        ge=1,
+        multiple_of=1,
+        description="Height of each tile of this tile matrix in pixels",
+    )
+    matrixWidth: int = Field(
+        ...,
+        ge=1,
+        multiple_of=1,
+        description="Width of the matrix (number of tiles in width)",
+    )
+    matrixHeight: int = Field(
+        ...,
+        ge=1,
+        multiple_of=1,
+        description="Height of the matrix (number of tiles in height)",
+    )
+    # variableMatrixWidths: Optional[List[variableMatrixWidth]] = Field(description="Describes the rows that has variable matrix width")
 
     class Config:
-        """Forbid additional items like variableMatrixWidth."""
+        """Forbid additional items like variableMatrixWidths."""
 
         extra = "forbid"
 
 
 class TileMatrixSet(BaseModel):
-    """Tile matrix set"""
+    """Tile Matrix Set Definition
+
+    A definition of a tile matrix set following the Tile Matrix Set standard.
+    For tileset metadata, such a description (in `tileMatrixSet` property) is only required for offline use,
+    as an alternative to a link with a `http://www.opengis.net/def/rel/ogc/1.0/tiling-scheme` relation type.
+
+    ref: https://github.com/opengeospatial/2D-Tile-Matrix-Set/blob/master/schemas/tms/2.0/json/tileMatrixSet.json
+
+    """
 
-    type: str = Field("TileMatrixSetType", const=True)
-    title: str
-    abstract: Optional[str]
-    keywords: Optional[List[str]]
-    identifier: str = Field(..., regex=r"^[\w\d_\-]+$")
-    supportedCRS: CRSType
-    wellKnownScaleSet: Optional[AnyHttpUrl] = None
-    boundingBox: Optional[TMSBoundingBox]
-    tileMatrix: List[TileMatrix]
+    title: Optional[str] = Field(
+        description="Title of this tile matrix set, normally used for display to a human"
+    )
+    description: Optional[str] = Field(
+        description="Brief narrative description of this tile matrix set, normally available for display to a human"
+    )
+    keywords: Optional[List[str]] = Field(
+        description="Unordered list of one or more commonly used or formalized word(s) or phrase(s) used to describe this tile matrix set"
+    )
+    id: Optional[str] = Field(
+        regex=r"^[\w\d_\-]+$",
+        description="Tile matrix set identifier. Implementation of 'identifier'",
+    )
+    uri: Optional[str] = Field(
+        description="Reference to an official source for this tileMatrixSet"
+    )
+    orderedAxes: Optional[List[str]]
+    crs: CRSType = Field(..., description="Coordinate Reference System (CRS)")
+    wellKnownScaleSet: Optional[AnyHttpUrl] = Field(
+        description="Reference to a well-known scale set"
+    )
+    boundingBox: Optional[TMSBoundingBox] = Field(
+        description="Minimum bounding rectangle surrounding the tile matrix set, in the supported CRS"
+    )
+    tileMatrices: List[TileMatrix] = Field(
+        ..., description="Describes scale levels and its tile matrices"
+    )
 
     # Private attributes
     _is_quadtree: bool = PrivateAttr()
-
-    # CRS transformation attributes
     _geographic_crs: CRSType = PrivateAttr(default=WGS84_CRS)
     _to_geographic: Transformer = PrivateAttr()
     _from_geographic: Transformer = PrivateAttr()
 
     class Config:
         """Configure TileMatrixSet."""
 
         arbitrary_types_allowed = True
         json_encoders = {CRS: lambda v: CRS_to_uri(v)}
 
     def __init__(self, **data):
         """Create PyProj transforms and check if TileMatrixSet supports quadkeys."""
+        if {"supportedCRS", "topLeftCorner"}.intersection(data):
+            raise DeprecationError(
+                "Tile Matrix Set must be version 2.0. Use morecantile <4.0 for TMS 1.0 support"
+            )
+
         super().__init__(**data)
 
-        self._is_quadtree = check_quadkey_support(self.tileMatrix)
+        self._is_quadtree = check_quadkey_support(self.tileMatrices)
 
         self._geographic_crs = data.get("_geographic_crs", WGS84_CRS)
 
         try:
             self._to_geographic = Transformer.from_crs(
-                self.supportedCRS, self._geographic_crs, always_xy=True
+                self.crs, self._geographic_crs, always_xy=True
             )
             self._from_geographic = Transformer.from_crs(
-                self._geographic_crs, self.supportedCRS, always_xy=True
+                self._geographic_crs, self.crs, always_xy=True
             )
         except ProjError:
             warnings.warn(
                 "Could not create coordinate Transformer from input CRS to the given geographic CRS"
                 "some methods might not be available.",
                 UserWarning,
             )
             self._to_geographic = None
             self._from_geographic = None
 
-    @validator("tileMatrix")
+    @validator("tileMatrices")
     def sort_tile_matrices(cls, v):
         """Sort matrices by identifier"""
-        return sorted(v, key=lambda m: int(m.identifier))
+        return sorted(v, key=lambda m: int(m.id))
 
     def __iter__(self):
         """Iterate over matrices"""
-        for matrix in self.tileMatrix:
+        for matrix in self.tileMatrices:
             yield matrix
 
     def __repr__(self):
         """Simplify default pydantic model repr."""
-        return f"<TileMatrixSet title='{self.title}' identifier='{self.identifier}'>"
+        return f"<TileMatrixSet title='{self.title}' id='{self.id}'>"
 
     @property
-    def crs(self) -> CRS:
-        """Fetch CRS from epsg"""
-        return self.supportedCRS
+    def geographic_crs(self) -> CRSType:
+        """Return the TMS's geographic CRS."""
+        return self._geographic_crs
 
     @property
     def rasterio_crs(self):
         """Return rasterio CRS."""
+        return to_rasterio_crs(self.crs)
 
-        import rasterio
-        from rasterio.env import GDALVersion
-
-        if GDALVersion.runtime().major < 3:
-            return rasterio.crs.CRS.from_wkt(self.crs.to_wkt(WktVersion.WKT1_GDAL))
-        else:
-            return rasterio.crs.CRS.from_wkt(self.crs.to_wkt())
+    @property
+    def rasterio_geographic_crs(self):
+        """Return the geographic CRS as a rasterio CRS."""
+        return to_rasterio_crs(self._geographic_crs)
 
     @property
     def minzoom(self) -> int:
         """TileMatrixSet minimum TileMatrix identifier"""
-        return int(self.tileMatrix[0].identifier)
+        return int(self.tileMatrices[0].id)
 
     @property
     def maxzoom(self) -> int:
         """TileMatrixSet maximum TileMatrix identifier"""
-        return int(self.tileMatrix[-1].identifier)
+        return int(self.tileMatrices[-1].id)
 
     @property
     def _invert_axis(self) -> bool:
         """Check if CRS has inverted AXIS (lat,lon) instead of (lon,lat)."""
-        return crs_axis_inverted(self.crs)
+        return (
+            ordered_axis_inverted(self.orderedAxes)
+            if self.orderedAxes
+            else crs_axis_inverted(self.crs)
+        )
+
+    @classmethod
+    def from_v1(cls, tms: Dict) -> "TileMatrixSet":
+        """
+        Makes a TMS from a v1 TMS definition
+
+                Attributes
+        ----------
+        supportedCRS: CRSType
+            Tile Matrix Set coordinate reference system
+        title: str
+            Title of TMS
+        abstract: str (optional)
+            Abstract of CRS
+        keywords: str (optional)
+            Keywords
+        identifier: str
+            TMS Identifier
+        wellKnownScaleSet: AnyHttpUrl (optional)
+            WKSS URL
+        boundingBox: TMSBoundingBox (optional)
+            Bounding box of TMS
+        tileMatrix: List[TileMatrix]
+            List of Tile Matrices
+
+        Returns:
+        --------
+        TileMatrixSet
+        """
+        v2_tms = tms.copy()
+
+        del v2_tms["type"]
+
+        v2_tms["crs"] = v2_tms.pop("supportedCRS")
+        v2_tms["tileMatrices"] = v2_tms.pop("tileMatrix")
+        v2_tms["id"] = v2_tms.pop("identifier")
+        mpu = meters_per_unit(CRS.from_user_input(v2_tms["crs"]))
+        for i in range(len(v2_tms["tileMatrices"])):
+            v2_tms["tileMatrices"][i]["cellSize"] = (
+                v2_tms["tileMatrices"][i]["scaleDenominator"] * 0.00028 / mpu
+            )
+            v2_tms["tileMatrices"][i]["pointOfOrigin"] = v2_tms["tileMatrices"][i].pop(
+                "topLeftCorner"
+            )
+            v2_tms["tileMatrices"][i]["id"] = v2_tms["tileMatrices"][i].pop(
+                "identifier"
+            )
+            del v2_tms["tileMatrices"][i]["type"]
+
+        return TileMatrixSet(**v2_tms)
 
     @classmethod
     def custom(
         cls,
         extent: List[float],
         crs: CRS,
         tile_width: int = 256,
         tile_height: int = 256,
         matrix_scale: Optional[List] = None,
         extent_crs: Optional[CRS] = None,
         minzoom: int = 0,
         maxzoom: int = 24,
-        title: str = "Custom TileMatrixSet",
-        identifier: str = "Custom",
+        title: Optional[str] = None,
+        id: Optional[str] = None,
+        ordered_axes: Optional[List[str]] = None,
         geographic_crs: CRS = WGS84_CRS,
+        **kwargs: Any,
     ):
         """
         Construct a custom TileMatrixSet.
 
         Attributes
         ----------
         crs: pyproj.CRS
@@ -258,121 +405,111 @@
         extent_crs: pyproj.CRS
             Extent's coordinate reference system, as a pyproj CRS object.
             (default: same as input crs)
         minzoom: int
             Tile Matrix Set minimum zoom level (default is 0).
         maxzoom: int
             Tile Matrix Set maximum zoom level (default is 24).
-        title: str
-            Tile Matrix Set title (default is 'Custom TileMatrixSet')
-        identifier: str
-            Tile Matrix Set identifier (default is 'Custom')
+        title: str, optional
+            Tile Matrix Set title
+        id: str, optional
+            Tile Matrix Set identifier
         geographic_crs: pyproj.CRS
             Geographic (lat,lon) coordinate reference system (default is EPSG:4326)
+        kwargs: Any
+            Attributes to forward to the TileMatrixSet
 
         Returns:
         --------
         TileMatrixSet
 
         """
         matrix_scale = matrix_scale or [1, 1]
 
-        tms: Dict[str, Any] = {
-            "title": title,
-            "identifier": identifier,
-            "supportedCRS": crs,
-            "tileMatrix": [],
-            "_geographic_crs": geographic_crs,
-        }
-
-        is_inverted = crs_axis_inverted(crs)
-
-        if is_inverted:
-            tms["boundingBox"] = TMSBoundingBox(
-                crs=extent_crs or crs,
-                lowerCorner=[extent[1], extent[0]],
-                upperCorner=[extent[3], extent[2]],
-            )
+        if ordered_axes:
+            is_inverted = ordered_axis_inverted(ordered_axes)
         else:
-            tms["boundingBox"] = TMSBoundingBox(
-                crs=extent_crs or crs,
-                lowerCorner=[extent[0], extent[1]],
-                upperCorner=[extent[2], extent[3]],
-            )
+            is_inverted = crs_axis_inverted(crs)
 
         if extent_crs:
             transform = Transformer.from_crs(extent_crs, crs, always_xy=True)
-            left, bottom, right, top = extent
-            bbox = BoundingBox(
-                *transform.transform_bounds(left, bottom, right, top, densify_pts=21)
-            )
-        else:
-            bbox = BoundingBox(*extent)
+            extent = transform.transform_bounds(*extent, densify_pts=21)
 
+        bbox = BoundingBox(*extent)
         x_origin = bbox.left if not is_inverted else bbox.top
         y_origin = bbox.top if not is_inverted else bbox.left
-
         width = abs(bbox.right - bbox.left)
         height = abs(bbox.top - bbox.bottom)
         mpu = meters_per_unit(crs)
+
+        tile_matrices: List[TileMatrix] = []
         for zoom in range(minzoom, maxzoom + 1):
             res = max(
                 width / (tile_width * matrix_scale[0]) / 2.0**zoom,
                 height / (tile_height * matrix_scale[1]) / 2.0**zoom,
             )
-            tms["tileMatrix"].append(
+            tile_matrices.append(
                 TileMatrix(
                     **{
-                        "identifier": str(zoom),
+                        "id": str(zoom),
                         "scaleDenominator": res * mpu / 0.00028,
-                        "topLeftCorner": [x_origin, y_origin],
+                        "cellSize": res,
+                        "pointOfOrigin": [x_origin, y_origin],
                         "tileWidth": tile_width,
                         "tileHeight": tile_height,
                         "matrixWidth": matrix_scale[0] * 2**zoom,
                         "matrixHeight": matrix_scale[1] * 2**zoom,
                     }
                 )
             )
 
-        return cls(**tms)
+        return cls(
+            crs=crs,
+            tileMatrices=tile_matrices,
+            id=id,
+            title=title,
+            _geographic_crs=geographic_crs,
+            **kwargs,
+        )
 
     def matrix(self, zoom: int) -> TileMatrix:
         """Return the TileMatrix for a specific zoom."""
-        for m in self.tileMatrix:
-            if m.identifier == str(zoom):
+        for m in self.tileMatrices:
+            if m.id == str(zoom):
                 return m
 
         matrix_scale = list(
             {
                 round(
-                    self.tileMatrix[idx].scaleDenominator
-                    / self.tileMatrix[idx - 1].scaleDenominator,
+                    self.tileMatrices[idx].scaleDenominator
+                    / self.tileMatrices[idx - 1].scaleDenominator,
                     2,
                 )
-                for idx in range(1, len(self.tileMatrix))
+                for idx in range(1, len(self.tileMatrices))
             }
         )
         if len(matrix_scale) > 1:
             raise InvalidZoomError(
                 f"TileMatrix not found for level: {zoom} - Unable to construct tileMatrix for TMS with variable scale"
             )
 
         warnings.warn(
             f"TileMatrix not found for level: {zoom} - Creating values from TMS Scale.",
             UserWarning,
         )
 
-        tile_matrix = self.tileMatrix[-1]
+        tile_matrix = self.tileMatrices[-1]
         factor = 1 / matrix_scale[0]
-        while not str(zoom) == tile_matrix.identifier:
+        while not str(zoom) == tile_matrix.id:
             tile_matrix = TileMatrix(
                 **{
-                    "identifier": str(int(tile_matrix.identifier) + 1),
+                    "id": str(int(tile_matrix.id) + 1),
                     "scaleDenominator": tile_matrix.scaleDenominator / factor,
-                    "topLeftCorner": tile_matrix.topLeftCorner,
+                    "cellSize": tile_matrix.cellSize / factor,
+                    "pointOfOrigin": tile_matrix.pointOfOrigin,
                     "tileWidth": tile_matrix.tileWidth,
                     "tileHeight": tile_matrix.tileHeight,
                     "matrixWidth": int(tile_matrix.matrixWidth * factor),
                     "matrixHeight": int(tile_matrix.matrixHeight * factor),
                 }
             )
 
@@ -511,18 +648,18 @@
         Tile
 
         """
         matrix = self.matrix(zoom)
         res = self._resolution(matrix)
 
         origin_x = (
-            matrix.topLeftCorner[1] if self._invert_axis else matrix.topLeftCorner[0]
+            matrix.pointOfOrigin[1] if self._invert_axis else matrix.pointOfOrigin[0]
         )
         origin_y = (
-            matrix.topLeftCorner[0] if self._invert_axis else matrix.topLeftCorner[1]
+            matrix.pointOfOrigin[0] if self._invert_axis else matrix.pointOfOrigin[1]
         )
 
         xtile = (
             math.floor((xcoord - origin_x) / float(res * matrix.tileWidth))
             if not math.isinf(xcoord)
             else 0
         )
@@ -583,18 +720,18 @@
         """
         t = _parse_tile_arg(*tile)
 
         matrix = self.matrix(t.z)
         res = self._resolution(matrix)
 
         origin_x = (
-            matrix.topLeftCorner[1] if self._invert_axis else matrix.topLeftCorner[0]
+            matrix.pointOfOrigin[1] if self._invert_axis else matrix.pointOfOrigin[0]
         )
         origin_y = (
-            matrix.topLeftCorner[0] if self._invert_axis else matrix.topLeftCorner[1]
+            matrix.pointOfOrigin[0] if self._invert_axis else matrix.pointOfOrigin[1]
         )
 
         xcoord = origin_x + t.x * res * matrix.tileWidth
         ycoord = origin_y - t.y * res * matrix.tileHeight
         return Coords(xcoord, ycoord)
 
     def xy_bounds(self, *tile: Tile) -> BoundingBox:
@@ -652,58 +789,27 @@
         left, top = self.ul(t)
         right, bottom = self.ul(Tile(t.x + 1, t.y + 1, t.z))
         return BoundingBox(left, bottom, right, top)
 
     @property
     def xy_bbox(self):
         """Return TMS bounding box in TileMatrixSet's CRS."""
-        if self.boundingBox:
-            left = (
-                self.boundingBox.lowerCorner[1]
-                if self._invert_axis
-                else self.boundingBox.lowerCorner[0]
-            )
-            bottom = (
-                self.boundingBox.lowerCorner[0]
-                if self._invert_axis
-                else self.boundingBox.lowerCorner[1]
-            )
-            right = (
-                self.boundingBox.upperCorner[1]
-                if self._invert_axis
-                else self.boundingBox.upperCorner[0]
-            )
-            top = (
-                self.boundingBox.upperCorner[0]
-                if self._invert_axis
-                else self.boundingBox.upperCorner[1]
-            )
-            if self.boundingBox.crs != self.crs:
-                transform = Transformer.from_crs(
-                    self.boundingBox.crs, self.crs, always_xy=True
-                )
-                left, bottom, right, top = transform.transform_bounds(
-                    left,
-                    bottom,
-                    right,
-                    top,
-                    densify_pts=21,
-                )
+        zoom = self.minzoom
+        matrix = self.matrix(zoom)
 
-        else:
-            zoom = self.minzoom
-            matrix = self.matrix(zoom)
-            left, top = self._ul(Tile(0, 0, zoom))
-            right, bottom = self._ul(
-                Tile(matrix.matrixWidth, matrix.matrixHeight, zoom)
-            )
+        left, top = self._ul(Tile(0, 0, zoom))
+        right, bottom = self._ul(Tile(matrix.matrixWidth, matrix.matrixHeight, zoom))
 
         return BoundingBox(left, bottom, right, top)
 
     @property
+    @cached(  # type: ignore
+        LRUCache(maxsize=512),
+        key=lambda self: hashkey(self.id, self.tileMatrices[0].pointOfOrigin),
+    )
     def bbox(self):
         """Return TMS bounding box in geographic coordinate reference system."""
         left, bottom, right, top = self.xy_bbox
         return BoundingBox(
             *self._to_geographic.transform_bounds(
                 left,
                 bottom,
@@ -740,15 +846,15 @@
         Parameters
         ----------
         west, south, east, north : sequence of float
             Bounding values in decimal degrees (geographic CRS).
         zooms : int or sequence of int
             One or more zoom levels.
         truncate : bool, optional
-            Whether or not to truncate inputs to web mercator limits.
+            Whether or not to truncate inputs to TMS limits.
 
         Yields
         ------
         Tile
 
         Notes
         -----
@@ -774,21 +880,26 @@
             # Clamp bounding values.
             w = max(self.bbox.left, w)
             s = max(self.bbox.bottom, s)
             e = min(self.bbox.right, e)
             n = min(self.bbox.top, n)
 
             for z in zooms:
-                ul_tile = self.tile(
+                nw_tile = self.tile(
                     w + LL_EPSILON, n - LL_EPSILON, z
                 )  # Not in mercantile
-                lr_tile = self.tile(e - LL_EPSILON, s + LL_EPSILON, z)
+                se_tile = self.tile(e - LL_EPSILON, s + LL_EPSILON, z)
+
+                minx = min(nw_tile.x, se_tile.x)
+                maxx = max(nw_tile.x, se_tile.x)
+                miny = min(nw_tile.y, se_tile.y)
+                maxy = max(nw_tile.y, se_tile.y)
 
-                for i in range(ul_tile.x, lr_tile.x + 1):
-                    for j in range(ul_tile.y, lr_tile.y + 1):
+                for i in range(minx, maxx + 1):
+                    for j in range(miny, maxy + 1):
                         yield Tile(i, j, z)
 
     def feature(
         self,
         tile: Tile,
         fid: Optional[str] = None,
         props: Optional[Dict] = None,
@@ -847,15 +958,15 @@
         feat: Dict[str, Any] = {
             "type": "Feature",
             "bbox": bbox,
             "id": xyz,
             "geometry": geom,
             "properties": {
                 "title": f"XYZ tile {xyz}",
-                "grid_name": self.identifier,
+                "grid_name": self.id,
                 "grid_crs": self.crs.to_string(),
             },
         }
 
         if projected:
             warnings.warn(
                 "CRS is no longer part of the GeoJSON specification."
@@ -1059,16 +1170,16 @@
         The children are ordered: top-left, top-right, bottom-right, bottom-left.
 
         Parameters
         ----------
         tile : Tile or sequence of int
             May be be either an instance of Tile or 3 ints, X, Y, Z.
         zoom : int, optional
-            Determines the *zoom* level of the returned parent tile.
-            This defaults to one lower than the tile (the immediate parent).
+            Determines the *zoom* level of the returned child tiles.
+            This defaults to one higher than the tile (the immediate children).
 
         Returns
         -------
         list: list of Tile
 
         """
         t = _parse_tile_arg(*tile)
```

### Comparing `morecantile-3.3.0/morecantile/scripts/cli.py` & `morecantile-4.0.0a0/morecantile/scripts/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,15 +427,15 @@
 ):
     """Create Custom TMS."""
     extent_crs = CRS.from_epsg(extent_epsg) if extent_epsg else None
 
     tms = morecantile.TileMatrixSet.custom(
         extent,
         CRS.from_epsg(epsg),
-        identifier=name,
+        id=name,
         minzoom=minzoom,
         maxzoom=maxzoom,
         tile_width=tile_width,
         tile_height=tile_height,
         extent_crs=extent_crs,
         title=title or "Custom TileMatrixSet",
     )
```

### Comparing `morecantile-3.3.0/morecantile/utils.py` & `morecantile-4.0.0a0/morecantile/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """morecantile utils."""
 
 import math
 from typing import Dict, List
 
 from pyproj import CRS
+from pyproj.enums import WktVersion
 
 from morecantile.commons import BoundingBox, Coords, Tile
 from morecantile.errors import TileArgParsingError
 
 
 def _parse_tile_arg(*args) -> Tile:
     """
@@ -96,7 +97,18 @@
         [
             (t.matrixWidth == t.matrixHeight)
             and is_power_of_two(t.matrixWidth)
             and ((t.matrixWidth * 2) == tms[i + 1].matrixWidth)
             for i, t in enumerate(tms[:-1])
         ]
     )
+
+
+def to_rasterio_crs(incrs: CRS):
+    """Convert a pyproj CRS to a rasterio CRS"""
+    from rasterio import crs
+    from rasterio.env import GDALVersion
+
+    if GDALVersion.runtime().major < 3:
+        return crs.CRS.from_wkt(incrs.to_wkt(WktVersion.WKT1_GDAL))
+    else:
+        return crs.CRS.from_wkt(incrs.to_wkt())
```

### Comparing `morecantile-3.3.0/pyproject.toml` & `morecantile-4.0.0a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -19,24 +19,26 @@
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = ["version"]
 dependencies = [
     "attrs",
     "pyproj~=3.1",
     "pydantic",
+    "cachetools",
 ]
 
 [project.optional-dependencies]
 rasterio = [
     "rasterio>=1.2.1",
 ]
 test = [
     "mercantile",
     "pytest",
     "pytest-cov",
+    "rasterio>=1.2.1",
 ]
 dev = [
     "pre-commit",
 ]
 docs = [
     "mkdocs",
     "mkdocs-material",
@@ -87,14 +89,15 @@
 no_strict_optional = true
 
 [tool.ruff]
 select = [
     "D1",  # pydocstyle errors
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
+    "F",  # flake8
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "B905",  # ignore zip() without an explicit strict= parameter, only support with python >3.10
```

### Comparing `morecantile-3.3.0/PKG-INFO` & `morecantile-4.0.0a0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morecantile
-Version: 3.3.0
+Version: 4.0.0a0
 Summary: Construct and use map tile grids (a.k.a TileMatrixSet / TMS).
 Keywords: GIS,TMS,TileMatrixSet,Map Tile
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -13,51 +13,37 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: attrs
 Requires-Dist: pyproj~=3.1
 Requires-Dist: pydantic
+Requires-Dist: cachetools
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: mkdocs ; extra == "docs"
 Requires-Dist: mkdocs-material ; extra == "docs"
 Requires-Dist: pygments ; extra == "docs"
 Requires-Dist: rasterio>=1.2.1 ; extra == "rasterio"
 Requires-Dist: mercantile ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
+Requires-Dist: rasterio>=1.2.1 ; extra == "test"
 Project-URL: Documentation, https://developmentseed.org/morecantile/
 Project-URL: Source, https://github.com/developmentseed/morecantile
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: rasterio
 Provides-Extra: test
 
 # Morecantile
 
-```
-    +-------------+-------------+  ymax
-    |             |             |
-    |    x: 0     |    x: 1     |
-    |    y: 0     |    y: 0     |
-    |    z: 1     |    z: 1     |
-    |             |             |
-    +-------------+-------------+
-    |             |             |
-    |    x: 0     |    x: 1     |
-    |    y: 1     |    y: 1     |
-    |    z: 1     |    z: 1     |
-    |             |             |
-    +-------------+-------------+  ymin
-
-xmin                            xmax
-```
-
 <p align="center">
-  <em>Construct and use map tile grids (a.k.a TileMatrixSet / TMS).</em>
+  <img height="500" src="https://github.com/developmentseed/morecantile/assets/10407788/a1523c6d-e255-4dc6-a201-20029715858a"/>
+  <p align="center">Construct and use map tile grids (a.k.a TileMatrixSet / TMS).</p>
+
 </p>
 <p align="center">
   <a href="https://github.com/developmentseed/morecantile/actions?query=workflow%3ACI" target="_blank">
       <img src="https://github.com/developmentseed/morecantile/workflows/CI/badge.svg" alt="Test">
   </a>
   <a href="https://codecov.io/gh/developmentseed/morecantile" target="_blank">
       <img src="https://codecov.io/gh/developmentseed/morecantile/branch/main/graph/badge.svg" alt="Coverage">
@@ -79,52 +65,97 @@
 
 **Source Code**: <a href="https://github.com/developmentseed/morecantile" target="_blank">https://github.com/developmentseed/morecantile</a>
 
 ---
 
 Morecantile is like [mercantile](https://github.com/mapbox/mercantile) (the best tool to work with Web Mercator tile indexes), but with support for other TileMatrixSet grids.
 
-**Morecantile** follows the **OGC Two Dimensional Tile Matrix Set** specification found in [http://docs.opengeospatial.org/is/17-083r2/17-083r2.html](http://docs.opengeospatial.org/is/17-083r2/17-083r2.html)
+**Morecantile** follows the **OGC Two Dimensional Tile Matrix Set** specification **2.0** found in [https://docs.ogc.org/is/17-083r4/17-083r4.html](https://docs.ogc.org/is/17-083r4/17-083r4.html)
+
+| Morecantile Version | OGC Specification Version | Link
+| ------------------- | ------------------------- |---------
+| 4.0                 | 2.0                       | https://docs.ogc.org/is/17-083r4/17-083r4.html
+| 3.0 and earlier     | 1.0                       | http://docs.opengeospatial.org/is/17-083r2/17-083r2.html
 
 **Note**: Variable matrix width tile set are not supported.
 
 ## Install
 
 ```bash
 $ python -m pip install -U pip
 $ python -m pip install morecantile
 
 # Or install from source:
-
 $ python -m pip install -U pip
 $ python -m pip install git+https://github.com/developmentseed/morecantile.git
 ```
 
+## Usage
+
+```python
+import morecantile
+
+tms = morecantile.tms.get("WebMercatorQuad")
+
+# Get TMS bounding box
+print(tms.xy_bbox)
+>>> BoundingBox(
+    left=-20037508.342789244,
+    bottom=-20037508.34278919,
+    right=20037508.34278919,
+    top=20037508.342789244,
+)
+
+# Get the bounds for tile Z=4, X=10, Y=10 in the TMS's CRS (e.g epsg:3857)
+print(tms.xy_bounds(morecantile.Tile(10, 10, 4)))
+>>> BoundingBox(
+    left=5009377.085697308,
+    bottom=-7514065.628545959,
+    right=7514065.628545959,
+    top=-5009377.085697308,
+)
+
+# Get the bounds for tile Z=4, X=10, Y=10 in Geographic CRS (e.g epsg:4326)
+print(tms.bounds(morecantile.Tile(10, 10, 4)))
+>>> BoundingBox(
+    left=44.999999999999964,
+    bottom=-55.776573018667634,
+    right=67.4999999999999,
+    top=-40.97989806962009,
+)
+```
+
+More info can be found at https://developmentseed.org/morecantile/usage/
+
 ### Defaults Grids
 
+`morecantile` provides a set of default TMS grids:
+
 - **CanadianNAD83_LCC**: Lambert conformal conic NAD83 for Canada - EPSG:3978
 - **EuropeanETRS89_LAEAQuad**: ETRS89-extended / LAEA Europe - EPGS:3035
 - **LINZAntarticaMapTilegrid**: LINZ Antarctic Map Tile Grid (Ross Sea Region) - EPSG:5482
-- **NZTM2000**: LINZ NZTM2000 Map Tile Grid - EPSG:2193
 - **NZTM2000Quad**: LINZ NZTM2000 Map Tile Grid - EPSG:2193
 - **UPSAntarcticWGS84Quad**: Universal Polar Stereographic WGS 84 Quad for Antarctic - EPSG:5042
 - **UPSArcticWGS84Quad**: Universal Polar Stereographic WGS 84 Quad for Arctic - EPSG:5041
 - **UTM31WGS84Quad**: Example of UTM grid - EPSG:32631
 - **WebMercatorQuad**: Spherical Mercator - EPGS:3857 (default grid for Web Mercator based maps)
 - **WGS1984Quad**: EPSG:4326 for the World - EPGS:4326 (WGS84)
 - **WorldCRS84Quad**: CRS84 for the World
 - **WorldMercatorWGS84Quad**: Elliptical Mercator projection - EPGS:3395
 
-ref: http://schemas.opengis.net/tms/1.0/json/examples/
+ref: https://schemas.opengis.net/tms/2.0/json/examples/tilematrixset/
 
 ## Implementations
 
 - [rio-tiler](https://github.com/cogeotiff/rio-tiler): Create tile from raster using Morecantile TMS.
-- [timvt](https://github.com/developmentseed/timvt): A lightweight PostGIS based dynamic vector tile server.
+- [titiler](https://github.com/developmentseed/titiler): A modern dynamic tile server built on top of FastAPI and Rasterio/GDAL.
+- [tipg](https://github.com/developmentseed/tipg): OGC Features and Tiles API.
 - [planetcantile](https://github.com/AndrewAnnex/planetcantile): Tile matrix sets for other planets.
+- [supermorecado](https://github.com/developmentseed/supermorecado): Extend the functionality of morecantile with additional commands.
+
 
 ## Changes
 
 See [CHANGES.md](https://github.com/developmentseed/morecantile/blob/main/CHANGES.md).
 
 ## Contribution & Development
```

#### html2text {}

```diff
@@ -1,58 +1,75 @@
-Metadata-Version: 2.1 Name: morecantile Version: 3.3.0 Summary: Construct and
+Metadata-Version: 2.1 Name: morecantile Version: 4.0.0a0 Summary: Construct and
 use map tile grids (a.k.a TileMatrixSet / TMS). Keywords:
 GIS,TMS,TileMatrixSet,Map Tile Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering :: GIS Requires-Dist: attrs Requires-Dist:
-pyproj~=3.1 Requires-Dist: pydantic Requires-Dist: pre-commit ; extra == "dev"
-Requires-Dist: mkdocs ; extra == "docs" Requires-Dist: mkdocs-material ; extra
-== "docs" Requires-Dist: pygments ; extra == "docs" Requires-Dist:
-rasterio>=1.2.1 ; extra == "rasterio" Requires-Dist: mercantile ; extra ==
-"test" Requires-Dist: pytest ; extra == "test" Requires-Dist: pytest-cov ;
-extra == "test" Project-URL: Documentation, https://developmentseed.org/
-morecantile/ Project-URL: Source, https://github.com/developmentseed/
-morecantile Provides-Extra: dev Provides-Extra: docs Provides-Extra: rasterio
-Provides-Extra: test # Morecantile ``` +-------------+-------------+ ymax | | |
-| x: 0 | x: 1 | | y: 0 | y: 0 | | z: 1 | z: 1 | | | | +-------------+----------
----+ | | | | x: 0 | x: 1 | | y: 1 | y: 1 | | z: 1 | z: 1 | | | | +-------------
-+-------------+ ymin xmin xmax ```
+pyproj~=3.1 Requires-Dist: pydantic Requires-Dist: cachetools Requires-Dist:
+pre-commit ; extra == "dev" Requires-Dist: mkdocs ; extra == "docs" Requires-
+Dist: mkdocs-material ; extra == "docs" Requires-Dist: pygments ; extra ==
+"docs" Requires-Dist: rasterio>=1.2.1 ; extra == "rasterio" Requires-Dist:
+mercantile ; extra == "test" Requires-Dist: pytest ; extra == "test" Requires-
+Dist: pytest-cov ; extra == "test" Requires-Dist: rasterio>=1.2.1 ; extra ==
+"test" Project-URL: Documentation, https://developmentseed.org/morecantile/
+Project-URL: Source, https://github.com/developmentseed/morecantile Provides-
+Extra: dev Provides-Extra: docs Provides-Extra: rasterio Provides-Extra: test #
+Morecantile
+[https://github.com/developmentseed/morecantile/assets/10407788/a1523c6d-e255-
+                            4dc6-a201-20029715858a]
          Construct and use map tile grids (a.k.a TileMatrixSet / TMS).
            [Test] [Coverage] [Package_version] [Downloads] [License]
 --- **Documentation**: https://developmentseed.org/morecantile/ **Source
 Code**: https://github.com/developmentseed/morecantile --- Morecantile is like
 [mercantile](https://github.com/mapbox/mercantile) (the best tool to work with
 Web Mercator tile indexes), but with support for other TileMatrixSet grids.
 **Morecantile** follows the **OGC Two Dimensional Tile Matrix Set**
-specification found in [http://docs.opengeospatial.org/is/17-083r2/17-
-083r2.html](http://docs.opengeospatial.org/is/17-083r2/17-083r2.html) **Note**:
-Variable matrix width tile set are not supported. ## Install ```bash $ python -
-m pip install -U pip $ python -m pip install morecantile # Or install from
-source: $ python -m pip install -U pip $ python -m pip install git+https://
-github.com/developmentseed/morecantile.git ``` ### Defaults Grids -
-**CanadianNAD83_LCC**: Lambert conformal conic NAD83 for Canada - EPSG:3978 -
-**EuropeanETRS89_LAEAQuad**: ETRS89-extended / LAEA Europe - EPGS:3035 -
-**LINZAntarticaMapTilegrid**: LINZ Antarctic Map Tile Grid (Ross Sea Region) -
-EPSG:5482 - **NZTM2000**: LINZ NZTM2000 Map Tile Grid - EPSG:2193 -
-**NZTM2000Quad**: LINZ NZTM2000 Map Tile Grid - EPSG:2193 -
-**UPSAntarcticWGS84Quad**: Universal Polar Stereographic WGS 84 Quad for
-Antarctic - EPSG:5042 - **UPSArcticWGS84Quad**: Universal Polar Stereographic
-WGS 84 Quad for Arctic - EPSG:5041 - **UTM31WGS84Quad**: Example of UTM grid -
-EPSG:32631 - **WebMercatorQuad**: Spherical Mercator - EPGS:3857 (default grid
-for Web Mercator based maps) - **WGS1984Quad**: EPSG:4326 for the World - EPGS:
-4326 (WGS84) - **WorldCRS84Quad**: CRS84 for the World -
-**WorldMercatorWGS84Quad**: Elliptical Mercator projection - EPGS:3395 ref:
-http://schemas.opengis.net/tms/1.0/json/examples/ ## Implementations - [rio-
-tiler](https://github.com/cogeotiff/rio-tiler): Create tile from raster using
-Morecantile TMS. - [timvt](https://github.com/developmentseed/timvt): A
-lightweight PostGIS based dynamic vector tile server. - [planetcantile](https:/
-/github.com/AndrewAnnex/planetcantile): Tile matrix sets for other planets. ##
-Changes See [CHANGES.md](https://github.com/developmentseed/morecantile/blob/
-main/CHANGES.md). ## Contribution & Development See [CONTRIBUTING.md](https://
+specification **2.0** found in [https://docs.ogc.org/is/17-083r4/17-083r4.html]
+(https://docs.ogc.org/is/17-083r4/17-083r4.html) | Morecantile Version | OGC
+Specification Version | Link | ------------------- | ------------------------
+- |--------- | 4.0 | 2.0 | https://docs.ogc.org/is/17-083r4/17-083r4.html | 3.0
+and earlier | 1.0 | http://docs.opengeospatial.org/is/17-083r2/17-083r2.html
+**Note**: Variable matrix width tile set are not supported. ## Install ```bash
+$ python -m pip install -U pip $ python -m pip install morecantile # Or install
+from source: $ python -m pip install -U pip $ python -m pip install git+https:/
+/github.com/developmentseed/morecantile.git ``` ## Usage ```python import
+morecantile tms = morecantile.tms.get("WebMercatorQuad") # Get TMS bounding box
+print(tms.xy_bbox) >>> BoundingBox( left=-20037508.342789244, bottom=-
+20037508.34278919, right=20037508.34278919, top=20037508.342789244, ) # Get the
+bounds for tile Z=4, X=10, Y=10 in the TMS's CRS (e.g epsg:3857) print
+(tms.xy_bounds(morecantile.Tile(10, 10, 4))) >>> BoundingBox
+( left=5009377.085697308, bottom=-7514065.628545959, right=7514065.628545959,
+top=-5009377.085697308, ) # Get the bounds for tile Z=4, X=10, Y=10 in
+Geographic CRS (e.g epsg:4326) print(tms.bounds(morecantile.Tile(10, 10, 4)))
+>>> BoundingBox( left=44.999999999999964, bottom=-55.776573018667634,
+right=67.4999999999999, top=-40.97989806962009, ) ``` More info can be found at
+https://developmentseed.org/morecantile/usage/ ### Defaults Grids `morecantile`
+provides a set of default TMS grids: - **CanadianNAD83_LCC**: Lambert conformal
+conic NAD83 for Canada - EPSG:3978 - **EuropeanETRS89_LAEAQuad**: ETRS89-
+extended / LAEA Europe - EPGS:3035 - **LINZAntarticaMapTilegrid**: LINZ
+Antarctic Map Tile Grid (Ross Sea Region) - EPSG:5482 - **NZTM2000Quad**: LINZ
+NZTM2000 Map Tile Grid - EPSG:2193 - **UPSAntarcticWGS84Quad**: Universal Polar
+Stereographic WGS 84 Quad for Antarctic - EPSG:5042 - **UPSArcticWGS84Quad**:
+Universal Polar Stereographic WGS 84 Quad for Arctic - EPSG:5041 -
+**UTM31WGS84Quad**: Example of UTM grid - EPSG:32631 - **WebMercatorQuad**:
+Spherical Mercator - EPGS:3857 (default grid for Web Mercator based maps) -
+**WGS1984Quad**: EPSG:4326 for the World - EPGS:4326 (WGS84) -
+**WorldCRS84Quad**: CRS84 for the World - **WorldMercatorWGS84Quad**:
+Elliptical Mercator projection - EPGS:3395 ref: https://schemas.opengis.net/
+tms/2.0/json/examples/tilematrixset/ ## Implementations - [rio-tiler](https://
+github.com/cogeotiff/rio-tiler): Create tile from raster using Morecantile TMS.
+- [titiler](https://github.com/developmentseed/titiler): A modern dynamic tile
+server built on top of FastAPI and Rasterio/GDAL. - [tipg](https://github.com/
+developmentseed/tipg): OGC Features and Tiles API. - [planetcantile](https://
+github.com/AndrewAnnex/planetcantile): Tile matrix sets for other planets. -
+[supermorecado](https://github.com/developmentseed/supermorecado): Extend the
+functionality of morecantile with additional commands. ## Changes See
+[CHANGES.md](https://github.com/developmentseed/morecantile/blob/main/
+CHANGES.md). ## Contribution & Development See [CONTRIBUTING.md](https://
 github.com/developmentseed/morecantile/blob/main/CONTRIBUTING.md) ## License
 See [LICENSE](https://github.com/developmentseed/morecantile/blob/main/LICENSE)
 ## Authors Created by [Development Seed](
 developmentseed.org>)
```

