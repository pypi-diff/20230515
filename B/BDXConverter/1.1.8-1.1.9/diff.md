# Comparing `tmp/BDXConverter-1.1.8.tar.gz` & `tmp/BDXConverter-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDXConverter-1.1.8.tar", last modified: Sun May 14 02:38:15 2023, max compression
+gzip compressed data, was "BDXConverter-1.1.9.tar", last modified: Sun May 14 07:36:35 2023, max compression
```

## Comparing `BDXConverter-1.1.8.tar` & `BDXConverter-1.1.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:15.097141 BDXConverter-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:15.085140 BDXConverter-1.1.8/BDXConverter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:15.089141 BDXConverter-1.1.8/BDXConverter/Converter/
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Converter/Converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Converter/ErrorClassDefine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Converter/FileOperation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Converter/Signature.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:15.089141 BDXConverter-1.1.8/BDXConverter/General/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/General/GeneralClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/General/Operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/General/Pool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/General/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:15.093141 BDXConverter-1.1.8/BDXConverter/Operation/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt16XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt16YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt16ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt16ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt32XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt32YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt32ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt32ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt8XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt8YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt8ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AssignDebugData.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/CreateConstantString.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/NOP.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithBlockStates.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithNBTData.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/SetCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/SubtractXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/SubtractYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/SubtractZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/UseRuntimeIDPool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/structOfChest.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:15.093141 BDXConverter-1.1.8/BDXConverter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/utils/getByte.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/utils/getString.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/utils/marshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/utils/marshalNBT_OldVersion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/utils/unmarshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/utils/unmarshalNBT_OldVersion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:15.085140 BDXConverter-1.1.8/BDXConverter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-05-14 02:38:15.000000 BDXConverter-1.1.8/BDXConverter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-14 02:38:15.000000 BDXConverter-1.1.8/BDXConverter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 02:38:15.000000 BDXConverter-1.1.8/BDXConverter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 02:38:15.000000 BDXConverter-1.1.8/BDXConverter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-14 02:38:15.000000 BDXConverter-1.1.8/BDXConverter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-05-14 02:38:15.097141 BDXConverter-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 02:38:15.097141 BDXConverter-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:36:35.432253 BDXConverter-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:36:35.424252 BDXConverter-1.1.9/BDXConverter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:36:35.424252 BDXConverter-1.1.9/BDXConverter/Converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Converter/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Converter/ErrorClassDefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Converter/FileOperation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Converter/Signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:36:35.424252 BDXConverter-1.1.9/BDXConverter/General/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/General/GeneralClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/General/Operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/General/Pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/General/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:36:35.432253 BDXConverter-1.1.9/BDXConverter/Operation/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddInt16XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddInt16YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddInt16ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddInt16ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddInt32XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddInt32YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddInt32ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddInt32ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddInt8XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddInt8YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddInt8ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AddZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/AssignDebugData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/CreateConstantString.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/NOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/PlaceBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/PlaceBlockWithBlockStates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/PlaceBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/PlaceBlockWithNBTData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/PlaceRuntimeBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/SetCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/SubtractXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/SubtractYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/SubtractZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/UseRuntimeIDPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/Operation/structOfChest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:36:35.432253 BDXConverter-1.1.9/BDXConverter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/utils/getByte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/utils/getString.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/utils/marshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/utils/marshalNBT_OldVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/utils/unmarshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/BDXConverter/utils/unmarshalNBT_OldVersion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:36:35.424252 BDXConverter-1.1.9/BDXConverter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-05-14 07:36:35.000000 BDXConverter-1.1.9/BDXConverter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-14 07:36:35.000000 BDXConverter-1.1.9/BDXConverter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 07:36:35.000000 BDXConverter-1.1.9/BDXConverter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 07:36:35.000000 BDXConverter-1.1.9/BDXConverter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-14 07:36:35.000000 BDXConverter-1.1.9/BDXConverter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-05-14 07:36:35.432253 BDXConverter-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 07:36:35.432253 BDXConverter-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-14 07:36:25.000000 BDXConverter-1.1.9/setup.py
```

### Comparing `BDXConverter-1.1.8/BDXConverter/Converter/Converter.py` & `BDXConverter-1.1.9/BDXConverter/Converter/Converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                 elif errorType == 2:
                     raise readError(reader.seek(0, 1))
                 # if meet error
                 self.BDXContent.append(struct)
                 # submit single datas
         # read datas from reader
         self.Signature.UnMarshal(reader)
-        if self.Signature.isLegacy == False:
+        if self.Signature.isLegacy == False and self.Signature.signedOrNeedToSign == True:
             reader.truncate(reader.seek(-1, 1))
             self.Signature.BDXContentWithInsideHeader = reader
             self.Signature.verifySignature()
         # signature
 
     def Loads(self, jsonDict: dict) -> None:
         BDXCommandPool: dict[int, GeneralClass] = GetBDXCommandPool()
```

### Comparing `BDXConverter-1.1.8/BDXConverter/Converter/ErrorClassDefine.py` & `BDXConverter-1.1.9/BDXConverter/Converter/ErrorClassDefine.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Converter/FileOperation.py` & `BDXConverter-1.1.9/BDXConverter/Converter/FileOperation.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Converter/Signature.py` & `BDXConverter-1.1.9/BDXConverter/Converter/Signature.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/General/GeneralClass.py` & `BDXConverter-1.1.9/BDXConverter/General/GeneralClass.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/General/Operation.py` & `BDXConverter-1.1.9/BDXConverter/General/Operation.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/General/Pool.py` & `BDXConverter-1.1.9/BDXConverter/General/Pool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/AddInt16XValue.py` & `BDXConverter-1.1.9/BDXConverter/Operation/AddInt16XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/AddInt16YValue.py` & `BDXConverter-1.1.9/BDXConverter/Operation/AddInt16YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/AddInt16ZValue.py` & `BDXConverter-1.1.9/BDXConverter/Operation/AddInt16ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/AddInt16ZValue0.py` & `BDXConverter-1.1.9/BDXConverter/Operation/AddInt16ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/AddInt32XValue.py` & `BDXConverter-1.1.9/BDXConverter/Operation/AddInt32XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/AddInt32YValue.py` & `BDXConverter-1.1.9/BDXConverter/Operation/AddInt32YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/AddInt32ZValue.py` & `BDXConverter-1.1.9/BDXConverter/Operation/AddInt32ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/AddInt32ZValue0.py` & `BDXConverter-1.1.9/BDXConverter/Operation/AddInt32ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/AddInt8XValue.py` & `BDXConverter-1.1.9/BDXConverter/Operation/AddInt8XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/AddInt8YValue.py` & `BDXConverter-1.1.9/BDXConverter/Operation/AddInt8YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/AddInt8ZValue.py` & `BDXConverter-1.1.9/BDXConverter/Operation/AddInt8ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/AssignDebugData.py` & `BDXConverter-1.1.9/BDXConverter/Operation/AssignDebugData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/CreateConstantString.py` & `BDXConverter-1.1.9/BDXConverter/Operation/CreateConstantString.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlock.py` & `BDXConverter-1.1.9/BDXConverter/Operation/PlaceBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithBlockStates.py` & `BDXConverter-1.1.9/BDXConverter/Operation/PlaceBlockWithBlockStates.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py` & `BDXConverter-1.1.9/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithChestData.py` & `BDXConverter-1.1.9/BDXConverter/Operation/PlaceBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py` & `BDXConverter-1.1.9/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithNBTData.py` & `BDXConverter-1.1.9/BDXConverter/Operation/PlaceBlockWithNBTData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithRuntimeId.py` & `BDXConverter-1.1.9/BDXConverter/Operation/PlaceBlockWithRuntimeId.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py` & `BDXConverter-1.1.9/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlock.py` & `BDXConverter-1.1.9/BDXConverter/Operation/PlaceRuntimeBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py` & `BDXConverter-1.1.9/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py` & `BDXConverter-1.1.9/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py` & `BDXConverter-1.1.9/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py` & `BDXConverter-1.1.9/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/SetCommandBlockData.py` & `BDXConverter-1.1.9/BDXConverter/Operation/SetCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/UseRuntimeIDPool.py` & `BDXConverter-1.1.9/BDXConverter/Operation/UseRuntimeIDPool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/Operation/structOfChest.py` & `BDXConverter-1.1.9/BDXConverter/Operation/structOfChest.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/utils/marshalNBT.py` & `BDXConverter-1.1.9/BDXConverter/utils/marshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/utils/marshalNBT_OldVersion.py` & `BDXConverter-1.1.9/BDXConverter/utils/marshalNBT_OldVersion.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/utils/unmarshalNBT.py` & `BDXConverter-1.1.9/BDXConverter/utils/unmarshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter/utils/unmarshalNBT_OldVersion.py` & `BDXConverter-1.1.9/BDXConverter/utils/unmarshalNBT_OldVersion.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/BDXConverter.egg-info/PKG-INFO` & `BDXConverter-1.1.9/BDXConverter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.1.8
+Version: 1.1.9
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -65,14 +65,16 @@
 
 
 # 注意事项
 ## 兼容性
 - 版本 `1.1.0` 不兼容之前的所有版本
 - 版本 `1.0.16` 在可视化和反可视化字典方面不兼容之前的版本
 
+
+
 ## 签名
 - `BDX` 文件格式是由 `PhoenixBuilder` 所定义，签名 `BDX` 文件则必须具备 `PhoenixBuilder` 账户
 - 由于一些原因，您需要自行获取 `签名` 时的 `Prove` 和 `PrivateSigningKey` ，以下展示了获取方法。有关本项目实现的签名功能，请见 [`BDXConverter/Converter/Signature.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Signature.py)
 
   ```python
   """
   import ecdsa
@@ -130,14 +132,15 @@
   ```
   - `PhoenixBuilder Auth Server` 使用了 `Cloudflared` 来代理(加速)它的 `Websocket` 服务器，因此您无法直接使用 `Python` 的 `Websocket` 库来连接此服务器。目前尚且未找到对应的解决办法，一个替代方案是使用 `Golang` 下的 `Websocket` 库与 `PhoenixBuilder Auth Server` 建立连接
     - 其他帮助信息另见 https://github.com/huashengdun/webssh/issues/141
 
 
 
 
+
 # 快速上手
 您可以利用 [`BDXConverter/Converter/FileOperation.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/FileOperation.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
 
 
 
 
 
@@ -148,14 +151,16 @@
 
 我们配置了自动化 `CD/CI 工作流` ，因此如果您是本项目的 `协作者` ，您可以通过更改 `version` 文件或通过手动触发的方式启动工作流，它会自动编译本项目并将将其上载到 `Pypi` 中。
 
 _[注：我们建议您在 `Python 3.10` 及以上的版本使用本项目，`3.7` 及以下的版本已不再受到 `Python` 的维护和更新]_
 
 
 
+
+
 # 第三方依赖
 本项目使用了 `brotli, nbtlib` 和 `pycryptodome` 总计 `3` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
 
 ```
 pip install brotli
 pip install nbtlib
 pip install pycryptodome
@@ -215,14 +220,18 @@
 
 
 # 什么是 `BDX` 文件
 `PhoenixBuilder` 是一个用于 `网易我的世界中国版 · 基岩版租赁服` 的商业化快速建造器，而 `BDX` 文件则是此建造器用于存储 `Minecraft` 建筑结构的 `私有文件格式` 。
 
 如果您希望解析 `BDX` 文件，敬请参阅 [`bdump-cn.md`](https://github.com/LNSSPsd/PhoenixBuilder/blob/main/doc/bdump/bdump-cn.md) 。
 
+
+
+
+
 # 关于 `PhoenixBuilder`
 - 您可以通过此链接访问 `PhoenixBuilder` 的存储库
    - [`PhoenixBuilder`](https://github.com/LNSSPsd/PhoenixBuilder/)
 - 您可以通过下述链接访问 `PhoenixBuilder` 的相关网站
    - [`用户中心`](https://uc.fastbuilder.pro/)
    - [`官方网站`](https://fastbuilder.pro/)
```

### Comparing `BDXConverter-1.1.8/BDXConverter.egg-info/SOURCES.txt` & `BDXConverter-1.1.9/BDXConverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/LICENSE` & `BDXConverter-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.8/PKG-INFO` & `BDXConverter-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.1.8
+Version: 1.1.9
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -65,14 +65,16 @@
 
 
 # 注意事项
 ## 兼容性
 - 版本 `1.1.0` 不兼容之前的所有版本
 - 版本 `1.0.16` 在可视化和反可视化字典方面不兼容之前的版本
 
+
+
 ## 签名
 - `BDX` 文件格式是由 `PhoenixBuilder` 所定义，签名 `BDX` 文件则必须具备 `PhoenixBuilder` 账户
 - 由于一些原因，您需要自行获取 `签名` 时的 `Prove` 和 `PrivateSigningKey` ，以下展示了获取方法。有关本项目实现的签名功能，请见 [`BDXConverter/Converter/Signature.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Signature.py)
 
   ```python
   """
   import ecdsa
@@ -130,14 +132,15 @@
   ```
   - `PhoenixBuilder Auth Server` 使用了 `Cloudflared` 来代理(加速)它的 `Websocket` 服务器，因此您无法直接使用 `Python` 的 `Websocket` 库来连接此服务器。目前尚且未找到对应的解决办法，一个替代方案是使用 `Golang` 下的 `Websocket` 库与 `PhoenixBuilder Auth Server` 建立连接
     - 其他帮助信息另见 https://github.com/huashengdun/webssh/issues/141
 
 
 
 
+
 # 快速上手
 您可以利用 [`BDXConverter/Converter/FileOperation.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/FileOperation.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
 
 
 
 
 
@@ -148,14 +151,16 @@
 
 我们配置了自动化 `CD/CI 工作流` ，因此如果您是本项目的 `协作者` ，您可以通过更改 `version` 文件或通过手动触发的方式启动工作流，它会自动编译本项目并将将其上载到 `Pypi` 中。
 
 _[注：我们建议您在 `Python 3.10` 及以上的版本使用本项目，`3.7` 及以下的版本已不再受到 `Python` 的维护和更新]_
 
 
 
+
+
 # 第三方依赖
 本项目使用了 `brotli, nbtlib` 和 `pycryptodome` 总计 `3` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
 
 ```
 pip install brotli
 pip install nbtlib
 pip install pycryptodome
@@ -215,14 +220,18 @@
 
 
 # 什么是 `BDX` 文件
 `PhoenixBuilder` 是一个用于 `网易我的世界中国版 · 基岩版租赁服` 的商业化快速建造器，而 `BDX` 文件则是此建造器用于存储 `Minecraft` 建筑结构的 `私有文件格式` 。
 
 如果您希望解析 `BDX` 文件，敬请参阅 [`bdump-cn.md`](https://github.com/LNSSPsd/PhoenixBuilder/blob/main/doc/bdump/bdump-cn.md) 。
 
+
+
+
+
 # 关于 `PhoenixBuilder`
 - 您可以通过此链接访问 `PhoenixBuilder` 的存储库
    - [`PhoenixBuilder`](https://github.com/LNSSPsd/PhoenixBuilder/)
 - 您可以通过下述链接访问 `PhoenixBuilder` 的相关网站
    - [`用户中心`](https://uc.fastbuilder.pro/)
    - [`官方网站`](https://fastbuilder.pro/)
```

### Comparing `BDXConverter-1.1.8/README.md` & `BDXConverter-1.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 
 
 # 注意事项
 ## 兼容性
 - 版本 `1.1.0` 不兼容之前的所有版本
 - 版本 `1.0.16` 在可视化和反可视化字典方面不兼容之前的版本
 
+
+
 ## 签名
 - `BDX` 文件格式是由 `PhoenixBuilder` 所定义，签名 `BDX` 文件则必须具备 `PhoenixBuilder` 账户
 - 由于一些原因，您需要自行获取 `签名` 时的 `Prove` 和 `PrivateSigningKey` ，以下展示了获取方法。有关本项目实现的签名功能，请见 [`BDXConverter/Converter/Signature.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Signature.py)
 
   ```python
   """
   import ecdsa
@@ -116,14 +118,15 @@
   ```
   - `PhoenixBuilder Auth Server` 使用了 `Cloudflared` 来代理(加速)它的 `Websocket` 服务器，因此您无法直接使用 `Python` 的 `Websocket` 库来连接此服务器。目前尚且未找到对应的解决办法，一个替代方案是使用 `Golang` 下的 `Websocket` 库与 `PhoenixBuilder Auth Server` 建立连接
     - 其他帮助信息另见 https://github.com/huashengdun/webssh/issues/141
 
 
 
 
+
 # 快速上手
 您可以利用 [`BDXConverter/Converter/FileOperation.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/FileOperation.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
 
 
 
 
 
@@ -134,14 +137,16 @@
 
 我们配置了自动化 `CD/CI 工作流` ，因此如果您是本项目的 `协作者` ，您可以通过更改 `version` 文件或通过手动触发的方式启动工作流，它会自动编译本项目并将将其上载到 `Pypi` 中。
 
 _[注：我们建议您在 `Python 3.10` 及以上的版本使用本项目，`3.7` 及以下的版本已不再受到 `Python` 的维护和更新]_
 
 
 
+
+
 # 第三方依赖
 本项目使用了 `brotli, nbtlib` 和 `pycryptodome` 总计 `3` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
 
 ```
 pip install brotli
 pip install nbtlib
 pip install pycryptodome
@@ -201,14 +206,18 @@
 
 
 # 什么是 `BDX` 文件
 `PhoenixBuilder` 是一个用于 `网易我的世界中国版 · 基岩版租赁服` 的商业化快速建造器，而 `BDX` 文件则是此建造器用于存储 `Minecraft` 建筑结构的 `私有文件格式` 。
 
 如果您希望解析 `BDX` 文件，敬请参阅 [`bdump-cn.md`](https://github.com/LNSSPsd/PhoenixBuilder/blob/main/doc/bdump/bdump-cn.md) 。
 
+
+
+
+
 # 关于 `PhoenixBuilder`
 - 您可以通过此链接访问 `PhoenixBuilder` 的存储库
    - [`PhoenixBuilder`](https://github.com/LNSSPsd/PhoenixBuilder/)
 - 您可以通过下述链接访问 `PhoenixBuilder` 的相关网站
    - [`用户中心`](https://uc.fastbuilder.pro/)
    - [`官方网站`](https://fastbuilder.pro/)
 
@@ -223,8 +232,8 @@
 - [ ] 可以自由地转换 `BDX` 和其他建筑文件格式
 
 
 
 
 
 # 其他
-本项目依照 [`MIT LICENSE`](./LICENSE) 许可证进行许可和授权。
+本项目依照 [`MIT LICENSE`](./LICENSE) 许可证进行许可和授权。
```

### Comparing `BDXConverter-1.1.8/setup.py` & `BDXConverter-1.1.9/setup.py`

 * *Files identical despite different names*

