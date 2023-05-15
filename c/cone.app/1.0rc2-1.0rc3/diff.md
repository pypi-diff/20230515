# Comparing `tmp/cone.app-1.0rc2.tar.gz` & `tmp/cone.app-1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cone.app-1.0rc2.tar", last modified: Wed Aug 12 11:45:40 2020, max compression
+gzip compressed data, was "dist/cone.app-1.0rc3.tar", last modified: Mon Oct 12 06:30:09 2020, max compression
```

## Comparing `cone.app-1.0rc2.tar` & `cone.app-1.0rc3.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1514 2020-07-09 09:13:30.000000 cone.app-1.0rc2/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2175 2020-08-12 11:44:47.000000 cone.app-1.0rc2/setup.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    24904 2020-08-12 11:44:59.000000 cone.app-1.0rc2/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)      138 2019-04-25 18:07:37.000000 cone.app-1.0rc2/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2949 2020-07-09 05:52:44.000000 cone.app-1.0rc2/TODO.rst
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    12708 2020-06-22 11:10:43.000000 cone.app-1.0rc2/src/cone/app/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/browser/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3091 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    15297 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/batch.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    13910 2020-06-23 12:14:35.000000 cone.app-1.0rc2/src/cone/app/browser/referencebrowser.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    10236 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/ajax.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    12762 2020-06-30 09:02:29.000000 cone.app-1.0rc2/src/cone/app/browser/actions.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/browser/static/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4549 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_428bca_256x240.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)       98 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      220 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-bg_flat_0_999999_40x100.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)      120 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-bg_inset-soft_95_fef1ec_1x100.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)       86 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)     3707 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_454545_256x240.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6988 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_555555_256x240.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4549 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_f0ad4e_256x240.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)     4369 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_ffffff_256x240.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)     3919 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_f6cf3b_256x240.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6986 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_999999_256x240.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)       99 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-bg_glass_75_ffffff_1x400.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)     3712 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_2e83ff_256x240.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)     3707 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_cd0a0a_256x240.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)      111 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-bg_glass_75_dadada_1x400.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)     3710 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_888888_256x240.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)      115 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-bg_glass_55_fbf9ee_1x400.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)     3710 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_222222_256x240.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)      110 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-bg_glass_75_e6e6e6_1x400.png
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)       87 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)    43824 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/jquery-ui-1.10.3.custom.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    84295 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/jquery-ui-1.10.3.custom.js
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)    22329 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/jquery-ui-1.10.3.custom.css
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)      112 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/jquery.ui.1.10.3.ie.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)      139 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/jquery-ui-1.10.3.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)      800 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/cookie_functions.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    92629 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jquery-1.9.1.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)   268381 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jquery-1.9.1.js
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/browser/static/typeahead/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    71417 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/typeahead/typeahead.bundle.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6240 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/typeahead/typeahead.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)      999 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/public.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1406 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/favicon.ico
--rw-r--r--   0 rnix      (1000) rnix      (1000)    16621 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jquery.migrate-1.2.1.js
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/browser/static/ionicons/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/browser/static/ionicons/css/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    47987 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/ionicons/css/ionicons.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)    42998 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/ionicons/css/ionicons.min.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)       31 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/ionicons/.gitignore
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/browser/static/ionicons/fonts/
--rw-r--r--   0 rnix      (1000) rnix      (1000)   164548 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/ionicons/fonts/ionicons.ttf
--rw-r--r--   0 rnix      (1000) rnix      (1000)    57276 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/ionicons/fonts/ionicons.woff
--rw-r--r--   0 rnix      (1000) rnix      (1000)   286345 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/ionicons/fonts/ionicons.svg
--rw-r--r--   0 rnix      (1000) rnix      (1000)   101984 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/ionicons/fonts/ionicons.eot
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/css/
--rw-r--r--   0 rnix      (1000) rnix      (1000)   132546 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/css/bootstrap.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)   109518 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)    18860 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.min.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)    21368 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.css
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/js/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    31819 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    60681 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/js/bootstrap.js
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/fonts/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    41280 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 rnix      (1000) rnix      (1000)    23320 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 rnix      (1000) rnix      (1000)    20335 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 rnix      (1000) rnix      (1000)    62927 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 rnix      (1000) rnix      (1000)       67 2020-08-12 10:25:44.000000 cone.app-1.0rc2/src/cone/app/browser/static/print.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)    21123 2020-08-12 09:19:29.000000 cone.app-1.0rc2/src/cone/app/browser/static/protected.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7199 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/static/jquery.migrate-1.2.1.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3811 2020-06-30 09:02:29.000000 cone.app-1.0rc2/src/cone/app/browser/static/styles.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)    17504 2020-06-15 06:03:46.000000 cone.app-1.0rc2/src/cone/app/browser/authoring.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2413 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/exception.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3700 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/login.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4048 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/contextmenu.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5563 2020-07-01 05:18:59.000000 cone.app-1.0rc2/src/cone/app/browser/copysupport.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2425 2020-06-15 07:12:36.000000 cone.app-1.0rc2/src/cone/app/browser/workflow.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7325 2020-06-15 06:03:46.000000 cone.app-1.0rc2/src/cone/app/browser/sharing.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/browser/templates/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1033 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/pathbar.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      700 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/resources.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      682 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/contextmenu_dropdown.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      551 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/contextmenu.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      561 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/navtree.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      979 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/navtree_recue.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      716 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/batched_items.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      420 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/logo.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2420 2020-06-22 11:10:43.000000 cone.app-1.0rc2/src/cone/app/browser/templates/mainmenu.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      363 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/not_found.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      220 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/sharing.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2571 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/batched_items_header.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      846 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/livesearch.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      845 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/add_dropdown.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      377 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/unauthorized.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      334 2020-06-15 06:03:46.000000 cone.app-1.0rc2/src/cone/app/browser/templates/footer.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1870 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/link_action.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      223 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/listing.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2283 2020-06-22 11:10:43.000000 cone.app-1.0rc2/src/cone/app/browser/templates/layout.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      697 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/byline.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      901 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/referencebrowser_pathbar.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7520 2020-08-12 11:21:44.000000 cone.app-1.0rc2/src/cone/app/browser/templates/table.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      627 2020-08-12 08:00:35.000000 cone.app-1.0rc2/src/cone/app/browser/templates/content_form.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/default_root.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      533 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/settings.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      916 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/action_dropdown.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      427 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/referencebrowser.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      402 2020-06-30 09:02:29.000000 cone.app-1.0rc2/src/cone/app/browser/templates/insufficient_privileges.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1438 2020-06-18 07:11:23.000000 cone.app-1.0rc2/src/cone/app/browser/templates/wf_dropdown.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1046 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/batched_items_footer.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      702 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/main.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      524 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/personaltools.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4362 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/templates/batch.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4713 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/form.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2127 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/settings.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3044 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/resources.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3534 2020-06-22 11:10:43.000000 cone.app-1.0rc2/src/cone/app/browser/utils.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    14705 2020-06-30 09:02:29.000000 cone.app-1.0rc2/src/cone/app/browser/layout.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7256 2020-08-12 09:47:20.000000 cone.app-1.0rc2/src/cone/app/browser/table.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7340 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/browser/contents.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      171 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/configure.zcml
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/locale/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/locale/de/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/locale/de/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5018 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/locale/de/LC_MESSAGES/cone.app.mo
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11417 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/locale/de/LC_MESSAGES/cone.app.po
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9896 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/locale/cone.app.pot
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/locale/en/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/locale/en/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4606 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/locale/en/LC_MESSAGES/cone.app.mo
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11000 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/locale/en/LC_MESSAGES/cone.app.po
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3816 2020-06-15 07:12:36.000000 cone.app-1.0rc2/src/cone/app/workflow.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7643 2020-06-30 09:02:29.000000 cone.app-1.0rc2/src/cone/app/security.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4915 2020-06-22 11:10:43.000000 cone.app-1.0rc2/src/cone/app/interfaces.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2980 2020-06-22 11:10:43.000000 cone.app-1.0rc2/src/cone/app/ugm.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      715 2020-07-01 05:18:59.000000 cone.app-1.0rc2/src/cone/app/compat.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    18346 2020-07-01 05:18:59.000000 cone.app-1.0rc2/src/cone/app/model.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1869 2020-02-03 10:06:50.000000 cone.app-1.0rc2/src/cone/app/utils.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/tests/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5002 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_exception.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3204 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    14792 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_form.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2394 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_testing.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2068 2020-06-18 07:11:23.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_workflow.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11044 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_sharing.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    38410 2020-06-15 06:03:46.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_referencebrowser.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    30511 2020-07-01 05:18:59.000000 cone.app-1.0rc2/src/cone/app/tests/test_model.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4015 2020-02-03 10:06:50.000000 cone.app-1.0rc2/src/cone/app/tests/test_utils.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8429 2020-07-01 05:18:59.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_copysupport.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5067 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_utils.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    13523 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_contents.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    16133 2020-06-15 06:03:46.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_ajax.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7976 2020-02-27 13:55:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_table.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    17821 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_security.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6965 2020-06-22 11:10:43.000000 cone.app-1.0rc2/src/cone/app/tests/test_app.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2977 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2299 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_login.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4570 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_contextmenu.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4141 2020-06-15 07:12:36.000000 cone.app-1.0rc2/src/cone/app/tests/test_workflow.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    49163 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_authoring.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    24683 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_actions.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    23548 2020-06-30 09:02:29.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_layout.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6227 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_settings.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    33452 2020-06-15 06:03:46.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_batch.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8108 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_browser_resources.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4537 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/tests/test_ugm.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/testing/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5084 2020-06-15 06:03:46.000000 cone.app-1.0rc2/src/cone/app/testing/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      959 2020-06-15 07:12:36.000000 cone.app-1.0rc2/src/cone/app/testing/dummy_workflow.zcml
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/testing/static/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       26 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/static/print2.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)       27 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/static/style1.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/static/script2.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/static/script1.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)       27 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/static/style2.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)       26 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/static/print1.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3313 2020-06-22 11:10:43.000000 cone.app-1.0rc2/src/cone/app/testing/mock.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      126 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/dummy_batched_items.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      393 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/dummy_form.yaml
--rw-r--r--   0 rnix      (1000) rnix      (1000)       36 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/dummy_action.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      234 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/dummy_main.pt
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/testing/data/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/testing/data/ugm/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/testing/data/ugm/userdata/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/testing/data/ugm/userdata/groups/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       50 2020-06-15 06:03:46.000000 cone.app-1.0rc2/src/cone/app/testing/data/ugm/userdata/groups/group1
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone/app/testing/data/ugm/userdata/users/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       42 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/data/ugm/userdata/users/max
--rw-r--r--   0 rnix      (1000) rnix      (1000)       44 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/data/ugm/userdata/users/manager
--rw-r--r--   0 rnix      (1000) rnix      (1000)       42 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/data/ugm/userdata/users/viewer
--rw-r--r--   0 rnix      (1000) rnix      (1000)       42 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/data/ugm/userdata/users/editor
--rw-r--r--   0 rnix      (1000) rnix      (1000)       44 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/data/ugm/userdata/users/sepp
--rw-r--r--   0 rnix      (1000) rnix      (1000)       40 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/data/ugm/userdata/users/admin
--rw-r--r--   0 rnix      (1000) rnix      (1000)       11 2020-07-01 12:55:14.000000 cone.app-1.0rc2/src/cone/app/testing/data/ugm/groups
--rw-r--r--   0 rnix      (1000) rnix      (1000)       81 2019-04-25 18:07:37.000000 cone.app-1.0rc2/src/cone/app/testing/data/ugm/roles
--rw-r--r--   0 rnix      (1000) rnix      (1000)      379 2020-07-01 12:55:14.000000 cone.app-1.0rc2/src/cone/app/testing/data/ugm/users
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone.app.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8415 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone.app.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone.app.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2019-04-25 18:08:00.000000 cone.app-1.0rc2/src/cone.app.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone.app.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      139 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone.app.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      331 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone.app.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone.app.egg-info/top_level.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)    35661 2020-08-12 11:45:40.000000 cone.app-1.0rc2/src/cone.app.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1130 2020-07-09 10:28:39.000000 cone.app-1.0rc2/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2020-08-12 11:45:40.000000 cone.app-1.0rc2/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)    35661 2020-08-12 11:45:40.000000 cone.app-1.0rc2/PKG-INFO
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2175 2020-10-12 06:29:32.000000 cone.app-1.0rc3/setup.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2949 2020-07-23 11:28:37.000000 cone.app-1.0rc3/TODO.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1514 2020-07-23 11:28:37.000000 cone.app-1.0rc3/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    25077 2020-10-12 06:29:48.000000 cone.app-1.0rc3/CHANGES.rst
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone.app.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      331 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone.app.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone.app.egg-info/top_level.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone.app.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone.app.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      139 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone.app.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8415 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone.app.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    35898 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone.app.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2020-05-13 20:10:09.000000 cone.app-1.0rc3/src/cone.app.egg-info/not-zip-safe
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7643 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/security.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    18346 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/model.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1869 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/utils.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3816 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/workflow.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      171 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/configure.zcml
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/locale/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/locale/de/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/locale/de/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5018 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/locale/de/LC_MESSAGES/cone.app.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11417 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/locale/de/LC_MESSAGES/cone.app.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/locale/en/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/locale/en/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4606 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/locale/en/LC_MESSAGES/cone.app.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11000 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/locale/en/LC_MESSAGES/cone.app.po
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9896 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/locale/cone.app.pot
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/testing/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       36 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/dummy_action.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3313 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/testing/mock.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      234 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/dummy_main.pt
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/testing/static/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/static/script1.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       26 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/static/print2.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       26 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/static/print1.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       27 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/static/style1.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       27 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/static/style2.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/static/script2.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      959 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/testing/dummy_workflow.zcml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      126 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/dummy_batched_items.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5084 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/testing/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/testing/data/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/testing/data/ugm/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      379 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/data/ugm/users
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       11 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/data/ugm/groups
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       81 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/data/ugm/roles
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/testing/data/ugm/userdata/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/testing/data/ugm/userdata/users/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       40 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/data/ugm/userdata/users/admin
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       44 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/data/ugm/userdata/users/manager
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       42 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/data/ugm/userdata/users/max
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       42 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/data/ugm/userdata/users/viewer
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       44 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/data/ugm/userdata/users/sepp
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       42 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/data/ugm/userdata/users/editor
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/testing/data/ugm/userdata/groups/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       50 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/testing/data/ugm/userdata/groups/group1
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      393 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/testing/dummy_form.yaml
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/browser/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3044 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/resources.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2413 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/exception.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    14705 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/browser/layout.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7256 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/table.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4713 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/form.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4048 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/contextmenu.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3534 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/browser/utils.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5563 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/browser/copysupport.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7325 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/browser/sharing.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/browser/static/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3811 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/browser/static/styles.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       67 2020-08-12 12:51:36.000000 cone.app-1.0rc3/src/cone/app/browser/static/print.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1406 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/favicon.ico
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/browser/static/ionicons/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       31 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/ionicons/.gitignore
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/browser/static/ionicons/css/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    42998 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/ionicons/css/ionicons.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    47987 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/ionicons/css/ionicons.css
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/browser/static/ionicons/fonts/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    57276 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/ionicons/fonts/ionicons.woff
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   101984 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/ionicons/fonts/ionicons.eot
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   164548 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/ionicons/fonts/ionicons.ttf
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   286345 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/ionicons/fonts/ionicons.svg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    21123 2020-08-12 12:51:36.000000 cone.app-1.0rc3/src/cone/app/browser/static/protected.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      999 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/public.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/browser/static/typeahead/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    71417 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/typeahead/typeahead.bundle.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6240 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/typeahead/typeahead.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7199 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jquery.migrate-1.2.1.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      800 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/cookie_functions.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    43824 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/jquery-ui-1.10.3.custom.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    84295 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/jquery-ui-1.10.3.custom.js
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)    22329 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/jquery-ui-1.10.3.custom.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      139 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/jquery-ui-1.10.3.rst
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)      112 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/jquery.ui.1.10.3.ie.css
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)       87 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      220 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-bg_flat_0_999999_40x100.png
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)     3707 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_454545_256x240.png
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)      115 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6988 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4549 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_428bca_256x240.png
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)     3712 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_2e83ff_256x240.png
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)     4369 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6986 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_999999_256x240.png
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)      120 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-bg_inset-soft_95_fef1ec_1x100.png
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)     3707 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_cd0a0a_256x240.png
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)      110 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)       99 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-bg_glass_75_ffffff_1x400.png
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)     3710 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_222222_256x240.png
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)       98 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-bg_glass_65_ffffff_1x400.png
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)       86 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4549 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_f0ad4e_256x240.png
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)     3919 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_f6cf3b_256x240.png
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)      111 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-bg_glass_75_dadada_1x400.png
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)     3710 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_888888_256x240.png
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/js/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    31819 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    60681 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/js/bootstrap.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/css/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    18860 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   109518 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   132546 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/css/bootstrap.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    21368 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.css
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/fonts/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    20335 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    41280 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    23320 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    62927 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    16621 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jquery.migrate-1.2.1.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   268381 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jquery-1.9.1.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    92629 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/static/jquery-1.9.1.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7340 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/contents.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    17504 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/authoring.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2425 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/browser/workflow.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3700 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/login.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    15297 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/batch.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10370 2020-09-29 15:46:29.000000 cone.app-1.0rc3/src/cone/app/browser/ajax.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3091 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2127 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/settings.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/browser/templates/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      845 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/add_dropdown.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      363 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/not_found.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2420 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/browser/templates/mainmenu.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      682 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/contextmenu_dropdown.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      697 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/byline.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      979 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/navtree_recue.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2571 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/batched_items_header.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1438 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/browser/templates/wf_dropdown.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7520 2020-08-12 12:51:36.000000 cone.app-1.0rc3/src/cone/app/browser/templates/table.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      702 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/main.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2283 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/browser/templates/layout.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1046 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/batched_items_footer.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      533 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/settings.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      223 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/listing.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      420 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/logo.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      524 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/personaltools.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      551 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/contextmenu.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      220 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/sharing.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      334 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/browser/templates/footer.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      901 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/referencebrowser_pathbar.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      427 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/referencebrowser.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/default_root.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      627 2020-08-12 12:51:36.000000 cone.app-1.0rc3/src/cone/app/browser/templates/content_form.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1870 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/link_action.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1033 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/pathbar.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      716 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/batched_items.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      561 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/navtree.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4362 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/batch.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      377 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/unauthorized.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      700 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/resources.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      402 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/browser/templates/insufficient_privileges.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      846 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/livesearch.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      916 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/browser/templates/action_dropdown.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    13910 2020-05-14 07:13:28.000000 cone.app-1.0rc3/src/cone/app/browser/referencebrowser.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12762 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/browser/actions.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12708 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-10-12 06:30:09.000000 cone.app-1.0rc3/src/cone/app/tests/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2299 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_login.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4570 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_contextmenu.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    30511 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/tests/test_model.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5067 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_utils.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    38410 2020-05-14 07:30:12.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_referencebrowser.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    16308 2020-09-29 15:46:29.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_ajax.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    33452 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_batch.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2068 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_workflow.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7976 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_table.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    14792 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_form.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6965 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/tests/test_app.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    23548 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_layout.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8429 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_copysupport.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4015 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_utils.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    49163 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_authoring.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4141 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/tests/test_workflow.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    24683 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_actions.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8108 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_resources.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3204 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    17821 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_security.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2394 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_testing.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6227 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_settings.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2977 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4537 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_ugm.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    13523 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_contents.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11044 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_sharing.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5002 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/app/tests/test_browser_exception.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2980 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/ugm.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      715 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/compat.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4915 2020-07-01 15:36:02.000000 cone.app-1.0rc3/src/cone/app/interfaces.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2020-05-13 20:05:13.000000 cone.app-1.0rc3/src/cone/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2020-10-12 06:30:09.000000 cone.app-1.0rc3/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      138 2020-05-13 20:05:13.000000 cone.app-1.0rc3/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    35898 2020-10-12 06:30:09.000000 cone.app-1.0rc3/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1130 2020-07-23 11:28:37.000000 cone.app-1.0rc3/README.rst
```

### Comparing `cone.app-1.0rc2/LICENSE.rst` & `cone.app-1.0rc3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/setup.py` & `cone.app-1.0rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '1.0rc2'
+version = '1.0rc3'
 shortdesc = 'Web application stub'
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
```

### Comparing `cone.app-1.0rc2/CHANGES.rst` & `cone.app-1.0rc3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changes
 =======
 
+1.0rc3 (2020-10-12)
+-------------------
+
+- ``cone.app.browser.ajax.AjaxEvent`` supports optional ``data`` argument
+  supported as of ``bdajax`` 1.13.
+  [rnix, 2020-09-29]
+
+
 1.0rc2 (2020-08-12)
 -------------------
 
 - Fix print CSS.
   [rnix, 2020-08-12]
 
 - Fix case when pasting to empty folder in copysupport JS.
```

### Comparing `cone.app-1.0rc2/TODO.rst` & `cone.app-1.0rc3/TODO.rst`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/__init__.py` & `cone.app-1.0rc3/src/cone/app/__init__.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/__init__.py` & `cone.app-1.0rc3/src/cone/app/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/batch.py` & `cone.app-1.0rc3/src/cone/app/browser/batch.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/referencebrowser.py` & `cone.app-1.0rc3/src/cone/app/browser/referencebrowser.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/ajax.py` & `cone.app-1.0rc3/src/cone/app/browser/ajax.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,18 +117,19 @@
 
 
 class AjaxEvent(object):
     """Ajax event configuration. Used to define continuation events for
     client side.
     """
 
-    def __init__(self, target, name, selector):
+    def __init__(self, target, name, selector, data=None):
         self.target = target
         self.name = name
         self.selector = selector
+        self.data = data
 
 
 class AjaxMessage(object):
     """Ajax Message configuration. Used to define continuation messages for
     client side.
     """
 
@@ -150,16 +151,17 @@
         self.css = css
         self.action = action
         self.target = target
         self.close = close
 
 
 class AjaxContinue(object):
-    """Convert ``AjaxAction`` and ``AjaxEvent`` instances to JSON response
-    definitions for bdajax continuation.
+    """Convert ``AjaxPath``, ``AjaxAction``, ``AjaxEvent``, ``AjaxMessage``
+    and  ``AjaxOverlay ``instances to JSON response definitions for bdajax
+    continuation.
     """
 
     def __init__(self, continuation):
         self.continuation = continuation
 
     @property
     def definitions(self):
@@ -188,15 +190,16 @@
                     'selector': definition.selector
                 })
             if isinstance(definition, AjaxEvent):
                 continuation.append({
                     'type': 'event',
                     'target': definition.target,
                     'name': definition.name,
-                    'selector': definition.selector
+                    'selector': definition.selector,
+                    'data': definition.data
                 })
             if isinstance(definition, AjaxMessage):
                 continuation.append({
                     'type': 'message',
                     'payload': definition.payload,
                     'flavor': definition.flavor,
                     'selector': definition.selector
```

### Comparing `cone.app-1.0rc2/src/cone/app/browser/actions.py` & `cone.app-1.0rc3/src/cone/app/browser/actions.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_428bca_256x240.png` & `cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_428bca_256x240.png`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_454545_256x240.png` & `cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_555555_256x240.png` & `cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_f0ad4e_256x240.png` & `cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_f0ad4e_256x240.png`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_ffffff_256x240.png` & `cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_f6cf3b_256x240.png` & `cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_f6cf3b_256x240.png`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_999999_256x240.png` & `cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_999999_256x240.png`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_2e83ff_256x240.png` & `cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_cd0a0a_256x240.png` & `cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_888888_256x240.png` & `cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/images/ui-icons_222222_256x240.png` & `cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/jquery-ui-1.10.3.custom.min.js` & `cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/jquery-ui-1.10.3.custom.min.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/jquery-ui-1.10.3.custom.js` & `cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/jquery-ui-1.10.3.custom.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jqueryui/jquery-ui-1.10.3.custom.css` & `cone.app-1.0rc3/src/cone/app/browser/static/jqueryui/jquery-ui-1.10.3.custom.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/cookie_functions.js` & `cone.app-1.0rc3/src/cone/app/browser/static/cookie_functions.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jquery-1.9.1.min.js` & `cone.app-1.0rc3/src/cone/app/browser/static/jquery-1.9.1.min.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jquery-1.9.1.js` & `cone.app-1.0rc3/src/cone/app/browser/static/jquery-1.9.1.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/typeahead/typeahead.bundle.js` & `cone.app-1.0rc3/src/cone/app/browser/static/typeahead/typeahead.bundle.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/typeahead/typeahead.css` & `cone.app-1.0rc3/src/cone/app/browser/static/typeahead/typeahead.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/public.js` & `cone.app-1.0rc3/src/cone/app/browser/static/public.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/favicon.ico` & `cone.app-1.0rc3/src/cone/app/browser/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jquery.migrate-1.2.1.js` & `cone.app-1.0rc3/src/cone/app/browser/static/jquery.migrate-1.2.1.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/ionicons/css/ionicons.css` & `cone.app-1.0rc3/src/cone/app/browser/static/ionicons/css/ionicons.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/ionicons/css/ionicons.min.css` & `cone.app-1.0rc3/src/cone/app/browser/static/ionicons/css/ionicons.min.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/ionicons/fonts/ionicons.ttf` & `cone.app-1.0rc3/src/cone/app/browser/static/ionicons/fonts/ionicons.ttf`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/ionicons/fonts/ionicons.woff` & `cone.app-1.0rc3/src/cone/app/browser/static/ionicons/fonts/ionicons.woff`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/ionicons/fonts/ionicons.svg` & `cone.app-1.0rc3/src/cone/app/browser/static/ionicons/fonts/ionicons.svg`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/ionicons/fonts/ionicons.eot` & `cone.app-1.0rc3/src/cone/app/browser/static/ionicons/fonts/ionicons.eot`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/css/bootstrap.css` & `cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/css/bootstrap.min.css` & `cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.min.css` & `cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.css` & `cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/js/bootstrap.min.js` & `cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/js/bootstrap.js` & `cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.woff` & `cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.eot` & `cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.svg` & `cone.app-1.0rc3/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/protected.js` & `cone.app-1.0rc3/src/cone/app/browser/static/protected.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/jquery.migrate-1.2.1.min.js` & `cone.app-1.0rc3/src/cone/app/browser/static/jquery.migrate-1.2.1.min.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/static/styles.css` & `cone.app-1.0rc3/src/cone/app/browser/static/styles.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/authoring.py` & `cone.app-1.0rc3/src/cone/app/browser/authoring.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/exception.py` & `cone.app-1.0rc3/src/cone/app/browser/exception.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/login.py` & `cone.app-1.0rc3/src/cone/app/browser/login.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/contextmenu.py` & `cone.app-1.0rc3/src/cone/app/browser/contextmenu.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/copysupport.py` & `cone.app-1.0rc3/src/cone/app/browser/copysupport.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/workflow.py` & `cone.app-1.0rc3/src/cone/app/browser/workflow.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/sharing.py` & `cone.app-1.0rc3/src/cone/app/browser/sharing.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/pathbar.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/pathbar.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/resources.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/resources.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/contextmenu_dropdown.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/contextmenu_dropdown.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/contextmenu.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/contextmenu.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/navtree.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/navtree.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/navtree_recue.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/navtree_recue.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/batched_items.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/batched_items.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/mainmenu.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/mainmenu.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/batched_items_header.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/batched_items_header.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/livesearch.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/livesearch.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/add_dropdown.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/add_dropdown.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/link_action.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/link_action.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/layout.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/byline.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/byline.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/referencebrowser_pathbar.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/referencebrowser_pathbar.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/table.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/table.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/content_form.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/content_form.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/settings.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/settings.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/action_dropdown.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/action_dropdown.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/wf_dropdown.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/wf_dropdown.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/batched_items_footer.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/batched_items_footer.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/main.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/main.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/personaltools.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/personaltools.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/templates/batch.pt` & `cone.app-1.0rc3/src/cone/app/browser/templates/batch.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/form.py` & `cone.app-1.0rc3/src/cone/app/browser/form.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/settings.py` & `cone.app-1.0rc3/src/cone/app/browser/settings.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/resources.py` & `cone.app-1.0rc3/src/cone/app/browser/resources.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/utils.py` & `cone.app-1.0rc3/src/cone/app/browser/utils.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/layout.py` & `cone.app-1.0rc3/src/cone/app/browser/layout.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/table.py` & `cone.app-1.0rc3/src/cone/app/browser/table.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/browser/contents.py` & `cone.app-1.0rc3/src/cone/app/browser/contents.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/locale/de/LC_MESSAGES/cone.app.mo` & `cone.app-1.0rc3/src/cone/app/locale/de/LC_MESSAGES/cone.app.mo`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/locale/de/LC_MESSAGES/cone.app.po` & `cone.app-1.0rc3/src/cone/app/locale/de/LC_MESSAGES/cone.app.po`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/locale/cone.app.pot` & `cone.app-1.0rc3/src/cone/app/locale/cone.app.pot`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/locale/en/LC_MESSAGES/cone.app.mo` & `cone.app-1.0rc3/src/cone/app/locale/en/LC_MESSAGES/cone.app.mo`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/locale/en/LC_MESSAGES/cone.app.po` & `cone.app-1.0rc3/src/cone/app/locale/en/LC_MESSAGES/cone.app.po`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/workflow.py` & `cone.app-1.0rc3/src/cone/app/workflow.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/security.py` & `cone.app-1.0rc3/src/cone/app/security.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/interfaces.py` & `cone.app-1.0rc3/src/cone/app/interfaces.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/ugm.py` & `cone.app-1.0rc3/src/cone/app/ugm.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/compat.py` & `cone.app-1.0rc3/src/cone/app/compat.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/model.py` & `cone.app-1.0rc3/src/cone/app/model.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/utils.py` & `cone.app-1.0rc3/src/cone/app/utils.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_exception.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_exception.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/__init__.py` & `cone.app-1.0rc3/src/cone/app/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_form.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_form.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_testing.py` & `cone.app-1.0rc3/src/cone/app/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_workflow.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_workflow.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_sharing.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_sharing.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_referencebrowser.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_referencebrowser.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_model.py` & `cone.app-1.0rc3/src/cone/app/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_utils.py` & `cone.app-1.0rc3/src/cone/app/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_copysupport.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_copysupport.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_utils.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_utils.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_contents.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_contents.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_ajax.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_ajax.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,28 +261,29 @@
         self.assertEqual(afc.next, 'false')
 
         # If continuation definitions and result, ``form`` returns empty
         # string, because form processing was successful. ``next`` returns a
         # JSON dump of given actions, which gets interpreted and executed on
         # client side
         action = AjaxAction(
-            'http://example.com',
-            'tilename',
-            'replace',
-            '.someselector'
+            target='http://example.com',
+            name='tilename',
+            mode='replace',
+            selector='.someselector'
         )
         event = AjaxEvent(
-            'http://example.com',
-            'contextchanged',
-            '.contextsensitiv'
+            target='http://example.com',
+            name='contextchanged',
+            selector='.contextsensitiv',
+            data=dict(key='value')
         )
         message = AjaxMessage(
-            'Some info message',
-            'info',
-            'None'
+            payload='Some info message',
+            flavor='info',
+            selector='None'
         )
         overlay = AjaxOverlay(
             selector='#ajax-overlay',
             action='someaction',
             target='http://example.com',
             close=False,
             content_selector='.overlay_content',
@@ -308,15 +309,18 @@
             "type": "action",
             "target": "http://example.com",
             "name": "tilename"
         }, {
             "selector": ".contextsensitiv",
             "type": "event",
             "target": "http://example.com",
-            "name": "contextchanged"
+            "name": "contextchanged",
+            "data": {
+                "key": "value"
+            }
         }, {
             "flavor": "info",
             "type": "message",
             "payload": "Some info message",
             "selector": "None"
         }, {
             "target": "http://example.com",
```

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_table.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_table.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_security.py` & `cone.app-1.0rc3/src/cone/app/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_app.py` & `cone.app-1.0rc3/src/cone/app/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_login.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_login.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_contextmenu.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_contextmenu.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_workflow.py` & `cone.app-1.0rc3/src/cone/app/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_authoring.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_authoring.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_actions.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_actions.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_layout.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_layout.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_settings.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_settings.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_batch.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_batch.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_browser_resources.py` & `cone.app-1.0rc3/src/cone/app/tests/test_browser_resources.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/tests/test_ugm.py` & `cone.app-1.0rc3/src/cone/app/tests/test_ugm.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/testing/__init__.py` & `cone.app-1.0rc3/src/cone/app/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/testing/dummy_workflow.zcml` & `cone.app-1.0rc3/src/cone/app/testing/dummy_workflow.zcml`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone/app/testing/mock.py` & `cone.app-1.0rc3/src/cone/app/testing/mock.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone.app.egg-info/SOURCES.txt` & `cone.app-1.0rc3/src/cone.app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/src/cone.app.egg-info/PKG-INFO` & `cone.app-1.0rc3/src/cone.app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cone.app
-Version: 1.0rc2
+Version: 1.0rc3
 Summary: Web application stub
 Home-page: https://github.com/bluedynamics/cone.app
 Author: Robert Niederreiter
 Author-email: dev@bluedynamics.com
 License: Simplified BSD
 Description: **``cone.app`` - Build Web Applications on top of the pyramid framework.**
         
@@ -50,14 +50,22 @@
         - Jens Klein
         - Georg Gogo. BERNHARD
         
         
         Changes
         =======
         
+        1.0rc3 (2020-10-12)
+        -------------------
+        
+        - ``cone.app.browser.ajax.AjaxEvent`` supports optional ``data`` argument
+          supported as of ``bdajax`` 1.13.
+          [rnix, 2020-09-29]
+        
+        
         1.0rc2 (2020-08-12)
         -------------------
         
         - Fix print CSS.
           [rnix, 2020-08-12]
         
         - Fix case when pasting to empty folder in copysupport JS.
```

### Comparing `cone.app-1.0rc2/README.rst` & `cone.app-1.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `cone.app-1.0rc2/PKG-INFO` & `cone.app-1.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cone.app
-Version: 1.0rc2
+Version: 1.0rc3
 Summary: Web application stub
 Home-page: https://github.com/bluedynamics/cone.app
 Author: Robert Niederreiter
 Author-email: dev@bluedynamics.com
 License: Simplified BSD
 Description: **``cone.app`` - Build Web Applications on top of the pyramid framework.**
         
@@ -50,14 +50,22 @@
         - Jens Klein
         - Georg Gogo. BERNHARD
         
         
         Changes
         =======
         
+        1.0rc3 (2020-10-12)
+        -------------------
+        
+        - ``cone.app.browser.ajax.AjaxEvent`` supports optional ``data`` argument
+          supported as of ``bdajax`` 1.13.
+          [rnix, 2020-09-29]
+        
+        
         1.0rc2 (2020-08-12)
         -------------------
         
         - Fix print CSS.
           [rnix, 2020-08-12]
         
         - Fix case when pasting to empty folder in copysupport JS.
```

