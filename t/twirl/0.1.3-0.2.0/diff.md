# Comparing `tmp/twirl-0.1.3.tar.gz` & `tmp/twirl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twirl-0.1.3.tar", last modified: Mon Mar 21 17:29:35 2022, max compression
+gzip compressed data, was "twirl-0.2.0.tar", max compression
```

## Comparing `twirl-0.1.3.tar` & `twirl-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,7 @@
-drwxr-xr-x   0 lgrcia     (501) staff       (20)        0 2022-03-21 17:29:35.925548 twirl-0.1.3/
--rw-r--r--   0 lgrcia     (501) staff       (20)     1289 2022-03-21 17:29:35.925426 twirl-0.1.3/PKG-INFO
--rw-r--r--   0 lgrcia     (501) staff       (20)      905 2022-01-21 16:05:58.000000 twirl-0.1.3/README.md
--rw-r--r--   0 lgrcia     (501) staff       (20)       38 2022-03-21 17:29:35.925586 twirl-0.1.3/setup.cfg
--rw-r--r--   0 lgrcia     (501) staff       (20)      908 2022-03-21 17:28:58.000000 twirl-0.1.3/setup.py
-drwxr-xr-x   0 lgrcia     (501) staff       (20)        0 2022-03-21 17:29:35.924667 twirl-0.1.3/twirl/
--rw-r--r--   0 lgrcia     (501) staff       (20)     2143 2022-03-21 17:29:13.000000 twirl-0.1.3/twirl/__init__.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     1898 2022-01-21 16:05:58.000000 twirl-0.1.3/twirl/config.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     8504 2022-01-21 16:05:58.000000 twirl-0.1.3/twirl/utils.py
-drwxr-xr-x   0 lgrcia     (501) staff       (20)        0 2022-03-21 17:29:35.925283 twirl-0.1.3/twirl.egg-info/
--rw-r--r--   0 lgrcia     (501) staff       (20)     1289 2022-03-21 17:29:35.000000 twirl-0.1.3/twirl.egg-info/PKG-INFO
--rw-r--r--   0 lgrcia     (501) staff       (20)      235 2022-03-21 17:29:35.000000 twirl-0.1.3/twirl.egg-info/SOURCES.txt
--rw-r--r--   0 lgrcia     (501) staff       (20)        1 2022-03-21 17:29:35.000000 twirl-0.1.3/twirl.egg-info/dependency_links.txt
--rw-r--r--   0 lgrcia     (501) staff       (20)       49 2022-03-21 17:29:35.000000 twirl-0.1.3/twirl.egg-info/requires.txt
--rw-r--r--   0 lgrcia     (501) staff       (20)        6 2022-03-21 17:29:35.000000 twirl-0.1.3/twirl.egg-info/top_level.txt
--rw-r--r--   0 lgrcia     (501) staff       (20)        1 2022-02-16 17:35:29.000000 twirl-0.1.3/twirl.egg-info/zip-safe
+-rw-r--r--   0        0        0     5003 2023-05-15 13:23:39.318920 twirl-0.2.0/README.md
+-rw-r--r--   0        0        0     3077 2023-05-15 13:23:39.326920 twirl-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2940 2023-05-15 13:23:39.326920 twirl-0.2.0/twirl/__init__.py
+-rw-r--r--   0        0        0     2721 2023-05-15 13:23:39.326920 twirl-0.2.0/twirl/geometry.py
+-rw-r--r--   0        0        0     1825 2023-05-15 13:23:39.326920 twirl-0.2.0/twirl/match.py
+-rw-r--r--   0        0        0     2145 2023-05-15 13:23:39.326920 twirl-0.2.0/twirl/quads.py
+-rw-r--r--   0        0        0     5967 1970-01-01 00:00:00.000000 twirl-0.2.0/PKG-INFO
```

