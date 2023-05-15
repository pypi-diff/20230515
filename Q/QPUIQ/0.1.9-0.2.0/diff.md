# Comparing `tmp/QPUIQ-0.1.9.tar.gz` & `tmp/QPUIQ-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QPUIQ-0.1.9.tar", last modified: Mon May  1 15:14:04 2023, max compression
+gzip compressed data, was "QPUIQ-0.2.0.tar", last modified: Mon May 15 21:55:43 2023, max compression
```

## Comparing `QPUIQ-0.1.9.tar` & `QPUIQ-0.2.0.tar`

### file list

```diff
@@ -1,74 +1,72 @@
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.670331 QPUIQ-0.1.9/
--rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.1.9/LICENSE.txt
--rw-r--r--   0 Bug        (504) staff       (20)     2889 2023-05-01 15:14:04.670198 QPUIQ-0.1.9/PKG-INFO
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.655351 QPUIQ-0.1.9/PUI/
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.658463 QPUIQ-0.1.9/PUI/PySide6/
--rw-r--r--   0 Bug        (504) staff       (20)     1109 2023-05-01 14:22:51.000000 QPUIQ-0.1.9/PUI/PySide6/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      498 2023-04-29 18:30:29.000000 QPUIQ-0.1.9/PUI/PySide6/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     2334 2023-05-01 15:09:58.000000 QPUIQ-0.1.9/PUI/PySide6/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-29 06:22:40.000000 QPUIQ-0.1.9/PUI/PySide6/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     3128 2023-05-01 15:09:30.000000 QPUIQ-0.1.9/PUI/PySide6/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:43:52.000000 QPUIQ-0.1.9/PUI/PySide6/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      807 2023-05-01 14:28:35.000000 QPUIQ-0.1.9/PUI/PySide6/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:43:58.000000 QPUIQ-0.1.9/PUI/PySide6/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      991 2023-04-30 15:12:34.000000 QPUIQ-0.1.9/PUI/PySide6/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:06.000000 QPUIQ-0.1.9/PUI/PySide6/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1326 2023-05-01 13:25:01.000000 QPUIQ-0.1.9/PUI/PySide6/window.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.660914 QPUIQ-0.1.9/PUI/Qt5/
--rw-r--r--   0 Bug        (504) staff       (20)      417 2023-04-29 17:06:45.000000 QPUIQ-0.1.9/PUI/Qt5/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      496 2023-04-29 18:30:13.000000 QPUIQ-0.1.9/PUI/Qt5/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     1138 2023-04-30 05:12:20.000000 QPUIQ-0.1.9/PUI/Qt5/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-23 17:44:21.000000 QPUIQ-0.1.9/PUI/Qt5/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1527 2023-04-26 17:40:36.000000 QPUIQ-0.1.9/PUI/Qt5/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:44:32.000000 QPUIQ-0.1.9/PUI/Qt5/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      541 2023-03-13 15:01:12.000000 QPUIQ-0.1.9/PUI/Qt5/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:44:38.000000 QPUIQ-0.1.9/PUI/Qt5/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:41.000000 QPUIQ-0.1.9/PUI/Qt5/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1297 2023-04-29 17:05:56.000000 QPUIQ-0.1.9/PUI/Qt5/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      488 2023-05-01 15:12:51.000000 QPUIQ-0.1.9/PUI/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      525 2023-05-01 12:18:54.000000 QPUIQ-0.1.9/PUI/decorator.py
--rw-r--r--   0 Bug        (504) staff       (20)     2627 2023-04-30 15:12:00.000000 QPUIQ-0.1.9/PUI/dom.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.663889 QPUIQ-0.1.9/PUI/flet/
--rw-r--r--   0 Bug        (504) staff       (20)      452 2023-04-29 19:08:30.000000 QPUIQ-0.1.9/PUI/flet/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      551 2023-04-29 19:19:55.000000 QPUIQ-0.1.9/PUI/flet/application.py
--rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.1.9/PUI/flet/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      647 2023-03-15 07:54:51.000000 QPUIQ-0.1.9/PUI/flet/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.1.9/PUI/flet/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      943 2023-04-14 18:19:33.000000 QPUIQ-0.1.9/PUI/flet/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:58:06.000000 QPUIQ-0.1.9/PUI/flet/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.1.9/PUI/flet/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      482 2023-04-29 19:19:13.000000 QPUIQ-0.1.9/PUI/flet/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     3309 2023-05-01 14:03:40.000000 QPUIQ-0.1.9/PUI/node.py
--rw-r--r--   0 Bug        (504) staff       (20)     8998 2023-05-01 12:23:44.000000 QPUIQ-0.1.9/PUI/state.py
--rw-r--r--   0 Bug        (504) staff       (20)      983 2023-03-16 07:50:08.000000 QPUIQ-0.1.9/PUI/timeline.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.666993 QPUIQ-0.1.9/PUI/tkinter/
--rw-r--r--   0 Bug        (504) staff       (20)      488 2023-04-30 08:13:51.000000 QPUIQ-0.1.9/PUI/tkinter/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      568 2023-04-29 18:55:09.000000 QPUIQ-0.1.9/PUI/tkinter/application.py
--rw-r--r--   0 Bug        (504) staff       (20)      541 2023-04-29 19:57:02.000000 QPUIQ-0.1.9/PUI/tkinter/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      528 2023-04-23 17:43:10.000000 QPUIQ-0.1.9/PUI/tkinter/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1729 2023-04-30 08:20:56.000000 QPUIQ-0.1.9/PUI/tkinter/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      403 2023-04-23 17:43:21.000000 QPUIQ-0.1.9/PUI/tkinter/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1642 2023-04-30 08:53:03.000000 QPUIQ-0.1.9/PUI/tkinter/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      468 2023-04-23 17:43:25.000000 QPUIQ-0.1.9/PUI/tkinter/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      694 2023-04-30 09:14:54.000000 QPUIQ-0.1.9/PUI/tkinter/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      866 2023-04-23 17:43:29.000000 QPUIQ-0.1.9/PUI/tkinter/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1530 2023-04-29 19:56:35.000000 QPUIQ-0.1.9/PUI/tkinter/window.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.669426 QPUIQ-0.1.9/PUI/urwid/
--rw-r--r--   0 Bug        (504) staff       (20)      469 2023-04-30 08:00:16.000000 QPUIQ-0.1.9/PUI/urwid/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)     1246 2023-04-29 19:07:03.000000 QPUIQ-0.1.9/PUI/urwid/application.py
--rw-r--r--   0 Bug        (504) staff       (20)       63 2023-03-14 09:21:15.000000 QPUIQ-0.1.9/PUI/urwid/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      678 2023-03-15 07:59:17.000000 QPUIQ-0.1.9/PUI/urwid/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      356 2023-03-16 07:54:05.000000 QPUIQ-0.1.9/PUI/urwid/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      734 2023-03-16 07:54:02.000000 QPUIQ-0.1.9/PUI/urwid/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      462 2023-03-15 00:27:06.000000 QPUIQ-0.1.9/PUI/urwid/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      674 2023-04-30 08:07:16.000000 QPUIQ-0.1.9/PUI/urwid/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      315 2023-04-29 19:07:06.000000 QPUIQ-0.1.9/PUI/urwid/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     2604 2023-04-30 15:11:41.000000 QPUIQ-0.1.9/PUI/view.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.670018 QPUIQ-0.1.9/QPUIQ.egg-info/
--rw-r--r--   0 Bug        (504) staff       (20)     2889 2023-05-01 15:14:04.000000 QPUIQ-0.1.9/QPUIQ.egg-info/PKG-INFO
--rw-r--r--   0 Bug        (504) staff       (20)     1315 2023-05-01 15:14:04.000000 QPUIQ-0.1.9/QPUIQ.egg-info/SOURCES.txt
--rw-r--r--   0 Bug        (504) staff       (20)        1 2023-05-01 15:14:04.000000 QPUIQ-0.1.9/QPUIQ.egg-info/dependency_links.txt
--rw-r--r--   0 Bug        (504) staff       (20)        4 2023-05-01 15:14:04.000000 QPUIQ-0.1.9/QPUIQ.egg-info/top_level.txt
--rw-r--r--   0 Bug        (504) staff       (20)     2629 2023-04-29 21:00:52.000000 QPUIQ-0.1.9/README.md
--rw-r--r--   0 Bug        (504) staff       (20)       38 2023-05-01 15:14:04.670371 QPUIQ-0.1.9/setup.cfg
--rw-r--r--   0 Bug        (504) staff       (20)      539 2023-04-29 10:19:13.000000 QPUIQ-0.1.9/setup.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-15 21:55:43.715850 QPUIQ-0.2.0/
+-rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.2.0/LICENSE.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     5972 2023-05-15 21:55:43.715700 QPUIQ-0.2.0/PKG-INFO
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-15 21:55:43.702451 QPUIQ-0.2.0/PUI/
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-15 21:55:43.706205 QPUIQ-0.2.0/PUI/PySide6/
+-rw-r--r--   0 Bug        (504) staff       (20)     1177 2023-05-15 20:37:16.000000 QPUIQ-0.2.0/PUI/PySide6/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      498 2023-04-29 18:30:29.000000 QPUIQ-0.2.0/PUI/PySide6/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3734 2023-05-15 20:35:11.000000 QPUIQ-0.2.0/PUI/PySide6/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      575 2023-05-14 18:07:46.000000 QPUIQ-0.2.0/PUI/PySide6/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2708 2023-05-12 01:01:59.000000 QPUIQ-0.2.0/PUI/PySide6/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      764 2023-05-14 14:59:50.000000 QPUIQ-0.2.0/PUI/PySide6/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2343 2023-05-14 16:38:10.000000 QPUIQ-0.2.0/PUI/PySide6/combobox.py
+-rw-r--r--   0 Bug        (504) staff       (20)      722 2023-05-14 18:07:33.000000 QPUIQ-0.2.0/PUI/PySide6/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      941 2023-05-10 09:26:37.000000 QPUIQ-0.2.0/PUI/PySide6/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      493 2023-05-04 13:36:49.000000 QPUIQ-0.2.0/PUI/PySide6/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      784 2023-05-14 14:54:11.000000 QPUIQ-0.2.0/PUI/PySide6/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3895 2023-05-14 15:12:52.000000 QPUIQ-0.2.0/PUI/PySide6/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1544 2023-05-14 18:06:04.000000 QPUIQ-0.2.0/PUI/PySide6/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      820 2023-05-04 13:36:56.000000 QPUIQ-0.2.0/PUI/PySide6/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1996 2023-05-12 05:40:38.000000 QPUIQ-0.2.0/PUI/PySide6/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      488 2023-05-15 21:54:54.000000 QPUIQ-0.2.0/PUI/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      432 2023-05-15 20:31:59.000000 QPUIQ-0.2.0/PUI/decorator.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2790 2023-05-13 06:35:30.000000 QPUIQ-0.2.0/PUI/dom.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-15 21:55:43.708682 QPUIQ-0.2.0/PUI/flet/
+-rw-r--r--   0 Bug        (504) staff       (20)      388 2023-05-12 01:01:47.000000 QPUIQ-0.2.0/PUI/flet/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      516 2023-05-06 22:58:40.000000 QPUIQ-0.2.0/PUI/flet/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.2.0/PUI/flet/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      482 2023-05-14 18:08:03.000000 QPUIQ-0.2.0/PUI/flet/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.2.0/PUI/flet/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      955 2023-05-15 17:33:27.000000 QPUIQ-0.2.0/PUI/flet/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:58:06.000000 QPUIQ-0.2.0/PUI/flet/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.2.0/PUI/flet/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      447 2023-05-06 22:58:40.000000 QPUIQ-0.2.0/PUI/flet/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     4214 2023-05-15 21:05:53.000000 QPUIQ-0.2.0/PUI/node.py
+-rw-r--r--   0 Bug        (504) staff       (20)    12370 2023-05-15 16:57:03.000000 QPUIQ-0.2.0/PUI/state.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-15 21:55:43.711782 QPUIQ-0.2.0/PUI/textual/
+-rw-r--r--   0 Bug        (504) staff       (20)      942 2023-05-15 21:44:28.000000 QPUIQ-0.2.0/PUI/textual/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1776 2023-05-15 21:49:20.000000 QPUIQ-0.2.0/PUI/textual/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)      223 2023-05-15 17:15:48.000000 QPUIQ-0.2.0/PUI/textual/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      421 2023-05-15 19:40:06.000000 QPUIQ-0.2.0/PUI/textual/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      531 2023-05-15 21:53:10.000000 QPUIQ-0.2.0/PUI/textual/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1288 2023-05-15 21:02:44.000000 QPUIQ-0.2.0/PUI/textual/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1014 2023-05-15 19:41:34.000000 QPUIQ-0.2.0/PUI/textual/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      484 2023-05-15 19:42:35.000000 QPUIQ-0.2.0/PUI/textual/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      634 2023-05-15 21:50:12.000000 QPUIQ-0.2.0/PUI/textual/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)      367 2023-05-15 20:40:47.000000 QPUIQ-0.2.0/PUI/textual/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      371 2023-05-15 21:11:27.000000 QPUIQ-0.2.0/PUI/textual/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      700 2023-05-15 21:46:56.000000 QPUIQ-0.2.0/PUI/textual/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      591 2023-05-15 18:04:39.000000 QPUIQ-0.2.0/PUI/textual/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1253 2023-05-15 20:38:31.000000 QPUIQ-0.2.0/PUI/timeline.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-15 21:55:43.714820 QPUIQ-0.2.0/PUI/tkinter/
+-rw-r--r--   0 Bug        (504) staff       (20)      436 2023-05-12 08:12:36.000000 QPUIQ-0.2.0/PUI/tkinter/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      554 2023-05-10 11:03:55.000000 QPUIQ-0.2.0/PUI/tkinter/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)      564 2023-05-10 11:04:22.000000 QPUIQ-0.2.0/PUI/tkinter/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      462 2023-05-14 18:07:17.000000 QPUIQ-0.2.0/PUI/tkinter/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1283 2023-05-12 18:42:45.000000 QPUIQ-0.2.0/PUI/tkinter/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      522 2023-05-14 18:06:49.000000 QPUIQ-0.2.0/PUI/tkinter/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2197 2023-05-12 09:01:37.000000 QPUIQ-0.2.0/PUI/tkinter/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      468 2023-04-23 17:43:25.000000 QPUIQ-0.2.0/PUI/tkinter/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      565 2023-05-12 15:00:48.000000 QPUIQ-0.2.0/PUI/tkinter/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      866 2023-04-23 17:43:29.000000 QPUIQ-0.2.0/PUI/tkinter/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1524 2023-05-12 08:31:21.000000 QPUIQ-0.2.0/PUI/tkinter/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      505 2023-05-07 08:48:56.000000 QPUIQ-0.2.0/PUI/utils.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3082 2023-05-15 20:36:28.000000 QPUIQ-0.2.0/PUI/view.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-15 21:55:43.715502 QPUIQ-0.2.0/QPUIQ.egg-info/
+-rw-r--r--   0 Bug        (504) staff       (20)     5972 2023-05-15 21:55:43.000000 QPUIQ-0.2.0/QPUIQ.egg-info/PKG-INFO
+-rw-r--r--   0 Bug        (504) staff       (20)     1345 2023-05-15 21:55:43.000000 QPUIQ-0.2.0/QPUIQ.egg-info/SOURCES.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        1 2023-05-15 21:55:43.000000 QPUIQ-0.2.0/QPUIQ.egg-info/dependency_links.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        4 2023-05-15 21:55:43.000000 QPUIQ-0.2.0/QPUIQ.egg-info/top_level.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     5712 2023-05-15 21:26:34.000000 QPUIQ-0.2.0/README.md
+-rw-r--r--   0 Bug        (504) staff       (20)       38 2023-05-15 21:55:43.715894 QPUIQ-0.2.0/setup.cfg
+-rw-r--r--   0 Bug        (504) staff       (20)      539 2023-04-29 10:19:13.000000 QPUIQ-0.2.0/setup.py
```

### Comparing `QPUIQ-0.1.9/LICENSE.txt` & `QPUIQ-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.9/PUI/PySide6/__init__.py` & `QPUIQ-0.2.0/PUI/PySide6/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 import PySide6
 from PySide6.QtWidgets import QSizePolicy, QLayout
 
 from .application import *
 from .button import *
 from .canvas import *
+from .checkbox import *
+from .combobox import *
 from .label import *
 from .layout import *
 from .progressbar import *
+from .radiobutton import *
 from .scroll import *
+from .text import *
 from .textfield import *
 from .window import *
 
 Application = QtApplication
 Window = QtWindow
 HBox = QtHBox
 VBox = QtVBox
 Label = QtLabel
 Button = QtButton
+Checkbox = QtCheckbox
+RadioButton = QtRadioButton
 Canvas = QtCanvas
-CanvasText = QtCanvasText
-CanvasLine = QtCanvasLine
-CanvasPolyline = QtCanvasPolyline
 TextField = QtLineEdit
 ProgressBar = QtProgressBar
 Scroll = QtScrollArea
 Spacer = QtSpacerItem
+Text = QtText
+Html = QtHtml
+MarkDown = QtMarkDown
+Combobox = QtComboBox
+ComboboxItem = QtComboBoxItem
 
 def QtPUI(func):
     """
     PUI.PySide6.PUI triggers update() by signal/slot
     """
     def func_wrapper(*args):
         class PUIViewWrapper(QPUIView):
             def __init__(self, name):
                 self.name = name
                 super().__init__()
 
             def content(self):
-                return self.__wrapped_content__()
-
-            def __wrapped_content__(self):
                 return func(*args)
+
         ret = PUIViewWrapper(func.__name__)
         return ret
 
     return func_wrapper
 
 PUI = QtPUI
```

### Comparing `QPUIQ-0.1.9/PUI/PySide6/button.py` & `QPUIQ-0.2.0/PUI/PySide6/button.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from .. import *
 from .base import *
 
 class QtButton(QtBaseWidget):
-    def __init__(self, text, callback=None):
+    def __init__(self, text):
         super().__init__()
         self.text = text
-        self.callback = callback
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
             self.ui.setText(self.text)
             try:
                 self.ui.clicked.disconnect()
             except:
                 pass
-            self.ui.clicked.connect(self.callback)
+            prev.callback = None
         else:
             self.ui = QtWidgets.QPushButton(text=self.text)
-            self.ui.clicked.connect(self.callback)
+        self.ui.clicked.connect(self._clicked)
+        super().update(prev)
```

### Comparing `QPUIQ-0.1.9/PUI/PySide6/canvas.py` & `QPUIQ-0.2.0/PUI/PySide6/canvas.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,109 +2,81 @@
 from .base import *
 
 from PySide6 import QtWidgets, QtGui
 from PySide6.QtGui import QPainter, QColor
 from PySide6.QtCore import QPoint
 
 class PUIQtCanvas(QtWidgets.QWidget):
-    def __init__(self, puinode, width=None, height=None):
-        self.puinode = puinode
+    def __init__(self, node, width=None, height=None):
+        self.node = node
         self.width = width
         self.height = height
         super().__init__()
 
     def minimumSizeHint(self):
         return QtCore.QSize(self.width, self.height)
 
     def paintEvent(self, event):
-        qpainter = QPainter()
-        qpainter.begin(self)
+        while self.node.retired_by:
+            self.node = self.node.retired_by
+        self.node.qpainter = QPainter()
+        self.node.qpainter.begin(self)
 
-        if not self.puinode.bgColor is None:
+        if not self.node.bgColor is None:
             bgBrush = QtGui.QBrush()
-            bgBrush.setColor(QtGui.QColor(self.puinode.bgColor))
+            bgBrush.setColor(QtGui.QColor(self.node.bgColor))
             bgBrush.setStyle(QtCore.Qt.SolidPattern)
-            rect = QtCore.QRect(0, 0, qpainter.device().width, qpainter.device().height)
-            qpainter.fillRect(rect, bgBrush)
+            rect = QtCore.QRect(0, 0, self.node.qpainter.device().width, self.node.qpainter.device().height)
+            self.node.qpainter.fillRect(rect, bgBrush)
 
-        for c in self.puinode.children:
-            c.draw(qpainter)
+        self.node.painter(self.node, *self.node.args)
 
-        qpainter.end()
+        self.node.qpainter.end()
+        self.node.qpainter = None
 
 class QtCanvas(QtBaseWidget):
-    def __init__(self, bgColor=None):
+    def __init__(self, painter, *args, bgColor=None):
         super().__init__()
         self.ui = None
+        self.painter = painter
+        self.args = args
         self.bgColor = bgColor
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
             self.ui.puinode = self
         else:
             self.ui = PUIQtCanvas(self, self.layout_width or 0, self.layout_height or 0)
         self.ui.update()
+        super().update(prev)
 
-class QtCanvasText(PUINode):
-    def __init__(self, x, y, text):
-        super().__init__()
-        self.x = x
-        self.y = y
-        self.text = text
-
-    def update(self, prev):
-        pass
-
-    def draw(self, qpainter):
-        qpainter.drawText(QPoint(int(self.x), int(self.y)), self.text)
-
-class QtCanvasLine(PUINode):
-    def __init__(self, x1, y1, x2, y2, color=None, width=None):
-        super().__init__()
-        self.x1 = x1
-        self.y1 = y1
-        self.x2 = x2
-        self.y2 = y2
-        self.color = color
-        self.width = width
-
-    def update(self, prev):
-        pass
-
-    def draw(self, qpainter):
-        pen = qpainter.pen()
-        color = pen.color()
-        width = pen.width()
-        if not self.color is None:
-            pen.setColor(QColor(self.color))
-        if not self.width is None:
-            pen.setWidth(self.width)
-        qpainter.setPen(pen)
-        qpainter.drawLine(self.x1, self.y1, self.x2, self.y2)
-        pen.setColor(color)
-        pen.setWidth(width)
-        qpainter.setPen(pen)
-
-class QtCanvasPolyline(PUINode):
-    def __init__(self, coords, color=None, width=None):
-        super().__init__()
-        self.coords = coords
-        self.color = color
-        self.width = width
-
-    def update(self, prev):
-        pass
+    def drawText(self, x, y, text):
+        self.qpainter.drawText(QPoint(int(x), int(y)), text)
 
-    def draw(self, qpainter):
-        pen = qpainter.pen()
-        color = pen.color()
-        width = pen.width()
-        if not self.color is None:
-            pen.setColor(QColor(self.color))
-        if not self.width is None:
-            pen.setWidth(self.width)
-        qpainter.setPen(pen)
-        qpainter.drawPolyline([QtCore.QPointF(x,y) for x,y in self.coords])
-        pen.setColor(color)
-        pen.setWidth(width)
-        qpainter.setPen(pen)
+    def drawLine(self, x1, y1, x2, y2, color=None, width=None):
+        pen = self.qpainter.pen()
+        orig_color = pen.color()
+        orig_width = pen.width()
+        if not color is None:
+            pen.setColor(QColor(color))
+        if not width is None:
+            pen.setWidth(width)
+        self.qpainter.setPen(pen)
+        self.qpainter.drawLine(x1, y1, x2, y2)
+        pen.setColor(orig_color)
+        pen.setWidth(orig_width)
+        self.qpainter.setPen(pen)
+
+    def drawPolyline(self, coords, color=None, width=None):
+        pen = self.qpainter.pen()
+        orig_color = pen.color()
+        orig_width = pen.width()
+        if not color is None:
+            pen.setColor(QColor(color))
+        if not width is None:
+            pen.setWidth(width)
+        self.qpainter.setPen(pen)
+        self.qpainter.drawPolyline([QtCore.QPointF(x,y) for x,y in coords])
+        pen.setColor(orig_color)
+        pen.setWidth(orig_width)
+        self.qpainter.setPen(pen)
```

### Comparing `QPUIQ-0.1.9/PUI/PySide6/layout.py` & `QPUIQ-0.2.0/PUI/PySide6/layout.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,25 +2,32 @@
 from .base import *
 
 class QtHBox(QtBaseLayout):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
-            from PySide6 import QtWidgets
             self.ui = QtWidgets.QHBoxLayout()
-            self.ui.setObjectName(self.key)
+        super().update(prev)
 
 class QtVBox(QtBaseLayout):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
             self.ui = QtWidgets.QVBoxLayout()
-            self.ui.setObjectName(self.key)
+        super().update(prev)
+
+class QtSpacerItem(PUINode):
+    terminal = True
 
-class QtSpacerItem(QtBaseWidget):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
             self.ui = QtWidgets.QSpacerItem(0, 0, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
+        super().update(prev)
+
+    def destroy(self, direct):
+        # self.ui.deleteLater() # QSpacerItem doesn't have .deleteLater()
+        self.ui = None
+        super().destroy(direct)
```

### Comparing `QPUIQ-0.1.9/PUI/PySide6/textfield.py` & `QPUIQ-0.2.0/PUI/PySide6/textfield.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,10 +16,11 @@
                 self.ui.textChanged.connect(self.on_textchanged)
             self.last_value = value
         else:
             self.last_value = value
             self.ui = QtWidgets.QLineEdit()
             self.ui.setText(str(value))
             self.ui.textChanged.connect(self.on_textchanged)
+        super().update(prev)
 
     def on_textchanged(self):
         self.model.value = self.ui.text()
```

### Comparing `QPUIQ-0.1.9/PUI/Qt5/button.py` & `QPUIQ-0.2.0/PUI/tkinter/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from .. import *
-from .base import *
-
-class QtButton(QtBaseWidget):
-    def __init__(self, text, callback=None):
+import tkinter as tk
+from tkinter import ttk
+class TkBaseWidget(PUINode):
+    def __init__(self, layout=None, side=None, **kwargs):
         super().__init__()
-        self.text = text
-        self.callback = callback
+        self.layout_type = layout
+        self.side = side
+        self.kwargs = kwargs
+
+    @property
+    def tkparent(self):
+        parent = self.parent
+        while not isinstance(parent, TkBaseWidget):
+            parent = parent.parent
+        return parent
 
-    def update(self, prev):
-        if prev and hasattr(prev, "ui"):
-            self.ui = prev.ui
-            self.ui.setText(self.text)
-            try:
-                self.ui.clicked.disconnect()
-            except:
-                pass
-            self.ui.clicked.connect(self.callback)
-        else:
-            self.ui = QtWidgets.QPushButton(text=self.text)
-            self.ui.clicked.connect(self.callback)
+    def destroy(self, direct):
+        if self.ui:
+            self.ui.destroy() # tk's destroy
+            self.ui = None
```

### Comparing `QPUIQ-0.1.9/PUI/Qt5/canvas.py` & `QPUIQ-0.2.0/PUI/textual/application.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,56 @@
+from typing import Type
+from textual.driver import Driver
 from .. import *
 from .base import *
+from textual.app import App, CSSPathType, ComposeResult
+from textual.containers import Vertical
+from textual.widgets import Button, Checkbox, Input, RadioButton
 
-from PyQt5 import QtWidgets
-from PyQt5.QtGui import QPainter, QColor
-from PyQt5.QtCore import QPoint
-
-class PUIQtCanvas(QtWidgets.QWidget):
-    def __init__(self, puinode):
-        self.puinode = puinode
-        super().__init__()
+class PUIApp(App):
 
-    def paintEvent(self, event):
-        qpainter = QPainter()
-        qpainter.begin(self)
-
-        for c in self.puinode.children:
-            c.draw(qpainter)
-
-        qpainter.end()
-
-class QtCanvas(QtBaseWidget):
-    def __init__(self, size=None, **kwargs):
-        super().__init__(**kwargs)
-        self.size = size
-
-    def update(self, prev):
-        if prev and hasattr(prev, "ui"):
-            self.ui = prev.ui
-            self.ui.puinode = self
-        else:
-            self.ui = PUIQtCanvas(self)
-        x = 0
-        y = 0
-        w = 0
-        h = 0
-        if not self.size is None:
-            w, h = self.size
-        self.ui.setGeometry(x, y, w, h)
-        self.ui.update()
+    def __init__(self, puiview, driver_class: Type[Driver] | None = None, css_path: CSSPathType | None = None, watch_css: bool = False):
+        super().__init__(driver_class, css_path, watch_css)
+        self.puiview = puiview
 
-class QtCanvasText(PUINode):
-    def __init__(self, x, y, text):
-        super().__init__()
-        self.x = x
-        self.y = y
-        self.text = text
+    def on_mount(self) -> None:
+        self.puiview.redraw()
+
+    def on_button_pressed(self, event: Button.Pressed) -> None:
+        event.button.puinode._clicked()
+
+    def on_radio_button_changed(self, event: RadioButton.Changed) -> None:
+        event.radio_button.puinode._changed(event.value)
+
+    def on_input_changed(self, event: Input.Changed) -> None:
+        event.input.puinode._changed(event.value)
+
+    def on_input_submitted(self, event: Input.Submitted) -> None:
+        event.input.puinode._submitted(event.value)
 
-    def update(self, prev):
-        pass
+    def on_checkbox_changed(self, event: Checkbox.Changed) -> None:
+        event.checkbox.puinode._changed(event.value)
 
-    def draw(self, qpainter):
-        qpainter.drawText(QPoint(int(self.x), int(self.y)), self.text)
+    def compose(self) -> ComposeResult:
+        yield Vertical(id="frame")
 
-class QtCanvasLine(PUINode):
-    def __init__(self, *args, **kwargs):
+class TApplication(PUIView):
+    def __init__(self):
         super().__init__()
-        self.args = args
-        self.kwargs = kwargs
+        self.ui = PUIApp(self)
 
-    def update(self, prev):
-        pass
+    def addChild(self, idx, child):
+        if idx>0:
+            raise RuntimeError("Textual port only support single window")
+        self.ui.query_one("#frame").mount(child.outer)
+
+    def redraw(self):
+        with self.ui.batch_update():
+            self.update()
+
+    def run(self):
+        self.setup()
+        # self.redraw() # need to be after on_mount
+        self.start()
 
-    def draw(self, qpainter):
-        qpainter.drawLine(*self.args)
+    def start(self):
+        self.ui.run()
```

### Comparing `QPUIQ-0.1.9/PUI/Qt5/textfield.py` & `QPUIQ-0.2.0/PUI/textual/textfield.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from .. import *
 from .base import *
 
-class QtLineEdit(QtBaseWidget):
+class TInput(TBase):
     def __init__(self, model):
         super().__init__()
         self.model = model
 
     def update(self, prev):
-        value = self.model.value
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
-            if prev.last_value != value:
-                self.ui.textChanged.disconnect()
-                self.ui.setText(str(value))
-                self.ui.textChanged.connect(self.on_textchanged)
-            self.last_value = value
+            model_value = self.model.value
+            if self.ui_text != model_value:
+                self.ui_text = model_value
+                self.ui.value = model_value
         else:
-            self.last_value = value
-            self.ui = QtWidgets.QLineEdit()
-            self.ui.setText(str(value))
-            self.ui.textChanged.connect(self.on_textchanged)
+            self.ui_text = self.model.value
+            self.ui = widgets.Input(self.ui_text)
 
-    def on_textchanged(self):
-        self.model.value = self.ui.text()
+        self.ui.puinode = self
+
+
+    def _changed(self, value):
+        self.ui_text = value
+        self.model.value = value
+
+    def _submitted(self, value):
+        pass
```

### Comparing `QPUIQ-0.1.9/PUI/Qt5/window.py` & `QPUIQ-0.2.0/PUI/textual/label.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 from .. import *
 from .base import *
 
-class QtWindow(PUINode):
-    def __init__(self, title=None, size=None):
-        super().__init__()
-        self.title = title
-        self.size = size
+class TLabel(TBase):
+    def __init__(self, text, **kwargs):
+        super().__init__(**kwargs)
+        self.text = text
 
-    def update(self, prev=None):
+    def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
+            self.widget = prev.widget
         else:
-            from PyQt5 import QtWidgets
-            self.ui = QtWidgets.QWidget()
-            self.ui.setObjectName("Window")
-            self.box = QtWidgets.QBoxLayout(QtWidgets.QBoxLayout.Direction.LeftToRight)
-            self.ui.setLayout(self.box)
-
-        if not self.title is None:
-            self.ui.setWindowTitle(self.title)
-        if not self.size is None:
-            self.ui.resize(*self.size)
-
-        super().update(prev)
-
-    def addChild(self, idx, child):
-        if isinstance(child, QtBaseLayout):
-            self.box.addLayout(child.ui)
-        elif isinstance(child, QtBaseWidget):
-            self.box.addWidget(child.ui)
-        else:
-            self.addChild(idx, child.children[0])
-
-    def removeChild(self, idx, child):
-        if isinstance(child, QtBaseLayout):
-            self.box.removeItem(child.ui)
-        elif isinstance(child, QtBaseWidget):
-            child.ui.setParent(None)
+            self.ui = containers.Container()
+            self.ui.set_styles("width: auto; height: auto;")
+            self.widget = None
+        if self.onClicked:
+            if self.widget is None or not isinstance(self.widget, widgets.Button):
+                if self.widget:
+                    self.widget.remove()
+                self.widget = widgets.Button(self.text)
+                self.widget.set_styles("height: 1; border-top: none; border-bottom: none; min-width: 0;")
+                self.widget.puinode = self
+                self.ui.mount(self.widget)
+            else:
+                self.widget.label = self.text
         else:
-            self.removeChild(idx, child.children[0])
+            if self.widget is None or not isinstance(self.widget, widgets.Label):
+                if self.widget:
+                    self.widget.remove()
+                self.widget = widgets.Label(self.text, markup=False)
+                self.ui.mount(self.widget)
+            else:
+                self.widget.update(self.text)
```

### Comparing `QPUIQ-0.1.9/PUI/dom.py` & `QPUIQ-0.2.0/PUI/dom.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # dprint = print
 dprint = lambda *x: x
 
-def recur_delete(node, idx, child):
+def recur_delete(node, idx, child, direct):
+    child.destroyed = True
     for sidx,sc in enumerate(child.children):
-        recur_delete(child, sidx, sc)
-    node.removeChild(idx, child)
-    child.destroy()
+        recur_delete(child, sidx, sc, False)
+    child.destroy(direct)
 
-def sync(node, oldDOM, newDOM, children_first):
+def sync(node, oldDOM, newDOM):
     dprint("syncing", node.key, len(oldDOM), len(newDOM))
     dprint("  ===OLD===")
     for c in oldDOM:
         dprint("   ", c.key)
     dprint("  ===NEW===")
     for c in newDOM:
         dprint("   ", c.key)
@@ -23,21 +23,21 @@
             oldMap[i] = None
             old = oldDOM[i]
             new = newDOM[i]
             try:
                 new.update(old)
             except:
                 import traceback
-                print("## <ERROR OF sync() >")
+                print("## <ERROR OF update() >")
                 print(node.key)
                 traceback.print_exc()
-                print("## </ERROR OF sync()>")
+                print("## </ERROR OF update()>")
 
             if not new.terminal:
-                sync(new, old.children, new.children, children_first)
+                sync(new, old.children, new.children)
             skipHead += 1
         else:
             break
 
     skipTail = 0
     # for i in range(0, min(len(oldDOM)-skipHead, len(newDOM)-skipHead)):
     #     if oldDOM[-1-i].key == newDOM[-1-i].key:
@@ -56,25 +56,35 @@
             old_idx = oldMap.index(new.key)
         except:
             old_idx = -1
         if old_idx >= 0:
             oldMap[old_idx] = None
             old = oldDOM[old_idx]
             node.removeChild(old_idx, old)
-            new.update(old)
-            if not new.terminal and children_first:
-                sync(new, old.children, new.children, children_first)
+            try:
+                new.update(old)
+            except:
+                import traceback
+                print("## <ERROR OF update() >")
+                print(new.key)
+                traceback.print_exc()
+                print("## </ERROR OF update()>")
+            if not new.terminal:
+                sync(new, old.children, new.children)
             node.addChild(new_idx, old)
-            if not new.terminal and not children_first:
-                sync(new, old.children, new.children, children_first)
         else:
-            new.update(None)
-            if not new.terminal and children_first:
-                sync(new, [], new.children, children_first)
+            try:
+                new.update(None)
+            except:
+                import traceback
+                print("## <ERROR OF update() >")
+                print(new.key)
+                traceback.print_exc()
+                print("## </ERROR OF update()>")
+            if not new.terminal:
+                sync(new, [], new.children)
             node.addChild(new_idx, new)
-            if not new.terminal and not children_first:
-                sync(new, [], new.children, children_first)
 
     for old_idx, key in enumerate(oldMap):
         if key:
             old = oldDOM[old_idx]
-            recur_delete(node, old_idx, old)
+            recur_delete(node, old_idx, old, True)
```

### Comparing `QPUIQ-0.1.9/PUI/flet/application.py` & `QPUIQ-0.2.0/PUI/flet/application.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from .. import *
 from .base import *
 
 class FApplication(PUIView):
     def __init__(self):
         super().__init__()
         self.ready = False
-        self.children_first = True
 
     def update(self, prev=None):
         if not self.ready:
             return
         super().update()
 
     def flet_app(self, page: ft.Page):
```

### Comparing `QPUIQ-0.1.9/PUI/flet/button.py` & `QPUIQ-0.2.0/PUI/tkinter/label.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from .. import *
 from .base import *
-
-class FElevatedButton(FBase):
-    def __init__(self, text, callback=None, **kwargs):
+class TkLabel(TkBaseWidget):
+    def __init__(self, text, **kwargs):
         super().__init__(**kwargs)
         self.text = text
-        self.callback = callback
-        self.kwargs = kwargs
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
-            self.ui.text = self.text
-            self.ui.on_click = self.on_click
-            self.ui.update()
+            self.ui.config(text = self.text)
         else:
-            self.ui = ft.ElevatedButton(text=self.text, on_click=self.on_click, expand=self.layout_weight, **self.kwargs)
-
-    def on_click(self, *args):
-        self.callback()
+            self.ui = tk.Label(self.parent.ui, text=self.text, **self.kwargs)
+            self.ui.bind("<Button-1>", self._clicked)
+        if self.onClicked:
+            self.ui.config(cursor="")
```

### Comparing `QPUIQ-0.1.9/PUI/flet/layout.py` & `QPUIQ-0.2.0/PUI/flet/layout.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,34 +5,34 @@
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
             self.ui = ft.Row(expand=self.layout_weight)
 
     def addChild(self, idx, child):
-        self.ui.controls.append(child.ui)
+        self.ui.controls.append(child.outer)
         try:
             self.ui.update()
         except:
             pass
 
     def removeChild(self, idx, child):
-        self.ui.controls.remove(child.ui)
+        self.ui.controls.remove(child.outer)
         self.ui.update()
 
 class FColumn(FBase):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
             self.ui = ft.Column(expand=self.layout_weight)
 
     def addChild(self, idx, child):
-        self.ui.controls.append(child.ui)
+        self.ui.controls.append(child.outer)
         try:
             self.ui.update()
         except:
             pass
 
     def removeChild(self, idx, child):
-        self.ui.controls.remove(child.ui)
+        self.ui.controls.remove(child.outer)
         self.ui.update()
```

### Comparing `QPUIQ-0.1.9/PUI/flet/textfield.py` & `QPUIQ-0.2.0/PUI/flet/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.9/PUI/node.py` & `QPUIQ-0.2.0/PUI/node.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 import threading
+from .utils import *
 
 tls = threading.local()
 
 class PuiViewNotFoundError(Exception): pass
 
 def find_puiview():
     try:
         return tls.puistack[-1]
     except:
         raise PuiViewNotFoundError()
 
 class PUINode():
+    supported = True
     terminal = False
     def __init__(self, *args):
         from .view import PUIView
 
         if not hasattr(self, "name"):
             self.name = None
 
+        self.destroyed = False
+        self.retired_by = None
+        self._debug = 0
+
         self.layout_weight = None
         self.layout_width = None
         self.layout_height = None
-        self.layout_params = {}
+        self.layout_padding = None
+        self.layout_margin = None
+
+        self.onClicked = None
 
         self.ui = None
         self.args = args
         try:
             self.root = find_puiview()
             self.parent = self.root.frames[-1]
         except PuiViewNotFoundError:
@@ -66,25 +75,31 @@
     def outer(self):
         return self.ui
 
     def comment(self):
         return None
 
     def update(self, prev):
-        return None
+        if prev:
+            prev.retired_by = self
 
-    def destroy(self):
-        return None
+    def destroy(self, direct):
+        self.root = None
+        self.parent = None
 
-    def addChild(self, idx, ui):
+    def addChild(self, idx, child):
         pass
 
-    def removeChild(self, idx, ui):
+    def removeChild(self, idx, child):
         pass
 
+    def debug(self, level=1):
+        self._debug = level
+        return self
+
     def __repr__(self):
         segs = []
         headline = [
             "  "*len(self.path),
             self.name or type(self).__name__,
             # f"@{str(id(self))}", # print view id
             " {",
@@ -108,19 +123,36 @@
             if i > 0:
                 segs.append(",\n")
             segs.append(c.__repr__())
         segs.append("\n")
         segs.append("".join(["  "*len(self.path), "}"]))
         return "".join(segs)
 
-    def layout(self, width=None, height=None, weight=None, **kwargs):
+    def layout(self, width=None, height=None, weight=None, padding=None, margin=None):
         if not width is None:
             self.layout_width = width
         if not height is None:
             self.layout_height = height
         if not weight is None:
             self.layout_weight = weight
+        if not padding is None:
+            self.layout_padding = trbl(padding)
+        if not margin is None:
+            self.layout_margin = trbl(margin)
+
+        return self
+
+    def click(self, callback, *cb_args, **cb_kwargs):
+        self.onClicked = callback
+        self.click_args = cb_args
+        self.click_kwargs = cb_kwargs
+        return self
 
-        for k,v in kwargs.items():
-            self.layout_params[k] = v
+    def _clicked(self, *args, **kwargs):
+        node = self
+        while node.retired_by:
+            node = node.retired_by
+        if node.onClicked:
+            node.onClicked(*self.click_args, **self.click_kwargs)
 
+    def qt(self, **kwargs):
         return self
```

### Comparing `QPUIQ-0.1.9/PUI/timeline.py` & `QPUIQ-0.2.0/PUI/timeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 from threading import Timer
 from .view import *
 
 class TimelineView(PUINode):
     def __init__(self, ttl_sec):
         super().__init__()
+        self.timer = None
         self.ttl_sec = ttl_sec
 
     def update(self, prev):
         if prev and hasattr(prev, "timer"):
             self.timer = prev.timer
         else:
             self.timer = Timer(self.ttl_sec, self.timer_cb)
             self.timer.start()
 
     def timer_cb(self):
-        try:
-            self.root.redraw()
-            self.timer = Timer(self.ttl_sec, self.timer_cb)
-            self.timer.start()
-        except:
-            pass
+        if not self.timer:
+            return
+        node = self
+        while node.retired_by:
+            node = node.retired_by
+        root = node.root
+        if not root:
+            return
+        root.redraw()
+        node.timer = Timer(self.ttl_sec, self.timer_cb)
+        node.timer.start()
 
     @property
-    def ui(self):
-        return self.children[0].ui
+    def inner(self):
+        return self.parent.inner
 
-    @ui.setter
-    def ui(self, new_ui):
-        pass
+    @property
+    def outer(self):
+        if self.children:
+            return self.children[0].outer
+        return None
 
-    def destroy(self):
+    def destroy(self, direct):
         timer = self.timer
         self.timer = None
         if timer:
             timer.cancel()
+        super().destroy(direct)
 
     def addChild(self, idx, child):
         self.parent.addChild(idx, child)
 
     def removeChild(self, idx, child):
         self.parent.removeChild(idx, child)
```

### Comparing `QPUIQ-0.1.9/PUI/tkinter/application.py` & `QPUIQ-0.2.0/PUI/tkinter/application.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 
         super().update(prev)
 
     def addChild(self, idx, child):
         pass
 
     def removeChild(self, idx, child):
-        child.ui.destroy()
+        pass
 
     def start(self):
         self.ui.mainloop()
```

### Comparing `QPUIQ-0.1.9/PUI/tkinter/canvas.py` & `QPUIQ-0.2.0/PUI/tkinter/canvas.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,42 @@
 from .. import *
 from .base import *
+import itertools
 class TkCanvas(TkBaseWidget):
     terminal = True
-    def __init__(self, size=None, **kwargs):
-        super().__init__(**kwargs)
+    def __init__(self, painter, *args, size=None, bgColor=None):
+        super().__init__()
+        self.painter = painter
+        self.args = args
         self.size = size
+        self.bgColor = bgColor
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
             self.ui = tk.Canvas(self.parent.ui, **self.kwargs)
         self.ui.delete("all")
 
-        for c in self.children:
-            c.update(None)
+        if self.bgColor:
+            self.ui.config(bg=f"#{self.bgColor:06X}")
 
+        self.painter(self, *self.args)
 
-class TkCanvasText(PUINode):
-    def __init__(self, x, y, text):
-        super().__init__()
-        self.x = x
-        self.y = y
-        self.text = text
+    def drawText(self, x, y, text):
+        self.ui.create_text(x, y, text=text)
 
-    def update(self, prev):
-        self.parent.ui.create_text(self.x, self.y, text=self.text)
-
-class TkCanvasLine(PUINode):
-    def __init__(self, x1, y1, x2, y2, color=None, width=None):
-        super().__init__()
-        self.x1 = x1
-        self.y1 = y1
-        self.x2 = x2
-        self.y2 = y2
-        self.color = color
-        self.width = width
-
-    def update(self, prev):
+    def drawLine(self, x1, y1, x2, y2, color=None, width=None):
         params = {}
-        if not self.color is None:
-            params["fill"] = f"#{self.color:06X}"
-        if not self.width is None:
-            params["width"] = self.width
-        self.parent.ui.create_line(self.x1, self.y1, self.x2, self.y2, **params)
-class TkCanvasPolyline(PUINode):
-    def __init__(self, coords, color=None, width=None):
-        super().__init__()
-        self.coords = coords
-        self.color = color
-        self.width = width
+        if not color is None:
+            params["fill"] = f"#{color:06X}"
+        if not width is None:
+            params["width"] = width
+        self.ui.create_line(x1, y1, x2, y2, **params)
 
-    def update(self, prev):
+    def drawPolyline(self, coords, color=None, width=None):
         params = {}
-        if not self.color is None:
-            params["fill"] = f"#{self.color:06X}"
-        if not self.width is None:
-            params["width"] = self.width
-        self.parent.ui.create_line(*self.coords, **params)
+        if not color is None:
+            params["fill"] = f"#{color:06X}"
+        if not width is None:
+            params["width"] = width
+        self.ui.create_line(*itertools.chain(*coords), **params)
```

### Comparing `QPUIQ-0.1.9/PUI/tkinter/layout.py` & `QPUIQ-0.2.0/PUI/tkinter/layout.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,47 +3,62 @@
 
 class TkHBox(TkBaseWidget):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
             self.ui = tk.Frame(self.tkparent.inner)
-            self.ui.rowconfigure(0, weight=1)
+            self.ui.grid_rowconfigure(0, weight=1)
 
     def addChild(self, idx, child):
         if isinstance(child, TkBaseWidget):
             child.ui.grid(row=0, column=idx, sticky='nsew')
-            if not child.layout_weight is None:
-                self.ui.columnconfigure(idx, weight=child.layout_weight)
+            if child.layout_weight is None:
+                self.ui.grid_columnconfigure(idx, weight=0)
+            else:
+                self.ui.grid_columnconfigure(idx, weight=child.layout_weight)
         elif child.children:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
+        self.ui.grid_columnconfigure(idx, weight=0)
         if isinstance(child, TkBaseWidget):
             child.ui.grid_forget()
         elif child.children:
             self.removeChild(idx, child.children[0])
 
 class TkVBox(TkBaseWidget):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
             self.ui = tk.Frame(self.tkparent.inner)
             self.ui.config(bg="white")
-            self.ui.columnconfigure(0, weight=1)
+            self.ui.grid_columnconfigure(0, weight=1)
 
     def addChild(self, idx, child):
         if isinstance(child, TkBaseWidget):
             child.ui.grid(row=idx, column=0, sticky='nsew')
-            if not child.layout_weight is None:
-                self.ui.rowconfigure(idx, weight=child.layout_weight)
+            if child.layout_weight is None:
+                self.ui.grid_rowconfigure(idx, weight=0)
+            else:
+                self.ui.grid_rowconfigure(idx, weight=child.layout_weight)
         elif child.children:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
+        self.ui.grid_rowconfigure(idx, weight=0)
         if isinstance(child, TkBaseWidget):
             child.ui.grid_forget()
         elif child.children:
             self.removeChild(idx, child.children[0])
 
+class TkSpacer(TkBaseWidget):
+    def __init__(self, *args):
+        super().__init__(*args)
+        self.layout_weight = 1
 
+    def update(self, prev):
+        if prev and hasattr(prev, "ui"):
+            self.ui = prev.ui
+        else:
+            self.ui = tk.Frame(self.tkparent.inner)
```

### Comparing `QPUIQ-0.1.9/PUI/tkinter/textfield.py` & `QPUIQ-0.2.0/PUI/tkinter/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.9/PUI/urwid/layout.py` & `QPUIQ-0.2.0/PUI/textual/layout.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 from .. import *
 from .base import *
 
-class UColumns(UBase):
+class TVertical(TBase):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
-            self.ui = urwid.Columns([])
+            self.ui = containers.Vertical()
+            self.ui.set_styles("height: auto;")
 
     def addChild(self, idx, child):
-        self.ui.contents.append((child.ui, self.ui.options()))
+        self.inner.mount(child.outer)
 
     def removeChild(self, idx, child):
-        self.ui.contents.pop(idx)
+        child.tremove()
 
-
-class UPile(UBase):
+class THorizontal(TBase):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
-            self.ui = urwid.Pile([])
+            self.ui = containers.Horizontal()
+            self.ui.set_styles("width: auto;")
 
     def addChild(self, idx, child):
-        self.ui.contents.append((child.ui, self.ui.options()))
+        self.inner.mount(child.outer)
 
     def removeChild(self, idx, child):
-        self.ui.contents.pop(idx)
+        child.tremove()
+
+class TSpacer(TBase):
+    def update(self, prev):
+        if prev and hasattr(prev, "ui"):
+            self.ui = prev.ui
+        else:
+            self.ui = widgets.Static("")
+            self.ui.set_styles("width: 1fr; height: 1fr;")
```

### Comparing `QPUIQ-0.1.9/PUI/view.py` & `QPUIQ-0.2.0/PUI/view.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 from .dom import *
 import time
 
 # dprint = print
 dprint = lambda *x: x
 
 class PUIView(PUINode):
+    terminal = True
     __ALLVIEWS__  = []
 
     @staticmethod
     def reload():
         for v in PUIView.__ALLVIEWS__:
             v.redraw()
 
     def __init__(self, *args, **kwargs):
-        self.children_first = True # default to bottom-up
         self.frames = []
-        self.last_children = []
+        self.dirty = False
+        self.updating = False
         super().__init__(*args, **kwargs)
         PUIView.__ALLVIEWS__.append(self)
 
     def __enter__(self):
         if not hasattr(tls, "puistack"):
             tls.puistack = []
         tls.puistack.append(self)
@@ -31,60 +32,84 @@
     def __exit__(self, ex_type, value, traceback):
         tls.puistack.pop()
         # print("exit", type(self).__name__, id(self))
         self.root.frames.pop()
         if ex_type is None: # don't consume exception
             return self
 
-    def destroy(self):
-        PUIView.__ALLVIEWS__.remove(self)
-        return super().destroy()
-
     def content(self):
         return None
 
     def dump(self):
         dprint(f"content() start", self.key)
         start = time.time()
         with self as scope:
             self.content()
         dprint(f"content() time: {time.time()-start:.5f}", self.key)
         return scope
 
+    def destroy(self, direct):
+        PUIView.__ALLVIEWS__.remove(self)
+        return super().destroy(direct)
+
     def redraw(self):
         self.update()
 
     def update(self, prev=None):
+        if self.retired_by:
+            return
+        if self.destroyed:
+            return
         update_start = time.time()
         dprint("update()", self.key)
         if prev:
-            self.last_children = prev.children
+            self.children = prev.children
+            prev.retired_by = self
+            PUIView.__ALLVIEWS__.remove(prev)
 
+        last_children = self.children
         self.children = []
         try:
             dprint(f"content() start", self.key)
             start = time.time()
-            with self as scope: # CRITICAL: this is the searching target for find_pui()
+            with self as scope: # init frame stack
                 self.content() # V-DOM builder
             dprint(f"content() time: {time.time()-start:.5f}", self.key)
         except:
             # prevent crash in hot-reloading
-            self.children = self.last_children
+            self.children = last_children
             import traceback
-            print("## <ERROR OF content() >")
+            print("## <ERROR OF content() >", self.key, id(self))
             traceback.print_exc()
             print("## </ERROR OF content()>")
-
+            return
 
         # print("PUIView.update", self) # print DOM
 
         start = time.time()
         dprint("sync() start", self.key)
-        sync(self, self.last_children, self.children, self.children_first)
+        sync(self, last_children, self.children)
         dprint(f"sync() time: {time.time()-start:.5f}", self.key)
 
-        self.last_children = self.children
         dprint(f"update() time: {time.time()-update_start:.5f}", self.key)
 
+    def setup(self):
+        pass
+
     def run(self):
+        self.setup()
         self.redraw()
         self.start()
+
+    @property
+    def inner(self):
+        if self.ui:
+            return self.ui
+        return self.parent.inner
+
+    @property
+    def outer(self):
+        if self.ui:
+            return self.ui
+        if self.children:
+            return self.children[0].outer
+        return None
```

### Comparing `QPUIQ-0.1.9/QPUIQ.egg-info/SOURCES.txt` & `QPUIQ-0.2.0/QPUIQ.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -3,62 +3,61 @@
 setup.py
 PUI/__init__.py
 PUI/decorator.py
 PUI/dom.py
 PUI/node.py
 PUI/state.py
 PUI/timeline.py
+PUI/utils.py
 PUI/view.py
 PUI/PySide6/__init__.py
 PUI/PySide6/application.py
 PUI/PySide6/base.py
 PUI/PySide6/button.py
 PUI/PySide6/canvas.py
+PUI/PySide6/checkbox.py
+PUI/PySide6/combobox.py
 PUI/PySide6/label.py
 PUI/PySide6/layout.py
 PUI/PySide6/progressbar.py
+PUI/PySide6/radiobutton.py
 PUI/PySide6/scroll.py
+PUI/PySide6/text.py
 PUI/PySide6/textfield.py
 PUI/PySide6/window.py
-PUI/Qt5/__init__.py
-PUI/Qt5/application.py
-PUI/Qt5/base.py
-PUI/Qt5/button.py
-PUI/Qt5/canvas.py
-PUI/Qt5/label.py
-PUI/Qt5/layout.py
-PUI/Qt5/progressbar.py
-PUI/Qt5/textfield.py
-PUI/Qt5/window.py
 PUI/flet/__init__.py
 PUI/flet/application.py
 PUI/flet/base.py
 PUI/flet/button.py
 PUI/flet/label.py
 PUI/flet/layout.py
 PUI/flet/progressbar.py
 PUI/flet/textfield.py
 PUI/flet/window.py
+PUI/textual/__init__.py
+PUI/textual/application.py
+PUI/textual/base.py
+PUI/textual/button.py
+PUI/textual/checkbox.py
+PUI/textual/label.py
+PUI/textual/layout.py
+PUI/textual/progressbar.py
+PUI/textual/radiobutton.py
+PUI/textual/scroll.py
+PUI/textual/text.py
+PUI/textual/textfield.py
+PUI/textual/window.py
 PUI/tkinter/__init__.py
 PUI/tkinter/application.py
 PUI/tkinter/base.py
 PUI/tkinter/button.py
 PUI/tkinter/canvas.py
 PUI/tkinter/label.py
 PUI/tkinter/layout.py
 PUI/tkinter/progressbar.py
 PUI/tkinter/scroll.py
 PUI/tkinter/textfield.py
 PUI/tkinter/window.py
-PUI/urwid/__init__.py
-PUI/urwid/application.py
-PUI/urwid/base.py
-PUI/urwid/button.py
-PUI/urwid/label.py
-PUI/urwid/layout.py
-PUI/urwid/progressbar.py
-PUI/urwid/scroll.py
-PUI/urwid/window.py
 QPUIQ.egg-info/PKG-INFO
 QPUIQ.egg-info/SOURCES.txt
 QPUIQ.egg-info/dependency_links.txt
 QPUIQ.egg-info/top_level.txt
```

### Comparing `QPUIQ-0.1.9/setup.py` & `QPUIQ-0.2.0/setup.py`

 * *Files identical despite different names*

