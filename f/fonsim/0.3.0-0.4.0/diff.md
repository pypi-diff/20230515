# Comparing `tmp/fonsim-0.3.0.tar.gz` & `tmp/fonsim-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fonsim-0.3.0.tar", last modified: Mon Apr  3 16:13:19 2023, max compression
+gzip compressed data, was "fonsim-0.4.0.tar", last modified: Mon May 15 17:26:10 2023, max compression
```

## Comparing `fonsim-0.3.0.tar` & `fonsim-0.4.0.tar`

### file list

```diff
@@ -1,82 +1,85 @@
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.277347 fonsim-0.3.0/
--rw-rw-r--   0 arend     (1000) arend     (1000)    34523 2022-05-16 00:07:54.000000 fonsim-0.3.0/LICENSE.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)     2775 2023-04-03 16:13:19.277347 fonsim-0.3.0/PKG-INFO
--rw-rw-r--   0 arend     (1000) arend     (1000)     2023 2023-03-26 21:33:21.000000 fonsim-0.3.0/README.md
--rw-rw-r--   0 arend     (1000) arend     (1000)      105 2022-05-16 00:07:54.000000 fonsim-0.3.0/pyproject.toml
--rw-rw-r--   0 arend     (1000) arend     (1000)       38 2023-04-03 16:13:19.277347 fonsim-0.3.0/setup.cfg
--rw-rw-r--   0 arend     (1000) arend     (1000)     1301 2023-04-03 15:54:40.000000 fonsim-0.3.0/setup.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.265378 fonsim-0.3.0/src/
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.269367 fonsim-0.3.0/src/fonsim/
--rw-rw-r--   0 arend     (1000) arend     (1000)      555 2023-03-28 00:27:47.000000 fonsim-0.3.0/src/fonsim/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      565 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/colors.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.273357 fonsim-0.3.0/src/fonsim/components/
--rw-rw-r--   0 arend     (1000) arend     (1000)      221 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/components/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     5448 2023-03-26 21:33:21.000000 fonsim-0.3.0/src/fonsim/components/actuators.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     5843 2023-03-26 21:33:21.000000 fonsim-0.3.0/src/fonsim/components/circulartube_autodiff.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3118 2023-03-26 21:33:21.000000 fonsim-0.3.0/src/fonsim/components/containers.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     2831 2023-03-26 21:33:21.000000 fonsim-0.3.0/src/fonsim/components/containers_autodiff.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      923 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/components/dummy.py
--rw-rw-r--   0 arend     (1000) arend     (1000)    11862 2023-03-26 21:33:21.000000 fonsim-0.3.0/src/fonsim/components/restrictors.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     5407 2023-03-26 21:33:21.000000 fonsim-0.3.0/src/fonsim/components/sources.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      227 2023-03-26 21:33:21.000000 fonsim-0.3.0/src/fonsim/components/terminals.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.273357 fonsim-0.3.0/src/fonsim/constants/
--rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.3.0/src/fonsim/constants/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      263 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/constants/norm.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      215 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/constants/physical.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.273357 fonsim-0.3.0/src/fonsim/conversion/
--rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.3.0/src/fonsim/conversion/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      897 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/conversion/indexmatch.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.273357 fonsim-0.3.0/src/fonsim/core/
--rw-rw-r--   0 arend     (1000) arend     (1000)      287 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/core/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)    15808 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/core/component.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     1963 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/core/node.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      277 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/core/setnumpythreads.py
--rw-rw-r--   0 arend     (1000) arend     (1000)    24487 2023-04-03 15:46:15.000000 fonsim-0.3.0/src/fonsim/core/simulation.py
--rw-rw-r--   0 arend     (1000) arend     (1000)    13814 2023-04-03 15:46:15.000000 fonsim-0.3.0/src/fonsim/core/solver.py
--rw-rw-r--   0 arend     (1000) arend     (1000)    11114 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/core/system.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3995 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/core/terminal.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3964 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/core/variable.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.273357 fonsim-0.3.0/src/fonsim/data/
--rw-rw-r--   0 arend     (1000) arend     (1000)      134 2022-05-16 00:07:54.000000 fonsim-0.3.0/src/fonsim/data/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3335 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/data/curve.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     4454 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/data/dataseries.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     4446 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/data/interpolate.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     6459 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/data/pvcurve.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     5365 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/data/writeout.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.273357 fonsim-0.3.0/src/fonsim/fluid/
--rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.3.0/src/fonsim/fluid/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     1867 2022-05-16 00:07:54.000000 fonsim-0.3.0/src/fonsim/fluid/fallback.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3329 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/fluid/fluid.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.277347 fonsim-0.3.0/src/fonsim/fluids/
--rw-rw-r--   0 arend     (1000) arend     (1000)       52 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/fluids/Bingham.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      758 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/fluids/IdealCompressible.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      869 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/fluids/IdealIncompressible.py
--rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.3.0/src/fonsim/fluids/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      503 2023-04-03 15:58:35.000000 fonsim-0.3.0/src/fonsim/notice_beta.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.277347 fonsim-0.3.0/src/fonsim/resources/
--rw-rw-r--   0 arend     (1000) arend     (1000)      979 2022-05-16 00:07:54.000000 fonsim-0.3.0/src/fonsim/resources/Measurement_60mm_balloon_actuator_01.csv
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.277347 fonsim-0.3.0/src/fonsim/visual/
--rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.3.0/src/fonsim/visual/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     1945 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/visual/plotting.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.277347 fonsim-0.3.0/src/fonsim/wave/
--rw-rw-r--   0 arend     (1000) arend     (1000)       75 2022-05-16 00:07:54.000000 fonsim-0.3.0/src/fonsim/wave/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     5357 2023-03-26 21:33:21.000000 fonsim-0.3.0/src/fonsim/wave/custom.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     1365 2023-03-23 19:19:04.000000 fonsim-0.3.0/src/fonsim/wave/wave.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.269367 fonsim-0.3.0/src/fonsim.egg-info/
--rw-rw-r--   0 arend     (1000) arend     (1000)     2775 2023-04-03 16:13:19.000000 fonsim-0.3.0/src/fonsim.egg-info/PKG-INFO
--rw-rw-r--   0 arend     (1000) arend     (1000)     1886 2023-04-03 16:13:19.000000 fonsim-0.3.0/src/fonsim.egg-info/SOURCES.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)        1 2023-04-03 16:13:19.000000 fonsim-0.3.0/src/fonsim.egg-info/dependency_links.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)       63 2023-04-03 16:13:19.000000 fonsim-0.3.0/src/fonsim.egg-info/requires.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)        7 2023-04-03 16:13:19.000000 fonsim-0.3.0/src/fonsim.egg-info/top_level.txt
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-03 16:13:19.277347 fonsim-0.3.0/tests/
--rw-rw-r--   0 arend     (1000) arend     (1000)     4168 2023-03-28 00:22:27.000000 fonsim-0.3.0/tests/test_basic.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     4153 2023-03-23 19:19:04.000000 fonsim-0.3.0/tests/test_component_autocall.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3015 2023-03-23 19:19:04.000000 fonsim-0.3.0/tests/test_custom.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3238 2023-03-23 19:19:04.000000 fonsim-0.3.0/tests/test_dataseries.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      711 2023-03-23 19:19:04.000000 fonsim-0.3.0/tests/test_indexmatch.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3893 2023-03-23 19:19:04.000000 fonsim-0.3.0/tests/test_interpolate.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     1751 2023-03-23 19:19:04.000000 fonsim-0.3.0/tests/test_node.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3205 2023-03-23 19:19:04.000000 fonsim-0.3.0/tests/test_pvcurve.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     7373 2023-03-23 19:19:04.000000 fonsim-0.3.0/tests/test_system.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     2684 2023-03-23 19:19:04.000000 fonsim-0.3.0/tests/test_terminal.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      697 2023-03-23 19:19:04.000000 fonsim-0.3.0/tests/test_variable.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.024949 fonsim-0.4.0/
+-rw-rw-r--   0 arend     (1000) arend     (1000)    34523 2022-05-16 00:07:54.000000 fonsim-0.4.0/LICENSE.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3060 2023-05-15 17:26:10.024949 fonsim-0.4.0/PKG-INFO
+-rw-rw-r--   0 arend     (1000) arend     (1000)     2309 2023-05-08 14:23:04.000000 fonsim-0.4.0/README.md
+-rw-rw-r--   0 arend     (1000) arend     (1000)      105 2022-05-16 00:07:54.000000 fonsim-0.4.0/pyproject.toml
+-rw-rw-r--   0 arend     (1000) arend     (1000)       38 2023-05-15 17:26:10.024949 fonsim-0.4.0/setup.cfg
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1334 2023-05-10 00:14:35.000000 fonsim-0.4.0/setup.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.004949 fonsim-0.4.0/src/
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.008949 fonsim-0.4.0/src/fonsim/
+-rw-rw-r--   0 arend     (1000) arend     (1000)      555 2023-05-05 15:10:16.000000 fonsim-0.4.0/src/fonsim/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      565 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/colors.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.012949 fonsim-0.4.0/src/fonsim/components/
+-rw-rw-r--   0 arend     (1000) arend     (1000)      269 2023-05-08 18:37:27.000000 fonsim-0.4.0/src/fonsim/components/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5574 2023-05-08 14:09:52.000000 fonsim-0.4.0/src/fonsim/components/actuators.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5843 2023-05-05 15:10:16.000000 fonsim-0.4.0/src/fonsim/components/circulartube_autodiff.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     6566 2023-05-08 14:09:52.000000 fonsim-0.4.0/src/fonsim/components/containers.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     2831 2023-05-05 15:10:16.000000 fonsim-0.4.0/src/fonsim/components/containers_autodiff.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      923 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/components/dummy.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)    12333 2023-05-14 23:39:01.000000 fonsim-0.4.0/src/fonsim/components/restrictors.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5680 2023-05-13 18:19:15.000000 fonsim-0.4.0/src/fonsim/components/sources.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      277 2023-05-08 14:23:04.000000 fonsim-0.4.0/src/fonsim/components/terminals.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     2211 2023-05-08 16:06:19.000000 fonsim-0.4.0/src/fonsim/components/valves.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.012949 fonsim-0.4.0/src/fonsim/constants/
+-rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/constants/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      263 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/constants/norm.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      215 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/constants/physical.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.012949 fonsim-0.4.0/src/fonsim/conversion/
+-rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/conversion/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      897 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/conversion/indexmatch.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.016949 fonsim-0.4.0/src/fonsim/core/
+-rw-rw-r--   0 arend     (1000) arend     (1000)      287 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/core/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)    22530 2023-05-08 20:53:03.000000 fonsim-0.4.0/src/fonsim/core/component.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1963 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/core/node.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      277 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/core/setnumpythreads.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)    42054 2023-05-08 16:32:15.000000 fonsim-0.4.0/src/fonsim/core/simulation.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)    19886 2023-05-14 23:39:01.000000 fonsim-0.4.0/src/fonsim/core/solver.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)    11114 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/core/system.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3995 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/core/terminal.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     4492 2023-05-08 14:23:04.000000 fonsim-0.4.0/src/fonsim/core/variable.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.016949 fonsim-0.4.0/src/fonsim/data/
+-rw-rw-r--   0 arend     (1000) arend     (1000)      134 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/data/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3335 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/data/curve.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     4454 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/data/dataseries.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     4446 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/data/interpolate.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     6459 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/data/pvcurve.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5365 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/data/writeout.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.016949 fonsim-0.4.0/src/fonsim/fluid/
+-rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/fluid/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1867 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/fluid/fallback.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3329 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/fluid/fluid.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.020949 fonsim-0.4.0/src/fonsim/fluids/
+-rw-rw-r--   0 arend     (1000) arend     (1000)       52 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/fluids/Bingham.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      758 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/fluids/IdealCompressible.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      869 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/fluids/IdealIncompressible.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/fluids/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      693 2023-05-13 18:19:15.000000 fonsim-0.4.0/src/fonsim/notice_beta.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.020949 fonsim-0.4.0/src/fonsim/resources/
+-rw-rw-r--   0 arend     (1000) arend     (1000)      979 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/resources/Measurement_60mm_balloon_actuator_01.csv
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.020949 fonsim-0.4.0/src/fonsim/visual/
+-rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/visual/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1977 2023-05-08 14:09:52.000000 fonsim-0.4.0/src/fonsim/visual/plotting.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.020949 fonsim-0.4.0/src/fonsim/wave/
+-rw-rw-r--   0 arend     (1000) arend     (1000)       75 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/wave/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5357 2023-05-05 15:10:16.000000 fonsim-0.4.0/src/fonsim/wave/custom.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1365 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/wave/wave.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.008949 fonsim-0.4.0/src/fonsim.egg-info/
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3060 2023-05-15 17:26:09.000000 fonsim-0.4.0/src/fonsim.egg-info/PKG-INFO
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1989 2023-05-15 17:26:10.000000 fonsim-0.4.0/src/fonsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)        1 2023-05-15 17:26:09.000000 fonsim-0.4.0/src/fonsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)       72 2023-05-15 17:26:09.000000 fonsim-0.4.0/src/fonsim.egg-info/requires.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)        7 2023-05-15 17:26:09.000000 fonsim-0.4.0/src/fonsim.egg-info/top_level.txt
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.024949 fonsim-0.4.0/tests/
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1309 2023-05-08 14:09:52.000000 fonsim-0.4.0/tests/test_basic.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     4153 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_component_autocall.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3015 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_custom.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3238 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_dataseries.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      711 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_indexmatch.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3893 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_interpolate.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1751 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_node.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3205 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_pvcurve.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5311 2023-05-08 14:09:52.000000 fonsim-0.4.0/tests/test_simulation_and_solver.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     4594 2023-05-13 18:19:15.000000 fonsim-0.4.0/tests/test_solver_infinite_flow.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     7373 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_system.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     2684 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_terminal.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1253 2023-05-08 14:23:04.000000 fonsim-0.4.0/tests/test_variable.py
```

### Comparing `fonsim-0.3.0/LICENSE.txt` & `fonsim-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/PKG-INFO` & `fonsim-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fonsim
-Version: 0.3.0
+Version: 0.4.0
 Summary: Fluidic Object-Oriented Network Simulator
-Home-page: https://fonsim.org
+Home-page: http://fonsim.org
 Author: Arne Baeyens, Bert Van Raemdonck
 Author-email: info@fonsim.org
 License: AGPLv3
 Keywords: simulator,simulation,flow,fluids,fluidic,soft robot,soro,soft robotics,soft robots
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
@@ -15,37 +15,41 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # FONSim
+[![PyPI version](https://badge.fury.io/py/fonsim.svg)](https://badge.fury.io/py/fonsim)
+[![Documentation Status](https://readthedocs.org/projects/fonsim/badge/?version=latest)](https://fonsim.readthedocs.io/en/latest/?badge=latest)
+![coverage](https://gitlab.com/abaeyens/fonsim/badges/master/coverage.svg)
 #### _Fluidic Object-oriented Network SIMulator_
 
 An object-oriented Python 3 library designed for simulating pneumatic and hydraulic systems in soft robots.
-Find the full documentation on [fonsim.org](https://fonsim.org).
+Find the full documentation on [fonsim.org](http://fonsim.org/).
 
 This project is available under the GNU Affero General Public License v3.0 (**agpl-3.0**) license.
 
 ### Installation
 The pre-packaged release version can be installed using `pip install fonsim`.
-See the [PyPi page](https://pypi.org/project/fonsim/) for more information.
+See the [PyPI page](https://pypi.org/project/fonsim/) for more information.
 
-Currently, FONSim resides in the alpha stage.
-Not all features work yet, and you may encounter bugs.
+Currently, FONSim resides in the beta stage.
+Some features do not work well yet, or are unintuitive to use correctly,
+and you may encounter bugs.
 We look forward to your feedback.
 
 
 ### How to get started
 The [examples directory](
   https://gitlab.com/abaeyens/fonsim/-/tree/master/examples)
 contains a set of examples showcasing various features of the simulator.
 We suggest to start with running the examples.
 Furthermore you may want to consult the documentation on
-[readthedocs.org](https://fonsim.readthedocs.io/en/feature-doc/introduction.html).
+[readthedocs.io](https://fonsim.readthedocs.io/).
 The code documentation is also available by the
 [Python help function](https://www.programiz.com/python-programming/docstrings#help).
 If something is not fully clear, please let us know.
 
 ### Key dependencies
 * matplotlib
 * numpy
@@ -74,8 +78,8 @@
 you can reach out by creating an issue on the
 [GitLab Issues](https://gitlab.com/abaeyens/fonsim/-/issues) page.
 The issues page is also the proper place to post suggestions and feedback.
 
 
 ## FAQ
 Please refer to the documentation on 
-[readthedocs.org](https://fonsim.readthedocs.io/en/feature-doc/introduction.html).
+[readthedocs.io](https://fonsim.readthedocs.io/).
```

### Comparing `fonsim-0.3.0/README.md` & `fonsim-0.4.0/src/fonsim.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,55 @@
+Metadata-Version: 2.1
+Name: fonsim
+Version: 0.4.0
+Summary: Fluidic Object-Oriented Network Simulator
+Home-page: http://fonsim.org
+Author: Arne Baeyens, Bert Van Raemdonck
+Author-email: info@fonsim.org
+License: AGPLv3
+Keywords: simulator,simulation,flow,fluids,fluidic,soft robot,soro,soft robotics,soft robots
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # FONSim
+[![PyPI version](https://badge.fury.io/py/fonsim.svg)](https://badge.fury.io/py/fonsim)
+[![Documentation Status](https://readthedocs.org/projects/fonsim/badge/?version=latest)](https://fonsim.readthedocs.io/en/latest/?badge=latest)
+![coverage](https://gitlab.com/abaeyens/fonsim/badges/master/coverage.svg)
 #### _Fluidic Object-oriented Network SIMulator_
 
 An object-oriented Python 3 library designed for simulating pneumatic and hydraulic systems in soft robots.
-Find the full documentation on [fonsim.org](https://fonsim.org).
+Find the full documentation on [fonsim.org](http://fonsim.org/).
 
 This project is available under the GNU Affero General Public License v3.0 (**agpl-3.0**) license.
 
 ### Installation
 The pre-packaged release version can be installed using `pip install fonsim`.
-See the [PyPi page](https://pypi.org/project/fonsim/) for more information.
+See the [PyPI page](https://pypi.org/project/fonsim/) for more information.
 
-Currently, FONSim resides in the alpha stage.
-Not all features work yet, and you may encounter bugs.
+Currently, FONSim resides in the beta stage.
+Some features do not work well yet, or are unintuitive to use correctly,
+and you may encounter bugs.
 We look forward to your feedback.
 
 
 ### How to get started
 The [examples directory](
   https://gitlab.com/abaeyens/fonsim/-/tree/master/examples)
 contains a set of examples showcasing various features of the simulator.
 We suggest to start with running the examples.
 Furthermore you may want to consult the documentation on
-[readthedocs.org](https://fonsim.readthedocs.io/en/feature-doc/introduction.html).
+[readthedocs.io](https://fonsim.readthedocs.io/).
 The code documentation is also available by the
 [Python help function](https://www.programiz.com/python-programming/docstrings#help).
 If something is not fully clear, please let us know.
 
 ### Key dependencies
 * matplotlib
 * numpy
@@ -54,8 +78,8 @@
 you can reach out by creating an issue on the
 [GitLab Issues](https://gitlab.com/abaeyens/fonsim/-/issues) page.
 The issues page is also the proper place to post suggestions and feedback.
 
 
 ## FAQ
 Please refer to the documentation on 
-[readthedocs.org](https://fonsim.readthedocs.io/en/feature-doc/introduction.html).
+[readthedocs.io](https://fonsim.readthedocs.io/).
```

### Comparing `fonsim-0.3.0/setup.py` & `fonsim-0.4.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fonsim",
-    version="0.3.0",
+    version="0.4.0",
     author="Arne Baeyens, Bert Van Raemdonck",
     author_email="info@fonsim.org",
     description="Fluidic Object-Oriented Network Simulator",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://fonsim.org',
+    url='http://fonsim.org',
     keywords='simulator, simulation, flow, fluids, fluidic, soft robot, soro, soft robotics, soft robots',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     package_data={'': ['resources/*.json',
                        'resources/*.csv',
                        ]},
     install_requires=['numpy', 'scipy', 'matplotlib',
                       'stringunitconverter',
                       'importlib_resources',
+                      'tabulate',
                       ],
     license='AGPLv3',
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Education",
         "License :: OSI Approved :: GNU Affero General Public License v3",
```

### Comparing `fonsim-0.3.0/src/fonsim/__init__.py` & `fonsim-0.4.0/src/fonsim/__init__.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/colors.py` & `fonsim-0.4.0/src/fonsim/colors.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/components/actuators.py` & `fonsim-0.4.0/src/fonsim/components/actuators.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,22 +53,23 @@
 
         self.set_terminals(Terminal('a', terminal_fluidic, {'pressure': 'p0', 'massflow': 'mf0'}),
                            Terminal('b', terminal_fluidic, {'pressure': 'p1', 'massflow': 'mf1'}))
         self.set_states(Variable('mass', 'local', label='mass'))
 
         # Custom functionality
         self.fluid = fluid
+        interpolation_opts = dict(extrapolate=False, extrapolate_derivative=True)
         if curve is None:
             filepath = 'resources/Measurement_60mm_balloon_actuator_01.csv'
             bs = pkgutil.get_data('fonsim', filepath)
             ds = dataseries.DataSeries(filename='.csv', bytestring=bs)
-            self.pvcurve = pvcurve.PVCurve(ds, autocorrect=True)
+            self.pvcurve = pvcurve.PVCurve(ds, autocorrect=True, **interpolation_opts)
         elif isinstance(curve, (str, bytes)):
             filename = curve
-            self.pvcurve = pvcurve.PVCurve(filename, autocorrect=True)
+            self.pvcurve = pvcurve.PVCurve(filename, autocorrect=True, **interpolation_opts)
         else:
             self.pvcurve = curve
 
         # Continue init based on fluid
         # Compatible fluids
         initfunction_by_compatible_fluids = collections.OrderedDict([
             (fd.IdealCompressible, freeactuator_compressible),
```

### Comparing `fonsim-0.3.0/src/fonsim/components/circulartube_autodiff.py` & `fonsim-0.4.0/src/fonsim/components/circulartube_autodiff.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/components/containers.py` & `fonsim-0.4.0/src/fonsim/components/containers_autodiff.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from ..core.variable import *
 import fonsim.fluid.fluid as fd
 
 import fonsim.constants.physical as cphy
 import fonsim.constants.norm as cnorm
 
 
-class Container(Component):
+class Container_autodiff(Component):
     """
     A Container object is a (by default, empty) container or tank.
     It has one terminal named 'a'.
     It has one state named 'mass',
     which represents the mass of the fluid inside the container.
 
     The fluid should be one of the fluids defined in the module ``fluids``.
@@ -47,54 +47,46 @@
         ])
         # Continue init based on fluid
         self.fluid.select_object_by_fluid(initfunction_by_compatible_fluids)(self)
         self.states[0].initial_value = volume*self.density
 
         @self.auto_state
         def update_state(dt, mf, m):
-            jacobian = {}
-            m_new = m + dt * mf
-            jacobian['m/p'] = 0
-            jacobian['m/mf'] = dt
-            return {'m': m_new}, jacobian
+            m_new = m + mf * dt
+            return {'m': m_new}
         self.update_state = update_state
 
 
 # Type hinting: mention Container class in arguments
-def container_incompressible(self: Container):
+def container_incompressible(self: Container_autodiff):
     """
     Init function, part specifically for incompressible fluids.
 
     :param self: Container object
     :return: None
     """
     @self.auto
     def evaluate_incompressible(t, mf):
-        values, jacobian = np.zeros(1, dtype=float), [{}]
-        values[0] = mf
-        jacobian[0]['mf'] = 1
-        return values, jacobian
+        residual = mf
+        return np.array([residual], dtype=float)
     self.evaluate = evaluate_incompressible
 
     self.density = self.fluid.rho
 
 
-def container_compressible(self: Container):
+def container_compressible(self: Container_autodiff):
     """
     Init function, part specifically for compressible fluids.
 
     :param self: Container object
     :return: None
     """
     self.mass_stp = self.volume * self.fluid.rho_stp
 
     @self.auto
     def evaluate_compressible(t, p, m):
-        values, jacobian = np.zeros([1], dtype=float), [{}]
-        values[0] = m * cnorm.pressure_atmospheric - self.mass_stp * p
-        jacobian[0]['m'] = cnorm.pressure_atmospheric
-        jacobian[0]['p'] = -self.mass_stp
-        return values, jacobian
+        residual = m * cnorm.pressure_atmospheric - self.mass_stp * p
+        return np.array([residual], dtype=float)
     self.evaluate = evaluate_compressible
 
     p0 = sum([t('pressure').initial_value for t in self.terminals]) / len(self.terminals)
     self.density = p0 / cnorm.pressure_atmospheric * self.fluid.rho_stp
```

### Comparing `fonsim-0.3.0/src/fonsim/components/dummy.py` & `fonsim-0.4.0/src/fonsim/components/dummy.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/components/restrictors.py` & `fonsim-0.4.0/src/fonsim/components/restrictors.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
 class CircularTube(Component):
     """
     Tube modeled as an elongated cylindrical shape.
     The terminal labels are 'a' and 'b'.
     It is stateless (the kinetic energy of the fluid in the tube is neglected).
 
+    The pressure drop is only due to major losses,
+    minor losses are neglected.
+    In case of compressible flow, the major losses are calculated
+    using the mean pressure of the two terminals.
     The fluid should be one of the fluids defined in the module ``fluids``.
 
     **TODO:**
      - include kinetic energy of fluid in tube
 
     :param label: label
     :param fluid: fluid
@@ -217,14 +221,18 @@
 
 class FlowRestrictor(Component):
     """
     Flow restrictor modeled as an orifice with a K-factor.
     Terminals are named 'a' and 'b'.
     It is stateless.
 
+    In case of compressible flow, the minor losses are calculated
+    using the mean pressure of the two terminals.
+    Values for the K-factor (minor loss coefficient) can be found
+    `here <https://www.engineeringtoolbox.com/minor-loss-coefficients-pipes-d_626.html>`_.
     The fluid should be one of the fluids defined in the module ``fluids``.
 
     :param label: label
     :param fluid: fluid
     :param diamter: diameter of orifice
     :param k: K-factor
     """
@@ -295,15 +303,15 @@
         sign = math.copysign(1, arguments[1])
         # Average density
         p_average = (arguments[0] + arguments[2])/2
         p_average = max(p_average, cnorm.pressure_atmospheric / 10)
         rho_average = self.fluid.rho_stp * p_average/cnorm.pressure_atmospheric
         drho_dp = self.fluid.rho_stp / cnorm.pressure_atmospheric / 2
         # Equation
-        r = 8 / math.pi * self.k / self.d ** 4
+        r = 8/math.pi**2 * self.k / self.d**4
         values[0] = delta_p - r/rho_average * mf**2 * sign
         jacobian_arguments[0][1] = -r/rho_average * 2 * mf
         jacobian_arguments[0][0] = 1 + r/rho_average**2 * drho_dp * mf**2 * sign
         jacobian_arguments[0][2] = -1 + r/rho_average**2 * drho_dp * mf**2 * sign
 
         # matter in = matter out
         values[1] = arguments[1] + arguments[3]
```

### Comparing `fonsim-0.3.0/src/fonsim/components/sources.py` & `fonsim-0.4.0/src/fonsim/components/sources.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,29 +11,26 @@
 import fonsim.fluid.fluid as fd
 
 import fonsim.constants.physical as cphy
 import fonsim.constants.norm as cnorm
 
 
 class PressureSource(Component):
-    """
-    Ideal pressure source.
+    """Ideal pressure source
+
     The pressure exactly equals the desired pressure
     and the flow is unlimited.
     It has one terminal 'a' and is stateless.
 
     The argument 'pressure' should be either a constant value
     or a callable method that takes a single argument,
     the argument being the elapsed time since the simulation start.
 
     The argument fluid should be one of the fluids defined in the module ``fluids``.
 
-    **TODO**
-     - Limit pressure to positive values.
-
     :param label: label
     :param fluid: fluid
     :param pressure: desired pressure
     """
     def __init__(self, label=None, fluid=None, pressure=None):
         Component.__init__(self, label)
 
@@ -49,19 +46,32 @@
         if callable(self.pressure):
             values[0] = arguments[0] - self.pressure(elapsed_time)
         else:
             values[0] = arguments[0] - self.pressure
         jacobian_arguments[0, 0] = 1
 
 
-class MassflowSource(Component):
+class Sink(PressureSource):
+    """Ideal pressure sink at atmospheric pressure
+
+    Wrapper of a :py:class:`.PressureSource`
+    set to atmospheric pressure (1013 mBar).
+
+    :param label: label
+    :param pressure: desired pressure
     """
-    Ideal massflow source.
+    def __init__(self, label=None, pressure=cnorm.pressure_atmospheric):
+        super().__init__(self, label, pressure=pressure)
+
+
+class MassflowSource(Component):
+    """Ideal massflow source
+
     The massflow exactly equals the desired massflow.
-    The pressure is limited to positive values.
+    A **positive* flow value means that fluid **exits** the source.
     It has one terminal 'a' and is stateless.
 
     The argument 'massflow' should be either a constant value
     or a callable method that takes a single argument,
     the argument being the elapsed time since the simulation start.
 
     The argument fluid should be one of the fluids defined in the module ``fluids``.
@@ -86,29 +96,26 @@
             values[0] = arguments[0] + self.massflow(elapsed_time)
         else:
             values[0] = arguments[0] + self.massflow
         jacobian_arguments[0, 0] = 1
 
 
 class VolumeflowSource(Component):
-    """
-    Ideal volumeflow source.
+    """Ideal volumeflow source
+
     The volumeflow exactly equals the desired volume flow.
-    The pressure is limited to positive values.
+    A **positive* flow value means that fluid **exits** the source
     It has one terminal 'a' and is stateless.
 
     The value 'volumeflow' should be either a constant value
     or a callable method that takes a single argument,
     the argument being the elapsed time since the simulation start.
 
     The fluid should be one of the fluids defined in the module ``fluids``.
 
-    **TODO**
-     - Limit pressure to positive values.
-
     :param label: label
     :param fluid: fluid
     :param volumeflow: desired volumeflow
     """
     def __init__(self, label=None, fluid=None, volumeflow=None):
         Component.__init__(self, label)
 
@@ -128,30 +135,28 @@
             (fd.IdealIncompressible, volumeflowsource_incompressible),
         ])
         # Continue init based on fluid
         self.fluid.select_object_by_fluid(initfunction_by_compatible_fluids)(self)
 
 
 def volumeflowsource_incompressible(self: VolumeflowSource):
-    """
-    Init function, part specifically for incompressible fluids.
+    """Init function, part specifically for incompressible fluids
 
     :param self: VolumeflowSource object
     :return: None
     """
     def evaluate(values, jacobian_state, jacobian_arguments, state, arguments, elapsed_time):
         vf = self.volumeflow(elapsed_time) if callable(self.volumeflow) else self.volumeflow
         values[0] = arguments[1] + vf*self.fluid.rho
         jacobian_arguments[0, 1] = 1
     self.evaluate = evaluate
 
 
 def volumeflowsource_compressible(self: VolumeflowSource):
-    """
-    Init function, part specifically for compressible fluids.
+    """Init function, part specifically for compressible fluids
 
     :param self: VolumeflowSource object
     :return: None
     """
     def evaluate(values, jacobian_state, jacobian_arguments, state, arguments, elapsed_time):
         vf = self.volumeflow(elapsed_time) if callable(self.volumeflow) else self.volumeflow
         a = self.fluid.rho_stp/cnorm.pressure_atmospheric
```

### Comparing `fonsim-0.3.0/src/fonsim/conversion/indexmatch.py` & `fonsim-0.4.0/src/fonsim/conversion/indexmatch.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/core/node.py` & `fonsim-0.4.0/src/fonsim/core/node.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/core/simulation.py` & `fonsim-0.4.0/src/fonsim/core/component.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,587 +1,521 @@
 """
-Class Simulation
+Class Component
 
-2020, July 22
+2020, July 21
 """
 
-import time
-import warnings
-
 import numpy as np
+import inspect
+import copy
+import warnings
 
-from . import solver as slv
-
+from fonsim.conversion import indexmatch
 
-class Simulation:
-    """
-    Class to convert network information
-    (how the components are connected to each other)
-    and component information
-    (equations for each component)
-    to a single non-linear system of equations
-    (function vector + Jacobian)
-    describing the whole system.
-
-    Solving this system is to be done by a solver.
-    This object contains a solver object in the property self.solver.
-    (Future functionality: possibility to select a solver manually etc.)
-
-    The Class Solver interacts heavily with the System class
-    and expects the following methods to be available:
-
-    - ``evaluate_equations()``
-    - ``update_state()``
-    - ``equation_to_string()``
-
-    as well as the following properties:
-
-    - ``system``
-    - ``phi``, ``H`` and ``A``
-    - ``arguments``
-    - ``nb_arguments`` and ``nb_network_equations``
-    - ``times`` and ``duration`` and ``verbose``
-
-    :param system_to_simulate: System object with components and how they are connected
-    :param duration: amount of time the system will be simulated for
-    :param step: initial time increment
-    :param step_min: minimal time increment during the simulation
-    :param step_max: maximal time increment during the simulation
-    :param max_steps: maximum amount of time increments before the
-                      simulation is terminated prematurely. A value of 0 disables this
-                      behavior (default)
-    :param verbose: level of information printed in the console
-                    during the simulation. All messages belonging to a level with a
-                    number lower than or equal to the provided parameter will be
-                    displayed, with the possible levels being:
-
-                     * -1: simulation start and end messages
-                     * 0 (default): simulation progress in % steps
-                     * 1: system matrices on iterations with bad convergence
-    """
-    def __init__(self, system_to_simulate, duration=10, step=None,
-                 step_min=None, step_max=None, max_steps=0, verbose=0):
 
-        # Check input
-        if step_min is not None and step_max is not None and step_min > step_max:
-            raise Warning('Parameter step_min should not be larger than step_max.')
-
-        # Assign arguments to properties
-        self.verbose = verbose
-
-        # Load system to simulate
-        self.system = system_to_simulate
-        connectivity_message = self.system.get_connectivity_message()
-        if len(connectivity_message) > 0 and self.verbose >= -1:
-            msg = '{}!'.format(connectivity_message) + \
-                  'Are you sure you did not forget any connections?'
-            warnings.warn(msg, UserWarning, stacklevel=2)
-
-        # Timing
-        self.duration = duration
-
-        # Resolve stepping settings
-        self.duration = duration
-        if step is None:
-            step_vals = [s for s in (step_max, step_min) if s is not None]
-            if len(step_vals) > 0:
-                step = sum(step_vals)/len(step_vals)
-            else:
-                step = self.duration/100.
-        self.max_steps = max_steps
+class Component:
+    """Components to build a system with
 
-        # Initialize matrix construction (dicts etc.)
-        self.arguments = []
-        self.nb_arguments = 0
-        self.nb_states = 0
-        self.phi_index_slice_by_component_by_component = {}
-        self.phi_index_by_component_argument = {}
-        self.state_index_slice_by_component = {}
-        self.states_index_by_component_argument = {}
-        self.nb_component_equations = 0
-        self.nb_network_equations = 0
-        self.init_matrixconstruction()
-
-        # Construct the matrices
-        # Initialize empty Jacobian
-        self.H = np.zeros((self.nb_arguments, self.nb_arguments))
-        # Fill network matrix
-        self.fill_network_matrix(self.H)
-        # Network matrix (= upper part of H)
-        # Note: A keeps pointing to upper part of H,
-        # so changing A will affect H as well.
-        self.A = self.H[:self.nb_network_equations, :]
-
-        # values vector = result of evaluated equations
-        # leave this to the solver...
-        #self.g = np.zeros(self.nb_arguments)
-
-        # Create the argument matrix, aka the matrix with the vector
-        # of all unknowns for each timestep
-        self.phi = np.array(0)
-        # and create the state matrix,
-        # which holds the internal component states for each timestep
-        self.state = np.array(0)
-        # These two arrays are filled by the method initialize_memory
-
-        # Time series (to be set by solver)
-        self.times = np.array(0)
-        # Step counter - denotes current step of simulation
-        self.simstep = 0
-
-        # Select the solver
-        # self.solver = slv.ImplicitEulerNewtonConstantTimeStep(self, step)
-        self.solver = slv.ImplicitEulerNewtonAdaptiveTimeStep(self, step,
-                                                              step_min, step_max)
-
-    def init_matrixconstruction(self):
-        """
-        Create some LUT-style lists and dicts
-        so data can be moved around quickly
-        in the simulation loop.
+    This base class provides a starting ground
+    to build components usable in a FONSim system.
+    Several examples are found in the FONSim standard library
+    (see the :py:mod:`fonsim.components` package).
+    Also, be sure to check out the
+    :doc:`tutorial on custom components</tutorials/custom_components>`.
+
+    **Interaction with other components**
+    The component terminals (instances of :py:class:`.Terminal`)
+    specify the possibilities for interaction with other components.
+    They are added using the method :py:meth:`.Component.set_terminals`.
+    Example of adding two fluidic terminals with labels 'a' and 'b':
+
+    .. code-block:: python
+
+       self.set_terminals(Terminal('a', terminal_fluidic, {'pressure': 'p0', 'massflow': 'mf0'}),
+                          Terminal('b', terminal_fluidic, {'pressure': 'p1', 'massflow': 'mf1'}))
+
+    The list ``terminal_fluidic`` contains two :py:class:`.Variable` instances,
+    one for pressure and one for massflow.
+    It is defined in
+    :repo:`components/terminals.py<src/fonsim/components/terminals.py>`.
+    If the :py:meth:`.Component.auto` and :py:meth:`.Component.auto_state`
+    methods are used to define  methods :py:meth:`.Component.evaluate`
+    and :py:meth:`.Component.update_state`,
+    then the variable labels 'p0', 'mf0' etc. will be used further on
+    (for an example, please see the tutorial linked to earlier on).
+    The lists of terminals and of the terminal variables are respectively
+    kept in the member variables ``terminals`` and ``arguments``.
+
+    **States**
+    State variables are added using the :py:meth:`.Component.set_states`
+    method. These variables are considered to be *local*
+    because they are not accessible to other components.
+    Example of adding a single state with label 'mass':
+
+    .. code-block:: python
+
+       self.set_states(Variable('mass', 'local', label='m', initial_value=5e-3))
+
+    The state variables are subsequently available as a list
+    in the member variable ``states``.
+
+    **Internal behavior**
+    The two methods :py:meth:`.Component.evaluate`
+    and :py:meth:`.Component.update_state` govern the internal behaviour.
+    The former specifies a relation between the terminal and state variables
+    that should be respected at each discrete timestep
+    and the latter expresses how the state variables change over a timestep
+    given a previous state and the terminal variables.
+
+    There are **two ways** to define these methods.
+    By far the easiest is to use the :py:meth:`.Component.auto`
+    and :py:meth:`.Component.auto_state` methods,
+    as a method or as a decorator, because this allows
+    to refer to the terminal and state variables by their label.
+    The documentation of these two methods discusses how to do so.
+    This is also the approach discussed
+    in the custom component tutorial mentioned earlier.
+
+    The second way is to conform to form of the :py:meth:`.Component.evaluate`
+    :py:meth:`.Component.update_state` methods.
+    This requires variables to be referred to by their index
+    in the passed arrays, making this method prone to errors if done manually.
+    Knowing the indices to use requires either searching the terminal variables
+    in the member variable ``arguments``
+    or putting the variables in that member variable in a particular order,
+    preferably using :py:meth:`.Component.set_arguments`.
+    Note that :py:meth:`.Component.set_terminals` modifies ``arguments``.
+
+    **Storage of the state and terminal variable values**
+    The state data (e.g. amount of fluid inside actuator)
+    is saved as 2D-array in the components themselves
+    (and the solver always refers to these)
+    while the argument data (e.g. pressure, flow in/out)
+    is saved as a list of _references_
+    to nameless 1D-arrays created by the solver.
+    The component object provides functionality for the solver
+    to allocate memory for the states,
+    but not for allocating the variables.
+    The solver takes care of calling these functions necessary.
+    The object property ``state_history`` holds the 2D-array
+    and object property ``argument_history`` holds a list
+    with references to the 1D-arrays.
 
-        :return: None
-        """
-        # collocate arguments (Variable objects) of all components into a list
+    :param label: Component name.
+    """
+    def __init__(self, label):
+        # component name
+        self.label = label
+
+        # terminals of component
+        self.terminals = []
+        # variables for the evaluation of the left-hand side of the residual
+        # and for the state update equation
         self.arguments = []
+        # other variables that are updated based on the solutions for the arguments
         self.states = []
-        for component in self.system.components:
-            self.arguments.extend(component.arguments)
-            self.states.extend(component.states)
-        self.nb_arguments = len(self.arguments)
-        self.nb_states = len(self.states)
-        # make a dict to quickly map arguments of a component
-        # to the indices of phi
-        self.phi_index_slice_by_component = {}
-        self.phi_index_by_component_argument = {}
-        self.state_index_slice_by_component = {}
-        self.state_index_by_component_state = {}
-        for component in self.system.components:
-            k = []
-            for i in range(len(component.arguments)):
-                arg = component.arguments[i]
-                phi_index = self.arguments.index(arg)
-                k.append(phi_index)
-                self.phi_index_by_component_argument[arg] = phi_index
-            self.phi_index_slice_by_component[component] = slice(k[0], k[-1]+1)
-            k = []
-            for i in range(len(component.states)):
-                s = component.states[i]
-                state_index = self.states.index(s)
-                k.append(state_index)
-                self.state_index_by_component_state[s] = state_index
-            self.state_index_slice_by_component[component] = slice(k[0], k[-1]+1)\
-                if len(k) else slice(0)
-        # Count number of component equations
-        self.nb_component_equations = sum(c.nb_equations for c in self.system.components)
-
-    def fill_network_matrix(self, A):
-        """
-        Fill the network matrix.
-        The network matrix is constant over the simulation, at least
-        supposing the network configuration does not change. It is thus
-        sufficient to calculate it a single time.
-
-        There are two types of network equations, one for across
-        variables and one for through variables. 
-        At each node, all across variables have to be equal. Thus for
-        each node n-1 equations, n being the number of components
-        attached to that node.
-        Concerning the through variables, the sum of all through
-        variables should be zero at each node, thus one equation for each
-        node.
-
-        :param A: system Jacobian matrix, numpy ndarray n x n, n=len(phi)
-        :return: None
-        """
-        irow = 0
-        for node in self.system.nodes:
-            # Get across variables to relate together
-            across_keys = set(var.key for var in node.get_variables(orientation='across'))
-            for key in across_keys:
-                # Get all across variables
-                variables = node.get_variables(key=key)
-                # Get their indices in the argument list
-                phi_indices = [self.phi_index_by_component_argument[arg] for arg in variables]
-                # Equate their values pair-wise
-                for pair1, pair2 in zip(phi_indices[:-1], phi_indices[1:]):
-                    A[irow, pair1] = 1
-                    A[irow, pair2] = -1
-                    irow += 1
-
-            # Get through variables to relate together
-            through_keys = set(var.key for var in node.get_variables(orientation='through'))
-            for key in through_keys:
-                # Get all through variables
-                variables = node.get_variables(key=key)
-                # Get their indices in the argument list
-                phi_indices = [self.phi_index_by_component_argument[arg] for arg in variables]
-                # Equate their sum to zero
-                A[irow, phi_indices] = 1
-                irow += 1
-
-        self.nb_network_equations = irow
-
-    def check_issolvable(self):
-        """
-        Warns when number of equations doesn't equal number of unknowns.
-        :return: None
-        """
-        is_solvable = self.nb_network_equations + self.nb_component_equations == self.nb_arguments
-        if not is_solvable:
-            msg = 'This system does not seem to be solvable! ' +\
-                  'The number of equations (network and component) ' +\
-                  'should equal the number of unknowns, however encountered:' +\
-                  '\n  nb of network eq:   ' + str(self.nb_network_equations) +\
-                  '\n  nb of component eq: ' + str(self.nb_component_equations) +\
-                  '\n  nb of unknowns:     ' + str(self.nb_arguments) + '.'
-            warnings.warn(msg, UserWarning, stacklevel=2)
-
-    def equation_to_string(self, equation_index):
-        """
-        Return a string describing the equation with the provided index
-        in a human-readable format. For a network equation, this string
-        contains the involved variables and their coefficients. For a
-        component equation, this string mentions the component label and
-        the index of the equation in the list of equations of that
-        particular component.
-
-        :param equation_index: index of the row in the simulation
-                               equation matrix corresponding to the desired equation
-        :return eq_str: string representing the equation
-        """
-        eq_str = ""
-        # handle network equations
-        if equation_index < self.nb_network_equations:
-            for coeff_ID, coeff in enumerate(self.A[equation_index, :]):
-                if coeff != 0:
-                    # add sign of coefficient
-                    if coeff < 0:
-                        eq_str += "- "
-                    elif len(eq_str) > 0:
-                        eq_str += "+ "
-                    # add value of coefficient
-                    if abs(coeff) != 1:
-                        eq_str += "{}*".format(abs(coeff))
-                    # add name of corresponding variable
-                    eq_str += "{} ".format(self.arguments[coeff_ID].short_str())
-        # handle component equations
-        else:
-            curr_eq_ind = self.nb_network_equations
-            comp_ind = 0
-            comp_eq_ind = 0
-            # find the index of the component and the index of the equation in
-            # the component matching with the global equation index
-            while curr_eq_ind < equation_index:
-                curr_eq_ind += 1
-                if comp_eq_ind < self.system.components[comp_ind].nb_equations-1:
-                    # transition to next equation in this component
-                    comp_eq_ind += 1
-                else:
-                    # transition to next component
-                    comp_eq_ind = 0
-                    comp_ind += 1
-            eq_str = "{} equation {}".format(
-                self.system.components[comp_ind].label, comp_eq_ind)
-
-        return eq_str.strip()
-
-    def print_equations(self):
-        """
-        Print a human-readable representation of the full system of
-        equations to the console.
-
-        :return: None
-        """
-        # get every equation string
-        eq_strs = [self.equation_to_string(i) for i in
-                   range(self.nb_network_equations+self.nb_component_equations)]
-        # get maximum equation text width for alignment
-        max_len = max([len(eq) for eq in eq_strs])
-        # print equations
-        for i, eq in enumerate(eq_strs):
-            print('eq {}: {} = {}'.format(i, eq.rjust(max_len), 0))
-
-    def map_phi_to_components(self, phi):
-        """
-        Send addresses of arguments over time to components, so one can
-        get the data from the component without passing by the Simulation
-        object. Furthermore, it avoids duplicating the data.
-
-        :param phi: numpy ndarray m x n with the argument vector over
-                    time (m = nb timesteps and n = nb arguments)
-        :return: None
-        """
-        for component, i in self.phi_index_slice_by_component.items():
-            component.argument_history = phi[:, i]
-
-    def map_state_to_components(self, state):
-        """
-        Send addresses of state over time to components, so one can
-        get the data from the component without passing by the Simulation
-        object. Furthermore, it avoids duplicating the data.
-
-        :param state: numpy ndarray m x n with the state vector over
-                      time (m = nb timesteps and n = nb states)
-        :return: None
-        """
-        for component, i in self.state_index_slice_by_component.items():
-            component.state_history = state[:, i]
-
-    def initialize_memory(self, nb_steps):
-        """
-        Initialize all arrays that will hold the simulation results
-        through time. This includes
-        - The vector with time values
-        - Component argument and state histories (in Component class)
-        - The simulation phi matrix with all arguments over time
-        All previously stored results are overwritten.
-        This method initializes the arrays with zeros
-        and therefore does not use the ``initial_value`` attribute
-        of the Variable objects.
-        
-        :param nb_steps: estimated amount of time steps in the simulation
-        :return: None
-        """
-        # Allocate time vector
-        # The values it contains are filled in by the solver
-        self.times = np.zeros(nb_steps)
-
-        # Allocate phi and state matrices
-        # And map them to the components
-        self.phi = np.zeros((nb_steps, self.nb_arguments), dtype=float)
-        self.state = np.zeros((nb_steps, self.nb_states), dtype=float)
-        self.map_phi_to_components(self.phi)
-        self.map_state_to_components(self.state)
-
-    def set_initial_values_phi(self, step=0):
-        """
-        Takes the initial values from the component argument Variable objects
-        and writes them to the simulation memory (matrix 'phi').
-
-        :param step: simulation step at which to write the initial value
-        :return: None
-        """
-        self.phi[step, :] = [a.initial_value for a in self.arguments]
-
-    def set_initial_values_state(self, step=0):
-        """
-        Takes the initial values from the component state Variable objects
-        and writes them to the simulation memory (matrix 'state').
-
-        :param step: simulation step at which to write the initial value
-        :return: None
-        """
-        self.state[step, :] = [s.initial_value for s in self.states]
-
-    def extend_memory(self, nb_extra_steps):
-        """
-        Increase the size of the simulation memory without overwriting
-        previous results. This deals with the same entities as described
-        in the documentation of initialize_memory
-
-        :param nb_extra_steps: amount of time steps by which to increase
-                               the memory
-        :return: None
-        """
-        # Extend time vector
-        self.times = np.append(self.times, 
-                               self.times[-1]*np.ones(nb_extra_steps))
-        # Extend phi and state matrices
-        self.phi = np.append(self.phi,
-                             self.phi[0, :]*np.ones((nb_extra_steps, 1)),
-                             axis=0)
-        self.state = np.append(self.state,
-                               np.zeros((nb_extra_steps, self.nb_states)),
-                               axis=0)
-        # Update links to argument and state results in components
-        self.map_phi_to_components(self.phi)
-        self.map_state_to_components(self.state)
-
-    def slice_memory(self, start_step, end_step):
-        """
-        Decrease the size of the simulation memory by taking a slice out
-        of it. This deals with the same entities as described in the
-        documentation of initialize_memory
-
-        # TODO update such that takes slice as argument
-
-        :param start_step: index of the first time step in the range to
-                           maintain
-        :param end_step: index of the first time step outside the range
-                         to maintain
-        :return: None
-        """
-        # Truncate time vector
-        self.times = self.times[start_step:end_step]
-        # Truncate phi and state matrices
-        self.phi = self.phi[start_step:end_step,:]
-        self.state = self.state[start_step:end_step, :]
-        # Update links to argument and state results in components
-        self.map_phi_to_components(self.phi)
-        self.map_state_to_components(self.state)
-
-    def run(self):
-        """
-        Run simulation, with the parameters specified previously.
+        # Initial values for the state
+        self.state_initial = []
+        # number of evaluation equations
+        self.nb_equations = 0
+        # maximum step change of arguments for iterative stepping
+        # Note: It appears this variable is not used anywhere?
+        self.arguments_stepsize = []
+
+        # References to calculated values
+        # Will hold 2D Numpy array
+        self.state_history = None
+        # Will hold 2D Numpy array
+        self.argument_history = None
+
+        # Autocall
+        # Two lists below are filled by the respective two autocall decorators
+        self.arg_indices = []
+        self.arg_indices_state = []
+
+    def evaluate(self, values, jacobian_state, jacobian_arguments, state, arguments, elapsed_time):
+        """
+        Evaluates the component internal equations.
+        **This method should be static**.
+
+        Note: only evaluate left-hand side (LH) of equation, equation should be structured such that RH is always zero.
+
+        :param values: array where the equation residuals will be stored.
+        :param jacobian_state: array where the jacobian to the state will be stored.
+        :param jacobian_arguments: array where the jacobian to the arguments will be stored.
+        :param state: numerical values belonging to the state Variables.
+        :param arguments: numerical values belonging to the Variables.
+        :param elapsed_time: ? TODO.
+        :return: None
+        """
+        # Empty here, as this method is to be overriden by child class definition.
+        # For usage examples, please see the standard components in ``src/fonsim/components/``.
+        pass
+
+    def update_state(self, state_new, jacobian, state, arguments, dt):
+        """
+        Evaluates the update to the component state.
+        **This method should be static**.
+
+        :param state_new: array where the new state values will be stored.
+        :param jacobian: array where the jacobian to the arguments will be stored.
+        :param state: numerical values belonging to the state Variables.
+        :param arguments: numerical values belonging to the Variables.
+        :param dt: time discretization timestep.
+        :return: None
+        """
+        # Empty here, as this method is to be overriden by child class definition.
+        # For usage examples, please see the standard components in ``src/fonsim/components/``.
+        pass
+
+    def set_terminals(self, *terminals):
+        """
+        Overwrite component terminals list with the provided Terminal
+        objects and attach those terminals to the component.
+
+        :param terminals: one or more Terminal objects
+        :return: None
+        """
+        self.terminals = list(terminals)
+        for t in self.terminals:
+            t.component = self
+        # Set arguments
+        args = []
+        for t in self.terminals:
+            args.extend(t.get_variables())
+        self.set_arguments(*args)
+
+    def set_arguments(self, *arguments):
+        """
+        Overwrite component arguments list with the provided Variable
+        objects.
+
+        :param arguments: one or more Variable objects
+        :return: None
+        """
+        self.arguments = list(arguments)
+
+    def set_states(self, *states):
+        """
+        Overwrite component states list with the provided Variable
+        objects.
+
+        :param states: one or more Variable objects
+        :return: None
+        """
+        self.states = list(states)
+
+    def _cache_argumentfetcher(self, f, extra_args=[]):
+        """
+        :param f: function that takes labels of function args as arguments,
+                  together with the other arguments `required_args`.
+        :return: list mapping argument and state indices to function arguments
+        """
+        extra_args = list(extra_args)
+        var_labels = [v.label for v in self.arguments + self.states]
+        func_args = list(inspect.signature(f).parameters.keys())
+        # build a list with for every argument in the function signature the
+        # index of the corresponding variable in var_labels
+        arg_indices = []
+        for func_arg in func_args:
+            for j, var in enumerate(var_labels + extra_args):
+                if func_arg == var:
+                    arg_indices.append(j)
+                    break
+
+        # check that extra arguments are not found in variables
+        extra_args_in_variables = set(extra_args) & set(var_labels)
+        if extra_args_in_variables:
+            msg = f'Name collision: extra argument(s) ' \
+                  f'`{"`, `".join(extra_args_in_variables)}` ' \
+                  f'found in argument and/or state variables ' \
+                  f'of component {self.label}.'
+            raise ValueError(msg)
+        # check if every argument in the signature is matched to a variable
+        unresolved_labels = set(func_args) - set(var_labels + extra_args)
+        if unresolved_labels:
+            terminal_labels = set(a.label for a in self.arguments)
+            state_labels = set(a.label for a in self.states)
+            msg = f'Suspect error in Variable labels of ' \
+                  f'component `{self.label}`: function {f.__name__} ' \
+                  f'references argument(s) `{"`, `".join(unresolved_labels)}`, ' \
+                  f'but no variables with those labels were found among ' \
+                  f'the terminal variables (`{"`, `".join(terminal_labels)}`)'
+            if state_labels:
+                msg += f' or state variables (`{"`, `".join(state_labels)}`)'
+            if extra_args:
+                msg += f' or the extra arguments (`{"`, `".join(extra_args)}`)'
+            msg += '.'
+            raise ValueError(msg)
+
+        return arg_indices
+
+    def _finite_diff_residuals(self, jac_args, jac_state, t,
+                    args, state, y, f, d_rel=1e-4, d_min=1e-12):
+        """
+        :param jac_args: numpy array where derivatives WILL BE WRITTEN
+        :param jac_state: numpy array where derivatives WILL BE WRITTEN
+        :param t: elapsed time
+        :param i: argument index to calculate derivatives to
+        :param args: arguments array
+        :param state: states array
+        :param y: residual array
+        :param f: evaluate residuals function
+        :param d_rel: (maximum) relative FD disturbance
+        :param d_min: minimum absolute FD disturbance
+        """
+        # TODO improve this so this method has less arguments?
+        # loop over all arguments that have an influence on the residual
+        nb_args = len(self.arguments)
+        for i in filter(lambda a: a < nb_args, self.arg_indices):
+            x = np.concatenate((args, state))
+            disturbance = max(abs(x[i]) * d_rel, d_min)
+            if x[i] < 0: disturbance *= -1
+            x[i] += disturbance
+            x = np.append(x, t)
+            y_mod = f(*x[self.arg_indices])
+            jac = (y_mod - y) / disturbance
+            if i < nb_args:
+                jac_args[:, i] = jac
+            else:
+                jac_state[:, i - nb_args] = jac
 
-        :return: None
+    def _finitediff_state(self, jacobian, dt,
+                         args, state, y, f, d_rel=1e-4, d_min=1e-12):
         """
-        # Check whether system is solvable
-        self.check_issolvable()
-
-        # Reset current simulation step index to zero
-        self.simstep = 0
-        # Reset simulation memory
-        self.initialize_memory(self.solver.get_nb_steps_estimate())
-        self.set_initial_values_phi()
-        self.set_initial_values_state()
-
-        # Simulation time steps at which a progress message will be printed
-        pstep = 5
-        progress_pts = [(p/100.*self.duration, p) for p in range(pstep, 101, pstep)]
-
-        # Do the simulation loop
-        if self.verbose >= -1:
-            print('\nSimulation progress:   0 %', end='', flush=True)
-            start_time_process = time.process_time()
-            start_time = time.time()
-
-        solver_convergence = True
-        while solver_convergence and \
-                self.times[self.simstep] < self.duration and \
-                (self.max_steps <= 0 or self.simstep <= self.max_steps):
-            # Increase memory size if necessary
-            if self.simstep+1 >= self.times.size:
-                self.extend_memory(self.solver.get_nb_steps_estimate() -
-                                   self.times.size)
-            # Run solver
-            solver_status = self.solver.run_step(self.simstep)
-            if solver_status is None:
-                solver_convergence = True
+        :param jacobian: numpy array where derivatives WILL BE WRITTEN
+        :param dt: timestep, required to call f
+        :param i: argument index to calculate derivatives to
+        :param args: arguments array
+        :param state: states array
+        :param y: new state array
+        :param f: state update function
+        :param d_rel: (maximum) relative FD disturbance
+        :param d_min: minimum absolute FD disturbance
+        """
+        # TODO improve this so this method has less arguments?
+        # loop over all arguments that have an influence on the residual
+        nb_args = len(self.arguments)
+        for i in filter(lambda a: a < nb_args, self.arg_indices):
+            x = np.concatenate((args, state))
+            disturbance = max(abs(x[i]) * d_rel, d_min)
+            if x[i] < 0: disturbance *= -1
+            x[i] += disturbance
+            x = np.append(x, dt)
+            y_acc = f(*x[self.arg_indices_state])
+            y_mod = np.array([y_acc[s.label] for s in self.states])
+            jacobian[:, i] = (y_mod - y) / disturbance
+
+    def auto(self, func):
+        """Wrapper for Component.evaluate
+        Wrapper that converts a function taking as arguments
+        terminal and state variable labels to a function taking arrays
+        and conforming to the :py:meth:`.Component.evaluate` signature.
+        Often used as a decorator.
+
+        If the given function ``func`` returns a Numpy array and a list,
+        then it is assumed that the former is the array of residuals
+        and the latter the component jacobian.
+        Else, if it returns one Numpy array,
+        it is assumed that that is the array of residuals,
+        and FONSim will automatically estimate the jacobian
+        using finite differences.
+
+        The following example demonstrates
+        the creation of a residual and a jacobian.
+        The third and the fourth line specify the derivatives
+        of the first residual (with array index 0)
+        respectively to the variables *mf0* and *mf1*.
+
+        .. code-block:: python
+
+           values, jacobian = np.zeros(1, dtype=float), [{},]
+           values[0] = mf0 + mf1
+           jacobian[0]['mf0'] = 1
+           jacobian[0]['mf1'] = 1
+           return values, jacobian
+
+        :param func: ``simplified update_state`` function
+        :return: new ``update_state`` function
+        """
+        nb_args = len(self.arguments)
+
+        # Cache argument fetcher
+        self.arg_indices = self._cache_argumentfetcher(func, extra_args=['t',])
+        # Cache manual jacobian writer
+        # label -> variable index of np.concatenate((arguments  states))
+        var_indices_by_label = dict((var.label, i) for i, var in enumerate(self.arguments + self.states))
+        # Register number of equations
+        init_vals = [v.initial_value for v in self.arguments + self.states] \
+            + [0, ] * (max(self.arg_indices) + 1 - len(self.arguments + self.states)) \
+            if self.arg_indices else []     # `max()` with empty list or array errors out
+        ret = func(*np.array(init_vals)[self.arg_indices])
+        if ret is None:
+            msg = f"The function {str(func)} of component {str(self)} " \
+                  f"returned None, however residual values and optionally " \
+                  f"their derivatives were expected. " \
+                  f"Perhaps the 'return' statement is missing or incomplete?"
+            raise RuntimeError(msg)
+        self.nb_equations = len(ret[0] if isinstance(ret, tuple) else ret)
+
+        # The new method, which will be returned
+        def evaluate_new(values, jacobian_state, jacobian_arguments, state, arguments, elapsed_time):
+            # Fetch args
+            args = np.concatenate((arguments, state, [elapsed_time,]))[self.arg_indices]
+            # Evaluation of equation residuals
+            ret = func(*args)
+            # Read in function return value
+            jacobian_given = isinstance(ret, tuple)
+            if jacobian_given:
+                values[:], jac = ret
             else:
-                if isinstance(solver_status, (list, tuple)):
-                    solver_convergence = solver_status[0]
-                    solver_message = solver_status[1]
-                else:
-                    solver_convergence = solver_status
-                    solver_message = ""
-            # Update simulation step index
-            self.simstep += 1
-            # Print some progress information
-            if self.verbose >= -1 and \
-               self.times[self.simstep] >= progress_pts[0][0]:
-                print('\b\b\b\b\b{:3d} %'.format(progress_pts[0][1]), end='')
-                del progress_pts[0]
-        print()
-
-        # Clean up excess memory when the simulation finishes
-        self.slice_memory(0, self.simstep+1)
-
-        # Print time data
-        if self.verbose >= -1:
-            # Get run time
-            end_time_process = time.process_time()
-            end_time = time.time()
-            run_time_process = end_time_process - start_time_process
-            run_time = end_time - start_time
-            # Print error messages
-            if not solver_convergence and len(solver_message) > 0:
-                print(solver_message)
-            elif self.max_steps > 0 and self.simstep >= self.max_steps:
-                print("Maximum number of simulation increments reached")
-            # Print exit messages
-            run_time_process_str = '{:.2f}'.format(run_time_process) + ' s'
-            run_time_str = '{:.2f}'.format(run_time) + ' s'
-            if self.times[self.simstep] < self.duration:
-                print('Simulation terminated after', run_time_str, '(process:', run_time_process_str + ')')
+                values[:] = ret
+            # Handle derivatives, manually specified or finite differences
+            if jacobian_given:
+                # ! not specified indices are not set to zero !
+                for i in range(self.nb_equations):
+                    for key, value in jac[i].items():
+                        j = var_indices_by_label[key]
+                        if j < nb_args:
+                            jacobian_arguments[i, j] = value
+                        else:
+                            jacobian_state[i, j-nb_args] = value
             else:
-                print('Simulation finished in', run_time_str, '(process:', run_time_process_str + ')')
-
-    def evaluate_equations(self, simstep, g, H, elapsed_time, dt):
-        """
-        Evaluate component equations to obtain evaluated function vector
-        (equation residuals) and jacobian.
-        This method will call the method ``Component.evaluate``
-        on each component.
-        This method will also call the method ``Component.update_state``
-        on each component.
-
-        Note: This function does not evaluate (or update) the network
-        equations (upper part of the jacobian 'H')!
-
-        :param simstep: simulation timestep index to start from
-        :param g: numpy ndarray for the evaluated function vector
-        :param H: numpy ndarray for the evaluated jacobian
-        :param elapsed_time: time elapsed
-        :param dt: timestep (0 for explicit Euler, dt for implicit Euler)
-        :return: None
-        """
-
-        # Counter of equation row index to write to
-        irow = self.nb_network_equations
-        for component in self.system.components:
-            nb_a = len(component.arguments)
-            nb_s = len(component.states)
-            ka = self.phi_index_slice_by_component[component]
-            ks = self.state_index_slice_by_component[component]
-
-            # Get references to arguments and state belonging to that component
-            arguments = self.phi[simstep+1, ka]
-            state = self.state[simstep, ks]
-            # Get references to residuals and large jacobian (will be written to)
-            k = component.nb_equations
-            jacobian_full = H[irow:irow+k, ka]
-            residuals = g[irow:irow+k]
-            irow += component.nb_equations
-
-            # Update state if nonzero timestep,
-            if dt != 0:
-                state_new = np.zeros(nb_s)
-                j_state2arg = np.zeros((nb_s, nb_a))
-                component.update_state(state_new, j_state2arg, state, arguments, dt)
+                self._finite_diff_residuals(jacobian_arguments, jacobian_state,
+                                            elapsed_time, arguments, state, values, func)
+        return evaluate_new
+
+    def auto_state(self, func):
+        """Wrapper for ``Component.update_state``
+        Wrapper that converts a function having as parameters
+        terminal and state variable labels to a function taking arrays
+        and conforming to the :py:meth:`.Component.update_state` signature.
+        Often used as a decorator.
+
+        If the given function ``func`` returns two dictionaries,
+        then it is assumed that the former contains the updated states
+        and the latter the component jacobian.
+        Else, if it returns only one dictionary,
+        it is assumed that it contains the updated states,
+        and FONSim will automatically estimate the jacobian
+        using finite differences.
+
+        The following example demonstrates
+        the creation of an updated state and a jacobian.
+        The third and the fourth line specify the derivatives
+        of the state *m*
+        respectively to the variables *p* and *mf*.
+
+        .. code-block:: python
+
+           jacobian = {}
+           m_new = m + dt * mf
+           jacobian['m/p'] = 0
+           jacobian['m/mf'] = dt
+           return {'m': m_new}, jacobian
+
+        :param func: ``simplified update_state`` function
+        :return: new ``update_state`` function
+        """
+        nb_args = len(self.arguments)
+        nb_states = len(self.states)
+
+        # Cache argument fetcher
+        self.arg_indices_state = self._cache_argumentfetcher(func, extra_args=['dt',])
+
+        # The new method, which will be returned
+        def update_state_new(state_new, jacobian, state, arguments, dt):
+            # Fetch args
+            args = np.concatenate((arguments, state, [dt,]))[self.arg_indices_state]
+            # Evaluation of equation residuals
+            ret = func(*args)
+            if ret is None:
+                msg = f"The function {str(func)} of component {str(self)} " \
+                      f"returned None, however state values and optionally " \
+                      f"their derivatives were expected. " \
+                      f"Perhaps the 'return' statement is missing or incomplete?"
+                raise RuntimeError(msg)
+            jacobian_given = isinstance(ret, tuple)
+            if jacobian_given:
+                vs, jac = ret
             else:
-                state_new = state[:]
-
-            # Allocate jacobians
-            j_val2state = np.zeros((component.nb_equations, nb_s))
-            j_val2arg = np.zeros((component.nb_equations, nb_a))
-
-            # state_new = (state + state_new)/2
-
-            # Evaluate residual equations
-            component.evaluate(residuals, j_val2state, j_val2arg, state_new, arguments, elapsed_time)
-
-            # combine state and argument jacobians
-            jacobian_full[:] = j_val2arg
-            if dt != 0:
-                jacobian_full[:] = jacobian_full + np.inner(j_val2state, j_state2arg.T)
+                vs = ret
+            # Write out new state
+            # ! the returned dictionary should contain values for all states !
+            state_new[:] = [vs[s.label] for s in self.states]
+            # Jacobian: manually specified or using finite differences
+            if jacobian_given:
+                # Transform back to numpy arrays
+                for j in range(nb_states):
+                    for i in range(nb_args):
+                        key = self.states[j].label + '/' + self.arguments[i].label
+                        jacobian[j, i] = jac[key] if key in jac else 0
+            else:
+                self._finitediff_state(jacobian,
+                                       dt, arguments, state, state_new, func)
+        return update_state_new
+
+    def get_terminal(self, terminallabel=None):
+        """
+        Returns Terminal object.
+        If no label given,
+        returns the first unconnected terminal.
+        If label given,
+        returns terminal with that label.
+        If no terminal found, returns None.
+
+        :param terminallabel: Label of terminal
+        :return: Terminal object
+        """
+        if terminallabel is None:
+            for terminal in self.terminals:
+                if terminal.isconnected is False:
+                    return terminal
+            return self.terminals[0]
+        else:
+            for terminal in self.terminals:
+                if terminal.label == terminallabel:
+                    return terminal
+        return None
+
+    def get_state(self, label):
+        """
+        Get simulation results.
+        Supports 'smart matching' by comparing string distances.
+
+        :param label: state label, e.g. 'volume'
+        :return: Numpy ndarray object
+        """
+        labels = [state.key for state in self.states]
+        state_index = indexmatch.get_index_of_best_match(label, labels)
+        return self.state_history[:, state_index]
+
+    def get_all(self, variable_key, terminal_label=None):
+        """
+        Get simulation results.
+        Supports 'smart matching' by comparing string distances.
+
+        :param variable_key: key of variable, e.g. 'pressure'
+        :param terminal_label: label of terminal, e.g. 'a'
+        :return: Numpy ndarray object and Terminal object
+        """
+        # Similarity scores for variable keys
+        sim_var = np.array([indexmatch.similar(variable_key, a.key) for a in self.arguments])
+        # Similarity scores for terminal labels, with the terminals belonging to the variables
+        sim_tmn = np.array([indexmatch.similar(terminal_label, a.terminal.label) for a in self.arguments])\
+            if terminal_label is not None else np.ones(len(self.arguments))
+        # Combined similarity scores using element-by-element multiplication
+        sim_com = np.multiply(sim_var, sim_tmn)
+        # Index of variable with highest combined similarity score
+        i = np.argmax(sim_com)
+        # Retrieve that variable and the terminal belonging to it
+        variable = self.arguments[i]
+        term = variable.terminal
+        # Return simulation data (1D Numpy array) and Terminal object
+        return self.argument_history[:, i], term
 
-    def update_state(self, simstep, dt):
+    def get(self, variable_key, terminal_label=None):
         """
-        Update the state variables in all components using the arguments
-        in self.phi at step n + 1 (n = 'simstep').
-        This method will call the method ``Component.update_state``
-        on each component.
-
-        :param simstep: simulation timestep index to start from
-        :param dt: timestep
-        :return: None
+        Same as method ``self.get_all``, but returns only the first return value.
         """
-        for component in self.system.components:
-            nb_a = len(component.arguments)
-            nb_s = len(component.states)
-            if len(component.states):
-                arguments = self.phi[(simstep+1, self.phi_index_slice_by_component[component])]
-
-                k = self.state_index_slice_by_component[component]
-                state = self.state[simstep, k]
-
-                state_new = np.zeros(nb_s)
-                j_state2arg = np.zeros((nb_s, nb_a))
-
-                component.update_state(state_new, j_state2arg, state, arguments, dt)
-
-                # state_new = (state_new + state)/2
-
-                # Write out state to component
-                self.state[simstep+1, k] = state_new
+        a, b = self.get_all(variable_key, terminal_label)
+        return a
```

### Comparing `fonsim-0.3.0/src/fonsim/core/solver.py` & `fonsim-0.4.0/src/fonsim/core/solver.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,349 +3,450 @@
 
 A solver takes care of solving the (non-linear)
 system of equations generated by the Simulation object.
 This object can interact with the Simulation object.
 
 The Simulation class expects the following methods
 from the solver object:
+
 - ``get_nb_steps_estimate()``
 - ``run_step(simulation_step_index)``
 
 Current solvers:
- 1. ImplicitEulerNewtonConstantTimeStep
- 2. ImplicitEulerNewtonAdaptiveTimeStep
+ 1. :py:class:`.solver.NewtonConstantTimeStep`
+ 2. :py:class:`.solver.NewtonAdaptiveTimeStep02`
 
 2020, July 23
 """
 
 import numpy as np
+from numpy.random import default_rng
+import inspect
 
 
-class ImplicitEulerNewton():
-    def __init__(self, simulation):
-        """
-        ImplicitEulerNewton class
-
-        :param simulation: Simulation object
-        """
+class BaseNewton:
+    """
+    Base class designed to ease creating new solvers
+    by providing common solver functionality
+    such as the Newton solver for solving systems of nonlinear equations.
+
+    The discretization method is set with the parameter ``discretization``.
+    The solver always solves the arguments for the selected timestep
+    (in the method ``run_step``),
+    and the solving is always done with the state values of that timestep,
+    however the handling of the state differs.
+    Most of the solvers in FONSim support several of the following
+    three discretization methods (specified as a string):
+
+    * **forward**: propagates the state to the next step.
+    * **backward**: propagates the state from the previous to the current step
+      with the arguments of the current step
+    * **tustin**: propagates the state from the previous to the current step
+      with the mean of the arguments of the previous
+      and the current step
+
+    :param simulation: Simulation object
+    :param supported_discretization_methods: the discretization methods
+                                             the inherited class supports,
+                                             must be set by child class
+    :param discretization: see above
+    """
+    def __init__(self, simulation, supported_discretization_methods,
+                 discretization):
         self.sim = simulation
 
-    def apply_solver_bias(self, bias=1e-12, step=0):
+        # Whether allowed to run on a simulation step
+        # that precedes the given step
+        self.go_backwards_allowed = True
+
+        # Discretization method
+        if not isinstance(discretization, str):
+            msg = f"The discretization method must be specified as a string, " \
+                  f"not as a {str(type(discretization))}."
+            raise ValueError(msg)
+        if discretization not in supported_discretization_methods:
+            msg = f"The selected discretization method '{str(discretization)}' " \
+                  f"is not supported by this solver, please select " \
+                  f"one of the following methods: " \
+                  f"{supported_discretization_methods}."
+            raise ValueError(msg)
+        self.discretization = discretization
+
+    def apply_solver_bias(self, bias=1e-12, step=0, quasirandom=False):
         """
         Give elements in the solution vector a small positive value, to
         ease starting the simulation
 
+        If ``quasirandom=True``, the assigned biases
+        come from a random number generator initialized with a constant seed
+        (i.e. the bias array is the same on each method call).
+
         :param bias: bias value added to the solution vector entries
         :param step: simulation step for which this bias is applied
+        :param quasirandom: whether to vary bias values
         :return: None
         """
-        for i in range(len(self.sim.phi)):
-            self.sim.phi[i][step] += bias
+        if quasirandom:
+            rng = default_rng(seed=12345)
+            bias *= (0.5 + 0.5*rng.random(self.sim.phi.shape[1]))
+        self.sim.phi[step, :] += bias
 
     def get_all_variables(self, simstep):
         """
         :param simstep: simulation step at which variables are queried
         :return: np array with the values of all arguments and component
                  states at the desired simulation step
         """
         # Get all argument values
         arguments = self.sim.phi[simstep,:]
         # Get all state values
         states = self.sim.state[simstep, :]
 
         return np.append(arguments, states)
 
-    def get_residual(self, simstep, res=None):
+    def get_residual(self, simstep, res=None, dt=None,
+                     discretization=None):
         """
         Evaluate the simulation system of equations at the provided
-        timestep to get the residual vector
+        timestep to get the residual vector.
+        See the related method :py:meth:`.Simulation.evaluate_equations`
+        for more documentation,
+        as most arguments are passed to that method unmodified.
 
         :param simstep: index of simulation timestep at which the system
                         of equations is evaluated
         :param res: optional initialized residual vector that will be
                     overwritten by this function in place
+        :param dt: timestep
+        :param discretization: discretization method, gets passed to
+                               :py:meth:`.Simulation.evaluate_equations`
         :return: evaluated residual vector
         """
         if res is None:
             res = np.zeros(self.sim.nb_arguments)
         elapsed_time = self.sim.times[simstep]
 
-        # Implicit Euler - evaluate equations and get updated jacobian H
-        self.sim.evaluate_equations(simstep-1, res, self.sim.H, 
-                                    elapsed_time, self.dt)
+        # Evaluate equations and get updated jacobian H
+        self.sim.evaluate_equations(simstep, res, self.sim.H,
+                                    elapsed_time, self.dt,
+                                    discretization)
         # evaluate network equations (can this be done more elegantly?)
         res[:self.sim.nb_network_equations] = np.dot(self.sim.A,
                                                      self.sim.phi[simstep,:])
 
         return res
 
-    def newton_solver(self, step, iterations=100, alpha=1.):
+    def newton_solver(self, step, iterations=100, alpha=1.,
+                      discretization=None, min_nb_iterations=1):
         """
         Newton method for solving the system equations and storing the
         solution in the simulation phi vector at an time step
 
         :param step: step index for which the system will be solved and
                      the solution will be stored. The initialization for the solver
                      can be done externally by setting self.sim.phi[step] to the
                      initial guess
         :param iterations: maximum number of newton solver iterations.
                            100 (default) gives good results although it often converges in
                            one step and otherwise mostly in less than ten
         :param alpha: correction constant for damped Newton method
+        :param discretization: discretization method, gets passed to
+                               :py:meth:`.solver.BaseNewton.get_residual`
         :return: flag indicating exit status of the solver for this step:
+
                  * 0: maximum amount of iterations reached without convergence
                  * 1: solver converged quickly
                  * 2: solver converged slowly
         """
         # Allocate residual vector
         residual = np.zeros(self.sim.nb_arguments)
         # Newton outer loop
         for i in range(iterations):
             # Get the residual vector
-            self.get_residual(step, residual)
-            # Solve the linear system
-            phi_correction = -np.linalg.solve(self.sim.H, residual)
-            # Apply the correction
-            self.sim.phi[step,:] = self.sim.phi[step,:] + alpha*phi_correction
+            self.get_residual(step, residual,
+                              discretization=discretization)
             # Look at error
-            max_error = np.max(np.abs(residual))
-            # the 0.1 is somewhat arbitrary. Better would be to set a max
-            # error for each equation, so the units and scale of each
-            # equation are taken into account. 0.1 gives ok results
-            if max_error < 0.1:
+            # residual is scaled with inverse of equation solving tolerances,
+            # aka when the scaled residual is smaller than 1.0,
+            # the desired error has been attained.
+            # The equation tolerances are updated every outer loop iteration
+            # because some components swap equations between iterations
+            # and thus the corresponding equation residuals change considerably.
+            if True:
+                self.sim.fill_component_equation_tolerances(
+                    self.sim.equation_tolerances, self.sim.equation_tolerances_inv)
+            residual_scaled = self.sim.equation_tolerances_inv * residual
+            max_error = np.max(np.abs(residual_scaled))
+            # See if the error is sufficiently small
+            # note: if the maximum error is sufficiently small
+            # already in the first iteration of this (inner) loop,
+            # no linear system solving is done
+            # and the argument values in this simulation step
+            # are kept the same as in the previous step
+            # (assuming they were initialized with the values
+            # from the previous step).
+            # Use 0.4 to avoid triggering
+            # the timestep sizing interpolation check.
+            if self.sim.verbose:
+                print(f'    max_error: {max_error:.1f}')
+            if np.isnan(max_error):
+                break
+            if max_error < 0.4 and i > min_nb_iterations:
                 #print("Outer loop converged in ", i + 1, "steps")
                 if i <= np.ceil(.1*iterations):
                     return 1
                 else:
                     return 2
+            # So the error is larger than desired
+            # Solve the linear system
+            try:
+                phi_correction = -np.linalg.solve(self.sim.H, residual)
+            except np.linalg.LinAlgError as e:
+                # probably singular matrix or so
+                if self.sim.verbose: print(e)
+                return 0
+            # Scale down the correction if it is so large
+            # that it would push any arguments outside their allowed range
+            max_correction_pos = self.sim.phi_range[:, 0] - self.sim.phi[step, :]
+            max_correction_neg = self.sim.phi_range[:, 1] - self.sim.phi[step, :]
+            rel_correction_pos = phi_correction / max_correction_pos
+            rel_correction_neg = phi_correction / max_correction_neg
+            times_too_large = max(np.amax(rel_correction_pos), np.amax(rel_correction_neg))
+            if alpha * times_too_large > 1:
+                # take 0.9 to keep a little distance from the limits
+                phi_correction *= 0.9 / times_too_large
+            # Apply the correction
+            self.sim.phi[step,:] = self.sim.phi[step,:] + alpha*phi_correction
+        if self.sim.verbose:
+            print(f'Exited without convergence with max_error {max_error:.1f}')
         return 0
 
+    def run_forward(self, step):
+        """Run forward solver on a single step"""
+        phi_old = self.sim.phi[step, :].copy()
+        if self.sim.verbose >= 1: print(f'run_forward simstep {step}')
+        status = self.newton_solver(step, discretization='forward')
+        if status == 0 and self.sim.verbose >= 1:
+            self.print_report(step)
+        if self.sim.verbose >= 1: print(f'end run_forward simstep {step}')
+        # If did not converge, reset original values
+        if status == 0:
+            self.sim.phi[step, :] = phi_old
+
     def print_report(self, simstep):
         """
         Print a report on the solver status at a certain simulation time
         step.
 
         :param simstep: index of simulation timestep for which the report
                         is generated
         :return: None
         """
-        np.set_printoptions(formatter={'float': '{: 0.0f}'.format})
         # display simulation time
         print("t = {}".format(self.sim.times[simstep]))
         # display argument values
         arg_str = ""
         for i in range(self.sim.nb_arguments):
             if i > 0:
                 arg_str += ", "
             arg_str += "{} = {}".format(self.sim.arguments[i].short_str(),
-                                        self.sim.phi[simstep+1,i])
+                                        self.sim.phi[simstep,i])
         print(arg_str)
 
         # display residuals of non-converging equations
         residuals = self.get_residual(simstep)
         for i in range(len(residuals)):
             if abs(residuals[i]) > 0.1:
                 print("eq {}: {} = {}".format(i, 
                       self.sim.equation_to_string(i), residuals[i]))
         # display system jacobian
-        print("B:\n", self.sim.H[self.sim.nb_network_equations:,:])
-
+        with np.printoptions(linewidth=300, formatter={'float': lambda f: f'{f:6.0f}'}) as opts:
+            print("B:\n", self.sim.H[self.sim.nb_network_equations:, :])
 
         print()
 
 
-class ImplicitEulerNewtonConstantTimeStep(ImplicitEulerNewton):
-    def __init__(self, simulation, step):
-        """
-        ImplicitEulerNewtonConstantTimeStep class
-
-        :param simulation: Simulation object
-        :param step: fixed time increment
-        """
-        super().__init__(simulation)
+class NewtonConstantTimeStep(BaseNewton):
+    """
+    Supported discretization methods:
+    'forward', 'backward' and 'tustin'.
+
+    Please see the base class for more information.
+
+    :param simulation: Simulation object
+    :param step: fixed time increment
+    :param discretization: discretization method
+    """
+    def __init__(self, simulation, step, discretization):
+        super().__init__(simulation, supported_discretization_methods={
+            'forward', 'backward', 'tustin',
+        }, discretization=discretization)
 
         # stepping
         self.dt = step
 
     def get_nb_steps_estimate(self):
         """
         :return: number of timesteps the solver needs
         """
         return int(np.ceil(self.sim.duration / self.dt)) + 1
 
     def run_step(self, simstep):
         """
         Run a single step of the solver.
-        Note: Calling it at step n ('simstep' = n)
-        results in it writing to the next step,
-        aka step n+1
+        Depending on the selected discretization
+        (``self.discretization``), different timestep indices
+        are used and affected (please see class doc).
 
         :param simstep: index of simulation timestep with the last results
         :return: None
         """
-        # First estimate for new arguments: arguments of previous step
-        self.sim.phi[simstep+1,:] = self.sim.phi[simstep, :]
-        if simstep <= 0:
-            self.apply_solver_bias(step=1)
-        # Update current time
-        self.sim.times[simstep+1] = (simstep+1) * self.dt
-        # Solve system for arguments
-        status = self.newton_solver(simstep+1)
-        # Report on solver convergence
-        if status == 0 and self.sim.verbose >= 1:
-            self.print_report(simstep+1)
-
-        # got the arguments, to finish update the state (with the updated
-        # arguments)
-        self.sim.update_state(simstep, self.dt)
+        if self.sim.verbose >= 1:
+            padding = '|   ' * (len(inspect.stack(0)) - 3)
+            print(padding + 'solver.run_step(simstep), simstep:', simstep)
+
+        # Solve arguments of first step, always using forward discretization
+        # (because no previous state is available)
+        if simstep == 0:
+            self.sim.times[0] = 0
+            self.apply_solver_bias(step=0, quasirandom=True)
+            self.run_forward(0)
+        # simstep > 0
+        else:
+            # Update the time where the propagated state will land
+            self.sim.times[simstep] = self.sim.times[simstep-1] + self.dt
 
+            # Propagate the state
+            if self.discretization == 'forward':
+                self.sim.update_state(simstep_args=simstep-1, simstep_state=simstep-1,
+                                      dt=self.dt, discretization=self.discretization)
+
+            # First estimate for new arguments: arguments of previous step
+            self.sim.phi[simstep, :] = self.sim.phi[simstep-1, :]
+            # Solve system for arguments
+            status = self.newton_solver(simstep, discretization=self.discretization)
+            # Report on solver convergence
+            if status == 0:
+                # Report on solver convergence
+                print(f'Solver failed to converge at step {simstep}')
+                if self.sim.verbose >= 1: self.print_report(simstep)
 
-class ImplicitEulerNewtonAdaptiveTimeStep(ImplicitEulerNewton):
-    def __init__(self, simulation, step, step_min, step_max,
-                 max_attempts=200):
-        """
-        ImplicitEulerNewtonAdaptiveTimeStep class
+            # Update the state with the new arguments
+            if self.discretization in ('backward', 'tustin'):
+                self.sim.update_state(simstep_args=simstep, simstep_state=simstep-1,
+                                      dt=self.dt, discretization=self.discretization)
+
+
+class NewtonAdaptiveTimeStep02(BaseNewton):
+    """
+    Supported discretization methods:
+    'backward' and 'tustin'.
+    'forward' is not yet supported.
+
+    Please see base class for more information.
+
+    :param simulation: Simulation object
+    :param step: minimum and maximum time increment
+    :param discretization: discretization method
+    """
+    def __init__(self, simulation, step, discretization):
+        super().__init__(simulation, supported_discretization_methods={
+            'backward', 'tustin',
+        }, discretization=discretization)
 
-        :param simulation: Simulation object
-        :param step: initial time increment
-        :param step_min: minimum possible time increment
-        :param step_max: maximum possible time increment
-        :param max_attempts: maximum allowed number of solver attempts
-                             within a time increment
-        :return: None
-        """
-        super().__init__(simulation)
+        # stepping
+        self.dt_min = step[0]
+        self.dt_max = step[1]
 
-        # time stepping
-        self.dt = step
-        self.dt_min = step_min if step_min is not None else 1e-4*self.dt
-        self.dt_max = step_max if step_max is not None else 1.5*self.dt
-        self.max_attempts = max_attempts
-
-        # keep track of the average and variance of the changes in arguments
-        nb_states = sum([len(c.states) for c in self.sim.system.components])
-        self.delta_av = np.zeros(self.sim.nb_arguments+nb_states)
-        self.delta_var = np.zeros(self.sim.nb_arguments+nb_states)
-
-    def update_delta_range(self, nb_points, delta):
-        """
-        Update the average and variance of the changes of simulation
-        variables (both arguments and states) over all simulation steps
-        with the change at the current step
-        
-        :param nb_points: amount of steps included in the last metrics
-        :param delta: new change in simulation arguments between
-                      consecutive steps to include in the metrics
-        :return: None
-        """
-        # Sign is irrelevant, only magnitude counts
-        delta = np.abs(delta)
-        # Calculate variance
-        if nb_points > 0:
-            self.delta_var = ((nb_points-1)*self.delta_var + \
-                             np.power(delta-self.delta_av,2.))/ nb_points
-        # Calculate average
-        self.delta_av = (nb_points*self.delta_av + delta)/ (nb_points+1)
-
-    def delta_in_range(self, delta):
-        """
-        Check whether a change in simulation variables (both arguments
-        and states) during a step is within an acceptable range compared
-        to the other simulation step results or it is abnormally large
-
-        :param delta: vector with change in all the arguments between
-                    consecutive simulation steps
-        :return in_range: True if delta is of an acceptable magnitude and
-                          False if it represents a change which is abnormally large
-        """
-        # Sign is irrelevant, only magnitude counts
-        delta = np.abs(delta)
-
-        # Loop over arguments
-        for var_ind in range(len(delta)):
-            # Only look at steps that are too big (too small is not an issue)
-            # and compare their deviation from the mean with the variance
-            # (rather than standard deviation since this requires taking
-            # square roots on a regular basis)
-            deviation = delta[var_ind] - self.delta_av[var_ind]
-            if deviation > 1.3e154 or (deviation > 0 and \
-               deviation**2 > 25*self.delta_var[var_ind]):
-                return False
+        self.dt = self.dt_min
 
-        return True
+        # Magic numbers for adjusting timestep
+        self.factor_decrease = 0.5
+        self.factor_increase = 1.5
+        self.threshold_increase = 0.5
 
     def get_nb_steps_estimate(self):
         """
-        :return: number of timesteps the solver thinks it will need to
-                 finish the simulation
+        :return: number of timesteps the solver needs
         """
-        if np.max(self.sim.times) > 0. and np.argmax(self.sim.times) > 0:
-            dt_av = np.max(self.sim.times) / np.argmax(self.sim.times)
-        else:
-            dt_av = self.dt
-        return int(np.ceil(self.sim.duration / dt_av)) + 1
+        return int(np.ceil(self.sim.duration / self.dt_min)) + 1
 
-    def run_step(self, simstep):
+    def run_step(self, simstep, recursion_allowed=True):
         """
         Run a single step of the solver.
-        Note: Calling it at step n ('simstep' = n)
-        results in it writing to the next step,
-        aka step n+1
-
-        :param simstep: index of timestep with the last simulated results
-        :return: list with as elements:
-                 * 0: boolean showing solver convergence for the simulation step
-                 * 1: string giving more information about the exit status
-        """
-        # Solve system for arguments
-        attempt = 1
-        try_decreasing_step = True
-        while attempt < self.max_attempts:
-            # First estimate for new arguments: values of previous step
-            self.sim.phi[simstep+1,:] = self.sim.phi[simstep, :] 
-            if simstep <= 0:
-                self.apply_solver_bias(step=1)
 
+        :param simstep: index of simulation timestep with the last results
+        :param recursion_allowed: whether it may call itself
+        :return: None
+        """
+        if self.sim.verbose >= 1:
+            padding = '|   ' * (len(inspect.stack(0)) - 3)
+            print(padding + 'solver.run_step(simstep), simstep:', simstep)
+
+        # Solve arguments of first step
+        if simstep == 0:
+            self.sim.times[0] = 0
+            self.apply_solver_bias(step=0, quasirandom=True)
+            self.run_forward(0)
+        else:
             # Update current time
-            self.sim.times[simstep+1] = self.sim.times[simstep] + self.dt
-            # Solve the system at the current time
-            status = self.newton_solver(simstep+1, alpha=1.)
-            solver_success = status in (1,2)
-            # Update the state with the updated arguments
-            self.sim.update_state(simstep, self.dt)
-            # Calculate how much all variables (arguments and states) 
-            # changed in this simulation step
-            delta = self.get_all_variables(simstep+1) - \
-                    self.get_all_variables(simstep)
-            reliable_result = simstep <= 1 or self.delta_in_range(delta)
-
-            # Stepping logic
-            if not (solver_success and reliable_result) and \
-               self.dt > self.dt_min and try_decreasing_step:
-                # No convergence reached, but it is still possible to
-                # decrease the time step size and try again
-                self.dt = max(self.dt_min, .1*self.dt)
-            elif not solver_success:
-                # No convergence reached even after decreasing the step
-                # size, so increase the step size gradually instead
-                try_decreasing_step = False
-                self.dt += self.dt_min
-            else:
-                # Accept found solution
-                break
-            attempt += 1
+            self.sim.times[simstep] = self.sim.times[simstep-1] + self.dt
+            # First estimate for new arguments: arguments of previous step
+            self.sim.phi[simstep, :] = self.sim.phi[simstep-1, :]
 
-        # Solver converged
-        if solver_success:
-            # Update metrics of what counts as a normal change in 
-            # variable values
-            self.update_delta_range(simstep, delta)
-            # Increase step time if convergence was swift
-            if attempt <= 1 and status == 1:
-                self.dt = min(self.dt_max, 1.5*self.dt)
-            return solver_success
-        # Solver did not converge
-        else:
             if self.sim.verbose >= 1:
+                print(padding + '| dt  [ms]:', '{:7.2f}'.format(self.dt*1000))
+                print(padding + '| t   [ms]:',
+                      '{:7.2f}'.format(self.sim.times[simstep-1] * 1e3) +
+                      ' -> {:7.2f}'.format(self.sim.times[simstep] * 1e3))
+
+            # Solve system for arguments
+            status = self.newton_solver(simstep, discretization=self.discretization)
+            # Solver did not converge and we're already at the smallest timestep
+            if status == 0 and self.dt == self.dt_min:
                 # Report on solver convergence
-                self.print_report(simstep+1)
-            return (solver_success, "Solver failed to converge")
+                print(f'Solver failed to converge at step {simstep}')
+                if self.sim.verbose >= 1: self.print_report(simstep)
+
+            # update the state with the updated arguments
+            self.sim.update_state(simstep_args=simstep, simstep_state=simstep-1,
+                                  dt=self.dt, discretization=self.discretization)
+
+        # Look whether timestep has to be adjusted
+        # and do recursive call if timestep decreased.
+        # Don't adjust it during the first five steps
+        # as then tolerances not yet well initialized.
+        if simstep < 5 or recursion_allowed is False:
+            pass
+        else:
+            # Check whether timestep sufficiently small
+            # by comparing the derived argument and state vectors at step `simstep`
+            # with the one interpolated between `simstep - 1` and `simstep + 1`.
+            t = self.sim.times
+            rico_arg_t = (self.sim.phi[simstep] - self.sim.phi[simstep-2]) / (t[simstep] - t[simstep-2])
+            phi_ip = self.sim.phi[simstep-2] + rico_arg_t * (t[simstep-1] - t[simstep-2])
+            rico_state_t = (self.sim.state[simstep] - self.sim.state[simstep-2]) / (t[simstep] - t[simstep-2])
+            state_ip = self.sim.state[simstep-2] + rico_state_t * (t[simstep-1] - t[simstep-2])
+            na, ns = self.sim.nb_arguments, self.sim.nb_states
+            interpolation_err = np.zeros(na+ns, dtype=float)
+            # also multiply the error with inverse of relative tolerances
+            # and take maximum absolute value
+            interpolation_err[:na] = (self.sim.phi[simstep] - phi_ip) * self.sim.argument_tolerances_inv
+            interpolation_err[na:na+ns] = (self.sim.state[simstep] - state_ip) * self.sim.state_tolerances_inv
+            np.abs(interpolation_err, out=interpolation_err)
+            max_error = np.max(interpolation_err)
+            if self.sim.verbose:
+                print(padding + '| max_error:', '{:5.1f}'.format(max_error))
+            # If too large, go back two steps and retry
+            # also do so on non-convergence
+            if (max_error > 1 or status == 0) and self.dt > self.dt_min:
+                # Reduce timestep
+                self.dt = max(self.dt*self.factor_decrease, self.dt_min)
+                # and run this step again, as well as the previous step
+                # (recursive calls)
+                if self.go_backwards_allowed:
+                    self.run_step(simstep-1, recursion_allowed=False)
+                self.run_step(simstep, recursion_allowed=self.go_backwards_allowed)
+            else:
+                # If error small, increase timestep
+                if max_error < self.threshold_increase:
+                    self.dt = min(self.dt*self.factor_increase, self.dt_max)
```

### Comparing `fonsim-0.3.0/src/fonsim/core/system.py` & `fonsim-0.4.0/src/fonsim/core/system.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/core/terminal.py` & `fonsim-0.4.0/src/fonsim/core/terminal.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/core/variable.py` & `fonsim-0.4.0/src/fonsim/core/variable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Class Variable
 
 2020, July 21
 """
 
+import numpy as np
 import warnings
 
 
 class Variable:
     """
     A ``Variable`` object is used to denote the presence of a yet unknown numerical value.
     For each Variable object, the solver will search for the optimal numerical values over time.
@@ -26,31 +27,39 @@
     such as pressure,
     while the latter is typically used with directional values,
     such as a massflow.
     'local' indicates that it will not be shared (feature WIP).
 
     :param key: type label, e.g. 'pressure', 'massflow'
     :param orientation: 'across', 'through' or 'free'.
-    :param initial_value: Initial value, default: 0
     :param terminal: Terminal object to which Variable object get connected, default: None
+    :param label: label, used to refer to a Variable instance later on
+    :param initial_value: Initial value, default: 0
+    :param range: tuple with min and max of allowed value range
     """
-    def __init__(self, key, orientation, initial_value=0., terminal=None, label='None'):
+    def __init__(self, key, orientation, terminal=None, label='None',
+                 initial_value=0., range=(-np.Inf, np.Inf)):
         # Check input
         if orientation not in ('across', 'through', 'local'):
             msg = 'Parameter "orientation" ' + \
                   'ought to have value "across" or "through" or "local", ' + \
                   'but encountered <' + orientation + '>.'
             warnings.warn(msg, UserWarning, stacklevel=2)
+        if not isinstance(range, tuple) or \
+                (isinstance(range, tuple) and len(range) != 2):
+            msg = "Parameter 'range' must be a tuple of length two."
+            raise ValueError(msg)
 
         # Assign arguments to object properties
         self.key = key
         self.orientation = orientation
-        self.initial_value = initial_value
         self.terminal = terminal
         self.label = str(label)
+        self.initial_value = initial_value
+        self.range = range
 
     def __str__(self):
         """
         Return a description string of the format
         ``Variable <self.key> of component <self.terminal.component.label>``.
         The component description part is only added
         if the variable belongs to the terminal of a component.
@@ -58,15 +67,15 @@
         :return: var_str: string with description of variable object
         """
         var_str = "Variable {}".format(self.key)
         if self.terminal is not None:
             var_str += " of component {}".format(self.terminal.component.label)
         return var_str
 
-    def short_str(self, nb_var_chars=1):
+    def short_str(self, nb_var_chars=1):    # pragma: no cover
         """
         Return a short string describing the variable more as a symbol than in
         words. This string contains the first n letters of the variable name
         as well as (if applicable) the port and component it is attached to.
 
         :param nb_var_chars: number of characters with which the variable key
                              is abbreviated. Set to 0 to avoid abbreviation.
@@ -86,9 +95,10 @@
         The returned variable has the same key, orientation and initial value
         but is otherwise unrelated to the Variable object
         it is called upon.
 
         :param terminal: Terminal object to attach the variable copy to
         :return variable: attached copy of the variable object
         """
-        return Variable(self.key, self.orientation, self.initial_value, 
-                        terminal, self.label)
+        return Variable(self.key, self.orientation,
+                        terminal=terminal, label=self.label,
+                        initial_value=self.initial_value, range=self.range)
```

### Comparing `fonsim-0.3.0/src/fonsim/data/curve.py` & `fonsim-0.4.0/src/fonsim/data/curve.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/data/dataseries.py` & `fonsim-0.4.0/src/fonsim/data/dataseries.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/data/interpolate.py` & `fonsim-0.4.0/src/fonsim/data/interpolate.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/data/pvcurve.py` & `fonsim-0.4.0/src/fonsim/data/pvcurve.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/data/writeout.py` & `fonsim-0.4.0/src/fonsim/data/writeout.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/fluid/fallback.py` & `fonsim-0.4.0/src/fonsim/fluid/fallback.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/fluid/fluid.py` & `fonsim-0.4.0/src/fonsim/fluid/fluid.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/fluids/IdealCompressible.py` & `fonsim-0.4.0/src/fonsim/fluids/IdealCompressible.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/fluids/IdealIncompressible.py` & `fonsim-0.4.0/src/fonsim/fluids/IdealIncompressible.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/resources/Measurement_60mm_balloon_actuator_01.csv` & `fonsim-0.4.0/src/fonsim/resources/Measurement_60mm_balloon_actuator_01.csv`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/visual/plotting.py` & `fonsim-0.4.0/src/fonsim/visual/plotting.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     :return: None
     """
     # Get unit multiplier
     m = 1/suc.get_factor(unit)
 
     # Plot data of all components
     for comp_c in components:
-        if len(comp_c) == 2:
+        if not isinstance(comp_c, str) and len(comp_c) == 2:
             comp = comp_c[0]
             term = comp_c[1]
         else:
             comp = comp_c
             term = None
         comp = sim.system.get(comp)
         data, term = comp.get_all(label, term)
```

### Comparing `fonsim-0.3.0/src/fonsim/wave/custom.py` & `fonsim-0.4.0/src/fonsim/wave/custom.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim/wave/wave.py` & `fonsim-0.4.0/src/fonsim/wave/wave.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/src/fonsim.egg-info/SOURCES.txt` & `fonsim-0.4.0/src/fonsim.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/fonsim/components/circulartube_autodiff.py
 src/fonsim/components/containers.py
 src/fonsim/components/containers_autodiff.py
 src/fonsim/components/dummy.py
 src/fonsim/components/restrictors.py
 src/fonsim/components/sources.py
 src/fonsim/components/terminals.py
+src/fonsim/components/valves.py
 src/fonsim/constants/__init__.py
 src/fonsim/constants/norm.py
 src/fonsim/constants/physical.py
 src/fonsim/conversion/__init__.py
 src/fonsim/conversion/indexmatch.py
 src/fonsim/core/__init__.py
 src/fonsim/core/component.py
@@ -56,10 +57,12 @@
 tests/test_component_autocall.py
 tests/test_custom.py
 tests/test_dataseries.py
 tests/test_indexmatch.py
 tests/test_interpolate.py
 tests/test_node.py
 tests/test_pvcurve.py
+tests/test_simulation_and_solver.py
+tests/test_solver_infinite_flow.py
 tests/test_system.py
 tests/test_terminal.py
 tests/test_variable.py
```

### Comparing `fonsim-0.3.0/tests/test_component_autocall.py` & `fonsim-0.4.0/tests/test_component_autocall.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/tests/test_custom.py` & `fonsim-0.4.0/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/tests/test_dataseries.py` & `fonsim-0.4.0/tests/test_dataseries.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/tests/test_indexmatch.py` & `fonsim-0.4.0/tests/test_indexmatch.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/tests/test_interpolate.py` & `fonsim-0.4.0/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/tests/test_node.py` & `fonsim-0.4.0/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/tests/test_pvcurve.py` & `fonsim-0.4.0/tests/test_pvcurve.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/tests/test_system.py` & `fonsim-0.4.0/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/tests/test_terminal.py` & `fonsim-0.4.0/tests/test_terminal.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.3.0/tests/test_variable.py` & `fonsim-0.4.0/tests/test_variable.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 Test variable.py
 2022, May 06
 """
 
 import collections.abc
+import warnings
 
 from fonsim.core.variable import Variable
 from fonsim.core.terminal import Terminal
 
+import pytest
+
 
 def test_hashable():
     # Test whether Variable object is hashable
     var = Variable(key='pressure', orientation='across')
     assert isinstance(var, collections.abc.Hashable)
 
 
@@ -22,7 +25,22 @@
     var_b = var_a.copy_and_attach(term)
 
     assert var_a != var_b
     assert var_a.key == var_b.key
     assert var_a.orientation == var_b.orientation
     assert var_a.terminal is None
     assert var_b.terminal == term
+
+
+@pytest.mark.parametrize('orientation, warning_expected', [
+    ('across', False), ('through', False), ('local', False),
+    ('over', True),
+])
+def test_unexpected_orientation(orientation, warning_expected):
+    """Method __init__ given parameter value check"""
+    if warning_expected:
+        with pytest.warns():
+            Variable(key='foo', orientation=orientation)
+    else:
+        with warnings.catch_warnings():
+            warnings.simplefilter('error')
+            Variable(key='foo', orientation=orientation)
```

