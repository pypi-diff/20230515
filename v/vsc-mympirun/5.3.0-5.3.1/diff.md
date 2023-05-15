# Comparing `tmp/vsc-mympirun-5.3.0.tar.gz` & `tmp/vsc-mympirun-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsc-mympirun-5.3.0.tar", last modified: Thu Feb 23 15:49:35 2023, max compression
+gzip compressed data, was "vsc-mympirun-5.3.1.tar", last modified: Mon May 15 15:37:01 2023, max compression
```

## Comparing `vsc-mympirun-5.3.0.tar` & `vsc-mympirun-5.3.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-02-23 15:49:35.498103 vsc-mympirun-5.3.0/
--rw-r--r--   0 kehoste    (501) staff       (20)    18092 2020-03-24 09:01:26.000000 vsc-mympirun-5.3.0/LICENSE
--rw-r--r--   0 kehoste    (501) staff       (20)    10405 2023-02-23 15:49:35.497284 vsc-mympirun-5.3.0/PKG-INFO
--rw-r--r--   0 kehoste    (501) staff       (20)     9797 2020-11-12 10:19:51.000000 vsc-mympirun-5.3.0/README.md
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-02-23 15:49:35.493725 vsc-mympirun-5.3.0/bin/
--rwxr-xr-x   0 kehoste    (501) staff       (20)     1516 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/bin/mympirun.py
--rw-r--r--   0 kehoste    (501) staff       (20)     5391 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/bin/mympisanity.py
--rwxr-xr-x   0 kehoste    (501) staff       (20)     1336 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/bin/mypmirun.py
--rwxr-xr-x   0 kehoste    (501) staff       (20)     2146 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/bin/mytaskprolog.py
--rwxr-xr-x   0 kehoste    (501) staff       (20)     1666 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/bin/mytasks.py
--rwxr-xr-x   0 kehoste    (501) staff       (20)     3123 2022-03-30 07:48:38.000000 vsc-mympirun-5.3.0/bin/pbsssh.sh
--rwxr-xr-x   0 kehoste    (501) staff       (20)     1266 2020-03-24 09:01:26.000000 vsc-mympirun-5.3.0/bin/sshsleep.sh
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-02-23 15:49:35.498794 vsc-mympirun-5.3.0/external_dist_only/
--rw-r--r--   0 kehoste    (501) staff       (20)    72704 2023-02-23 15:49:35.498858 vsc-mympirun-5.3.0/external_dist_only/shared_setup_dist_only.py
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-02-23 15:49:35.492497 vsc-mympirun-5.3.0/lib/
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-02-23 15:49:35.493851 vsc-mympirun-5.3.0/lib/vsc/
--rw-r--r--   0 kehoste    (501) staff       (20)     1206 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/__init__.py
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-02-23 15:49:35.494377 vsc-mympirun-5.3.0/lib/vsc/mympirun/
--rw-r--r--   0 kehoste    (501) staff       (20)     1206 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/__init__.py
--rw-r--r--   0 kehoste    (501) staff       (20)    13427 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/common.py
--rw-r--r--   0 kehoste    (501) staff       (20)     2330 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/factory.py
--rw-r--r--   0 kehoste    (501) staff       (20)     5088 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/main.py
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-02-23 15:49:35.495090 vsc-mympirun-5.3.0/lib/vsc/mympirun/mpi/
--rw-r--r--   0 kehoste    (501) staff       (20)     1206 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/mpi/__init__.py
--rw-r--r--   0 kehoste    (501) staff       (20)    11781 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/mpi/intelmpi.py
--rw-r--r--   0 kehoste    (501) staff       (20)    37560 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/mpi/mpi.py
--rw-r--r--   0 kehoste    (501) staff       (20)     4428 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/mpi/mpich.py
--rw-r--r--   0 kehoste    (501) staff       (20)    11686 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/mpi/openmpi.py
--rw-r--r--   0 kehoste    (501) staff       (20)     4341 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/mpi/option.py
--rw-r--r--   0 kehoste    (501) staff       (20)     6419 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/option.py
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-02-23 15:49:35.495763 vsc-mympirun-5.3.0/lib/vsc/mympirun/pmi/
--rw-r--r--   0 kehoste    (501) staff       (20)     1206 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/pmi/__init__.py
--rw-r--r--   0 kehoste    (501) staff       (20)    11724 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/pmi/mpi.py
--rw-r--r--   0 kehoste    (501) staff       (20)     2970 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/pmi/option.py
--rw-r--r--   0 kehoste    (501) staff       (20)     1406 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/pmi/pmi.py
--rw-r--r--   0 kehoste    (501) staff       (20)     6022 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/pmi/sched.py
--rw-r--r--   0 kehoste    (501) staff       (20)     8415 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/pmi/slurm.py
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-02-23 15:49:35.496378 vsc-mympirun-5.3.0/lib/vsc/mympirun/rm/
--rw-r--r--   0 kehoste    (501) staff       (20)     1206 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/rm/__init__.py
--rw-r--r--   0 kehoste    (501) staff       (20)     2091 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/rm/local.py
--rw-r--r--   0 kehoste    (501) staff       (20)     3221 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/rm/pbs.py
--rw-r--r--   0 kehoste    (501) staff       (20)     8653 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/rm/sched.py
--rw-r--r--   0 kehoste    (501) staff       (20)     1369 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/rm/scoop.py
--rw-r--r--   0 kehoste    (501) staff       (20)     4011 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.0/lib/vsc/mympirun/rm/slurm.py
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-02-23 15:49:35.497101 vsc-mympirun-5.3.0/lib/vsc_mympirun.egg-info/
--rw-r--r--   0 kehoste    (501) staff       (20)    10405 2023-02-23 15:49:35.000000 vsc-mympirun-5.3.0/lib/vsc_mympirun.egg-info/PKG-INFO
--rw-r--r--   0 kehoste    (501) staff       (20)     1137 2023-02-23 15:49:35.000000 vsc-mympirun-5.3.0/lib/vsc_mympirun.egg-info/SOURCES.txt
--rw-r--r--   0 kehoste    (501) staff       (20)      648 2023-02-23 15:49:35.000000 vsc-mympirun-5.3.0/lib/vsc_mympirun.egg-info/dependency_links.txt
--rw-r--r--   0 kehoste    (501) staff       (20)        4 2023-02-23 15:49:35.000000 vsc-mympirun-5.3.0/lib/vsc_mympirun.egg-info/namespace_packages.txt
--rw-r--r--   0 kehoste    (501) staff       (20)        1 2023-02-23 15:49:35.000000 vsc-mympirun-5.3.0/lib/vsc_mympirun.egg-info/not-zip-safe
--rw-r--r--   0 kehoste    (501) staff       (20)       40 2023-02-23 15:49:35.000000 vsc-mympirun-5.3.0/lib/vsc_mympirun.egg-info/requires.txt
--rw-r--r--   0 kehoste    (501) staff       (20)        4 2023-02-23 15:49:35.000000 vsc-mympirun-5.3.0/lib/vsc_mympirun.egg-info/top_level.txt
--rw-r--r--   0 kehoste    (501) staff       (20)      201 2023-02-23 15:49:35.497736 vsc-mympirun-5.3.0/setup.cfg
--rw-r--r--   0 kehoste    (501) staff       (20)     8038 2023-02-23 15:49:35.498040 vsc-mympirun-5.3.0/setup.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-05-15 15:37:00.999335 vsc-mympirun-5.3.1/
+-rw-r--r--   0 kehoste    (501) staff       (20)    18092 2020-03-24 09:01:26.000000 vsc-mympirun-5.3.1/LICENSE
+-rw-r--r--   0 kehoste    (501) staff       (20)    10405 2023-05-15 15:37:00.998662 vsc-mympirun-5.3.1/PKG-INFO
+-rw-r--r--   0 kehoste    (501) staff       (20)     9797 2020-11-12 10:19:51.000000 vsc-mympirun-5.3.1/README.md
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-05-15 15:37:00.993963 vsc-mympirun-5.3.1/bin/
+-rwxr-xr-x   0 kehoste    (501) staff       (20)     1516 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/bin/mympirun.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     5391 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/bin/mympisanity.py
+-rwxr-xr-x   0 kehoste    (501) staff       (20)     1336 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/bin/mypmirun.py
+-rwxr-xr-x   0 kehoste    (501) staff       (20)     2146 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/bin/mytaskprolog.py
+-rwxr-xr-x   0 kehoste    (501) staff       (20)     1666 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/bin/mytasks.py
+-rwxr-xr-x   0 kehoste    (501) staff       (20)     3123 2022-03-30 07:48:38.000000 vsc-mympirun-5.3.1/bin/pbsssh.sh
+-rwxr-xr-x   0 kehoste    (501) staff       (20)     1266 2020-03-24 09:01:26.000000 vsc-mympirun-5.3.1/bin/sshsleep.sh
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-05-15 15:37:01.000037 vsc-mympirun-5.3.1/external_dist_only/
+-rw-r--r--   0 kehoste    (501) staff       (20)    70782 2023-05-15 15:37:01.000122 vsc-mympirun-5.3.1/external_dist_only/shared_setup_dist_only.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-05-15 15:37:00.992265 vsc-mympirun-5.3.1/lib/
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-05-15 15:37:00.994153 vsc-mympirun-5.3.1/lib/vsc/
+-rw-r--r--   0 kehoste    (501) staff       (20)     1206 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/__init__.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-05-15 15:37:00.995214 vsc-mympirun-5.3.1/lib/vsc/mympirun/
+-rw-r--r--   0 kehoste    (501) staff       (20)     1206 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/__init__.py
+-rw-r--r--   0 kehoste    (501) staff       (20)    13427 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/common.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     2330 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/factory.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     5088 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/main.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-05-15 15:37:00.996042 vsc-mympirun-5.3.1/lib/vsc/mympirun/mpi/
+-rw-r--r--   0 kehoste    (501) staff       (20)     1206 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/mpi/__init__.py
+-rw-r--r--   0 kehoste    (501) staff       (20)    11781 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/mpi/intelmpi.py
+-rw-r--r--   0 kehoste    (501) staff       (20)    37560 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/mpi/mpi.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     4428 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/mpi/mpich.py
+-rw-r--r--   0 kehoste    (501) staff       (20)    11686 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/mpi/openmpi.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     4341 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/mpi/option.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     6419 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/option.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-05-15 15:37:00.996896 vsc-mympirun-5.3.1/lib/vsc/mympirun/pmi/
+-rw-r--r--   0 kehoste    (501) staff       (20)     1206 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/pmi/__init__.py
+-rw-r--r--   0 kehoste    (501) staff       (20)    11724 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/pmi/mpi.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     2970 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/pmi/option.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     1406 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/pmi/pmi.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     6022 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/pmi/sched.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     8415 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/pmi/slurm.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-05-15 15:37:00.997739 vsc-mympirun-5.3.1/lib/vsc/mympirun/rm/
+-rw-r--r--   0 kehoste    (501) staff       (20)     1206 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/rm/__init__.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     2091 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/rm/local.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     3221 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/rm/pbs.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     8653 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/rm/sched.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     1369 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/rm/scoop.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     4011 2023-02-23 15:49:31.000000 vsc-mympirun-5.3.1/lib/vsc/mympirun/rm/slurm.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-05-15 15:37:00.998469 vsc-mympirun-5.3.1/lib/vsc_mympirun.egg-info/
+-rw-r--r--   0 kehoste    (501) staff       (20)    10405 2023-05-15 15:37:00.000000 vsc-mympirun-5.3.1/lib/vsc_mympirun.egg-info/PKG-INFO
+-rw-r--r--   0 kehoste    (501) staff       (20)     1137 2023-05-15 15:37:00.000000 vsc-mympirun-5.3.1/lib/vsc_mympirun.egg-info/SOURCES.txt
+-rw-r--r--   0 kehoste    (501) staff       (20)      645 2023-05-15 15:37:00.000000 vsc-mympirun-5.3.1/lib/vsc_mympirun.egg-info/dependency_links.txt
+-rw-r--r--   0 kehoste    (501) staff       (20)        4 2023-05-15 15:37:00.000000 vsc-mympirun-5.3.1/lib/vsc_mympirun.egg-info/namespace_packages.txt
+-rw-r--r--   0 kehoste    (501) staff       (20)        1 2023-05-15 15:37:00.000000 vsc-mympirun-5.3.1/lib/vsc_mympirun.egg-info/not-zip-safe
+-rw-r--r--   0 kehoste    (501) staff       (20)       40 2023-05-15 15:37:00.000000 vsc-mympirun-5.3.1/lib/vsc_mympirun.egg-info/requires.txt
+-rw-r--r--   0 kehoste    (501) staff       (20)        4 2023-05-15 15:37:00.000000 vsc-mympirun-5.3.1/lib/vsc_mympirun.egg-info/top_level.txt
+-rw-r--r--   0 kehoste    (501) staff       (20)      200 2023-05-15 15:37:00.998945 vsc-mympirun-5.3.1/setup.cfg
+-rw-r--r--   0 kehoste    (501) staff       (20)     8037 2023-05-15 15:37:00.999268 vsc-mympirun-5.3.1/setup.py
```

### Comparing `vsc-mympirun-5.3.0/LICENSE` & `vsc-mympirun-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/PKG-INFO` & `vsc-mympirun-5.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsc-mympirun
-Version: 5.3.0
+Version: 5.3.1
 Summary: `mympirun` is a tool to make it easier for users of HPC clusters to run MPI programs with good performance.
 Home-page: https://github.com/hpcugent/vsc-mympirun
 Author: Stijn De Weirdt;Kenneth Hoste
 Author-email: stijn.deweirdt@ugent.be, kenneth.hoste@ugent.be
 Maintainer: Stijn De Weirdt;Kenneth Hoste
 Maintainer-email: stijn.deweirdt@ugent.be, kenneth.hoste@ugent.be
 License: GPLv2
```

### Comparing `vsc-mympirun-5.3.0/README.md` & `vsc-mympirun-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/bin/mympirun.py` & `vsc-mympirun-5.3.1/bin/mympirun.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/bin/mympisanity.py` & `vsc-mympirun-5.3.1/bin/mympisanity.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/bin/mypmirun.py` & `vsc-mympirun-5.3.1/bin/mypmirun.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/bin/mytaskprolog.py` & `vsc-mympirun-5.3.1/bin/mytaskprolog.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/bin/mytasks.py` & `vsc-mympirun-5.3.1/bin/mytasks.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/bin/pbsssh.sh` & `vsc-mympirun-5.3.1/bin/pbsssh.sh`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/bin/sshsleep.sh` & `vsc-mympirun-5.3.1/bin/sshsleep.sh`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/external_dist_only/shared_setup_dist_only.py` & `vsc-mympirun-5.3.1/external_dist_only/shared_setup_dist_only.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,21 +27,17 @@
 """
 Shared module for vsc software setup
 
 @author: Stijn De Weirdt (Ghent University)
 @author: Andy Georges (Ghent University)
 """
 
-from __future__ import print_function
 import sys
 
-if sys.version_info < (3, 0):
-    import __builtin__
-else:
-    import builtins as __builtin__  # make builtins accessible via same way as in Python 3
+import builtins as __builtin__  # make builtins accessible via same way as in Python 3
 
 import glob
 import hashlib
 import inspect
 import json
 import os
 import shutil
@@ -91,15 +87,16 @@
         'function': None,
         'allowmods': [],
     })
 
 # Keep this for legacy reasons, setuptools didn't used to be a requirement
 has_setuptools = True
 
-# redo log info / warn / error
+# redo log info / warn / error so it shows loglevel in log message
+# distutils log does not support formatters
 # don't do it twice
 if log.Log.__name__ != 'NewLog':
     # make a map between level and names
     log_levels = dict([(getattr(log, x), x) for x in dir(log) if x == x.upper()])
 
     OrigLog = log.Log
 
@@ -165,15 +162,15 @@
 DEFAULT_LIB_DIR = 'lib'
 
 URL_GH_HPCUGENT = 'https://github.com/hpcugent/%(name)s'
 URL_GHUGENT_HPCUGENT = 'https://github.ugent.be/hpcugent/%(name)s'
 
 RELOAD_VSC_MODS = False
 
-VERSION = '0.17.32'
+VERSION = '0.18.2'
 
 log.info('This is (based on) vsc.install.shared_setup %s' % VERSION)
 log.info('(using setuptools version %s located at %s)' % (setuptools.__version__, setuptools.__file__))
 
 # list of non-vsc packages that do not need python- prefix for correct rpm dependencies
 # vsc packages should be handled with clusterbuildrpm
 # dependencies starting with python- are also not re-prefixed
@@ -1467,76 +1464,49 @@
                         new_target[k] = type(v)()
                     new_target[k].update(v)
                 else:
                     new_target[k] = type(v)()
                     new_target[k] += v
 
         tests_requires = new_target.setdefault('tests_require', [])
-        if sys.version_info < (2, 7):
-            # py26 support dropped in 0.8, and the old versions don't detect enough
-            log.info('no prospector support in py26 (or older)')
-            tests_requires = [x for x in tests_requires if 'prospector' not in x]
-        elif sys.version_info < (3, 0):
-            log.info('adding prospector to tests_require')
-            # limit version to avoid pulling in python 3.x only versions
-            tests_requires.append('zipp < 2.0')
-            tests_requires.append('configparser < 5.0')
-            # Python 2.x support was removed in pydocstyle 4.0, so stick to latest release before 4.0
-            tests_requires.append('pydocstyle < 4.0')
-            # fix from https://github.com/PyCQA/prospector/pull/323 required to avoid infinite recursion
-            tests_requires.append('prospector >= 1.1.6.4, < 1.3')
-            # mock 4.x is no longer compatible with Python 2
-            tests_requires.append('mock < 4.0')
-            # isort 5.0 is no longer compatible with Python 2
-            tests_requires.append('isort < 5.0')
-            # pyyaml > 5.4.1 fails for python 2.7
-            tests_requires.append('pyyaml >= 5.4.1, < 6.0')
-            # lazy_object_proxy 1.7.0 no longer compatible with python 2
-            tests_requires.append('lazy_object_proxy < 1.7.0')
-            # requirements-detector 1.0.0 no longer compatible with python 2
-            tests_requires.append('requirements-detector < 1.0.0')
-            # singledispatch 4.0.0 no longer compatible with python 2
-            tests_requires.append('singledispatch < 4.0.0')
-        else:
-            # soft pinning of (transitive) dependencies of prospector
-            # ('~=' means stick to compatible release, https://www.python.org/dev/peps/pep-0440/#compatible-release);
-            # updating these must be done in lockstep, see setup.cfg or pyproject.toml or whatever at:
-            # - https://github.com/PyCQA/pylint/blob/v2.12.2/setup.cfg
-            # - https://github.com/PyCQA/flake8/blob/3.9.2/setup.cfg
-            # - https://github.com/PyCQA/prospector/blob/1.5.3.1/pyproject.toml
-
-            # To figure out requirements of what needs what: grep name_of_tool .eggs.py3/*/*/requires.txt
+        # soft pinning of (transitive) dependencies of prospector
+        # ('~=' means stick to compatible release, https://www.python.org/dev/peps/pep-0440/#compatible-release);
+        # updating these must be done in lockstep, see setup.cfg or pyproject.toml or whatever at:
+        # - https://github.com/PyCQA/pylint/blob/v2.12.2/setup.cfg
+        # - https://github.com/PyCQA/flake8/blob/3.9.2/setup.cfg
+        # - https://github.com/PyCQA/prospector/blob/1.5.3.1/pyproject.toml
+        # To figure out requirements of what needs what: grep name_of_tool .eggs.py3/*/*/requires.txt
+        tests_requires.extend([
+            'mock',
+        ])
+        if sys.version_info < (3, 7):
             tests_requires.extend([
-                'mock',
+                'pyflakes~=2.3.0',
+                'pycodestyle~=2.7.0',
+                'pylint~=2.12.2',
+                'prospector~=1.5.3.1',
+                'flake8~=3.9.2',
+                'pylint-plugin-utils < 0.7',
+                'pylint-django~=2.4.4',
+                # platformdirs >= 2.4.0 requires Python 3.7, use older versions for running tests with Python 3.6
+                'platformdirs < 2.4.0',
+                'typing-extensions < 4.2.0', # higher requires python 3.7
+                'lazy-object-proxy < 1.8.0', # higher requires python 3.7
+                'jsonpickle < 3.0.0', # higher requires python 3.7
+                'importlib-metadata < 5.0.0', # no longer compatible with python 3.7
+                'isort < 5.11.0',
+            ])
+        else:  # tested for fedora37 py3.11
+            tests_requires.extend([
+                'flake8 < 5.0.0',
+                'astroid <= 2.12.0-dev0',
+                'pyflakes < 2.5.0',
+                'pylint~=2.14.4',
+                'prospector~=1.7.7',
             ])
-            if sys.version_info < (3, 7):
-                tests_requires.extend([
-                    'pyflakes~=2.3.0',
-                    'pycodestyle~=2.7.0',
-                    'pylint~=2.12.2',
-                    'prospector~=1.5.3.1',
-                    'flake8~=3.9.2',
-                    'pylint-plugin-utils < 0.7',
-                    'pylint-django~=2.4.4',
-                    # platformdirs >= 2.4.0 requires Python 3.7, use older versions for running tests with Python 3.6
-                    'platformdirs < 2.4.0',
-                    'typing-extensions < 4.2.0', # higher requires python 3.7
-                    'lazy-object-proxy < 1.8.0', # higher requires python 3.7
-                    'jsonpickle < 3.0.0', # higher requires python 3.7
-                    'importlib-metadata < 5.0.0', # no longer compatible with python 3.7
-                    'isort < 5.11.0',
-                ])
-            else:  # tested for fedora37 py3.11
-                tests_requires.extend([
-                    'flake8 < 5.0.0',
-                    'astroid <= 2.12.0-dev0',
-                    'pyflakes < 2.5.0',
-                    'pylint~=2.14.4',
-                    'prospector~=1.7.7',
-                ])
 
         new_target['tests_require'] = tests_requires
 
         if self.private_repo:
             urls = [
                 ('github.com', 'git+https://'),
                 ('github.ugent.be', 'git+ssh://git@'),
@@ -1728,19 +1698,15 @@
     install_requires = [
         # setuptools 42.0 changed easy_install to use pip if it's available,
         # but vsc-install relies on the setuptools' behaviour of ignoring failing dependency installations and
         # just continuing with the next entry in dependency_links
         'setuptools < %s' % MAX_SETUPTOOLS_VERSION,
     ]
 
-    # mock 4.0 only supports Python 3+
-    if sys.version_info < (3, 0):
-        install_requires.append('mock < 4.0')
-    else:
-        install_requires.append('mock')
+    install_requires.append('mock')
 
     PACKAGE = {
         'version': VERSION,
         'author': [sdw, ag, jt],
         'maintainer': [sdw, ag, jt],
         'install_requires': install_requires,
         'setup_requires': [
```

### Comparing `vsc-mympirun-5.3.0/lib/vsc/__init__.py` & `vsc-mympirun-5.3.1/lib/vsc/__init__.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/__init__.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/__init__.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/common.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/common.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/factory.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/factory.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/main.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/main.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/mpi/__init__.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/mpi/__init__.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/mpi/intelmpi.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/mpi/intelmpi.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/mpi/mpi.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/mpi/mpi.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/mpi/mpich.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/mpi/mpich.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/mpi/openmpi.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/mpi/openmpi.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/mpi/option.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/mpi/option.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/option.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/option.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/pmi/__init__.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/pmi/__init__.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/pmi/mpi.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/pmi/mpi.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/pmi/option.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/pmi/option.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/pmi/pmi.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/pmi/pmi.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/pmi/sched.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/pmi/sched.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/pmi/slurm.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/pmi/slurm.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/rm/__init__.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/rm/__init__.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/rm/local.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/rm/local.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/rm/pbs.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/rm/pbs.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/rm/sched.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/rm/sched.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/rm/scoop.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/rm/scoop.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc/mympirun/rm/slurm.py` & `vsc-mympirun-5.3.1/lib/vsc/mympirun/rm/slurm.py`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc_mympirun.egg-info/PKG-INFO` & `vsc-mympirun-5.3.1/lib/vsc_mympirun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsc-mympirun
-Version: 5.3.0
+Version: 5.3.1
 Summary: `mympirun` is a tool to make it easier for users of HPC clusters to run MPI programs with good performance.
 Home-page: https://github.com/hpcugent/vsc-mympirun
 Author: Stijn De Weirdt;Kenneth Hoste
 Author-email: stijn.deweirdt@ugent.be, kenneth.hoste@ugent.be
 Maintainer: Stijn De Weirdt;Kenneth Hoste
 Maintainer-email: stijn.deweirdt@ugent.be, kenneth.hoste@ugent.be
 License: GPLv2
```

### Comparing `vsc-mympirun-5.3.0/lib/vsc_mympirun.egg-info/SOURCES.txt` & `vsc-mympirun-5.3.1/lib/vsc_mympirun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vsc-mympirun-5.3.0/lib/vsc_mympirun.egg-info/dependency_links.txt` & `vsc-mympirun-5.3.1/lib/vsc_mympirun.egg-info/dependency_links.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+git+https://github.com/hpcugent/vsc-install.git#egg=vsc-install-0.18.2
+git+ssh://git@github.ugent.be/hpcugent/vsc-install.git#egg=vsc-install-0.18.2
+git+ssh://git@github.com/hpcugent/vsc-install.git#egg=vsc-install-0.18.2
 git+https://github.com/hpcugent/vsc-install.git#egg=vsc-install-0.15.1
 git+ssh://git@github.ugent.be/hpcugent/vsc-install.git#egg=vsc-install-0.15.1
 git+ssh://git@github.com/hpcugent/vsc-install.git#egg=vsc-install-0.15.1
-git+https://github.com/hpcugent/vsc-install.git#egg=vsc-install-0.17.32
-git+ssh://git@github.ugent.be/hpcugent/vsc-install.git#egg=vsc-install-0.17.32
-git+ssh://git@github.com/hpcugent/vsc-install.git#egg=vsc-install-0.17.32
-git+https://github.com/hpcugent/vsc-base.git#egg=vsc-base-3.0.1
-git+ssh://git@github.ugent.be/hpcugent/vsc-base.git#egg=vsc-base-3.0.1
-git+ssh://git@github.com/hpcugent/vsc-base.git#egg=vsc-base-3.0.1
+git+https://github.com/hpcugent/vsc-base.git#egg=vsc-base-3.5.3
+git+ssh://git@github.ugent.be/hpcugent/vsc-base.git#egg=vsc-base-3.5.3
+git+ssh://git@github.com/hpcugent/vsc-base.git#egg=vsc-base-3.5.3
```

### Comparing `vsc-mympirun-5.3.0/setup.py` & `vsc-mympirun-5.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 """
 Setup for mympirun
 """
 import os
 import sys
 
 # Inserted shared_setup_dist_only
-# Based on shared_setup version 0.17.32
+# Based on shared_setup version 0.18.2
 import os
 import sys
 sys.path.insert(0, os.path.join(os.path.dirname(__file__), 'external_dist_only'))
 
 import shared_setup_dist_only as shared_setup
 from shared_setup_dist_only import vsc_setup, log, sdw, kh
 
@@ -43,22 +43,22 @@
 
 # hardcoded list, to avoid ugly hacks in order to be able to import from vsc.mympirun in setup.py...
 # this list is checked to be synced via a dedicated unit test
 MYMPIRUN_ALIASES = ['ihmpirun', 'impirun', 'm2hmpirun', 'm2mpirun', 'mhmpirun', 'mmpirun', 'myscoop', 'ompirun']
 
 PACKAGE = {
     'install_requires': [
-        'vsc-base >= 3.0.1',
+        'vsc-base >= 3.5.3',
         'vsc-install >= 0.15.1',
         'IPy',
     ],
     'tests_require': [
         'mock',
     ],
-    'version': '5.3.0',
+    'version': '5.3.1',
     'author': [sdw, kh],
     'maintainer': [sdw, kh],
     'zip_safe': False,
 }
 
 
 class mympirun_vsc_install_scripts(vsc_setup.vsc_install_scripts):
```

