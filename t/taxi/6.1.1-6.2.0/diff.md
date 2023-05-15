# Comparing `tmp/taxi-6.1.1.tar.gz` & `tmp/taxi-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taxi-6.1.1.tar", last modified: Tue Sep 21 19:57:15 2021, max compression
+gzip compressed data, was "taxi-6.2.0.tar", last modified: Mon May 15 09:34:50 2023, max compression
```

## Comparing `taxi-6.1.1.tar` & `taxi-6.2.0.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxr-xr-x   0 sephi     (1000) users      (100)        0 2021-09-21 19:57:15.866049 taxi-6.1.1/
--rw-r--r--   0 sephi     (1000) users      (100)      497 2017-11-27 10:47:51.000000 taxi-6.1.1/LICENSE
--rw-r--r--   0 sephi     (1000) users      (100)       17 2018-08-04 17:18:28.000000 taxi-6.1.1/MANIFEST.in
--rw-r--r--   0 sephi     (1000) users      (100)     3345 2021-09-21 19:57:15.866049 taxi-6.1.1/PKG-INFO
--rw-r--r--   0 sephi     (1000) users      (100)     2247 2021-05-25 13:06:12.000000 taxi-6.1.1/README.rst
--rw-r--r--   0 sephi     (1000) users      (100)      206 2021-09-21 19:57:15.866049 taxi-6.1.1/setup.cfg
--rwxr-xr-x   0 sephi     (1000) users      (100)     1220 2021-05-25 13:02:27.000000 taxi-6.1.1/setup.py
-drwxr-xr-x   0 sephi     (1000) users      (100)        0 2021-09-21 19:57:15.858049 taxi-6.1.1/taxi/
--rw-r--r--   0 sephi     (1000) users      (100)       22 2021-09-21 19:57:13.000000 taxi-6.1.1/taxi/__init__.py
--rw-r--r--   0 sephi     (1000) users      (100)     3965 2020-07-04 18:27:23.000000 taxi-6.1.1/taxi/aliases.py
-drwxr-xr-x   0 sephi     (1000) users      (100)        0 2021-09-21 19:57:15.859049 taxi-6.1.1/taxi/backends/
--rw-r--r--   0 sephi     (1000) users      (100)     2885 2019-12-27 16:53:18.000000 taxi-6.1.1/taxi/backends/__init__.py
--rw-r--r--   0 sephi     (1000) users      (100)      202 2019-12-27 16:53:18.000000 taxi-6.1.1/taxi/backends/dummy.py
-drwxr-xr-x   0 sephi     (1000) users      (100)        0 2021-09-21 19:57:15.862049 taxi-6.1.1/taxi/commands/
--rw-r--r--   0 sephi     (1000) users      (100)      154 2019-12-27 16:53:18.000000 taxi-6.1.1/taxi/commands/__init__.py
--rw-r--r--   0 sephi     (1000) users      (100)     4232 2020-06-23 14:42:39.000000 taxi-6.1.1/taxi/commands/alias.py
--rw-r--r--   0 sephi     (1000) users      (100)     1055 2019-12-27 16:53:18.000000 taxi-6.1.1/taxi/commands/autofill.py
--rw-r--r--   0 sephi     (1000) users      (100)    10770 2021-09-06 19:46:11.000000 taxi-6.1.1/taxi/commands/base.py
--rw-r--r--   0 sephi     (1000) users      (100)     1508 2020-08-06 06:42:38.000000 taxi-6.1.1/taxi/commands/clean_aliases.py
--rw-r--r--   0 sephi     (1000) users      (100)     4481 2020-08-06 06:42:38.000000 taxi-6.1.1/taxi/commands/commit.py
--rw-r--r--   0 sephi     (1000) users      (100)      190 2020-08-06 06:42:38.000000 taxi-6.1.1/taxi/commands/config.py
--rw-r--r--   0 sephi     (1000) users      (100)     2158 2019-12-27 16:53:18.000000 taxi-6.1.1/taxi/commands/current.py
--rw-r--r--   0 sephi     (1000) users      (100)     2809 2020-08-06 06:42:38.000000 taxi-6.1.1/taxi/commands/edit.py
--rw-r--r--   0 sephi     (1000) users      (100)     4937 2021-03-08 07:59:00.000000 taxi-6.1.1/taxi/commands/plugin.py
--rw-r--r--   0 sephi     (1000) users      (100)     3747 2020-08-06 06:42:38.000000 taxi-6.1.1/taxi/commands/project.py
--rw-r--r--   0 sephi     (1000) users      (100)     1910 2020-08-06 06:42:38.000000 taxi-6.1.1/taxi/commands/show.py
--rwxr-xr-x   0 sephi     (1000) users      (100)     1692 2020-08-06 06:42:38.000000 taxi-6.1.1/taxi/commands/start.py
--rw-r--r--   0 sephi     (1000) users      (100)      990 2020-08-06 06:42:38.000000 taxi-6.1.1/taxi/commands/status.py
--rw-r--r--   0 sephi     (1000) users      (100)     1248 2020-08-06 06:42:38.000000 taxi-6.1.1/taxi/commands/stop.py
--rw-r--r--   0 sephi     (1000) users      (100)      882 2019-12-27 16:53:18.000000 taxi-6.1.1/taxi/commands/types.py
--rw-r--r--   0 sephi     (1000) users      (100)     1716 2020-08-06 06:42:38.000000 taxi-6.1.1/taxi/commands/update.py
-drwxr-xr-x   0 sephi     (1000) users      (100)        0 2021-09-21 19:57:15.863049 taxi-6.1.1/taxi/etc/
--rw-r--r--   0 sephi     (1000) users      (100)     2186 2020-08-06 06:42:38.000000 taxi-6.1.1/taxi/etc/taxirc.sample
--rw-r--r--   0 sephi     (1000) users      (100)     1019 2020-08-18 06:22:45.000000 taxi-6.1.1/taxi/exceptions.py
--rw-r--r--   0 sephi     (1000) users      (100)     4487 2021-02-15 10:44:34.000000 taxi-6.1.1/taxi/plugins.py
--rw-r--r--   0 sephi     (1000) users      (100)     8813 2020-08-06 06:42:38.000000 taxi-6.1.1/taxi/projects.py
--rwxr-xr-x   0 sephi     (1000) users      (100)     6770 2020-08-06 06:42:38.000000 taxi-6.1.1/taxi/settings.py
-drwxr-xr-x   0 sephi     (1000) users      (100)        0 2021-09-21 19:57:15.864049 taxi-6.1.1/taxi/timesheet/
--rw-r--r--   0 sephi     (1000) users      (100)      229 2017-11-27 10:47:51.000000 taxi-6.1.1/taxi/timesheet/__init__.py
--rw-r--r--   0 sephi     (1000) users      (100)    21292 2021-08-17 15:52:56.000000 taxi-6.1.1/taxi/timesheet/entry.py
--rw-r--r--   0 sephi     (1000) users      (100)     1095 2017-11-27 10:47:51.000000 taxi-6.1.1/taxi/timesheet/flags.py
--rw-r--r--   0 sephi     (1000) users      (100)      687 2019-12-27 16:53:18.000000 taxi-6.1.1/taxi/timesheet/lines.py
--rw-r--r--   0 sephi     (1000) users      (100)    15725 2021-08-17 17:53:05.000000 taxi-6.1.1/taxi/timesheet/parser.py
--rw-r--r--   0 sephi     (1000) users      (100)    14613 2021-09-21 15:36:07.000000 taxi-6.1.1/taxi/timesheet/timesheet.py
--rw-r--r--   0 sephi     (1000) users      (100)     1526 2019-12-27 16:53:18.000000 taxi-6.1.1/taxi/timesheet/utils.py
-drwxr-xr-x   0 sephi     (1000) users      (100)        0 2021-09-21 19:57:15.864049 taxi-6.1.1/taxi/ui/
--rw-r--r--   0 sephi     (1000) users      (100)    17475 2020-08-06 06:42:38.000000 taxi-6.1.1/taxi/ui/__init__.py
--rw-r--r--   0 sephi     (1000) users      (100)       53 2019-12-27 16:53:18.000000 taxi-6.1.1/taxi/ui/tty.py
-drwxr-xr-x   0 sephi     (1000) users      (100)        0 2021-09-21 19:57:15.866049 taxi-6.1.1/taxi/utils/
--rw-r--r--   0 sephi     (1000) users      (100)        0 2017-11-27 10:47:51.000000 taxi-6.1.1/taxi/utils/__init__.py
--rw-r--r--   0 sephi     (1000) users      (100)     1820 2019-12-27 16:53:18.000000 taxi-6.1.1/taxi/utils/date.py
--rw-r--r--   0 sephi     (1000) users      (100)      150 2020-05-25 05:36:12.000000 taxi-6.1.1/taxi/utils/file.py
--rw-r--r--   0 sephi     (1000) users      (100)     1735 2019-12-27 16:53:18.000000 taxi-6.1.1/taxi/utils/structures.py
--rw-r--r--   0 sephi     (1000) users      (100)      797 2019-12-27 16:53:18.000000 taxi-6.1.1/taxi/utils/terminal.py
-drwxr-xr-x   0 sephi     (1000) users      (100)        0 2021-09-21 19:57:15.859049 taxi-6.1.1/taxi.egg-info/
--rwxr-xr-x   0 sephi     (1000) users      (100)     3345 2021-09-21 19:57:15.000000 taxi-6.1.1/taxi.egg-info/PKG-INFO
--rwxr-xr-x   0 sephi     (1000) users      (100)     1146 2021-09-21 19:57:15.000000 taxi-6.1.1/taxi.egg-info/SOURCES.txt
--rwxr-xr-x   0 sephi     (1000) users      (100)        1 2021-09-21 19:57:15.000000 taxi-6.1.1/taxi.egg-info/dependency_links.txt
--rwxr-xr-x   0 sephi     (1000) users      (100)      107 2021-09-21 19:57:15.000000 taxi-6.1.1/taxi.egg-info/entry_points.txt
--rwxr-xr-x   0 sephi     (1000) users      (100)       47 2017-10-31 09:04:20.000000 taxi-6.1.1/taxi.egg-info/pbr.json
--rwxr-xr-x   0 sephi     (1000) users      (100)       26 2021-09-21 19:57:15.000000 taxi-6.1.1/taxi.egg-info/requires.txt
--rwxr-xr-x   0 sephi     (1000) users      (100)        5 2021-09-21 19:57:15.000000 taxi-6.1.1/taxi.egg-info/top_level.txt
+drwxr-xr-x   0 sephi     (1000) users      (100)        0 2023-05-15 09:34:50.074943 taxi-6.2.0/
+-rw-r--r--   0 sephi     (1000) users      (100)      497 2017-11-27 10:47:51.000000 taxi-6.2.0/LICENSE
+-rw-r--r--   0 sephi     (1000) users      (100)       17 2018-08-04 17:18:28.000000 taxi-6.2.0/MANIFEST.in
+-rw-r--r--   0 sephi     (1000) users      (100)     2832 2023-05-15 09:34:50.074943 taxi-6.2.0/PKG-INFO
+-rw-r--r--   0 sephi     (1000) users      (100)     2247 2022-08-04 08:30:15.000000 taxi-6.2.0/README.rst
+-rw-r--r--   0 sephi     (1000) users      (100)      206 2023-05-15 09:34:50.075943 taxi-6.2.0/setup.cfg
+-rwxr-xr-x   0 sephi     (1000) users      (100)     1174 2023-03-07 12:23:52.000000 taxi-6.2.0/setup.py
+drwxr-xr-x   0 sephi     (1000) users      (100)        0 2023-05-15 09:34:50.065943 taxi-6.2.0/taxi/
+-rw-r--r--   0 sephi     (1000) users      (100)       22 2023-05-15 09:34:47.000000 taxi-6.2.0/taxi/__init__.py
+-rw-r--r--   0 sephi     (1000) users      (100)     3965 2020-07-04 18:27:23.000000 taxi-6.2.0/taxi/aliases.py
+drwxr-xr-x   0 sephi     (1000) users      (100)        0 2023-05-15 09:34:50.066943 taxi-6.2.0/taxi/backends/
+-rw-r--r--   0 sephi     (1000) users      (100)     2885 2019-12-27 16:53:18.000000 taxi-6.2.0/taxi/backends/__init__.py
+-rw-r--r--   0 sephi     (1000) users      (100)      202 2019-12-27 16:53:18.000000 taxi-6.2.0/taxi/backends/dummy.py
+drwxr-xr-x   0 sephi     (1000) users      (100)        0 2023-05-15 09:34:50.070943 taxi-6.2.0/taxi/commands/
+-rw-r--r--   0 sephi     (1000) users      (100)      154 2019-12-27 16:53:18.000000 taxi-6.2.0/taxi/commands/__init__.py
+-rw-r--r--   0 sephi     (1000) users      (100)     4393 2023-05-15 06:59:00.000000 taxi-6.2.0/taxi/commands/alias.py
+-rw-r--r--   0 sephi     (1000) users      (100)     1055 2019-12-27 16:53:18.000000 taxi-6.2.0/taxi/commands/autofill.py
+-rw-r--r--   0 sephi     (1000) users      (100)    10770 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/commands/base.py
+-rw-r--r--   0 sephi     (1000) users      (100)     1508 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/commands/clean_aliases.py
+-rw-r--r--   0 sephi     (1000) users      (100)     4481 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/commands/commit.py
+-rw-r--r--   0 sephi     (1000) users      (100)      190 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/commands/config.py
+-rw-r--r--   0 sephi     (1000) users      (100)     2158 2019-12-27 16:53:18.000000 taxi-6.2.0/taxi/commands/current.py
+-rw-r--r--   0 sephi     (1000) users      (100)     2809 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/commands/edit.py
+-rw-r--r--   0 sephi     (1000) users      (100)     4940 2022-08-04 08:39:31.000000 taxi-6.2.0/taxi/commands/plugin.py
+-rw-r--r--   0 sephi     (1000) users      (100)     3747 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/commands/project.py
+-rw-r--r--   0 sephi     (1000) users      (100)     1910 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/commands/show.py
+-rwxr-xr-x   0 sephi     (1000) users      (100)     1692 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/commands/start.py
+-rw-r--r--   0 sephi     (1000) users      (100)      990 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/commands/status.py
+-rw-r--r--   0 sephi     (1000) users      (100)     1248 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/commands/stop.py
+-rw-r--r--   0 sephi     (1000) users      (100)      882 2019-12-27 16:53:18.000000 taxi-6.2.0/taxi/commands/types.py
+-rw-r--r--   0 sephi     (1000) users      (100)     1716 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/commands/update.py
+drwxr-xr-x   0 sephi     (1000) users      (100)        0 2023-05-15 09:34:50.071943 taxi-6.2.0/taxi/etc/
+-rw-r--r--   0 sephi     (1000) users      (100)     2186 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/etc/taxirc.sample
+-rw-r--r--   0 sephi     (1000) users      (100)     1019 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/exceptions.py
+-rw-r--r--   0 sephi     (1000) users      (100)     4487 2021-02-15 10:44:34.000000 taxi-6.2.0/taxi/plugins.py
+-rw-r--r--   0 sephi     (1000) users      (100)     8967 2023-05-15 06:59:00.000000 taxi-6.2.0/taxi/projects.py
+-rwxr-xr-x   0 sephi     (1000) users      (100)     6770 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/settings.py
+drwxr-xr-x   0 sephi     (1000) users      (100)        0 2023-05-15 09:34:50.073943 taxi-6.2.0/taxi/timesheet/
+-rw-r--r--   0 sephi     (1000) users      (100)      229 2017-11-27 10:47:51.000000 taxi-6.2.0/taxi/timesheet/__init__.py
+-rw-r--r--   0 sephi     (1000) users      (100)    21292 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/timesheet/entry.py
+-rw-r--r--   0 sephi     (1000) users      (100)     1095 2017-11-27 10:47:51.000000 taxi-6.2.0/taxi/timesheet/flags.py
+-rw-r--r--   0 sephi     (1000) users      (100)      687 2019-12-27 16:53:18.000000 taxi-6.2.0/taxi/timesheet/lines.py
+-rw-r--r--   0 sephi     (1000) users      (100)    15725 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/timesheet/parser.py
+-rw-r--r--   0 sephi     (1000) users      (100)    14613 2022-08-04 08:30:15.000000 taxi-6.2.0/taxi/timesheet/timesheet.py
+-rw-r--r--   0 sephi     (1000) users      (100)     1526 2019-12-27 16:53:18.000000 taxi-6.2.0/taxi/timesheet/utils.py
+drwxr-xr-x   0 sephi     (1000) users      (100)        0 2023-05-15 09:34:50.073943 taxi-6.2.0/taxi/ui/
+-rw-r--r--   0 sephi     (1000) users      (100)    17621 2023-05-15 06:59:00.000000 taxi-6.2.0/taxi/ui/__init__.py
+-rw-r--r--   0 sephi     (1000) users      (100)       53 2019-12-27 16:53:18.000000 taxi-6.2.0/taxi/ui/tty.py
+drwxr-xr-x   0 sephi     (1000) users      (100)        0 2023-05-15 09:34:50.074943 taxi-6.2.0/taxi/utils/
+-rw-r--r--   0 sephi     (1000) users      (100)        0 2017-11-27 10:47:51.000000 taxi-6.2.0/taxi/utils/__init__.py
+-rw-r--r--   0 sephi     (1000) users      (100)     1820 2019-12-27 16:53:18.000000 taxi-6.2.0/taxi/utils/date.py
+-rw-r--r--   0 sephi     (1000) users      (100)      150 2020-05-25 05:36:12.000000 taxi-6.2.0/taxi/utils/file.py
+-rw-r--r--   0 sephi     (1000) users      (100)     1735 2019-12-27 16:53:18.000000 taxi-6.2.0/taxi/utils/structures.py
+-rw-r--r--   0 sephi     (1000) users      (100)      797 2019-12-27 16:53:18.000000 taxi-6.2.0/taxi/utils/terminal.py
+drwxr-xr-x   0 sephi     (1000) users      (100)        0 2023-05-15 09:34:50.066943 taxi-6.2.0/taxi.egg-info/
+-rw-r--r--   0 sephi     (1000) users      (100)     2832 2023-05-15 09:34:50.000000 taxi-6.2.0/taxi.egg-info/PKG-INFO
+-rw-r--r--   0 sephi     (1000) users      (100)     1123 2023-05-15 09:34:50.000000 taxi-6.2.0/taxi.egg-info/SOURCES.txt
+-rw-r--r--   0 sephi     (1000) users      (100)        1 2023-05-15 09:34:50.000000 taxi-6.2.0/taxi.egg-info/dependency_links.txt
+-rw-r--r--   0 sephi     (1000) users      (100)      106 2023-05-15 09:34:50.000000 taxi-6.2.0/taxi.egg-info/entry_points.txt
+-rw-r--r--   0 sephi     (1000) users      (100)       26 2023-05-15 09:34:50.000000 taxi-6.2.0/taxi.egg-info/requires.txt
+-rw-r--r--   0 sephi     (1000) users      (100)        5 2023-05-15 09:34:50.000000 taxi-6.2.0/taxi.egg-info/top_level.txt
```

### Comparing `taxi-6.1.1/PKG-INFO` & `taxi-6.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,75 @@
 Metadata-Version: 2.1
 Name: taxi
-Version: 6.1.1
+Version: 6.2.0
 Summary: Taxi: timesheeting made easy
 Home-page: https://github.com/liip/taxi
 Author: Sylvain Fankhauser
 Author-email: sylvain.fankhauser@liip.ch
 License: wtfpl
-Description: .. image:: https://raw.githubusercontent.com/sephii/taxi/main/doc/images/taxi.png
-        
-        What is Taxi ?
-        ==============
-        
-        Taxi is a timesheeting tool that focuses on simplicity to help you write your
-        timesheets without wasting time. All you'll do is edit a text file and write
-        down what you've worked on and how long, like so::
-        
-            23/01/2014
-        
-            pingpong 09:00-10:00 Play ping-pong
-            infra         -11:00 Repair coffee machine
-        
-        You can then get a summary of your timesheet::
-        
-            Staging changes :
-        
-            # Thursday 23 january #
-            pingpong (123/456)             1.00  Play ping-pong
-            infra (123/42)                 1.00  Repair coffee machine
-                                           2.00
-        
-            Total                          2.00
-        
-            Use `taxi ci` to commit staging changes to the server
-        
-        Through the use of backends, Taxi allows you to push your timesheets to
-        different systems.
-        
-        Getting started
-        ===============
-        
-        Refer to the `"Installation" section
-        <https://taxi-timesheets.readthedocs.io/en/main/userguide.html#installation>`_
-        in the docs.
-        
-        .. _supported_backends:
-        
-        Supported backends
-        ==================
-        
-        * `zebra <https://github.com/sephii/taxi-zebra>`__ : Liip's zebra backend
-        * `tempo <https://github.com/alexandreblin/taxi-tempo>`__ : Atlassian JIRA's `Tempo Timesheets <https://tempo.io>`__ backend
-        * `tipee <https://github.com/alexandreblin/taxi-tipee>`__ : Gammadia's `tipee <https://tipee.ch>`__ backend
-        * `bexio <https://github.com/alexandreblin/taxi-bexio>`__ : Bexio `Timesheets <https://bexio.com>`__ backend
-        * `multi <https://github.com/alexandreblin/taxi-multi>`__ : a special backend to push entries over multiple other backends
-        * `clockify <https://github.com/sephii/taxi-clockify>`__ : backend for the free timesheeting tool `clockify.me <https://clockify.me/>`_
-        
-        Contrib packages
-        ================
-        
-        These resources, not part of Taxi core, provide an enhanced experience for certain use cases.
-        
-        * `Cabdriver <https://github.com/metaodi/cabdriver>`_ (generate taxi entries based on Google Calendar, Slack, etc)
-        * `Syntax highlighting for VSCode <https://marketplace.visualstudio.com/items?itemName=LeBen.taxi-syntax-highlighting>`_
-        * `Vim plugin <https://github.com/schtibe/taxi.vim>`_ (features syntax highlighting, auto completion)
-        
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+.. image:: https://raw.githubusercontent.com/sephii/taxi/main/doc/images/taxi.png
+
+What is Taxi ?
+==============
+
+Taxi is a timesheeting tool that focuses on simplicity to help you write your
+timesheets without wasting time. All you'll do is edit a text file and write
+down what you've worked on and how long, like so::
+
+    23/01/2014
+
+    pingpong 09:00-10:00 Play ping-pong
+    infra         -11:00 Repair coffee machine
+
+You can then get a summary of your timesheet::
+
+    Staging changes :
+
+    # Thursday 23 january #
+    pingpong (123/456)             1.00  Play ping-pong
+    infra (123/42)                 1.00  Repair coffee machine
+                                   2.00
+
+    Total                          2.00
+
+    Use `taxi ci` to commit staging changes to the server
+
+Through the use of backends, Taxi allows you to push your timesheets to
+different systems.
+
+Getting started
+===============
+
+Refer to the `"Installation" section
+<https://taxi-timesheets.readthedocs.io/en/main/userguide.html#installation>`_
+in the docs.
+
+.. _supported_backends:
+
+Supported backends
+==================
+
+* `zebra <https://github.com/sephii/taxi-zebra>`__ : Liip's zebra backend
+* `tempo <https://github.com/alexandreblin/taxi-tempo>`__ : Atlassian JIRA's `Tempo Timesheets <https://tempo.io>`__ backend
+* `tipee <https://github.com/alexandreblin/taxi-tipee>`__ : Gammadia's `tipee <https://tipee.ch>`__ backend
+* `bexio <https://github.com/alexandreblin/taxi-bexio>`__ : Bexio `Timesheets <https://bexio.com>`__ backend
+* `multi <https://github.com/alexandreblin/taxi-multi>`__ : a special backend to push entries over multiple other backends
+* `clockify <https://github.com/sephii/taxi-clockify>`__ : backend for the free timesheeting tool `clockify.me <https://clockify.me/>`_
+
+Contrib packages
+================
+
+These resources, not part of Taxi core, provide an enhanced experience for certain use cases.
+
+* `Cabdriver <https://github.com/metaodi/cabdriver>`_ (generate taxi entries based on Google Calendar, Slack, etc)
+* `Syntax highlighting for VSCode <https://marketplace.visualstudio.com/items?itemName=LeBen.taxi-syntax-highlighting>`_
+* `Vim plugin <https://github.com/schtibe/taxi.vim>`_ (features syntax highlighting, auto completion)
```

### Comparing `taxi-6.1.1/README.rst` & `taxi-6.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/setup.py` & `taxi-6.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,22 +21,21 @@
     url='https://github.com/liip/taxi',
     install_requires=install_requires,
     license='wtfpl',
     include_package_data=False,
     package_data={
         'taxi': ['etc/*']
     },
-    python_requires=">=3.5",
+    python_requires='>=3.8',
     entry_points={
         'taxi.backends': 'dummy = taxi.backends.dummy:DummyBackend',
         'console_scripts': 'taxi = taxi.commands.base:cli'
     },
     classifiers=[
         'Environment :: Console',
         'Development Status :: 5 - Production/Stable',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-    ]
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+    ],
 )
```

### Comparing `taxi-6.1.1/taxi/aliases.py` & `taxi-6.2.0/taxi/aliases.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/backends/__init__.py` & `taxi-6.2.0/taxi/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/commands/alias.py` & `taxi-6.2.0/taxi/commands/alias.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 @click.pass_context
 def list_(ctx, search_string, reverse, backend, used, inactive):
     """
     List configured aliases. Aliases in red belong to inactive projects and trying to push entries to these aliases
     will probably result in an error.
     """
     if not reverse:
-        list_aliases(ctx, search_string, backend, used, inactive=inactive)
+        list_aliases(ctx, search_string, backend, used, include_inactive=inactive)
     else:
         show_mapping(ctx, search_string, backend)
 
 
 @alias.command()
 @click.argument('alias', required=True)
 @click.argument('mapping', required=True)
@@ -98,15 +98,15 @@
         ctx.obj['view'].mapping_detail(
             (alias, m),
             ctx.obj['projects_db'].get(m.mapping[0], m.backend)
             if m.mapping is not None else None
         )
 
 
-def list_aliases(ctx, search, backend, used, inactive):
+def list_aliases(ctx, search, backend, used, include_inactive: bool):
     aliases_mappings = aliases_database.filter_from_alias(search, backend)
 
     if used:
         timesheet_collection = get_timesheet_collection_for_context(ctx)
         aliases_count = timesheet_collection.get_popular_aliases(limit=None)
         used_aliases = set(alias for alias, count in aliases_count)
 
@@ -115,12 +115,14 @@
         )
 
     for alias, m in aliases_mappings.items():
         if m.mapping is not None:
             project, activity = ctx.obj['projects_db'].mapping_to_project(m)
         else:
             project = None
+            activity = None
 
-        if not inactive and (not project or not project.is_active()):
-            continue
+        project_is_active = project and project.is_active()
+        activity_is_active = activity and activity.is_active()
 
-        ctx.obj['view'].alias_detail((alias, m), project)
+        if include_inactive or (project_is_active and activity_is_active):
+            ctx.obj['view'].alias_detail((alias, m), project)
```

### Comparing `taxi-6.1.1/taxi/commands/autofill.py` & `taxi-6.2.0/taxi/commands/autofill.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/commands/base.py` & `taxi-6.2.0/taxi/commands/base.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/commands/clean_aliases.py` & `taxi-6.2.0/taxi/commands/clean_aliases.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/commands/commit.py` & `taxi-6.2.0/taxi/commands/commit.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/commands/current.py` & `taxi-6.2.0/taxi/commands/current.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/commands/edit.py` & `taxi-6.2.0/taxi/commands/edit.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/commands/plugin.py` & `taxi-6.2.0/taxi/commands/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 
 def ensure_inside_venv(ctx):
     """
     Display an error and exit if the program is not run from inside a
     virtualenv.
     """
-    if not hasattr(sys, 'real_prefix'):
+    if sys.base_prefix == sys.exec_prefix:
         echo_error("You're not supposed to use the plugin commands with a "
                    "system-wide install of Taxi. Please install the specific "
                    "packages for your operating system instead.")
         sys.exit(2)
 
 
 @cli.group()
```

### Comparing `taxi-6.1.1/taxi/commands/project.py` & `taxi-6.2.0/taxi/commands/project.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/commands/show.py` & `taxi-6.2.0/taxi/commands/show.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/commands/start.py` & `taxi-6.2.0/taxi/commands/start.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/commands/status.py` & `taxi-6.2.0/taxi/commands/status.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/commands/stop.py` & `taxi-6.2.0/taxi/commands/stop.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/commands/types.py` & `taxi-6.2.0/taxi/commands/types.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/commands/update.py` & `taxi-6.2.0/taxi/commands/update.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/etc/taxirc.sample` & `taxi-6.2.0/taxi/etc/taxirc.sample`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/exceptions.py` & `taxi-6.2.0/taxi/exceptions.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/plugins.py` & `taxi-6.2.0/taxi/plugins.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/projects.py` & `taxi-6.2.0/taxi/projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,17 +114,21 @@
         Converts a (project, activity) tuple to a string in the format xxx/yyy, or a (project, activity, role) tuple in
         the format xxx/yyy/zzz.
         """
         return '/'.join(str(part) for part in t if part is not None)
 
 
 class Activity:
-    def __init__(self, id, name):
+    def __init__(self, id: str, name: str, active: bool = True):
         self.id = id
         self.name = name
+        self._active = active
+
+    def is_active(self) -> bool:
+        return self._active
 
 
 class ProjectsDb:
     PROJECTS_FILE = 'projects.json'
 
     def __init__(self, path):
         self.path = path
@@ -264,15 +268,15 @@
     def decode(self, s):
         s = super(LocalProjectsDbDecoder, self).decode(s)
 
         projects = s['projects']
         projects_copy = []
         for project in projects:
             project['activities'] = [
-                Activity(str(activity['id']), activity['name'])
+                Activity(str(activity['id']), activity['name'], activity.get('_active', True))
                 for activity in project['activities']
             ]
             project['id'] = str(project['id'])
             for date_type in ['start_date', 'end_date']:
                 if project[date_type] is not None:
                     project[date_type] = datetime.datetime.strptime(
                         project[date_type], '%Y-%m-%d').date()
```

### Comparing `taxi-6.1.1/taxi/settings.py` & `taxi-6.2.0/taxi/settings.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/timesheet/entry.py` & `taxi-6.2.0/taxi/timesheet/entry.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/timesheet/flags.py` & `taxi-6.2.0/taxi/timesheet/flags.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/timesheet/lines.py` & `taxi-6.2.0/taxi/timesheet/lines.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/timesheet/parser.py` & `taxi-6.2.0/taxi/timesheet/parser.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/timesheet/timesheet.py` & `taxi-6.2.0/taxi/timesheet/timesheet.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/timesheet/utils.py` & `taxi-6.2.0/taxi/timesheet/utils.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/ui/__init__.py` & `taxi-6.2.0/taxi/ui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,38 +155,41 @@
 
         # Handle local aliases
         if not mapping.is_mapped():
             self.msg("[%s] %s -> not mapped" % (mapping.backend, alias))
             return
 
         mapping_name = Project.tuple_to_str(mapping.mapping)
+        mapping_is_active = True
 
         if not project:
             project_name = ''
         else:
+            mapping_is_active &= project.is_active()
             if mapping.mapping[1] is None:
                 project_name = project.name
                 mapping_name = mapping.mapping[0]
             else:
                 activity = project.get_activity(mapping.mapping[1])
 
                 if activity is None:
                     project_name = '%s, ?' % (project.name)
                 else:
+                    mapping_is_active &= activity.is_active()
                     project_name = '%s, %s' % (project.name, activity.name)
 
         if alias_first:
             args = [mapping.backend, alias, mapping_name]
         else:
             args = [mapping.backend, mapping_name, alias]
 
         args.append(' (%s)' % project_name if project_name else '')
         text = "[%s] %s -> %s%s" % tuple(args)
 
-        if project and project.is_active():
+        if project and mapping_is_active:
             self.msg(text)
         else:
             self.msg(click.style(text, fg='red'))
 
     def mapping_detail(self, mapping, project):
         self._show_mapping(mapping, project, False)
```

### Comparing `taxi-6.1.1/taxi/utils/date.py` & `taxi-6.2.0/taxi/utils/date.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/utils/structures.py` & `taxi-6.2.0/taxi/utils/structures.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi/utils/terminal.py` & `taxi-6.2.0/taxi/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `taxi-6.1.1/taxi.egg-info/PKG-INFO` & `taxi-6.2.0/taxi.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,75 @@
 Metadata-Version: 2.1
 Name: taxi
-Version: 6.1.1
+Version: 6.2.0
 Summary: Taxi: timesheeting made easy
 Home-page: https://github.com/liip/taxi
 Author: Sylvain Fankhauser
 Author-email: sylvain.fankhauser@liip.ch
 License: wtfpl
-Description: .. image:: https://raw.githubusercontent.com/sephii/taxi/main/doc/images/taxi.png
-        
-        What is Taxi ?
-        ==============
-        
-        Taxi is a timesheeting tool that focuses on simplicity to help you write your
-        timesheets without wasting time. All you'll do is edit a text file and write
-        down what you've worked on and how long, like so::
-        
-            23/01/2014
-        
-            pingpong 09:00-10:00 Play ping-pong
-            infra         -11:00 Repair coffee machine
-        
-        You can then get a summary of your timesheet::
-        
-            Staging changes :
-        
-            # Thursday 23 january #
-            pingpong (123/456)             1.00  Play ping-pong
-            infra (123/42)                 1.00  Repair coffee machine
-                                           2.00
-        
-            Total                          2.00
-        
-            Use `taxi ci` to commit staging changes to the server
-        
-        Through the use of backends, Taxi allows you to push your timesheets to
-        different systems.
-        
-        Getting started
-        ===============
-        
-        Refer to the `"Installation" section
-        <https://taxi-timesheets.readthedocs.io/en/main/userguide.html#installation>`_
-        in the docs.
-        
-        .. _supported_backends:
-        
-        Supported backends
-        ==================
-        
-        * `zebra <https://github.com/sephii/taxi-zebra>`__ : Liip's zebra backend
-        * `tempo <https://github.com/alexandreblin/taxi-tempo>`__ : Atlassian JIRA's `Tempo Timesheets <https://tempo.io>`__ backend
-        * `tipee <https://github.com/alexandreblin/taxi-tipee>`__ : Gammadia's `tipee <https://tipee.ch>`__ backend
-        * `bexio <https://github.com/alexandreblin/taxi-bexio>`__ : Bexio `Timesheets <https://bexio.com>`__ backend
-        * `multi <https://github.com/alexandreblin/taxi-multi>`__ : a special backend to push entries over multiple other backends
-        * `clockify <https://github.com/sephii/taxi-clockify>`__ : backend for the free timesheeting tool `clockify.me <https://clockify.me/>`_
-        
-        Contrib packages
-        ================
-        
-        These resources, not part of Taxi core, provide an enhanced experience for certain use cases.
-        
-        * `Cabdriver <https://github.com/metaodi/cabdriver>`_ (generate taxi entries based on Google Calendar, Slack, etc)
-        * `Syntax highlighting for VSCode <https://marketplace.visualstudio.com/items?itemName=LeBen.taxi-syntax-highlighting>`_
-        * `Vim plugin <https://github.com/schtibe/taxi.vim>`_ (features syntax highlighting, auto completion)
-        
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+.. image:: https://raw.githubusercontent.com/sephii/taxi/main/doc/images/taxi.png
+
+What is Taxi ?
+==============
+
+Taxi is a timesheeting tool that focuses on simplicity to help you write your
+timesheets without wasting time. All you'll do is edit a text file and write
+down what you've worked on and how long, like so::
+
+    23/01/2014
+
+    pingpong 09:00-10:00 Play ping-pong
+    infra         -11:00 Repair coffee machine
+
+You can then get a summary of your timesheet::
+
+    Staging changes :
+
+    # Thursday 23 january #
+    pingpong (123/456)             1.00  Play ping-pong
+    infra (123/42)                 1.00  Repair coffee machine
+                                   2.00
+
+    Total                          2.00
+
+    Use `taxi ci` to commit staging changes to the server
+
+Through the use of backends, Taxi allows you to push your timesheets to
+different systems.
+
+Getting started
+===============
+
+Refer to the `"Installation" section
+<https://taxi-timesheets.readthedocs.io/en/main/userguide.html#installation>`_
+in the docs.
+
+.. _supported_backends:
+
+Supported backends
+==================
+
+* `zebra <https://github.com/sephii/taxi-zebra>`__ : Liip's zebra backend
+* `tempo <https://github.com/alexandreblin/taxi-tempo>`__ : Atlassian JIRA's `Tempo Timesheets <https://tempo.io>`__ backend
+* `tipee <https://github.com/alexandreblin/taxi-tipee>`__ : Gammadia's `tipee <https://tipee.ch>`__ backend
+* `bexio <https://github.com/alexandreblin/taxi-bexio>`__ : Bexio `Timesheets <https://bexio.com>`__ backend
+* `multi <https://github.com/alexandreblin/taxi-multi>`__ : a special backend to push entries over multiple other backends
+* `clockify <https://github.com/sephii/taxi-clockify>`__ : backend for the free timesheeting tool `clockify.me <https://clockify.me/>`_
+
+Contrib packages
+================
+
+These resources, not part of Taxi core, provide an enhanced experience for certain use cases.
+
+* `Cabdriver <https://github.com/metaodi/cabdriver>`_ (generate taxi entries based on Google Calendar, Slack, etc)
+* `Syntax highlighting for VSCode <https://marketplace.visualstudio.com/items?itemName=LeBen.taxi-syntax-highlighting>`_
+* `Vim plugin <https://github.com/schtibe/taxi.vim>`_ (features syntax highlighting, auto completion)
```

### Comparing `taxi-6.1.1/taxi.egg-info/SOURCES.txt` & `taxi-6.2.0/taxi.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 taxi/plugins.py
 taxi/projects.py
 taxi/settings.py
 taxi.egg-info/PKG-INFO
 taxi.egg-info/SOURCES.txt
 taxi.egg-info/dependency_links.txt
 taxi.egg-info/entry_points.txt
-taxi.egg-info/pbr.json
 taxi.egg-info/requires.txt
 taxi.egg-info/top_level.txt
 taxi/backends/__init__.py
 taxi/backends/dummy.py
 taxi/commands/__init__.py
 taxi/commands/alias.py
 taxi/commands/autofill.py
```

