# Comparing `tmp/oqpy-0.1.2.tar.gz` & `tmp/oqpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oqpy-0.1.2.tar", max compression
+gzip compressed data, was "oqpy-0.2.0.tar", max compression
```

## Comparing `oqpy-0.1.2.tar` & `oqpy-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,11 @@
--rw-r--r--   0        0        0    11328 2022-10-20 16:34:51.863893 oqpy-0.1.2/LICENSE
--rw-r--r--   0        0        0       71 2022-10-20 16:34:51.864132 oqpy-0.1.2/NOTICE
--rw-r--r--   0        0        0     5672 2022-10-22 16:51:31.156458 oqpy-0.1.2/README.md
--rw-r--r--   0        0        0     1011 2022-11-22 17:39:48.198978 oqpy-0.1.2/oqpy/__init__.py
--rw-r--r--   0        0        0    10916 2022-11-22 17:38:49.228042 oqpy-0.1.2/oqpy/base.py
--rw-r--r--   0        0        0    10737 2022-11-22 17:38:49.228470 oqpy-0.1.2/oqpy/classical_types.py
--rw-r--r--   0        0        0     3627 2022-10-20 16:34:51.865859 oqpy-0.1.2/oqpy/control_flow.py
--rw-r--r--   0        0        0    20803 2022-11-22 17:38:49.230079 oqpy-0.1.2/oqpy/program.py
--rw-r--r--   0        0        0     2480 2022-10-20 16:34:51.866312 oqpy-0.1.2/oqpy/pulse.py
--rw-r--r--   0        0        0     4196 2022-11-22 17:38:49.230517 oqpy-0.1.2/oqpy/quantum_types.py
--rw-r--r--   0        0        0     6660 2022-10-20 16:34:51.866612 oqpy-0.1.2/oqpy/subroutines.py
--rw-r--r--   0        0        0     2506 2022-10-20 16:34:51.866749 oqpy-0.1.2/oqpy/timing.py
--rw-r--r--   0        0        0     3654 2022-11-23 00:23:22.711979 oqpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6988 1970-01-01 00:00:00.000000 oqpy-0.1.2/setup.py
--rw-r--r--   0        0        0     7112 1970-01-01 00:00:00.000000 oqpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      231 2022-05-24 00:17:51.382265 oqpy-0.2.0/oqpy/__init__.py
+-rw-r--r--   0        0        0     7473 2022-05-24 21:39:51.720076 oqpy-0.2.0/oqpy/classical_types.py
+-rw-r--r--   0        0        0     1426 2022-05-24 01:36:30.322238 oqpy-0.2.0/oqpy/control_flow.py
+-rw-r--r--   0        0        0     4692 2022-05-24 16:12:12.287830 oqpy-0.2.0/oqpy/program.py
+-rw-r--r--   0        0        0     4184 2022-05-24 21:37:15.893169 oqpy-0.2.0/oqpy/pulse.py
+-rw-r--r--   0        0        0     3452 2022-05-24 01:48:30.150772 oqpy-0.2.0/oqpy/quantum_types.py
+-rw-r--r--   0        0        0     2904 2022-05-24 01:36:51.410320 oqpy-0.2.0/oqpy/subroutines.py
+-rw-r--r--   0        0        0      776 2022-05-24 01:37:28.557215 oqpy-0.2.0/oqpy/timing.py
+-rw-r--r--   0        0        0     1494 2022-05-24 00:17:51.399757 oqpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      670 2022-05-24 21:55:40.479668 oqpy-0.2.0/setup.py
+-rw-r--r--   0        0        0      447 2022-05-24 21:55:40.479915 oqpy-0.2.0/PKG-INFO
```

