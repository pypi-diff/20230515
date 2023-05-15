# Comparing `tmp/lzy-booting-0.1.tar.gz` & `tmp/lzy-booting-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lzy-booting-0.1.tar", last modified: Fri Mar 10 08:47:14 2023, max compression
+gzip compressed data, was "lzy-booting-0.2.tar", last modified: Mon May 15 10:07:49 2023, max compression
```

## Comparing `lzy-booting-0.1.tar` & `lzy-booting-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 08:47:14.187893 lzy-booting-0.1/
--rw-rw-rw-   0        0        0       83 2023-03-10 08:47:14.187893 lzy-booting-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      721 2023-03-10 08:42:16.000000 lzy-booting-0.1/booting.py
-drwxrwxrwx   0        0        0        0 2023-03-10 08:47:14.186900 lzy-booting-0.1/lzy_booting.egg-info/
--rw-rw-rw-   0        0        0       83 2023-03-10 08:47:14.000000 lzy-booting-0.1/lzy_booting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-03-10 08:47:14.000000 lzy-booting-0.1/lzy_booting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 08:47:14.000000 lzy-booting-0.1/lzy_booting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-10 08:47:14.000000 lzy-booting-0.1/lzy_booting.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-10 08:47:14.188889 lzy-booting-0.1/setup.cfg
--rw-rw-rw-   0        0        0      279 2023-03-10 08:47:00.000000 lzy-booting-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:07:49.828049 lzy-booting-0.2/
+-rw-rw-rw-   0        0        0       83 2023-05-15 10:07:49.826479 lzy-booting-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1196 2023-05-15 10:00:55.000000 lzy-booting-0.2/booting.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:07:49.826479 lzy-booting-0.2/lzy_booting.egg-info/
+-rw-rw-rw-   0        0        0       83 2023-05-15 10:07:49.000000 lzy-booting-0.2/lzy_booting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-05-15 10:07:49.000000 lzy-booting-0.2/lzy_booting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 10:07:49.000000 lzy-booting-0.2/lzy_booting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-15 10:07:49.000000 lzy-booting-0.2/lzy_booting.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 10:07:49.828049 lzy-booting-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      211 2023-05-15 10:01:53.000000 lzy-booting-0.2/setup.py
```

