# Comparing `tmp/JBPhD-2.1.3.tar.gz` & `tmp/JBPhD-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBPhD-2.1.3.tar", last modified: Sun May 14 18:11:59 2023, max compression
+gzip compressed data, was "JBPhD-2.1.4.tar", last modified: Mon May 15 11:19:37 2023, max compression
```

## Comparing `JBPhD-2.1.3.tar` & `JBPhD-2.1.4.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 18:11:58.000000 JBPhD-2.1.3/
-drwxrwxrwx   0        0        0        0 2023-05-14 18:11:58.000000 JBPhD-2.1.3/JBPhD.egg-info/
--rw-rw-rw-   0        0        0      201 2023-05-14 18:11:58.000000 JBPhD-2.1.3/JBPhD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1629 2023-05-14 18:11:58.000000 JBPhD-2.1.3/JBPhD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 18:11:58.000000 JBPhD-2.1.3/JBPhD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-14 18:11:58.000000 JBPhD-2.1.3/JBPhD.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      135 2023-05-14 18:11:58.000000 JBPhD-2.1.3/JBPhD.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-14 18:11:58.000000 JBPhD-2.1.3/JBPhD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2023-05-07 16:04:18.000000 JBPhD-2.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      201 2023-05-14 18:12:00.000000 JBPhD-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-07 16:42:22.000000 JBPhD-2.1.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 18:11:58.000000 JBPhD-2.1.3/Task/
--rw-rw-rw-   0        0        0     2336 2023-04-20 18:29:48.000000 JBPhD-2.1.3/Task/Api.json
--rw-rw-rw-   0        0        0     2332 2023-04-30 20:14:46.000000 JBPhD-2.1.3/Task/Api2.json
--rw-rw-rw-   0        0        0   256511 2023-05-07 17:28:42.000000 JBPhD-2.1.3/Task/Back_Right.PNG
--rw-rw-rw-   0        0        0    60437 2023-02-02 09:16:10.000000 JBPhD-2.1.3/Task/Consent Form.docx
--rw-rw-rw-   0        0        0     1555 2023-05-12 13:01:46.000000 JBPhD-2.1.3/Task/Consent Form.txt
--rw-rw-rw-   0        0        0      998 2023-05-08 15:55:22.000000 JBPhD-2.1.3/Task/Dependencies.py
--rw-rw-rw-   0        0        0    12092 2023-05-12 14:41:32.000000 JBPhD-2.1.3/Task/Dependency Installation.py
--rw-rw-rw-   0        0        0      552 2023-05-06 17:47:44.000000 JBPhD-2.1.3/Task/Email Output.py
--rw-rw-rw-   0        0        0      202 2023-05-07 16:32:10.000000 JBPhD-2.1.3/Task/Experimental Run Trial.py
--rw-rw-rw-   0        0        0     4855 2023-05-06 18:07:04.000000 JBPhD-2.1.3/Task/Export.py
--rw-rw-rw-   0        0        0   249107 2023-05-07 17:28:42.000000 JBPhD-2.1.3/Task/Front_Left.PNG
--rw-rw-rw-   0        0        0   249006 2023-05-07 17:28:42.000000 JBPhD-2.1.3/Task/Front_Right.PNG
--rw-rw-rw-   0        0        0      883 2023-04-14 22:45:36.000000 JBPhD-2.1.3/Task/Graph.py
--rw-rw-rw-   0        0        0   281708 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/ImageSample.PNG
--rw-rw-rw-   0        0        0   256274 2023-05-07 17:28:42.000000 JBPhD-2.1.3/Task/Inverse_Back_Left.PNG
--rw-rw-rw-   0        0        0      384 2023-04-24 19:08:56.000000 JBPhD-2.1.3/Task/Location.py
--rw-rw-rw-   0        0        0       54 2023-05-07 14:35:12.000000 JBPhD-2.1.3/Task/MANIFEST.in.txt
--rw-rw-rw-   0        0        0    14031 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/Manikin Back Down Left.png
--rw-rw-rw-   0        0        0    13918 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/Manikin Back Up Right.png
--rw-rw-rw-   0        0        0    16784 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/Manikin front Down Right.png
--rw-rw-rw-   0        0        0    20357 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/Manikin front Up Right.png
--rw-rw-rw-   0        0        0        2 2023-05-12 14:39:40.000000 JBPhD-2.1.3/Task/N-Back count.txt
--rw-rw-rw-   0        0        0    18823 2023-05-04 21:33:20.000000 JBPhD-2.1.3/Task/N-Back.py
--rw-rw-rw-   0        0        0      625 2023-05-07 22:18:00.000000 JBPhD-2.1.3/Task/Output Test.py
-drwxrwxrwx   0        0        0        0 2023-05-14 18:11:58.000000 JBPhD-2.1.3/Task/Participant 1/
--rw-rw-rw-   0        0        0      222 2023-05-13 14:00:22.000000 JBPhD-2.1.3/Task/Participant 1/Dependency Installation Usage.csv
--rw-rw-rw-   0        0        0       70 2023-05-13 14:00:14.000000 JBPhD-2.1.3/Task/Participant 1/Export Usage.csv
--rw-rw-rw-   0        0        0       70 2023-05-13 14:00:14.000000 JBPhD-2.1.3/Task/Participant 1/Task Usage.csv
--rwxrwxrwx   0        0        0      680 2023-04-23 19:01:06.000000 JBPhD-2.1.3/Task/Python Install.bat
--rw-rw-rw-   0        0        0       20 2023-05-07 14:41:38.000000 JBPhD-2.1.3/Task/README.txt.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 10:25:18.000000 JBPhD-2.1.3/Task/RT count.txt
--rw-rw-rw-   0        0        0    17652 2023-05-01 10:34:26.000000 JBPhD-2.1.3/Task/Reaction Time Task - Copy.py
--rwxrwxrwx   0        0        0      448 2023-05-07 14:17:02.000000 JBPhD-2.1.3/Task/Suffix.bat
--rw-rw-rw-   0        0        0        1 2023-05-07 20:23:30.000000 JBPhD-2.1.3/Task/Switch Count.txt
--rw-rw-rw-   0        0        0    24158 2023-05-07 20:29:12.000000 JBPhD-2.1.3/Task/Switching.py
--rw-rw-rw-   0        0        0    13325 2023-05-14 17:58:08.000000 JBPhD-2.1.3/Task/Task.py
-drwxrwxrwx   0        0        0        0 2023-05-14 18:11:58.000000 JBPhD-2.1.3/Task/__pycache__/
--rw-rw-rw-   0        0        0     5027 2023-05-07 22:15:14.000000 JBPhD-2.1.3/Task/__pycache__/Dependencies.cpython-311.pyc
--rw-rw-rw-   0        0        0     6694 2023-05-06 18:08:18.000000 JBPhD-2.1.3/Task/__pycache__/Export.cpython-311.pyc
--rw-rw-rw-   0        0        0      696 2023-05-04 10:46:06.000000 JBPhD-2.1.3/Task/__pycache__/Location.cpython-311.pyc
--rw-rw-rw-   0        0        0    18767 2023-05-07 22:15:14.000000 JBPhD-2.1.3/Task/__pycache__/Task.cpython-311.pyc
--rw-rw-rw-   0        0        0      931 2023-05-05 14:18:56.000000 JBPhD-2.1.3/Task/__pycache__/spwf.cpython-311.pyc
--rw-rw-rw-   0        0        0     3162 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/asterisk.png
--rw-rw-rw-   0        0        0    47189 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/circle.jpg
--rw-rw-rw-   0        0        0      860 2023-04-30 18:46:22.000000 JBPhD-2.1.3/Task/cpudeps.py
--rw-rw-rw-   0        0        0      871 2023-04-30 19:06:50.000000 JBPhD-2.1.3/Task/cpudepsinstall.py
--rw-rw-rw-   0        0        0      854 2023-04-30 19:09:00.000000 JBPhD-2.1.3/Task/cpuexp.py
--rw-rw-rw-   0        0        0      854 2023-04-30 18:43:34.000000 JBPhD-2.1.3/Task/cpunbak.py
--rw-rw-rw-   0        0        0      861 2023-04-30 18:43:22.000000 JBPhD-2.1.3/Task/cpurt.py
--rw-rw-rw-   0        0        0      857 2023-04-30 18:43:54.000000 JBPhD-2.1.3/Task/cpuswitch.py
--rw-rw-rw-   0        0        0      852 2023-04-30 18:42:22.000000 JBPhD-2.1.3/Task/cputask.py
--rw-rw-rw-   0        0        0    12363 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/greendot.png
--rw-rw-rw-   0        0        0    38788 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/greentick.png
--rw-rw-rw-   0        0        0       54 2023-05-07 14:31:32.000000 JBPhD-2.1.3/Task/help.txt
--rw-rw-rw-   0        0        0      491 2023-05-14 16:12:16.000000 JBPhD-2.1.3/Task/pins.csv
--rw-rw-rw-   0        0        0    24503 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/redcross.png
--rw-rw-rw-   0        0        0    98588 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/reddot.png
--rw-rw-rw-   0        0        0      566 2023-05-07 14:26:16.000000 JBPhD-2.1.3/Task/setup.py
--rw-rw-rw-   0        0        0      472 2023-05-05 14:17:12.000000 JBPhD-2.1.3/Task/spwf.py
--rw-rw-rw-   0        0        0       44 2023-04-24 16:27:34.000000 JBPhD-2.1.3/Task/spwfoutput.txt
--rw-rw-rw-   0        0        0      100 2023-04-24 16:27:34.000000 JBPhD-2.1.3/Task/spwfvalue.txt
--rw-rw-rw-   0        0        0       14 2023-05-13 14:00:14.000000 JBPhD-2.1.3/Task/suffix.txt
--rw-rw-rw-   0        0        0   161693 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/trial.jpeg
--rw-rw-rw-   0        0        0   432254 2023-05-04 10:35:10.000000 JBPhD-2.1.3/Task/uop.ico
--rw-rw-rw-   0        0        0     3908 2023-05-04 10:32:40.000000 JBPhD-2.1.3/Task/uop.jpeg
--rw-rw-rw-   0        0        0     7038 2023-04-16 20:40:14.000000 JBPhD-2.1.3/Task/uop.png
--rw-rw-rw-   0        0        0       42 2023-05-14 18:12:00.000000 JBPhD-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0      837 2023-05-14 17:59:00.000000 JBPhD-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:19:38.000000 JBPhD-2.1.4/
+drwxrwxrwx   0        0        0        0 2023-05-15 11:19:38.000000 JBPhD-2.1.4/JBPhD.egg-info/
+-rw-rw-rw-   0        0        0      201 2023-05-15 11:19:38.000000 JBPhD-2.1.4/JBPhD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1646 2023-05-15 11:19:38.000000 JBPhD-2.1.4/JBPhD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 11:19:38.000000 JBPhD-2.1.4/JBPhD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-15 11:19:38.000000 JBPhD-2.1.4/JBPhD.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      135 2023-05-15 11:19:38.000000 JBPhD-2.1.4/JBPhD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-15 11:19:38.000000 JBPhD-2.1.4/JBPhD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2023-05-07 16:04:18.000000 JBPhD-2.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      201 2023-05-15 11:19:38.000000 JBPhD-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-07 16:42:22.000000 JBPhD-2.1.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 11:19:38.000000 JBPhD-2.1.4/Task/
+-rw-rw-rw-   0        0        0     2336 2023-04-20 18:29:48.000000 JBPhD-2.1.4/Task/Api.json
+-rw-rw-rw-   0        0        0     2332 2023-04-30 20:14:46.000000 JBPhD-2.1.4/Task/Api2.json
+-rw-rw-rw-   0        0        0   256511 2023-05-07 17:28:42.000000 JBPhD-2.1.4/Task/Back_Right.PNG
+-rw-rw-rw-   0        0        0    60437 2023-02-02 09:16:10.000000 JBPhD-2.1.4/Task/Consent Form.docx
+-rw-rw-rw-   0        0        0     1555 2023-05-12 13:01:46.000000 JBPhD-2.1.4/Task/Consent Form.txt
+-rw-rw-rw-   0        0        0      998 2023-05-08 15:55:22.000000 JBPhD-2.1.4/Task/Dependencies.py
+-rw-rw-rw-   0        0        0    12423 2023-05-15 10:35:30.000000 JBPhD-2.1.4/Task/Dependency Installation.py
+-rw-rw-rw-   0        0        0      552 2023-05-06 17:47:44.000000 JBPhD-2.1.4/Task/Email Output.py
+-rw-rw-rw-   0        0        0      202 2023-05-07 16:32:10.000000 JBPhD-2.1.4/Task/Experimental Run Trial.py
+-rw-rw-rw-   0        0        0     4855 2023-05-06 18:07:04.000000 JBPhD-2.1.4/Task/Export.py
+-rw-rw-rw-   0        0        0   249107 2023-05-07 17:28:42.000000 JBPhD-2.1.4/Task/Front_Left.PNG
+-rw-rw-rw-   0        0        0   249006 2023-05-07 17:28:42.000000 JBPhD-2.1.4/Task/Front_Right.PNG
+-rw-rw-rw-   0        0        0      883 2023-04-14 22:45:36.000000 JBPhD-2.1.4/Task/Graph.py
+-rw-rw-rw-   0        0        0   281708 2023-04-07 13:54:00.000000 JBPhD-2.1.4/Task/ImageSample.PNG
+-rw-rw-rw-   0        0        0   256274 2023-05-07 17:28:42.000000 JBPhD-2.1.4/Task/Inverse_Back_Left.PNG
+-rw-rw-rw-   0        0        0      384 2023-04-24 19:08:56.000000 JBPhD-2.1.4/Task/Location.py
+-rw-rw-rw-   0        0        0       54 2023-05-07 14:35:12.000000 JBPhD-2.1.4/Task/MANIFEST.in.txt
+-rw-rw-rw-   0        0        0    14031 2023-04-07 13:54:00.000000 JBPhD-2.1.4/Task/Manikin Back Down Left.png
+-rw-rw-rw-   0        0        0    13918 2023-04-07 13:54:00.000000 JBPhD-2.1.4/Task/Manikin Back Up Right.png
+-rw-rw-rw-   0        0        0    16784 2023-04-07 13:54:00.000000 JBPhD-2.1.4/Task/Manikin front Down Right.png
+-rw-rw-rw-   0        0        0    20357 2023-04-07 13:54:00.000000 JBPhD-2.1.4/Task/Manikin front Up Right.png
+-rw-rw-rw-   0        0        0        2 2023-05-12 14:39:40.000000 JBPhD-2.1.4/Task/N-Back count.txt
+-rw-rw-rw-   0        0        0    18723 2023-05-15 11:01:42.000000 JBPhD-2.1.4/Task/N-Back.py
+-rw-rw-rw-   0        0        0      625 2023-05-07 22:18:00.000000 JBPhD-2.1.4/Task/Output Test.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:19:38.000000 JBPhD-2.1.4/Task/Participant 99/
+-rw-rw-rw-   0        0        0   101383 2023-05-15 10:35:54.000000 JBPhD-2.1.4/Task/Participant 99/Dependency Installation Usage.csv
+-rw-rw-rw-   0        0        0   146832 2023-05-15 10:28:50.000000 JBPhD-2.1.4/Task/Participant 99/Export Usage.csv
+-rw-rw-rw-   0        0        0   150289 2023-05-15 10:34:06.000000 JBPhD-2.1.4/Task/Participant 99/Task Usage.csv
+-rwxrwxrwx   0        0        0      680 2023-04-23 19:01:06.000000 JBPhD-2.1.4/Task/Python Install.bat
+-rw-rw-rw-   0        0        0       20 2023-05-07 14:41:38.000000 JBPhD-2.1.4/Task/README.txt.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 11:12:42.000000 JBPhD-2.1.4/Task/RT count.txt
+-rw-rw-rw-   0        0        0    17794 2023-05-15 11:15:34.000000 JBPhD-2.1.4/Task/Reaction Time Task - Copy.py
+-rwxrwxrwx   0        0        0      448 2023-05-07 14:17:02.000000 JBPhD-2.1.4/Task/Suffix.bat
+-rw-rw-rw-   0        0        0        2 2023-05-15 10:24:12.000000 JBPhD-2.1.4/Task/Switch Count.txt
+-rw-rw-rw-   0        0        0    24157 2023-05-15 10:24:58.000000 JBPhD-2.1.4/Task/Switching.py
+-rw-rw-rw-   0        0        0    13655 2023-05-15 10:34:06.000000 JBPhD-2.1.4/Task/Task.py
+-rw-rw-rw-   0        0        0     6700 2023-05-15 10:06:40.000000 JBPhD-2.1.4/Task/Trial.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:19:38.000000 JBPhD-2.1.4/Task/__pycache__/
+-rw-rw-rw-   0        0        0     5027 2023-05-07 22:15:14.000000 JBPhD-2.1.4/Task/__pycache__/Dependencies.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6694 2023-05-06 18:08:18.000000 JBPhD-2.1.4/Task/__pycache__/Export.cpython-311.pyc
+-rw-rw-rw-   0        0        0      696 2023-05-04 10:46:06.000000 JBPhD-2.1.4/Task/__pycache__/Location.cpython-311.pyc
+-rw-rw-rw-   0        0        0    18767 2023-05-07 22:15:14.000000 JBPhD-2.1.4/Task/__pycache__/Task.cpython-311.pyc
+-rw-rw-rw-   0        0        0      931 2023-05-05 14:18:56.000000 JBPhD-2.1.4/Task/__pycache__/spwf.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3162 2023-04-07 13:54:00.000000 JBPhD-2.1.4/Task/asterisk.png
+-rw-rw-rw-   0        0        0    47189 2023-04-07 13:54:00.000000 JBPhD-2.1.4/Task/circle.jpg
+-rw-rw-rw-   0        0        0      860 2023-04-30 18:46:22.000000 JBPhD-2.1.4/Task/cpudeps.py
+-rw-rw-rw-   0        0        0      871 2023-04-30 19:06:50.000000 JBPhD-2.1.4/Task/cpudepsinstall.py
+-rw-rw-rw-   0        0        0      854 2023-04-30 19:09:00.000000 JBPhD-2.1.4/Task/cpuexp.py
+-rw-rw-rw-   0        0        0      854 2023-04-30 18:43:34.000000 JBPhD-2.1.4/Task/cpunbak.py
+-rw-rw-rw-   0        0        0      861 2023-04-30 18:43:22.000000 JBPhD-2.1.4/Task/cpurt.py
+-rw-rw-rw-   0        0        0      857 2023-04-30 18:43:54.000000 JBPhD-2.1.4/Task/cpuswitch.py
+-rw-rw-rw-   0        0        0      852 2023-04-30 18:42:22.000000 JBPhD-2.1.4/Task/cputask.py
+-rw-rw-rw-   0        0        0    12363 2023-04-07 13:54:00.000000 JBPhD-2.1.4/Task/greendot.png
+-rw-rw-rw-   0        0        0    38788 2023-04-07 13:54:00.000000 JBPhD-2.1.4/Task/greentick.png
+-rw-rw-rw-   0        0        0       54 2023-05-07 14:31:32.000000 JBPhD-2.1.4/Task/help.txt
+-rw-rw-rw-   0        0        0      491 2023-05-14 16:12:16.000000 JBPhD-2.1.4/Task/pins.csv
+-rw-rw-rw-   0        0        0    24503 2023-04-07 13:54:00.000000 JBPhD-2.1.4/Task/redcross.png
+-rw-rw-rw-   0        0        0    98588 2023-04-07 13:54:00.000000 JBPhD-2.1.4/Task/reddot.png
+-rw-rw-rw-   0        0        0      566 2023-05-07 14:26:16.000000 JBPhD-2.1.4/Task/setup.py
+-rw-rw-rw-   0        0        0      472 2023-05-05 14:17:12.000000 JBPhD-2.1.4/Task/spwf.py
+-rw-rw-rw-   0        0        0       44 2023-04-24 16:27:34.000000 JBPhD-2.1.4/Task/spwfoutput.txt
+-rw-rw-rw-   0        0        0      100 2023-04-24 16:27:34.000000 JBPhD-2.1.4/Task/spwfvalue.txt
+-rw-rw-rw-   0        0        0       14 2023-05-15 10:34:06.000000 JBPhD-2.1.4/Task/suffix.txt
+-rw-rw-rw-   0        0        0   161693 2023-04-07 13:54:00.000000 JBPhD-2.1.4/Task/trial.jpeg
+-rw-rw-rw-   0        0        0   432254 2023-05-04 10:35:10.000000 JBPhD-2.1.4/Task/uop.ico
+-rw-rw-rw-   0        0        0     3908 2023-05-04 10:32:40.000000 JBPhD-2.1.4/Task/uop.jpeg
+-rw-rw-rw-   0        0        0     7038 2023-04-16 20:40:14.000000 JBPhD-2.1.4/Task/uop.png
+-rw-rw-rw-   0        0        0       42 2023-05-15 11:19:38.000000 JBPhD-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      837 2023-05-15 11:17:38.000000 JBPhD-2.1.4/setup.py
```

### Comparing `JBPhD-2.1.3/JBPhD.egg-info/SOURCES.txt` & `JBPhD-2.1.4/JBPhD.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 Task/README.txt.txt
 Task/RT count.txt
 Task/Reaction Time Task - Copy.py
 Task/Suffix.bat
 Task/Switch Count.txt
 Task/Switching.py
 Task/Task.py
+Task/Trial.py
 Task/asterisk.png
 Task/circle.jpg
 Task/cpudeps.py
 Task/cpudepsinstall.py
 Task/cpuexp.py
 Task/cpunbak.py
 Task/cpurt.py
@@ -59,15 +60,15 @@
 Task/spwfoutput.txt
 Task/spwfvalue.txt
 Task/suffix.txt
 Task/trial.jpeg
 Task/uop.ico
 Task/uop.jpeg
 Task/uop.png
-Task/Participant 1/Dependency Installation Usage.csv
-Task/Participant 1/Export Usage.csv
-Task/Participant 1/Task Usage.csv
+Task/Participant 99/Dependency Installation Usage.csv
+Task/Participant 99/Export Usage.csv
+Task/Participant 99/Task Usage.csv
 Task/__pycache__/Dependencies.cpython-311.pyc
 Task/__pycache__/Export.cpython-311.pyc
 Task/__pycache__/Location.cpython-311.pyc
 Task/__pycache__/Task.cpython-311.pyc
 Task/__pycache__/spwf.cpython-311.pyc
```

### Comparing `JBPhD-2.1.3/Task/Api.json` & `JBPhD-2.1.4/Task/Api.json`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Api2.json` & `JBPhD-2.1.4/Task/Api2.json`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Back_Right.PNG` & `JBPhD-2.1.4/Task/Back_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Consent Form.docx` & `JBPhD-2.1.4/Task/Consent Form.docx`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Consent Form.txt` & `JBPhD-2.1.4/Task/Consent Form.txt`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Dependencies.py` & `JBPhD-2.1.4/Task/Dependencies.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Dependency Installation.py` & `JBPhD-2.1.4/Task/Dependency Installation.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,20 +175,30 @@
         if all_buttons_clicked == True:
             order = random.randint(1, 2)
             if order == 1:
                 file_path = "Reaction Time Task - Copy.py"
             else:
                 file_path = "N-Back.py"
             
-            subprocess.run([python_path, file_path], check=True)
+            subprocess.run([python_path, "Trial.py"], check=True)
             import Export
         
     root = tk.Tk()
     fontsize = ("Helvetica", 16)
     fontsize1 = ("Helvetica", 18)
+    fontsizesmall = ("Helvetica", 12)
+
+    root.attributes("-fullscreen", True)
+    root.attributes("-topmost", False)
+
+    def exit_program():
+        root.destroy()
+
+    exit_button = tk.Button(root, text="Exit", command=exit_program, font=fontsizesmall)
+    exit_button.pack(side="top", anchor="ne", padx=10, pady=5)
 
     ## Set window to full screen
     root.attributes('-fullscreen', True)
 
     time_label = tk.Label(root, text="", font=fontsize)
 
     # function to update the time label
@@ -248,15 +258,15 @@
     
     button4 = tk.Button(root, text="Start the Task", command=taskstart, font=fontsize)
     button4.pack(expand=False, side=tk.TOP, padx=0, pady=0, anchor="center")
 
     image_file = Image.open("uop.png")
     image = ImageTk.PhotoImage(image_file)
     image_label = tk.Label(root, image=image)
-    image_label.place(relx=1, rely=0, anchor="ne", x=-20, y=20)
+    image_label.place(relx=1, rely=0, anchor="ne", x=-20, y=40)
     update_time()   
 
     root.mainloop()
 
     root.quit()
 
 startup()
```

### Comparing `JBPhD-2.1.3/Task/Email Output.py` & `JBPhD-2.1.4/Task/Email Output.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Export.py` & `JBPhD-2.1.4/Task/Export.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Front_Left.PNG` & `JBPhD-2.1.4/Task/Front_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Front_Right.PNG` & `JBPhD-2.1.4/Task/Front_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Graph.py` & `JBPhD-2.1.4/Task/Graph.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/ImageSample.PNG` & `JBPhD-2.1.4/Task/ImageSample.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Inverse_Back_Left.PNG` & `JBPhD-2.1.4/Task/Inverse_Back_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Manikin Back Down Left.png` & `JBPhD-2.1.4/Task/Manikin Back Down Left.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Manikin Back Up Right.png` & `JBPhD-2.1.4/Task/Manikin Back Up Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Manikin front Down Right.png` & `JBPhD-2.1.4/Task/Manikin front Down Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Manikin front Up Right.png` & `JBPhD-2.1.4/Task/Manikin front Up Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/N-Back.py` & `JBPhD-2.1.4/Task/N-Back.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,25 +294,23 @@
         endRT = time.time()
         draw_text("Incorrect!", (WINDOW_SIZE[0] // 2, FONT_SIZE * 2), BLACK)
         screen.fill(WHITE)
         screen.blit(incorrectinterval, incorrectintervaldimensions)
         pygame.time.wait(1000)
         pygame.display.update()
         pygame.time.wait(1000)
-        print("Incorrect")
 
     def correct():
         endRT = time.time()
         draw_text("Incorrect!", (WINDOW_SIZE[0] // 2, FONT_SIZE * 2), BLACK)
         screen.fill(WHITE)
         screen.blit(correctinterval, correctintervaldimensions)
         pygame.time.wait(1000)
         pygame.display.update()
         pygame.time.wait(1000)
-        print("Correct")
 
     while running:
         starterRT = time.time()# Handle events
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 running = False
             elif event.type == pygame.KEYDOWN:
@@ -361,18 +359,14 @@
         draw_text(str(sequence[current_index]), (WINDOW_SIZE[0] // 2, WINDOW_SIZE[1] // 2), BLACK)
         now = datetime.now()
 
         outputtime = now.strftime("%H:%M:%S")
 
         print(f'Stimulus Presentation Time {outputtime}')
 
-        
-
-
-        # Update the score
         #draw_text(f"Score: {score}", (WINDOW_SIZE[0] // 2, FONT_SIZE), BLACK)
 
         # Update the display
         pygame.display.update()
 
         # Move to the next digit
         current_index += 1
@@ -491,17 +485,15 @@
         pygame.time.wait(2000)
 
         draw_text(str(sequence[current_index]), (WINDOW_SIZE[0] // 2, WINDOW_SIZE[1] // 2), BLACK)
         now = datetime.now()
 
         outputtime = now.strftime("%H:%M:%S")
 
-        print(f'Stimulus Presentation Time {outputtime}')
-
-        
+        print(f'Stimulus Presentation Time {outputtime}')        
 
 
         # Update the score
         #draw_text(f"Score: {score}", (WINDOW_SIZE[0] // 2, FONT_SIZE), BLACK)
 
         # Update the display
         pygame.display.update()
```

### Comparing `JBPhD-2.1.3/Task/Output Test.py` & `JBPhD-2.1.4/Task/Output Test.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Python Install.bat` & `JBPhD-2.1.4/Task/Python Install.bat`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/Reaction Time Task - Copy.py` & `JBPhD-2.1.4/Task/Reaction Time Task - Copy.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,16 @@
 
         screen.blit(text2, text2_rect)
         screen.blit(text, text_rect)
 
         # Update the display
         pygame.display.update()
 
-    pygame.display.update()
+    pygame.time.wait(500)
+
         
 def intro():
     os.environ['SDL_VIDEO_CENTERED'] = '1'
 
     score = 0
     
     #random_number = random.randint(11111,99999)
@@ -124,24 +125,23 @@
     #SCREEN_HEIGHT = 1000
     BLACK = (0, 0, 0)
     WHITE = (255, 255, 255)
     GREEN = (0, 255, 0)
     RED = (255, 0, 0)
     screen = pygame.display.set_mode(size, pygame.RESIZABLE)
 
-    screen.fill(WHITE)
+    #screen.fill(WHITE)
 
     pygame.display.set_caption("Task")
 
     # Loop until the user clicks the close button.
     done = False
 
     clock = pygame.time.Clock()
 
-
     # font
     font = pygame.font.Font(None, 32)
 
     display_instructions = True
     instruction_page = 1
 
     DISPLAYSURF = pygame.display.set_mode((SCREEN_WIDTH, SCREEN_HEIGHT), pygame.RESIZABLE)
@@ -201,62 +201,64 @@
             if event.type == pygame.QUIT:
                 Game_Running = False
             pygame.event.pump()
 
             if event.type == pygame.KEYDOWN:
                 if event.key == pygame.K_f and order == 2:
                     endRT = time.time()
-                    print("RT is: ", 60*(endRT - starterRT))
+                    #print("RT is: ", 60*(endRT - starterRT))
                     screen.fill(WHITE)
                     score += 1
                     screen.blit(correctinterval, correctintervaldimensions)
-                    pygame.time.wait(1000)
+                    pygame.time.wait(500)
                     pygame.display.update()
                     pygame.time.wait(1000)
                     Game_Running = False
                     
                 elif event.key == pygame.K_j and order == 1:
                     endRT = time.time()
-                    print("RT is: ", 60*(endRT - starterRT))
+                    #print("RT is: ", 60*(endRT - starterRT))
                     screen.fill(WHITE)
                     score += 1
                     screen.blit(correctinterval, correctintervaldimensions)
-                    pygame.time.wait(1000)
+                    pygame.time.wait(500)
                     pygame.display.update()
                     pygame.time.wait(1000)
                     Game_Running = False
                     
                 else:  # if incorrect key was pressed
                     endRT = time.time()
-                    print("RT is: ", 60*(endRT - starterRT))
+                    #print("RT is: ", 60*(endRT - starterRT))
                     screen.fill(WHITE)
+                    score += 1
                     screen.blit(incorrectinterval, incorrectintervaldimensions)
-                    pygame.time.wait(1000)
+                    pygame.time.wait(500)
+                    pygame.display.update()
                     pygame.time.wait(1000)
                     Game_Running = False
 
         pygame.display.update()
         pygame.time.delay(wait)
 
     #trialcounter += 1
-    print("Score", score)
-    print("Trial Count", trialcounter)
+    #print("Score", score)
+    #print("Trial Count", trialcounter)
 
 def practice():
 
+    screen.fill(WHITE)
     os.environ["SDL_VIDEO_CENTERED"] = "1"
 
     score = 0
 
     # Loop until the user clicks the close button.
     done = False
 
     clock = pygame.time.Clock()
 
-
     # font
     font = pygame.font.Font(None, 32)
 
     display_instructions = True
     instruction_page = 1
 
     DISPLAYSURF = pygame.display.set_mode(
@@ -282,15 +284,15 @@
     if timer == 4:
      wait = 1400
     if timer == 5:
      wait = 1500
 
     while Game_Running:
 
-        DISPLAYSURF.fill(WHITE)
+        #DISPLAYSURF.fill(WHITE)
 
         if order == 2:
             ImageSample = pygame.image.load("asterisk.png")
             
         else:
             ImageSample = pygame.image.load("circle.jpg")
 
@@ -337,39 +339,39 @@
                     screen.fill(WHITE)
                     screen.blit(incorrectinterval, incorrectintervaldimensions)
                     pygame.time.wait(500)
                     pygame.display.update()
                     pygame.time.wait(500)
                     Game_Running = False
 
-        pygame.display.flip()
+        pygame.display.update()
         pygame.time.delay(1000)
 
 def exitscreen():
     os.environ["SDL_VIDEO_CENTERED"] = "1"
 
     df = pd.read_csv(filename2, usecols=[2], header=None)
     mean = df.mean().values[0]
 
     accuracydf = pd.read_csv(filename, usecols=[2], header=None)
     accuracydf = accuracydf.round(1)
 
     counter = accuracydf.count().values[0]
     formatted_num = "{:.2f}".format(mean)
-    #print(formatted_num)
+    ##print(formatted_num)
 
 
     totalscore = accuracydf.sum().values[0]
 
-    #print(totalscore,counter)
+    ##print(totalscore,counter)
     finalscore = totalscore / counter * 100
-    #print("Percentage" , finalscore)
+    ##print("Percentage" , finalscore)
 
     formatted_acc = "{:.1f}".format(finalscore)
-    #print(formatted_acc)
+    ##print(formatted_acc)
     # font
     font = pygame.font.Font(None, 32)
 
     DISPLAYSURF = pygame.display.set_mode(
         (SCREEN_WIDTH, SCREEN_HEIGHT), pygame.RESIZABLE
     )
 
@@ -435,15 +437,15 @@
     DISPLAYSURF = pygame.display.set_mode(
         (SCREEN_WIDTH, SCREEN_HEIGHT), pygame.FULLSCREEN
     )
 
     # DISPLAYSURF.fill(WHITE)
 
     order = random.randint(1, 2)
-    print(order)
+    #print(order)
 
 
     Game_Running = True
 
     starterRT = time.time()
 
     while Game_Running:
@@ -464,15 +466,15 @@
 
         correctinterval = pygame.image.load("greentick.png")
         correctintervaldimensions = correctinterval.get_rect(center=screen.get_rect().center)
 
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 Game_Running = False
-            pygame.event.pump()
+           # pygame.event.pump()
             
             if event.type == pygame.KEYDOWN:
                 if event.key == pygame.K_f and order == 1:
                     endRT = time.time()
                     RT = endRT - starterRT
                     score += 1
                     pygame.time.wait(1000)
@@ -487,15 +489,16 @@
 
                 else:  # if incorrect key was pressed
                     endRT = time.time()
                     RT = endRT - starterRT
                     pygame.time.wait(1000)
                     Game_Running = False
 
-        pygame.display.update()
+        screen.fill(WHITE)
+        #pygame.display.update()
         pygame.time.delay(wait)
 
     with open(filename, mode="a+") as file:
         file.write(f"{date_time_string}, {count}, {score}, Reaction Time\n")
 
     with open(filename2, mode="a+") as file:
         file.write(f"{date_time_string}, {count}, {RT}, Reaction Time\n")
@@ -513,25 +516,25 @@
     mean = df.mean().values[0]
 
     accuracydf = pd.read_csv(filename, usecols=[2], header=None)
     accuracydf = accuracydf.round(1)
 
     counter = accuracydf.count().values[0]
     formatted_num = "{:.2f}".format(mean)
-    #print(formatted_num)
+    ##print(formatted_num)
 
 
     totalscore = accuracydf.sum().values[0]
 
-    #print(totalscore,counter)
+    ##print(totalscore,counter)
     finalscore = totalscore / counter * 100
-    #print("Percentage" , finalscore)
+    ##print("Percentage" , finalscore)
 
     formatted_acc = "{:.1f}".format(finalscore)
-    #print(formatted_acc)
+    ##print(formatted_acc)
     # font
     font = pygame.font.Font(None, 32)
 
     DISPLAYSURF = pygame.display.set_mode(
         (SCREEN_WIDTH, SCREEN_HEIGHT), pygame.RESIZABLE
     )
```

### Comparing `JBPhD-2.1.3/Task/Switching.py` & `JBPhD-2.1.4/Task/Switching.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
         remaining_time = duration - elapsed_time
         if remaining_time < 0:
             remaining_time = 0
 
         # Create a text surface with the remaining time
         text2 = font.render(str(remaining_time), True, BLACK)
-        text2_rect = text2.get_rect(center=(SCREEN_WIDTH / 2, SCREEN_HEIGHT / 2 + 350))
+        text2_rect = text2.get_rect(center=(SCREEN_WIDTH / 2, SCREEN_HEIGHT / 2 + 450))
         screen.blit(text2, text2_rect)
 
 
         incorrectinterval = pygame.image.load("redcross.png")
         incorrectintervaldimensions = incorrectinterval.get_rect(
             center=screen.get_rect().center
         )
@@ -438,15 +438,15 @@
 
 def show_welcome_screen():
     os.environ["SDL_VIDEO_CENTERED"] = "1"
 
     score = 0
 
     # font
-    font = pygame.font.Font(None, 32)
+    font = pygame.font.Font(None, 64)
 
     order = 1
 
     start_time = pygame.time.get_ticks()
 
     Game_Running = True
 
@@ -457,15 +457,15 @@
     screen.fill(WHITE)
     pygame.display.set_caption("Welcome to the Task")
     font = pygame.font.Font(None, 60)
     text = font.render("Welcome to the Task", True, BLACK)
     text_rect = text.get_rect(center=(SCREEN_WIDTH / 2, SCREEN_HEIGHT / 2))
     screen.blit(text, text_rect)
 
-    timeout = 15
+    timeout = 5
 
     running = True
     while running:
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 running = False
 
@@ -496,15 +496,15 @@
 
 
 def nback():
     os.environ["SDL_VIDEO_CENTERED"] = "1"
     score = 0
 
     # font
-    font = pygame.font.Font(None, 32)
+    font = pygame.font.Font(None, 48)
 
     order = 1
 
     Game_Running = True
 
     starterRT = time.time()
 
@@ -762,15 +762,15 @@
     screen.blit(text, text_rect)
 
     pygame.display.update()
     # pygame.time.delay(500)
     pygame.time.delay(10000)
 
 def trialorder():
-    for i in range(0, 10):
+    for i in range(0, 40):
         torder = random.randint(1, 2)
         if torder == 1:
             nback()
         else:
             nbackball()
```

### Comparing `JBPhD-2.1.3/Task/Task.py` & `JBPhD-2.1.4/Task/Task.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,25 +224,33 @@
                     file_path = "Switching.py"
                     subprocess.run([python_path, file_path], check=True)
                     subprocess.run([python_path, 'Export.py'], check=True)            
 
             fontsize = ("Helvetica", 18)
             fontsize1 = ("Helvetica", 22)
             fontsize2 = ("Helvetica", 12)
+            fontsizesmall = ("Helvetica", 12)
 
-            root.attributes('-fullscreen', True)
+            root.attributes("-fullscreen", True)
+            root.attributes("-topmost", False)
+
+            def exit_program():
+                root.destroy()
+
+            exit_button = tk.Button(root, text="Exit", command=exit_program, font=fontsizesmall)
+            exit_button.pack(side="top", anchor="ne", padx=10, pady=5)
 
             time_label = tk.Label(root, text="", font=fontsize)
 
             def update_time():
                 current_time = time.strftime("%H:%M:%S")
                 time_label.config(text=current_time)
                 time_label.after(1000, update_time)
                 
-            time_label.pack(side=tk.TOP, padx=20, pady=10, anchor="nw")
+            time_label.pack(side=tk.TOP, padx=20, pady=0, anchor="nw")
 
             welcome_frame = tk.Frame(root)
             welcome_frame.pack(side=tk.TOP, fill=tk.X)
 
             welcome_label = tk.Label(welcome_frame, text="Welcome back!", font=fontsize1)
             welcome_label.pack(pady=position)
 
@@ -319,16 +327,16 @@
 
             button12 = tk.Button(button12_frame, text="Email for assistance or queries", command=emailsupport, font=fontsize)
             button12.pack(side=tk.LEFT, pady=10)
 
             image_file = Image.open("uop.png")
             image2 = ImageTk.PhotoImage(image_file)
             image_label = tk.Label(root, image=image2)
-            image_label.place(relx=1, rely=0, anchor="ne", x=-20, y=20)
-            update_time()   
+            image_label.place(relx=1, rely=0, anchor="ne", x=-20, y=40)
+            update_time()
 
             root.mainloop()            
 
             root.quit()
             cpurun.terminate()
             subprocess.run([python_path, 'Export.py'], check=True)
```

### Comparing `JBPhD-2.1.3/Task/__pycache__/Dependencies.cpython-311.pyc` & `JBPhD-2.1.4/Task/__pycache__/Dependencies.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/__pycache__/Export.cpython-311.pyc` & `JBPhD-2.1.4/Task/__pycache__/Export.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/__pycache__/Location.cpython-311.pyc` & `JBPhD-2.1.4/Task/__pycache__/Location.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/__pycache__/Task.cpython-311.pyc` & `JBPhD-2.1.4/Task/__pycache__/Task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/__pycache__/spwf.cpython-311.pyc` & `JBPhD-2.1.4/Task/__pycache__/spwf.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/asterisk.png` & `JBPhD-2.1.4/Task/asterisk.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/circle.jpg` & `JBPhD-2.1.4/Task/circle.jpg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/cpudeps.py` & `JBPhD-2.1.4/Task/cpudeps.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/cpudepsinstall.py` & `JBPhD-2.1.4/Task/cpudepsinstall.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/cpuexp.py` & `JBPhD-2.1.4/Task/cpuexp.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/cpunbak.py` & `JBPhD-2.1.4/Task/cpunbak.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/cpurt.py` & `JBPhD-2.1.4/Task/cpurt.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/cpuswitch.py` & `JBPhD-2.1.4/Task/cpuswitch.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/cputask.py` & `JBPhD-2.1.4/Task/cputask.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/greendot.png` & `JBPhD-2.1.4/Task/greendot.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/greentick.png` & `JBPhD-2.1.4/Task/greentick.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/redcross.png` & `JBPhD-2.1.4/Task/redcross.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/reddot.png` & `JBPhD-2.1.4/Task/reddot.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/setup.py` & `JBPhD-2.1.4/Task/setup.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/trial.jpeg` & `JBPhD-2.1.4/Task/trial.jpeg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/uop.ico` & `JBPhD-2.1.4/Task/uop.ico`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/uop.jpeg` & `JBPhD-2.1.4/Task/uop.jpeg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/Task/uop.png` & `JBPhD-2.1.4/Task/uop.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.3/setup.py` & `JBPhD-2.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 packagereqs = ['sendgrid', 'psutil', 'plyer', 'cryptography', 'pygame', 'pandas', 'google-auth', 'google-auth-oauthlib', 'google-auth-httplib2', 'google-api-python-client', 'Pillow']
 
 with open('README.txt', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='JBPhD',
-    version='2.1.3',
+    version='2.1.4',
     packages=find_namespace_packages(include=['Task']),
     install_requires=packagereqs,
     entry_points={
         'console_scripts': [
             'myproject = myproject.main:main'
         ]
     },
```

