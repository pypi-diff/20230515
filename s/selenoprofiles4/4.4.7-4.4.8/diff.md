# Comparing `tmp/selenoprofiles4-4.4.7.tar.gz` & `tmp/selenoprofiles4-4.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenoprofiles4-4.4.7.tar", last modified: Wed Mar 22 14:51:57 2023, max compression
+gzip compressed data, was "selenoprofiles4-4.4.8.tar", last modified: Mon May 15 12:42:35 2023, max compression
```

## Comparing `selenoprofiles4-4.4.7.tar` & `selenoprofiles4-4.4.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-03-22 14:51:57.082681 selenoprofiles4-4.4.7/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-01-10 21:24:14.000000 selenoprofiles4-4.4.7/LICENSE
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      127 2023-02-09 09:55:59.000000 selenoprofiles4-4.4.7/MANIFEST.in
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1169 2023-03-22 14:51:57.082681 selenoprofiles4-4.4.7/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      673 2023-02-27 17:28:28.000000 selenoprofiles4-4.4.7/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 selenoprofiles4-4.4.7/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      886 2023-03-22 14:51:57.082681 selenoprofiles4-4.4.7/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       94 2023-02-08 17:12:03.000000 selenoprofiles4-4.4.7/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-03-22 14:51:57.070681 selenoprofiles4-4.4.7/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-03-22 14:51:57.074681 selenoprofiles4-4.4.7/src/selenoprofiles4/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   343939 2023-03-09 16:21:01.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/MMlib3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       90 2023-01-10 21:45:21.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-03-22 14:16:52.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/_version.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     4871 2023-02-09 09:55:29.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/blaster_parser.awk
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-03-22 14:51:57.074681 selenoprofiles4-4.4.7/src/selenoprofiles4/exoneratecfg/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     2121 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/exoneratecfg/BLOSUM62sel
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     5719 2023-02-17 09:42:28.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/load_config.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)   489146 2023-03-22 14:48:17.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/selenoprofiles4.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    20560 2023-02-26 22:10:55.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/selenoprofiles_build_profile.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    16099 2023-02-23 10:36:04.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/selenoprofiles_database.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     7039 2023-02-17 12:06:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/selenoprofiles_join_alignments.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    48453 2023-02-24 16:49:37.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/selenoprofiles_tree_drawer.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-03-22 14:51:57.078681 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1767 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/BLOSUM62sel.bla
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc1.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc1.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc10.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc10.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc11.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc11.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc12.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc12.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc13.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc13.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc14.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc14.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc16.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc16.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc2.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc2.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc21.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc21.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc22.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc22.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc23.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc23.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc24.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc24.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc25.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc25.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc26.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc26.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc27.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc27.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc28.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc28.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc29.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc29.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc3.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc3.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc30.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc30.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        0 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc31.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        0 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc31.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc4.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc4.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc5.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc5.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc6.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc6.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc9.sec
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.gc9.std
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      418 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/codon.table.sec
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-03-22 14:51:57.074681 selenoprofiles4-4.4.7/src/selenoprofiles4.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1169 2023-03-22 14:51:57.000000 selenoprofiles4-4.4.7/src/selenoprofiles4.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     3158 2023-03-22 14:51:57.000000 selenoprofiles4-4.4.7/src/selenoprofiles4.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-03-22 14:51:57.000000 selenoprofiles4-4.4.7/src/selenoprofiles4.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       84 2023-03-22 14:51:57.000000 selenoprofiles4-4.4.7/src/selenoprofiles4.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       16 2023-03-22 14:51:57.000000 selenoprofiles4-4.4.7/src/selenoprofiles4.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-05-15 12:42:35.459452 selenoprofiles4-4.4.8/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-01-10 21:24:14.000000 selenoprofiles4-4.4.8/LICENSE
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      127 2023-02-09 09:55:59.000000 selenoprofiles4-4.4.8/MANIFEST.in
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1169 2023-05-15 12:42:35.459452 selenoprofiles4-4.4.8/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      673 2023-02-27 17:28:28.000000 selenoprofiles4-4.4.8/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 selenoprofiles4-4.4.8/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      886 2023-05-15 12:42:35.459452 selenoprofiles4-4.4.8/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       94 2023-02-08 17:12:03.000000 selenoprofiles4-4.4.8/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-05-15 12:42:35.447452 selenoprofiles4-4.4.8/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-05-15 12:42:35.451452 selenoprofiles4-4.4.8/src/selenoprofiles4/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   343939 2023-03-09 16:21:01.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/MMlib3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       90 2023-01-10 21:45:21.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-05-15 12:39:42.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/_version.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     4871 2023-02-09 09:55:29.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/blaster_parser.awk
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-05-15 12:42:35.451452 selenoprofiles4-4.4.8/src/selenoprofiles4/exoneratecfg/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     2121 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/exoneratecfg/BLOSUM62sel
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     5719 2023-02-17 09:42:28.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/load_config.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)   489214 2023-05-15 12:39:06.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/selenoprofiles4.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    20560 2023-02-26 22:10:55.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/selenoprofiles_build_profile.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    16099 2023-02-23 10:36:04.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/selenoprofiles_database.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     7039 2023-02-17 12:06:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/selenoprofiles_join_alignments.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    48453 2023-02-24 16:49:37.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/selenoprofiles_tree_drawer.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-05-15 12:42:35.459452 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1767 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/BLOSUM62sel.bla
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc1.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc1.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc10.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc10.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc11.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc11.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc12.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc12.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc13.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc13.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc14.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc14.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc16.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc16.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc2.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc2.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc21.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc21.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc22.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc22.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc23.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc23.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc24.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc24.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc25.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc25.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc26.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc26.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc27.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc27.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc28.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc28.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc29.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc29.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc3.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc3.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc30.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc30.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        0 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc31.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        0 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc31.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc4.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc4.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc5.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc5.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc6.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc6.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc9.sec
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      419 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.gc9.std
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      418 2023-01-10 21:25:39.000000 selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/codon.table.sec
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-05-15 12:42:35.451452 selenoprofiles4-4.4.8/src/selenoprofiles4.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1169 2023-05-15 12:42:35.000000 selenoprofiles4-4.4.8/src/selenoprofiles4.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     3158 2023-05-15 12:42:35.000000 selenoprofiles4-4.4.8/src/selenoprofiles4.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-05-15 12:42:35.000000 selenoprofiles4-4.4.8/src/selenoprofiles4.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       84 2023-05-15 12:42:35.000000 selenoprofiles4-4.4.8/src/selenoprofiles4.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       16 2023-05-15 12:42:35.000000 selenoprofiles4-4.4.8/src/selenoprofiles4.egg-info/top_level.txt
```

### Comparing `selenoprofiles4-4.4.7/LICENSE` & `selenoprofiles4-4.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `selenoprofiles4-4.4.7/PKG-INFO` & `selenoprofiles4-4.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenoprofiles4
-Version: 4.4.7
+Version: 4.4.8
 Summary: Gene finding pipeline for selenoprotein and selenocysteine machinery
 Home-page: https://github.com/marco-mariotti/selenoprofiles4
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `selenoprofiles4-4.4.7/README.md` & `selenoprofiles4-4.4.8/README.md`

 * *Files identical despite different names*

### Comparing `selenoprofiles4-4.4.7/setup.cfg` & `selenoprofiles4-4.4.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `selenoprofiles4-4.4.7/src/selenoprofiles4/MMlib3.py` & `selenoprofiles4-4.4.8/src/selenoprofiles4/MMlib3.py`

 * *Files identical despite different names*

### Comparing `selenoprofiles4-4.4.7/src/selenoprofiles4/blaster_parser.awk` & `selenoprofiles4-4.4.8/src/selenoprofiles4/blaster_parser.awk`

 * *Files identical despite different names*

### Comparing `selenoprofiles4-4.4.7/src/selenoprofiles4/exoneratecfg/BLOSUM62sel` & `selenoprofiles4-4.4.8/src/selenoprofiles4/exoneratecfg/BLOSUM62sel`

 * *Files identical despite different names*

### Comparing `selenoprofiles4-4.4.7/src/selenoprofiles4/load_config.py` & `selenoprofiles4-4.4.8/src/selenoprofiles4/load_config.py`

 * *Files identical despite different names*

### Comparing `selenoprofiles4-4.4.7/src/selenoprofiles4/selenoprofiles4.py` & `selenoprofiles4-4.4.8/src/selenoprofiles4/selenoprofiles4.py`

 * *Files 0% similar despite different names*

```diff
@@ -7572,15 +7572,15 @@
                                     intron, phase=False
                                 )  # the stop codon maybe right on the intron boundary
 
                                 if b:
                                     introns_index_and_distances_and_direction.append(
                                         [intron_index, -1, "boundary"]
                                     )  # -1 is to ensure it will be first after sorting
-                                elif d:
+                                elif d: #old_p2g.__dict__
                                     introns_index_and_distances_and_direction.append(
                                         [intron_index, d - 1, "downstream"]
                                     )
                                 elif u:
                                     introns_index_and_distances_and_direction.append(
                                         [intron_index, u - 1, "upstream"]
                                     )
@@ -7590,21 +7590,22 @@
                         )  # sorting: first value refers now to closest intron
                         (
                             nearest_intron_index,
                             distance,
                             direction,
                         ) = introns_index_and_distances_and_direction[0]
 
+
                         if distance <= max_codons_removed * 3:
                             n_stop_codons_removed += 1
                             if direction == "downstream":
                                 gene_portion_to_remove = self.subseq(
                                     3 * (pos - n_gaps_in_target) + 1, distance + 3
                                 )
-                                n_aminoacids_to_remove = distance / 3
+                                n_aminoacids_to_remove = distance // 3
                                 n_nucleotides_left_at_intron_boundary = distance % 3
                                 if (
                                     n_nucleotides_left_at_intron_boundary
                                 ):  # in this case there must be another exon downstream which carries the rest of the codon, which we want to remove.
                                     n_aminoacids_to_remove += 1
 
                                     exon_to_remodel = self.exons[nearest_intron_index]
@@ -7640,15 +7641,15 @@
                                         n_gaps += 1
 
                             elif direction == "upstream":
                                 gene_portion_to_remove = self.subseq(
                                     3 * (pos - n_gaps_in_target) + 1 - distance,
                                     distance + 3,
                                 )
-                                n_aminoacids_to_remove = distance / 3
+                                n_aminoacids_to_remove = distance // 3
                                 n_nucleotides_left_at_intron_boundary = distance % 3
                                 if (
                                     n_nucleotides_left_at_intron_boundary
                                 ):  # in this case there must be another exon downstream which carries the rest of the codon, which we want to remove.
                                     n_aminoacids_to_remove += 1
                                     exon_to_remodel = self.exons[
                                         nearest_intron_index - 1
@@ -7668,14 +7669,15 @@
                                     ):  # to avoid bug when we have a single nt exon (which is a prediction bug by itself, but anyway)
                                         self.add_exon(
                                             exon_to_remodel[0], exon_to_remodel[1]
                                         )
 
                                 positions_in_alignment_to_remove = 0
                                 n_gaps = 0  # not counting the positions of the stop
+
                                 while (
                                     positions_in_alignment_to_remove
                                     != n_aminoacids_to_remove + n_gaps
                                 ):
                                     positions_in_alignment_to_remove += 1
                                     if (
                                         self.alignment.seq_of("t")[
@@ -7710,14 +7712,15 @@
                                         : pos - positions_in_alignment_to_remove
                                     ]
                                     + "-" * (1 + positions_in_alignment_to_remove)
                                     + a.alignment.seq_of("t")[pos + 1 :],
                                 )
                             self.__dict__ = a.__dict__
                             self.reset_derived_data()
+
                             if not silent:
                                 write(
                                     (
                                         self.profile.name
                                         + "."
                                         + self.id
                                         + " ["
@@ -7733,26 +7736,27 @@
                                 )
 
                             self.alignment.remove_useless_gaps()
                             self.clean_unaligned_tails()
                             return self.clean_inframe_stop_codons(
                                 max_codons_removed=max_codons_removed, silent=silent
                             )  # instead of continuing the cycle through the positions, since it is difficult to take into account the reduction of the alignment, we just rerun the same function to see if it is necessary to cut off more codons from the prediction
-            except:
+            except Exception as err:
                 self.__dict__ = old_p2g.__dict__
                 printerr(
                     "clean_inframe_stop_codons WARNING can't process "
                     + self.profile.name
                     + "."
                     + self.id
                     + " ("
                     + self.prediction_program()
                     + ") : skipping !",
                     1,
                 )
+                #raise err
                 # if opt['debug']: raise
 
     def clean_unaligned_tails(self):
         """This function checks if there are unaligned portion of query or target at the N or C terminal and clean the prediction by removing them. """
         removed_something = False
         index = 0  # end of n-.terminal tail of unaliged query
         while (
@@ -10047,15 +10051,15 @@
 
 def bSecisearch(p2g, silent=False, full=False):
     """ Performs a complete bsecisearch searche with bseblastian (crash if not installed). Parse secis and restore their coordinates cosindering their parent gene so that they are absolute. Add the secis to the .features list of the p2g object. If silent!=True, it prints a message for every bSECIS found.    """
     # cutting 3' UTR
     cds_seq = p2g.cds()
     prot_seq = p2g.protein()
     sec_ugas = []  # pos codon based, 0 based
-    for codon_index in range(len(cds_seq) / 3):
+    for codon_index in range(len(cds_seq) // 3):
         if (
             prot_seq[codon_index] == "U"
         ):  # and cds_seq[codon_index*3:codon_index*3+3]   =='TGA'
             sec_ugas.append(codon_index)
     if sec_ugas:
         ### cutting from 5 nts before the first uga, to 100 nts after the last one  (generally there's only one)
         pos_start_subsequence = sec_ugas[0] * 3 + 1 - 5  ## 1 based, nt based
```

### Comparing `selenoprofiles4-4.4.7/src/selenoprofiles4/selenoprofiles_build_profile.py` & `selenoprofiles4-4.4.8/src/selenoprofiles4/selenoprofiles_build_profile.py`

 * *Files identical despite different names*

### Comparing `selenoprofiles4-4.4.7/src/selenoprofiles4/selenoprofiles_database.py` & `selenoprofiles4-4.4.8/src/selenoprofiles4/selenoprofiles_database.py`

 * *Files identical despite different names*

### Comparing `selenoprofiles4-4.4.7/src/selenoprofiles4/selenoprofiles_join_alignments.py` & `selenoprofiles4-4.4.8/src/selenoprofiles4/selenoprofiles_join_alignments.py`

 * *Files identical despite different names*

### Comparing `selenoprofiles4-4.4.7/src/selenoprofiles4/selenoprofiles_tree_drawer.py` & `selenoprofiles4-4.4.8/src/selenoprofiles4/selenoprofiles_tree_drawer.py`

 * *Files identical despite different names*

### Comparing `selenoprofiles4-4.4.7/src/selenoprofiles4/wisecfg/BLOSUM62sel.bla` & `selenoprofiles4-4.4.8/src/selenoprofiles4/wisecfg/BLOSUM62sel.bla`

 * *Files identical despite different names*

### Comparing `selenoprofiles4-4.4.7/src/selenoprofiles4.egg-info/PKG-INFO` & `selenoprofiles4-4.4.8/src/selenoprofiles4.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenoprofiles4
-Version: 4.4.7
+Version: 4.4.8
 Summary: Gene finding pipeline for selenoprotein and selenocysteine machinery
 Home-page: https://github.com/marco-mariotti/selenoprofiles4
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `selenoprofiles4-4.4.7/src/selenoprofiles4.egg-info/SOURCES.txt` & `selenoprofiles4-4.4.8/src/selenoprofiles4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

