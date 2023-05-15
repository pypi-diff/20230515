# Comparing `tmp/utx-1.3.3.tar.gz` & `tmp/utx-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/utx-pypi/utx-pypi/dist/.tmp-8uv_bazl/utx-1.3.3.tar", last modified: Thu Feb  2 14:05:44 2023, max compression
+gzip compressed data, was "/home/runner/work/utx-pypi/utx-pypi/dist/.tmp-cfstm47f/utx-1.3.4.tar", last modified: Mon May 15 08:13:02 2023, max compression
```

## Comparing `utx-1.3.3.tar` & `utx-1.3.4.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (116)    11361 2023-02-02 14:05:35.000000 utx-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      240 2023-02-02 14:05:35.000000 utx-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     7261 2023-02-02 14:05:44.000000 utx-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6352 2023-02-02 14:05:35.000000 utx-1.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-02 14:05:44.000000 utx-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1761 2023-02-02 14:05:35.000000 utx-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/
--rw-r--r--   0 runner    (1001) docker     (116)      148 2023-02-02 14:05:35.000000 utx-1.3.3/utx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/cli/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:35.000000 utx-1.3.3/utx/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8641 2023-02-02 14:05:35.000000 utx-1.3.3/utx/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     1669 2023-02-02 14:05:35.000000 utx-1.3.3/utx/cli/fixture.py
--rw-r--r--   0 runner    (1001) docker     (116)    11215 2023-02-02 14:05:35.000000 utx-1.3.3/utx/cli/func.py
--rw-r--r--   0 runner    (1001) docker     (116)     2184 2023-02-02 14:05:35.000000 utx-1.3.3/utx/cli/plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)    18430 2023-02-02 14:05:35.000000 utx-1.3.3/utx/cli/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (116)    14963 2023-02-02 14:05:35.000000 utx-1.3.3/utx/cli/scaffold_web.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/core/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/core/css/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3653 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/comparison_table_model.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/core/css/css/
--rw-r--r--   0 runner    (1001) docker     (116)     2017 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/css/monokai_sublime.min.css
--rw-r--r--   0 runner    (1001) docker     (116)    17032 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/css/report.css
--rw-r--r--   0 runner    (1001) docker     (116)     1215 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/custom_report.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/core/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (116)  8164040 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/fonts/SourceHanSansCN-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (116)    20127 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (116)   108738 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (116)    45404 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (116)    23424 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (116)    18028 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/core/css/image/
--rw-r--r--   0 runner    (1001) docker     (116)    16657 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/arrow.png
--rw-r--r--   0 runner    (1001) docker     (116)      667 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/back.svg
--rw-r--r--   0 runner    (1001) docker     (116)     3705 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/broken.png
--rw-r--r--   0 runner    (1001) docker     (116)      729 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/close.svg
--rw-r--r--   0 runner    (1001) docker     (116)     2175 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/console_hover.svg
--rw-r--r--   0 runner    (1001) docker     (116)     2177 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/console_normal.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1013 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/copy.svg
--rw-r--r--   0 runner    (1001) docker     (116)     2532 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/download_log.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1935 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/eye.svg
--rw-r--r--   0 runner    (1001) docker     (116)      941 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/fail.svg
--rw-r--r--   0 runner    (1001) docker     (116)      623 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/less.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1308 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/maximize.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1031 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/minimize.svg
--rw-r--r--   0 runner    (1001) docker     (116)      684 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/more.svg
--rw-r--r--   0 runner    (1001) docker     (116)     2044 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/open_in_new_tab.svg
--rw-r--r--   0 runner    (1001) docker     (116)      499 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/order.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1253 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/step_fail.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1124 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/step_success.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1141 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/success.svg
--rw-r--r--   0 runner    (1001) docker     (116)    25732 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/target.png
--rw-r--r--   0 runner    (1001) docker     (116)      820 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/image/time.svg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/core/css/js/
--rw-r--r--   0 runner    (1001) docker     (116)    35951 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/core/css/js/echarts/
--rw-r--r--   0 runner    (1001) docker     (116)   406678 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/js/echarts/echarts.common.min.js
--rw-r--r--   0 runner    (1001) docker     (116)     3355 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/js/echarts/pfm_charts.js
--rw-r--r--   0 runner    (1001) docker     (116)     3842 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/js/echarts/shine.js
--rw-r--r--   0 runner    (1001) docker     (116)   184850 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (116)    93106 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/js/jquery-1.10.2.min.js
--rw-r--r--   0 runner    (1001) docker     (116)    24870 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/js/jquery-lang.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/core/css/js/langpack/
--rw-r--r--   0 runner    (1001) docker     (116)     2457 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/js/langpack/zh_CN.js
--rw-r--r--   0 runner    (1001) docker     (116)     5414 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/js/lazyload.js
--rw-r--r--   0 runner    (1001) docker     (116)    12768 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/js/paging.js
--rw-r--r--   0 runner    (1001) docker     (116)    26745 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/js/report.js
--rw-r--r--   0 runner    (1001) docker     (116)    15336 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/log_template.html
--rw-r--r--   0 runner    (1001) docker     (116)    21684 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/report.py
--rw-r--r--   0 runner    (1001) docker     (116)     2042 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/summary_template.html
--rw-r--r--   0 runner    (1001) docker     (116)     1954 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/summary_template_pool.html
--rw-r--r--   0 runner    (1001) docker     (116)    10399 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/css/summary_template_v2.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/core/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13222 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/utils/hook.py
--rw-r--r--   0 runner    (1001) docker     (116)    10707 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/utils/runner.py
--rw-r--r--   0 runner    (1001) docker     (116)    15595 2023-02-02 14:05:35.000000 utx-1.3.3/utx/core/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/mod/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2023-02-02 14:05:35.000000 utx-1.3.3/utx/mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1001 2023-02-02 14:05:35.000000 utx-1.3.3/utx/mod/load.py
--rw-r--r--   0 runner    (1001) docker     (116)      467 2023-02-02 14:05:35.000000 utx-1.3.3/utx/mod/main.py
--rw-r--r--   0 runner    (1001) docker     (116)      698 2023-02-02 14:05:35.000000 utx-1.3.3/utx/mod/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/mod/plugins/
--rw-r--r--   0 runner    (1001) docker     (116)       27 2023-02-02 14:05:35.000000 utx-1.3.3/utx/mod/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      327 2023-02-02 14:05:35.000000 utx-1.3.3/utx/mod/plugins/pg_1.py
--rw-r--r--   0 runner    (1001) docker     (116)      328 2023-02-02 14:05:35.000000 utx-1.3.3/utx/mod/plugins/pg_2.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/mod/report/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:35.000000 utx-1.3.3/utx/mod/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1848 2023-02-02 14:05:35.000000 utx-1.3.3/utx/mod/report/pocoui.py
--rw-r--r--   0 runner    (1001) docker     (116)     4270 2023-02-02 14:05:35.000000 utx-1.3.3/utx/mod/report/seleniumui.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/scripts/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:35.000000 utx-1.3.3/utx/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      893 2023-02-02 14:05:35.000000 utx-1.3.3/utx/scripts/ipa_pkg.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     4048 2023-02-02 14:05:35.000000 utx-1.3.3/utx/scripts/ipa_sign.sh
--rw-r--r--   0 runner    (1001) docker     (116)    14276 2023-02-02 14:05:35.000000 utx-1.3.3/utx/scripts/plistdump-tcp-proxy.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      774 2023-02-02 14:05:35.000000 utx-1.3.3/utx/scripts/run-usbmuxd-proxy.sh
--rw-r--r--   0 runner    (1001) docker     (116)     3179 2023-02-02 14:05:35.000000 utx-1.3.3/utx/scripts/uitest_screenrecord.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/selenium/
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-02 14:05:35.000000 utx-1.3.3/utx/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1585 2023-02-02 14:05:35.000000 utx-1.3.3/utx/selenium/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)    35262 2023-02-02 14:05:35.000000 utx-1.3.3/utx/selenium/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx/selenium/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:35.000000 utx-1.3.3/utx/selenium/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2354 2023-02-02 14:05:35.000000 utx-1.3.3/utx/selenium/utils/airtest_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    30098 2023-02-02 14:05:35.000000 utx-1.3.3/utx/selenium/utils/six.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-02 14:05:44.000000 utx-1.3.3/utx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7261 2023-02-02 14:05:44.000000 utx-1.3.3/utx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2701 2023-02-02 14:05:44.000000 utx-1.3.3/utx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-02 14:05:44.000000 utx-1.3.3/utx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       41 2023-02-02 14:05:44.000000 utx-1.3.3/utx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      225 2023-02-02 14:05:44.000000 utx-1.3.3/utx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        4 2023-02-02 14:05:44.000000 utx-1.3.3/utx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-15 08:12:53.000000 utx-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-15 08:12:53.000000 utx-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-05-15 08:13:02.000000 utx-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-15 08:12:53.000000 utx-1.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 08:13:02.000000 utx-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-15 08:12:53.000000 utx-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-15 08:12:53.000000 utx-1.3.4/utx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:53.000000 utx-1.3.4/utx/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-15 08:12:53.000000 utx-1.3.4/utx/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-15 08:12:53.000000 utx-1.3.4/utx/cli/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-05-15 08:12:53.000000 utx-1.3.4/utx/cli/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-15 08:12:53.000000 utx-1.3.4/utx/cli/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18494 2023-05-15 08:12:53.000000 utx-1.3.4/utx/cli/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-05-15 08:12:53.000000 utx-1.3.4/utx/cli/scaffold_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/core/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/comparison_table_model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/core/css/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/css/monokai_sublime.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/css/report.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/custom_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/core/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)  8164040 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/fonts/SourceHanSansCN-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/core/css/image/
+-rw-r--r--   0 runner    (1001) docker     (123)    16657 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/broken.png
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/console_hover.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/console_normal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/download_log.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/eye.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/fail.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/less.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/maximize.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/minimize.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/more.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/open_in_new_tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/order.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/step_fail.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/step_success.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/success.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25732 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/target.png
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/image/time.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/core/css/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    35951 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/core/css/js/echarts/
+-rw-r--r--   0 runner    (1001) docker     (123)   406678 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/js/echarts/echarts.common.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/js/echarts/pfm_charts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/js/echarts/shine.js
+-rw-r--r--   0 runner    (1001) docker     (123)   184850 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    93106 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/js/jquery-1.10.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24870 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/js/jquery-lang.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/core/css/js/langpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/js/langpack/zh_CN.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/js/lazyload.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/js/paging.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29472 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/js/report.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/log_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22855 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/summary_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/summary_template_pool.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/css/summary_template_v2.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14034 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/utils/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/utils/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-05-15 08:12:53.000000 utx-1.3.4/utx/core/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/mod/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:53.000000 utx-1.3.4/utx/mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-15 08:12:53.000000 utx-1.3.4/utx/mod/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-15 08:12:53.000000 utx-1.3.4/utx/mod/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-15 08:12:53.000000 utx-1.3.4/utx/mod/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/mod/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 08:12:53.000000 utx-1.3.4/utx/mod/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-15 08:12:53.000000 utx-1.3.4/utx/mod/plugins/pg_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-15 08:12:53.000000 utx-1.3.4/utx/mod/plugins/pg_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/mod/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:53.000000 utx-1.3.4/utx/mod/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-15 08:12:53.000000 utx-1.3.4/utx/mod/report/pocoui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-15 08:12:53.000000 utx-1.3.4/utx/mod/report/seleniumui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:53.000000 utx-1.3.4/utx/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-15 08:12:53.000000 utx-1.3.4/utx/scripts/ipa_pkg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4048 2023-05-15 08:12:53.000000 utx-1.3.4/utx/scripts/ipa_sign.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-05-15 08:12:53.000000 utx-1.3.4/utx/scripts/plistdump-tcp-proxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-05-15 08:12:53.000000 utx-1.3.4/utx/scripts/run-usbmuxd-proxy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-15 08:12:53.000000 utx-1.3.4/utx/scripts/uitest_screenrecord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/selenium/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:53.000000 utx-1.3.4/utx/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-15 08:12:53.000000 utx-1.3.4/utx/selenium/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35985 2023-05-15 08:12:53.000000 utx-1.3.4/utx/selenium/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx/selenium/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:53.000000 utx-1.3.4/utx/selenium/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-15 08:12:53.000000 utx-1.3.4/utx/selenium/utils/airtest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30042 2023-05-15 08:12:53.000000 utx-1.3.4/utx/selenium/utils/six.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:13:02.000000 utx-1.3.4/utx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-05-15 08:13:02.000000 utx-1.3.4/utx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-15 08:13:02.000000 utx-1.3.4/utx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 08:13:02.000000 utx-1.3.4/utx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 08:13:02.000000 utx-1.3.4/utx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 08:13:02.000000 utx-1.3.4/utx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 08:13:02.000000 utx-1.3.4/utx.egg-info/top_level.txt
```

### Comparing `utx-1.3.3/LICENSE` & `utx-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/PKG-INFO` & `utx-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utx
-Version: 1.3.3
+Version: 1.3.4
 Summary: UTX will help you write ui automated tests more easily!
 Home-page: https://github.com/openutx
 Author: lijiawei
 Author-email: jiawei.li2@qq.com
 License: Apache License 2.0
 Keywords: utx,airtest,pytest,selenium,ui,tools
 Platform: any
```

### Comparing `utx-1.3.3/README.md` & `utx-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/setup.py` & `utx-1.3.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,64 @@
 #!/usr/bin/env python
-# -*- coding:utf-8 -*-
-from setuptools import setup, find_packages
+from setuptools import find_packages
+from setuptools import setup
+
 from utx import __version__
 
-with open('README.md', encoding='utf-8') as f:
+with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="utx",
-    version="{}".format(__version__),
+    version=f"{__version__}",
     keywords=["utx", "airtest", "pytest", "selenium", "ui", "tools"],
-    description='UTX will help you write ui automated tests more easily!',
+    description="UTX will help you write ui automated tests more easily!",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    license='Apache License 2.0',
-
+    long_description_content_type="text/markdown",
+    license="Apache License 2.0",
     url="https://github.com/openutx",
     author="lijiawei",
     author_email="jiawei.li2@qq.com",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console :: Curses",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: Implementation :: CPython"
+        "Programming Language :: Python :: Implementation :: CPython",
     ],
     entry_points="""
     [console_scripts]
     utx = utx.cli.cli:main
     """,
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
-    install_requires=["airtest", "tenacity", "allure-pytest", "pocoui",
-                      "tidevice", "faker", "jmespath", "loguru", "pytest-xdist",
-                      "PyYAML", "allure-python-commons", "pytest-rerunfailures", "pyOpenSSL",
-                      "pyasn1", "selenium~=3.14.0", "pynput", "tqdm", "popups", "webdriver-manager", "PyUserInput",
-                      "pyperclip"]
-
+    install_requires=[
+        "airtest",
+        "tenacity",
+        "allure-pytest",
+        "pocoui",
+        "tidevice",
+        "faker",
+        "jmespath",
+        "loguru",
+        "pytest-xdist",
+        "PyYAML",
+        "allure-python-commons",
+        "pytest-rerunfailures",
+        "pyOpenSSL",
+        "pyasn1",
+        "selenium~=3.14.0",
+        "pynput",
+        "tqdm",
+        "popups",
+        "webdriver-manager",
+        "PyUserInput",
+        "pyperclip",
+    ],
 )
```

### Comparing `utx-1.3.3/utx/cli/cli.py` & `utx-1.3.4/utx/cli/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,136 +1,141 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  8/17/2021 6:49 PM
 @Desc    :  Command line.
 """
-
 import argparse
 import os
 import random
 import subprocess
 import sys
 
 from airtest.core.android.adb import ADB
 from loguru import logger
 
-from utx.cli.scaffold_web import init_parser_scaffold_web, main_scaffold_web
-from utx.core.utils.tools import decryption, check_port, plat, get_host_ip
-from utx import __description__, __version__
-from utx.cli.scaffold import init_parser_scaffold, main_scaffold, init_parser_install, main_install, \
-    init_parser_uninstall, main_uninstall
+from utx import __description__
+from utx import __version__
+from utx.cli.scaffold import init_parser_install
+from utx.cli.scaffold import init_parser_scaffold
+from utx.cli.scaffold import init_parser_uninstall
+from utx.cli.scaffold import main_install
+from utx.cli.scaffold import main_scaffold
+from utx.cli.scaffold import main_uninstall
+from utx.cli.scaffold_web import init_parser_scaffold_web
+from utx.cli.scaffold_web import main_scaffold_web
+from utx.core.utils.tools import check_port
+from utx.core.utils.tools import decryption
+from utx.core.utils.tools import get_host_ip
+from utx.core.utils.tools import plat
 
 
 def main():
-    """Parse command line options and run commands.
-    """
+    """Parse command line options and run commands."""
     parser = argparse.ArgumentParser(description=__description__)
 
     parser.add_argument(
         "-v", "--version", dest="version", action="store_true", help="show version"
     )
     subparsers = parser.add_subparsers(help="sub-command help")
     sub_parser_scaffold = init_parser_scaffold(subparsers)
     sub_parser_scaffold_web = init_parser_scaffold_web(subparsers)
     sub_parser_install = init_parser_install(subparsers)
     sub_parser_uninstall = init_parser_uninstall(subparsers)
     subparsers.add_parser(
         "test", help="debug iOS devices(UTX driver needs to be installed)."
     )
 
-    subparsers.add_parser(
-        "adb", help="complete adb debugging capability."
-    )
+    subparsers.add_parser("adb", help="complete adb debugging capability.")
     subparsers.add_parser(
         "remote", help="open Android device remote debugging port(5555)."
     )
     subparsers.add_parser(
         "proxy", help=f"enable device global proxy({get_host_ip()}:8888)."
     )
-    subparsers.add_parser(
-        'unproxy', help=f"disable device global proxy."
-    )
+    subparsers.add_parser("unproxy", help=f"disable device global proxy.")
     # show device info
-    subparsers.add_parser(
-        "list", help="show connected iOS devices."
-    )
-    subparsers.add_parser(
-        "info", help="show current connected iOS device info."
-    )
-    subparsers.add_parser(
-        "applist", help="list packages on iOS devices."
-    )
+    subparsers.add_parser("list", help="show connected iOS devices.")
+    subparsers.add_parser("info", help="show current connected iOS device info.")
+    subparsers.add_parser("applist", help="list packages on iOS devices.")
 
     if len(sys.argv) == 1:
         # utx
         parser.print_help()
         sys.exit(0)
     elif len(sys.argv) == 2:
         # print help for sub-commands
         if sys.argv[1] in ["-v", "--version"]:
             # utx -v
             print(f"{__version__}")
         elif sys.argv[1] == "test":
             # utx -test
-            logger.info('UTX will connect your IOS device.')
+            logger.info("UTX will connect your IOS device.")
             logger.warning(
-                'Please make sure the IOS phone is connected to the computer and the UTX driver is installed!')
-            devices = '{} list'.format(decryption(b'dGlkZXZpY2U='))
+                "Please make sure the IOS phone is connected to the computer and the UTX driver is installed!"
+            )
+            devices = "{} list".format(decryption(b"dGlkZXZpY2U="))
             d = os.popen(devices)
             if len(d.readlines()) == 0:
-                logger.error('No device detected!')
+                logger.error("No device detected!")
                 sys.exit()
 
-            res = subprocess.run('{} applist'.format(decryption(b'dGlkZXZpY2U=')), shell=True, stdout=subprocess.PIPE,
-                                 stderr=subprocess.PIPE)
+            res = subprocess.run(
+                "{} applist".format(decryption(b"dGlkZXZpY2U=")),
+                shell=True,
+                capture_output=True,
+            )
             utx_driver = res.stdout.decode("utf-8", "ignore")
 
-            if 'WebDriverAgentRunner' not in utx_driver:
-                logger.error('UTX driver(WDA.ipa) is not installed!')
+            if "WebDriverAgentRunner" not in utx_driver:
+                logger.error("UTX driver(WDA.ipa) is not installed!")
                 sys.exit()
             else:
                 pass
 
             proxy = str(random.randint(50000, 60000) + 1)
             check_port(port=proxy)
-            logger.info('Debug address:http://127.0.0.1:{}'.format(proxy))
+            logger.info(f"Debug address:http://127.0.0.1:{proxy}")
             try:
-                subprocess.call('{} wdaproxy --port {}'.format(decryption(b'dGlkZXZpY2U='), proxy), shell=True)
+                subprocess.call(
+                    "{} wdaproxy --port {}".format(decryption(b"dGlkZXZpY2U="), proxy),
+                    shell=True,
+                )
             except KeyboardInterrupt:
                 check_port(port=proxy)
                 sys.exit()
             finally:
-                if plat() != 'Windows':
-                    os.system('clear')
+                if plat() != "Windows":
+                    os.system("clear")
                 else:
-                    os.system('cls')
-                logger.error('')
-                logger.error('-------------------- utx end --------------------------')
+                    os.system("cls")
+                logger.error("")
+                logger.error("-------------------- utx end --------------------------")
 
-                logger.error('Disconnect and end debugging!')
+                logger.error("Disconnect and end debugging!")
 
         elif sys.argv[1] == "remote":
             # utx remote
-            os.system(f'{ADB.builtin_adb_path()} tcpip 5555')
+            os.system(f"{ADB.builtin_adb_path()} tcpip 5555")
 
         elif sys.argv[1] == "proxy":
             # utx proxy
             os.system(
-                f'{ADB.builtin_adb_path()} {decryption(b"c2hlbGwgc2V0dGluZ3MgcHV0IGdsb2JhbCBodHRwX3Byb3h5")} {get_host_ip()}:8888')
+                f'{ADB.builtin_adb_path()} {decryption(b"c2hlbGwgc2V0dGluZ3MgcHV0IGdsb2JhbCBodHRwX3Byb3h5")} {get_host_ip()}:8888'
+            )
 
         elif sys.argv[1] == "unproxy":
             # utx proxy
-            os.system(f'{ADB.builtin_adb_path()} {decryption(b"c2hlbGwgc2V0dGluZ3MgcHV0IGdsb2JhbCBodHRwX3Byb3h5IDow")}')
+            os.system(
+                f'{ADB.builtin_adb_path()} {decryption(b"c2hlbGwgc2V0dGluZ3MgcHV0IGdsb2JhbCBodHRwX3Byb3h5IDow")}'
+            )
 
         elif sys.argv[1] == "adb":
             # utx adb
-            os.system(f'{ADB.builtin_adb_path()}')
+            os.system(f"{ADB.builtin_adb_path()}")
 
         elif sys.argv[1] in ["-h", "--help"]:
             # utx -h
             parser.print_help()
 
         elif sys.argv[1] == "install":
             # utx install
@@ -138,39 +143,39 @@
 
         elif sys.argv[1] == "uninstall":
             # utx uninstall
             sub_parser_uninstall.print_help()
 
         elif sys.argv[1] == "list":
             # utx list
-            os.system('{} list'.format(decryption(b'dGlkZXZpY2U=')))
+            os.system("{} list".format(decryption(b"dGlkZXZpY2U=")))
 
         elif sys.argv[1] == "info":
             # utx info
-            os.system('{} info'.format(decryption(b'dGlkZXZpY2U=')))
+            os.system("{} info".format(decryption(b"dGlkZXZpY2U=")))
 
         elif sys.argv[1] == "applist":
             # utx applist
-            os.system('{} applist'.format(decryption(b'dGlkZXZpY2U=')))
+            os.system("{} applist".format(decryption(b"dGlkZXZpY2U=")))
 
         elif sys.argv[1] == "startproject":
             # utx startproject
             sub_parser_scaffold.print_help()
 
         elif sys.argv[1] == "startproject-web":
             # utx startproject-web
             sub_parser_scaffold_web.print_help()
         else:
             parser.print_help()
         sys.exit(0)
 
     elif sys.argv[1] == "adb":
         del sys.argv[0:2]
-        args = ' '.join([str(i) for i in sys.argv])
-        os.system('{} {}'.format(ADB.builtin_adb_path(), args))
+        args = " ".join([str(i) for i in sys.argv])
+        os.system(f"{ADB.builtin_adb_path()} {args}")
         sys.exit(0)
 
     args = parser.parse_args()
 
     if args.version:
         print(f"{__version__}")
         sys.exit(0)
@@ -185,15 +190,15 @@
         main_install(args)
 
     if sys.argv[1] == "uninstall":
         main_uninstall(args)
 
 
 def cli_env():
-    parser = argparse.ArgumentParser(description='manual to this script')
+    parser = argparse.ArgumentParser(description="manual to this script")
     parser.add_argument("--device", type=str)
     parser.add_argument("--platform", type=str)
     parser.add_argument("--wda", type=str)
     parser.add_argument("--init", type=str)
 
     args = parser.parse_args()
     cli_device = args.device
@@ -205,15 +210,15 @@
 
 
 def cli_env_v2():
     """
     cli param v2
     :return: param dict
     """
-    parser = argparse.ArgumentParser(description='manual to this script cli_env v2')
+    parser = argparse.ArgumentParser(description="manual to this script cli_env v2")
     parser.add_argument("--device", type=str)
     parser.add_argument("--platform", type=str)
     parser.add_argument("--wda", type=str)
     parser.add_argument("--init", type=str)
     parser.add_argument("--package", type=str)
     parser.add_argument("--filename", type=str)
     parser.add_argument("--times", type=str)
@@ -244,36 +249,36 @@
 
     duration = args.duration
     whitelist = args.whitelist
     throttle = args.throttle
     widget = args.widget
 
     cli_result = {
-        'device': device,
-        'platform': platform,
-        'wda': wda,
-        'init': init,
-        'package': package,
-        'filename': filename,
-        'times': times,
-        'name': name,
-        'is_all': is_all,
-        'record': record,
-        'proxy': proxy,
-        'cases': cases,
-        'duration': duration,
-        'whitelist': whitelist,
-        'throttle': throttle,
-        'widget': widget,
+        "device": device,
+        "platform": platform,
+        "wda": wda,
+        "init": init,
+        "package": package,
+        "filename": filename,
+        "times": times,
+        "name": name,
+        "is_all": is_all,
+        "record": record,
+        "proxy": proxy,
+        "cases": cases,
+        "duration": duration,
+        "whitelist": whitelist,
+        "throttle": throttle,
+        "widget": widget,
     }
     return cli_result
 
 
 def cli_web_env():
-    parser = argparse.ArgumentParser(description='manual to this script')
+    parser = argparse.ArgumentParser(description="manual to this script")
 
     parser.add_argument("--headless", type=str)
 
     args = parser.parse_args()
 
     cli_headless = args.headless
```

### Comparing `utx-1.3.3/utx/cli/fixture.py` & `utx-1.3.4/utx/cli/fixture.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  8/17/2021 6:49 PM
 @Desc    :  Provide some fixtures
 """
-
 import os
 
 import jmespath
 import pytest
 import yaml
 from faker import Faker
 from loguru import logger
@@ -24,15 +21,15 @@
     Project.dir = session.config.cache.get("project_dir", None)
     if not Project.dir:
         # First time run, no pytest_cache
         cwd = os.getcwd()
         tests = cwd.find("tests")
         # tests
         if tests > 0:
-            Project.dir = cwd[:cwd.find("tests")]
+            Project.dir = cwd[: cwd.find("tests")]
         # root
         else:
             Project.dir = cwd
 
 
 @pytest.fixture(scope="session")
 def faker_ch():
@@ -44,23 +41,24 @@
     return Faker()
 
 
 @pytest.fixture(scope="session")
 def pd():
     try:
         import pandas
+
         return pandas
     except ModuleNotFoundError:
         pass
 
 
 @pytest.fixture(scope="session")
 def config():
     config_path = os.path.join(Project.dir, "conf.yaml")
-    with open(config_path, "r", encoding="utf-8") as f:
+    with open(config_path, encoding="utf-8") as f:
         conf = yaml.load(f.read(), Loader=yaml.FullLoader)
         return conf
 
 
 @pytest.fixture(scope="session")
 def files_dir():
     return os.path.join(Project.dir, "files")
```

### Comparing `utx-1.3.3/utx/cli/plugin.py` & `utx-1.3.4/utx/cli/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  8/17/2021 6:49 PM
 @Desc    :  plugin.py
 """
-
 import os
 import shutil
 import tempfile
 
 import allure_commons
 from allure_commons.logger import AllureFileLogger
 from allure_pytest.listener import AllureListener
@@ -25,20 +22,22 @@
 class Plugin:
     @staticmethod
     def pytest_addoption(parser):
         parser.addoption(
             "--utx-reports",
             action="store_const",
             const=True,
-            help="Create utx allure HTML reports."
+            help="Create utx allure HTML reports.",
         )
 
     @staticmethod
     def _utx_reports(config):
-        if config.getoption("--utx-reports") and not config.getoption("allure_report_dir"):
+        if config.getoption("--utx-reports") and not config.getoption(
+            "allure_report_dir"
+        ):
             return True
         else:
             return False
 
     @staticmethod
     def pytest_configure(config):
         if Plugin._utx_reports(config):
@@ -52,15 +51,22 @@
             allure_commons.plugin_manager.register(file_logger)
             config.add_cleanup(cleanup_factory(file_logger))
 
     @staticmethod
     def pytest_sessionfinish(session):
         if Plugin._utx_reports(session.config):
             reports_dir = os.path.join(Project.dir, "reports")
-            new_report = os.path.join(reports_dir, "report-" + current_time().replace(":", "-").replace(" ", "-"))
+            new_report = os.path.join(
+                reports_dir,
+                "report-" + current_time().replace(":", "-").replace(" ", "-"),
+            )
             if os.path.exists(reports_dir):
                 his_reports = os.listdir(reports_dir)
                 if his_reports:
-                    latest_report_history = os.path.join(reports_dir, his_reports[-1], "history")
-                    shutil.copytree(latest_report_history, os.path.join(allure_temp, "history"))
+                    latest_report_history = os.path.join(
+                        reports_dir, his_reports[-1], "history"
+                    )
+                    shutil.copytree(
+                        latest_report_history, os.path.join(allure_temp, "history")
+                    )
             os.system(f"allure generate {allure_temp} -o {new_report}  --clean")
             shutil.rmtree(allure_temp)
```

### Comparing `utx-1.3.3/utx/cli/scaffold.py` & `utx-1.3.4/utx/cli/scaffold.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  8/24/2021 1:35 PM
 @Desc    :  Scaffold Generator.
 """
-
 import os
 import platform
 import sys
 
 from loguru import logger
+
 from utx.core.utils.tools import decryption
 
 
 class ExtraArgument:
     create_venv = False
 
 
@@ -28,22 +26,26 @@
     )
 
     return install_parser
 
 
 def creat_install(filepath_or_url):
     if filepath_or_url is None:
-        logger.error('UTX install: error: the following arguments are required: filepath_or_url')
+        logger.error(
+            "UTX install: error: the following arguments are required: filepath_or_url"
+        )
         return 1
     elif filepath_or_url.endswith(".ipa"):
-        os.system('{} install {}'.format(decryption(b'dGlkZXZpY2U='), filepath_or_url))
+        os.system("{} install {}".format(decryption(b"dGlkZXZpY2U="), filepath_or_url))
     elif filepath_or_url.startswith("http"):
-        os.system('{} install {}'.format(decryption(b'dGlkZXZpY2U='), filepath_or_url))
+        os.system("{} install {}".format(decryption(b"dGlkZXZpY2U="), filepath_or_url))
     else:
-        logger.error('UTX install: error: the following arguments are required: filepath_or_url')
+        logger.error(
+            "UTX install: error: the following arguments are required: filepath_or_url"
+        )
         return 1
 
 
 def main_install(args):
     sys.exit(creat_install(args.filepath_or_url))
 
 
@@ -56,20 +58,24 @@
     )
 
     return uninstall_parser
 
 
 def creat_uninstall(bundle_id):
     if bundle_id is None:
-        logger.error('UTX uninstall: error: the following arguments are required: bundle_id')
+        logger.error(
+            "UTX uninstall: error: the following arguments are required: bundle_id"
+        )
         return 1
-    elif bundle_id.replace('.', '').isalnum():
-        os.system('{} uninstall {}'.format(decryption(b'dGlkZXZpY2U='), bundle_id))
+    elif bundle_id.replace(".", "").isalnum():
+        os.system("{} uninstall {}".format(decryption(b"dGlkZXZpY2U="), bundle_id))
     else:
-        logger.error('UTX uninstall: error: the following arguments are required: bundle_id')
+        logger.error(
+            "UTX uninstall: error: the following arguments are required: bundle_id"
+        )
         return 1
 
 
 def main_uninstall(args):
     sys.exit(creat_uninstall(args.bundle_id))
 
 
@@ -86,16 +92,15 @@
         action="store_true",
         help="create virtual environment in the project, and install utx.",
     )
     return sub_parser_scaffold
 
 
 def create_scaffold(project_name):
-    """ Create scaffold with specified project name.
-    """
+    """Create scaffold with specified project name."""
     if os.path.isdir(project_name):
         logger.warning(
             f"Project folder {project_name} exists, please specify a new project name."
         )
         return 1
     elif os.path.isfile(project_name):
         logger.warning(
@@ -573,23 +578,23 @@
     if ExtraArgument.create_venv:
         os.chdir(project_name)
         print("\nCreating virtual environment")
         os.system("python -m venv venv")
         print("Created virtual environment: venv")
 
         print("Installing utx")
-        if platform.system().lower() == 'windows':
+        if platform.system().lower() == "windows":
             os.chdir("venv")
             os.chdir("Scripts")
             os.system("pip install utx")
-        elif platform.system().lower() == 'linux':
+        elif platform.system().lower() == "linux":
             os.chdir("venv")
             os.chdir("bin")
             os.system("pip install utx")
-        elif platform.system().lower() == 'darwin':
+        elif platform.system().lower() == "darwin":
             os.chdir("venv")
             os.chdir("bin")
             os.system("pip install utx")
 
 
 def main_scaffold(args):
     ExtraArgument.create_venv = args.create_venv
```

### Comparing `utx-1.3.3/utx/cli/scaffold_web.py` & `utx-1.3.4/utx/cli/scaffold_web.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  11/4/2021 10:14 AM
 @Desc    :  Scaffold web Generator.
 """
-
 import os
 import platform
 import sys
 
 from loguru import logger
 
 
@@ -31,16 +28,15 @@
         action="store_true",
         help="create virtual environment in the project, and install utx.",
     )
     return sub_parser_scaffold
 
 
 def create_scaffold_web(project_name):
-    """ Create scaffold with specified project name.
-    """
+    """Create scaffold with specified project name."""
     if os.path.isdir(project_name):
         logger.warning(
             f"Project folder {project_name} exists, please specify a new project name."
         )
         return 1
     elif os.path.isfile(project_name):
         logger.warning(
@@ -487,23 +483,23 @@
     if ExtraArgument.create_venv:
         os.chdir(project_name)
         print("\nCreating virtual environment")
         os.system("python -m venv venv")
         print("Created virtual environment: venv")
 
         print("Installing utx")
-        if platform.system().lower() == 'windows':
+        if platform.system().lower() == "windows":
             os.chdir("venv")
             os.chdir("Scripts")
             os.system("pip install utx")
-        elif platform.system().lower() == 'linux':
+        elif platform.system().lower() == "linux":
             os.chdir("venv")
             os.chdir("bin")
             os.system("pip install utx")
-        elif platform.system().lower() == 'darwin':
+        elif platform.system().lower() == "darwin":
             os.chdir("venv")
             os.chdir("bin")
             os.system("pip install utx")
 
 
 def main_scaffold_web(args):
     ExtraArgument.create_venv = args.create_venv
```

### Comparing `utx-1.3.3/utx/core/css/comparison_table_model.json` & `utx-1.3.4/utx/core/css/comparison_table_model.json`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/css/monokai_sublime.min.css` & `utx-1.3.4/utx/core/css/css/monokai_sublime.min.css`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/css/report.css` & `utx-1.3.4/utx/core/css/css/report.css`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 .container-fluid{
   margin: auto;
   padding-right: 100px;
   padding-left: 100px;
   margin-bottom: 220px;
   min-width: 960px;
-  min-height: calc(100% - 222px);
+  min-height: calc(100%);
   position: relative;
 }
 #back_multi .back {
   position: fixed;
   left: 20px;
   top: 50px;
   width: 50px;
@@ -189,25 +189,30 @@
   word-break: break-word;
 }
 .summary .airdesc.collapse .desc-content{
   height: 160px;
 }
 
 .gallery{
+  min-height: 18vh;
   margin-bottom: 30px;
 }
 .gallery .info-title{
   margin-bottom: 10px;
 }
 .gallery .content{
   background: rgb(18,28,52);
   overflow-x: scroll;
   white-space: nowrap;
   background: #121c34;
   padding-top: 20px;
+  z-index: 3;
+}
+.gallery .placeholder {
+  background-color: #121c34;
 }
 .gallery .thumbnail {
   display: inline-block;
   border: solid 1px transparent;
 }
 .gallery .thumbnail.active {
   border: solid 1px rgb(74,144,226);
@@ -338,22 +343,23 @@
   -moz-box-align: stretch;
   -moz-align-items: stretch;
   -ms-flex-align: stretch;
   align-items: stretch;
 }
 .step-left{
   min-width: 320px;
-  padding: 30px 20px;
+  padding: 30px 50px 30px 20px;
   width: 32%;
   max-width: 500px;
+  max-height: 900px;
+  overflow-y: auto;
 }
 .step-right{
   border-left: dashed 1px rgb(102,102,102);
   padding: 30px 0px 0 60px;
-  margin-left: 30px;
   vertical-align: top;
   min-height: 500px;
   width: 100%;
   max-width: calc(100% - 410px);
   max-width: calc(100% - 600px);
 }
 .step-left .step {
@@ -563,14 +569,15 @@
   background: transparent;
   color: rgb(74,144,226);
 }
 .row.gif-wrap {
   position: fixed;
   bottom: 0;
   right: 0;
+  z-index: 4;
 }
 .row.gif-wrap .menu{
   display: block;
   text-align: right;
   background: rgba(0, 0, 0, 0.7);
   min-width: 100px;
   height: 38px;
@@ -632,15 +639,15 @@
 .mask {
   position: fixed;
   left: 0;
   top: 0;
   width: 100%;
   height: 100%;
   background: rgba(255, 255, 255, 0.2);
-  z-index: 2;
+  z-index: 4;
   display: none;
 }
 .mask .content {
   width: 80%;
   height: calc(100% - 140px);
   margin: auto;
   margin-top: 60px;
@@ -686,15 +693,15 @@
 }
 
 .footer {
   height: 120px;
   color: #999;
   min-width: 1160px;
   border-top: solid 1px #172036;
-  position: relative;
+  position: absolute;
   width: 100%;
   bottom: -219px;
   left: 0;
 }
 .footer-content {
   display: flex;
   align-items: center;
@@ -835,8 +842,8 @@
   background-color: #9f9f9f;
   -webkit-border-radius: 4px;
 }
 
 
 /* 分页 */
 
-.ui-paging-container{color:#666;font-size:12px}.ui-paging-container ul{overflow:hidden;text-align:center}.ui-paging-container li,.ui-paging-container ul{list-style:none}.ui-paging-container li{display:inline-block;padding:3px 6px;margin-left:5px;color:#666}.ui-paging-container li.ui-pager{cursor:pointer;border:1px solid #ddd;border-radius:2px}.ui-paging-container li.focus,.ui-paging-container li.ui-pager:hover{background-color:#288df0;color:#FFF}.ui-paging-container li.ui-paging-ellipse{border:none}.ui-paging-container li.ui-paging-toolbar{padding:0}.ui-paging-container li.ui-paging-toolbar select{height:22px;border:1px solid #ddd;color:#666}.ui-paging-container li.ui-paging-toolbar input{vertical-align:top;line-height:20px;height:20px;padding:0;border:1px solid #ddd;text-align:center;width:30px;margin:0 0 0 5px}.ui-paging-container li.ui-paging-toolbar a{text-decoration:none;display:inline-block;height:20px;border:1px solid #ddd;vertical-align:top;border-radius:2px;line-height:20px;padding:0 3px;cursor:pointer;margin-left:5px;color:#666}.ui-paging-container li.ui-pager-disabled,.ui-paging-container li.ui-pager-disabled:hover{background-color:#f6f6f6;cursor:default;border:none;color:#ddd}
+.ui-paging-container{color:#666;font-size:12px}.ui-paging-container ul{overflow:hidden;text-align:center}.ui-paging-container li,.ui-paging-container ul{list-style:none}.ui-paging-container li{display:inline-block;padding:3px 6px;margin-left:5px;color:#666}.ui-paging-container li.ui-pager{cursor:pointer;border:1px solid #ddd;border-radius:2px}.ui-paging-container li.focus,.ui-paging-container li.ui-pager:hover{background-color:#288df0;color:#FFF}.ui-paging-container li.ui-paging-ellipse{border:none}.ui-paging-container li.ui-paging-toolbar{padding:0}.ui-paging-container li.ui-paging-toolbar select{height:22px;border:1px solid #ddd;color:#666}.ui-paging-container li.ui-paging-toolbar input{vertical-align:top;line-height:20px;height:20px;padding:0;border:1px solid #ddd;text-align:center;width:30px;margin:0 0 0 5px}.ui-paging-container li.ui-paging-toolbar a{text-decoration:none;display:inline-block;height:20px;border:1px solid #ddd;vertical-align:top;border-radius:2px;line-height:20px;padding:0 3px;cursor:pointer;margin-left:5px;color:#666}.ui-paging-container li.ui-pager-disabled,.ui-paging-container li.ui-pager-disabled:hover{background-color:#f6f6f6;cursor:default;border:none;color:#ddd}
```

### Comparing `utx-1.3.3/utx/core/css/custom_report.py` & `utx-1.3.4/utx/core/css/custom_report.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  9/14/2021 4:36 PM
 @Desc    :  Custom Report line.
 """
-import io
 import os
+
 import jinja2
 
 CUSTOM_HTML_TPL = "summary_template_v2.html"
 CUSTOM_STATIC_DIR = os.path.dirname(__file__)
 
 
-def gen_report(results=None, report_path=None, report_name='utx_summary.html'):
+def gen_report(results=None, report_path=None, report_name="utx_summary.html"):
     """
     gen_report
     :param report_name: custom name
     :param results: results list
     :param report_path: report_path
     :return: custom report html
     """
     format_list = []
     for i in results:
         if i not in format_list:
             format_list.append(i)
 
     for f in format_list:
         result = []
-        for res in f['result']:
+        for res in f["result"]:
             if res not in result:
                 result.append(res)
-        f['result'] = result
+        f["result"] = result
 
     env = jinja2.Environment(
         loader=jinja2.FileSystemLoader(CUSTOM_STATIC_DIR),
         extensions=(),
-        autoescape=True
+        autoescape=True,
     )
     template = env.get_template(CUSTOM_HTML_TPL, CUSTOM_STATIC_DIR)
     html = template.render({"results": format_list})
     output_file = os.path.join(report_path, report_name)
-    with io.open(output_file, 'w', encoding="utf-8") as f:
+    with open(output_file, "w", encoding="utf-8") as f:
         f.write(html)
     print(output_file)
```

### Comparing `utx-1.3.3/utx/core/css/fonts/SourceHanSansCN-Regular.ttf` & `utx-1.3.4/utx/core/css/fonts/SourceHanSansCN-Regular.ttf`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/fonts/glyphicons-halflings-regular.eot` & `utx-1.3.4/utx/core/css/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/fonts/glyphicons-halflings-regular.svg` & `utx-1.3.4/utx/core/css/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/fonts/glyphicons-halflings-regular.ttf` & `utx-1.3.4/utx/core/css/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/fonts/glyphicons-halflings-regular.woff` & `utx-1.3.4/utx/core/css/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/fonts/glyphicons-halflings-regular.woff2` & `utx-1.3.4/utx/core/css/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/arrow.png` & `utx-1.3.4/utx/core/css/image/arrow.png`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/back.svg` & `utx-1.3.4/utx/core/css/image/back.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/broken.png` & `utx-1.3.4/utx/core/css/image/broken.png`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/close.svg` & `utx-1.3.4/utx/core/css/image/close.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/console_hover.svg` & `utx-1.3.4/utx/core/css/image/console_hover.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/console_normal.svg` & `utx-1.3.4/utx/core/css/image/console_normal.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/copy.svg` & `utx-1.3.4/utx/core/css/image/copy.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/download_log.svg` & `utx-1.3.4/utx/core/css/image/download_log.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/eye.svg` & `utx-1.3.4/utx/core/css/image/eye.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/fail.svg` & `utx-1.3.4/utx/core/css/image/fail.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/less.svg` & `utx-1.3.4/utx/core/css/image/less.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/maximize.svg` & `utx-1.3.4/utx/core/css/image/maximize.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/minimize.svg` & `utx-1.3.4/utx/core/css/image/minimize.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/more.svg` & `utx-1.3.4/utx/core/css/image/more.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/open_in_new_tab.svg` & `utx-1.3.4/utx/core/css/image/open_in_new_tab.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/step_fail.svg` & `utx-1.3.4/utx/core/css/image/step_fail.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/step_success.svg` & `utx-1.3.4/utx/core/css/image/step_success.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/success.svg` & `utx-1.3.4/utx/core/css/image/success.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/target.png` & `utx-1.3.4/utx/core/css/image/target.png`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/image/time.svg` & `utx-1.3.4/utx/core/css/image/time.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/js/bootstrap.min.js` & `utx-1.3.4/utx/core/css/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/js/echarts/echarts.common.min.js` & `utx-1.3.4/utx/core/css/js/echarts/echarts.common.min.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/js/echarts/pfm_charts.js` & `utx-1.3.4/utx/core/css/js/echarts/pfm_charts.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/js/echarts/shine.js` & `utx-1.3.4/utx/core/css/js/echarts/shine.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/js/highlight.min.js` & `utx-1.3.4/utx/core/css/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/js/jquery-1.10.2.min.js` & `utx-1.3.4/utx/core/css/js/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/js/jquery-lang.js` & `utx-1.3.4/utx/core/css/js/jquery-lang.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/js/langpack/zh_CN.js` & `utx-1.3.4/utx/core/css/js/langpack/zh_CN.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/js/lazyload.js` & `utx-1.3.4/utx/core/css/js/lazyload.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/js/paging.js` & `utx-1.3.4/utx/core/css/js/paging.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/js/report.js` & `utx-1.3.4/utx/core/css/js/report.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -19,14 +19,15 @@
     this.stepRight = $('#step-right')
     this.magnifyContainer = $('#magnify .content')
     this.magnifyPic = $('#magnify')
     this.scale = 0
     this.order = 'acc' // or dec
     this.duration = 'acc' // or dec
     this.status = 'acc' // or dec
+    this.thumbnail_step_list = []
 
     this.init = function() {
         // 初始化
         this.initStepData()
         this.bindEvents()
         this.init_gallery()
         this.init_pagenation()
@@ -117,14 +118,41 @@
         })
         $("#close-console").click(function() {
             $('#console').fadeOut(300)
         })
         $("#show-console").click(function() {
             $('#console').fadeIn(300)
         })
+        document.body.onkeydown = (e) => {
+            e = window.event || e;
+            switch (e.keyCode) {
+                case 37:
+                    //左键
+                    this.jumpToPreThumbNail()
+                    break;
+                case 38:
+                    //向上键
+                    //禁用触发页面滚动
+                    e.preventDefault();
+                    this.jumpToPreThumbNail()
+                    break;
+                case 39:
+                    //右键
+                    this.jumpToNextThumbNail()
+                    break;
+                case 40:
+                    //向下键
+                    //禁用触发页面滚动
+                    e.preventDefault();
+                    this.jumpToNextThumbNail()
+                    break;
+                default:
+                    break;
+            }
+        }
     }
 
     this.sortSteps = function(attr, rev) {
         //第二个参数没有传递 默认升序排列
         if (rev == undefined) {
             rev = 1;
         } else {
@@ -184,14 +212,22 @@
                 step.duration_ms = getDelta(step.time, this.data.run_start)
             } else {
                 step.duration_ms = getDelta(step.time, this.steps[i - 1].time)
             }
             step.duration = getFormatDuration(step.duration_ms)
             step.index = i
             step.status = step.traceback ? 'fail' : 'success'
+            this.thumbnail_step_list = this.original_steps.map(function(step) {
+                if (step.screen && step.screen.thumbnail) {
+                    return step.index
+                }
+            })
+            this.thumbnail_step_list = this.thumbnail_step_list.filter((val) => {
+                return val != null
+            })
         }
     }
 
     this.init_gallery = function() {
         var that = this
         var fragment = this.original_steps.map(function(step) {
             if (step.screen && step.screen.thumbnail) {
@@ -217,14 +253,42 @@
         this.steps = [].concat(this.original_steps)
         this.currentPage = Math.floor(step / this.pagesize) + 1
         this.setPagenation()
         this.setStepRight(step)
         $('.steps .filter').removeClass('active')
     }
 
+    this.jumpToNextThumbNail = function() {
+        this.jumpToThumbNail('next')
+    }
+
+    this.jumpToPreThumbNail = function() {
+        this.jumpToThumbNail('pre')
+    }
+
+    this.jumpToThumbNail = function(op) {
+        let cur_thumbnail_step_index = this.thumbnail_step_list.findIndex((val) => {
+            return val == this.currentStep
+        })
+        let nxt_thumbnail_step_index = 0
+
+        if (op == 'next') {
+            if (cur_thumbnail_step_index < this.thumbnail_step_list.length - 1) {
+                nxt_thumbnail_step_index = this.thumbnail_step_list[cur_thumbnail_step_index + 1]
+            }
+        } else if (op == 'pre') {
+            if (cur_thumbnail_step_index > 0) {
+                nxt_thumbnail_step_index = this.thumbnail_step_list[cur_thumbnail_step_index - 1]
+            }
+        }
+        this.currentStep = nxt_thumbnail_step_index
+        this.currentPage = Math.ceil(this.currentStep / this.pagesize)
+        this.setSteps(this.currentStep)
+    }
+
     this.showMagnifyPic = function(fragment) {
         this.magnifyContainer.html(fragment)
         this.magnifyContainer.children().removeAttr('style')
         var fancybox = this.magnifyContainer.find('.fancybox')
         if (fancybox.length > 0) {
             var that = this
             $('#magnify .fancybox .screen').load(function(e) {
@@ -285,15 +349,15 @@
             .format(success, pass, step.index + 1, title)
         var infos = this.getStepRightInfo(step)
         var args = this.getStepRightArgs(step)
         this.stepRight.html(head + infos + args)
     }
 
     this.getStepRightInfo = function(step) {
-        // HTML 本步骤成功与否、耗时 
+        // HTML 本步骤成功与否、耗时
         try {
             return ("<div class='step-infos'>" +
                 "<div class='infos-li'>" +
                 "<span lang='en'>Status: </span>" +
                 "<span class='content-val %s'>%s</span>" +
                 "<img src='%simage/step_%s.svg'>" +
                 "</div>" +
@@ -782,21 +846,53 @@
     $('.summary #result-desc').html("[%s]".format(result))
 }
 
 function init_page() {
     $('.summary .info-sub.start').html(getFormatDate(data.run_start))
     $('.summary .info-sub.time').html(getFormatTime(data.run_start) + '-' + getFormatTime(data.run_end))
     $('.summary .info-value.duration').html(getFormatDuration(getDelta(data.run_end, data.run_start)))
+    setImgAffix()
 }
 
 function hideFancybox(img) {
     // 图片加载失败的情况下，隐藏整个div
     $(img).parent().hide();
 }
 
+function setImgAffix() {
+    // 延迟触发，等待其他元素渲染完成再去获取，否则获取的值有误
+    setTimeout(() => {
+        // 获取页面加载时快览与页面顶端的距离
+        var stickyHeaderTop = $('.gallery .content').offset().top
+        // 在快览滑动到顶端时将其设置为固钉，添加页面滚动的监听事件
+        $(window).scroll(function() {
+            if ($(window).scrollTop() > stickyHeaderTop) {
+                $('.gallery .content').css({
+                    position: 'fixed',
+                    top: '0px'
+                })
+            } else {
+                $('.gallery .content').css({
+                    position: 'relative',
+                    top: '0px'
+                })
+            }
+        })
+        // 计算需要占位的高度
+        var placeHolderHeight = $('.gallery .placeholder').height()
+        var placeHolderWidth = $('.gallery .content').width()
+        $('.gallery .placeholder').css({
+            minHeight: placeHolderHeight
+        })
+        $('.gallery .content').css({
+            maxWidth: placeHolderWidth
+        })
+    }, 500)
+}
+
 $(function() {
     init_page()
     stepPanel = new StepPannel(data)
     stepPanel.init()
     $("img").error(function() {
         var orsrc = $(this).attr("src")
         if (!orsrc) {
```

### Comparing `utx-1.3.3/utx/core/css/report.py` & `utx-1.3.4/utx/core/css/report.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,84 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  8/31/2021 10:42 PM
 @Desc    :  Report line.
 """
-
 import json
 import os
-import io
 import re
-import six
-import sys
-from PIL import Image
 import shutil
-import jinja2
+import sys
 import traceback
 from copy import deepcopy
 from datetime import datetime
-from jinja2 import pass_eval_context
-from markupsafe import Markup, escape
-from airtest.aircv import imread, get_resolution
-from airtest.core.settings import Settings as ST
+
+import jinja2
+from airtest.aircv import get_resolution
+from airtest.aircv import imread
 from airtest.aircv.utils import compress_image
-from airtest.utils.compat import decode_path, script_dir_name
 from airtest.cli.info import get_script_info
+from airtest.core.settings import Settings as ST
+from airtest.utils.compat import decode_path
+from airtest.utils.compat import script_dir_name
 from airtest.utils.logger import get_logger
+from jinja2 import pass_eval_context
+from markupsafe import escape
+from markupsafe import Markup
+from PIL import Image
 from six import PY3
 
 LOGGING = get_logger(__name__)
 DEFAULT_LOG_DIR = "log"
 DEFAULT_LOG_FILE = "log.txt"
 HTML_TPL = "log_template.html"
 HTML_FILE = "log.html"
 STATIC_DIR = os.path.dirname(__file__)
 
 
-_paragraph_re = re.compile(r'(?:\r\n|\r|\n){2,}')
+_paragraph_re = re.compile(r"(?:\r\n|\r|\n){2,}")
 
 
 @pass_eval_context
 def nl2br(eval_ctx, value):
-    result = u'\n\n'.join(u'<p>%s</p>' % p.replace('\n', '<br>\n')
-                          for p in _paragraph_re.split(escape(value)))
+    result = "\n\n".join(
+        "<p>%s</p>" % p.replace("\n", "<br>\n")
+        for p in _paragraph_re.split(escape(value))
+    )
     if eval_ctx.autoescape:
         result = Markup(result)
     return result
 
 
 def timefmt(timestamp):
     """
     Formatting of timestamp in Jinja2 templates
     :param timestamp: timestamp of steps
     :return: "%Y-%m-%d %H:%M:%S"
     """
     return datetime.fromtimestamp(timestamp).strftime("%Y-%m-%d %H:%M:%S")
 
 
-class LogToHtml(object):
-    """Convert log to html display """
+class LogToHtml:
+    """Convert log to html display"""
+
     scale = 0.5
 
-    def __init__(self, script_root, log_root="", static_root="", export_dir=None, script_name="", logfile=None, lang="en", plugins=None):
+    def __init__(
+        self,
+        script_root,
+        log_root="",
+        static_root="",
+        export_dir=None,
+        script_name="",
+        logfile=None,
+        lang="en",
+        plugins=None,
+    ):
         self.log = []
         self.script_root = script_root
         self.script_name = script_name
         if not self.script_name or os.path.isfile(self.script_root):
             self.script_root, self.script_name = script_dir_name(self.script_root)
         self.log_root = log_root or ST.LOG_DIR or os.path.join(".", DEFAULT_LOG_DIR)
         self.static_root = static_root or STATIC_DIR
@@ -89,130 +101,139 @@
             except:
                 LOGGING.error(traceback.format_exc())
 
     def _load(self):
         logfile = os.path.join(self.log_root, self.logfile)
         if not PY3:
             logfile = logfile.encode(sys.getfilesystemencoding())
-        with io.open(logfile, encoding="utf-8") as f:
+        with open(logfile, encoding="utf-8") as f:
             for line in f.readlines():
                 self.log.append(json.loads(line))
 
     def _analyse(self):
-        """ 解析log成可渲染的dict """
+        """解析log成可渲染的dict"""
         steps = []
         children_steps = []
 
         for log in self.log:
-            depth = log['depth']
+            depth = log["depth"]
 
             if not self.run_start:
-                self.run_start = log.get('data', {}).get('start_time', '') or log["time"]
+                self.run_start = (
+                    log.get("data", {}).get("start_time", "") or log["time"]
+                )
             self.run_end = log["time"]
 
             if depth == 0:
                 # single log line, not in stack
                 steps.append(log)
             elif depth == 1:
                 step = deepcopy(log)
                 step["__children__"] = children_steps
                 steps.append(step)
                 children_steps = []
             else:
                 children_steps.insert(0, log)
 
         translated_steps = [self._translate_step(s) for s in steps]
+        if len(translated_steps) > 0 and translated_steps[-1].get("traceback"):
+            # Final Error
+            self.test_result = False
         return translated_steps
 
     def _translate_step(self, step):
         """translate single step"""
         name = step["data"]["name"]
         title = self._translate_title(name, step)
         code = self._translate_code(step)
         desc = self._translate_desc(step, code)
         screen = self._translate_screen(step, code)
         info = self._translate_info(step)
         assertion = self._translate_assertion(step)
 
-        # set test failed if any traceback exists
-        if info[0]:
-            self.test_result = False
-
         translated = {
             "title": title,
             "time": step["time"],
             "code": code,
             "screen": screen,
             "desc": desc,
             "traceback": info[0],
             "log": info[1],
             "assert": assertion,
         }
         return translated
 
     def _translate_assertion(self, step):
-        if "assert_" in step["data"].get("name", "") and "msg" in step["data"].get("call_args", {}):
+        if "assert_" in step["data"].get("name", "") and "msg" in step["data"].get(
+            "call_args", {}
+        ):
             return step["data"]["call_args"]["msg"]
 
     def _translate_screen(self, step, code):
-        if step['tag'] not in ["function", "info"] or not step.get("__children__"):
+        if step["tag"] not in ["function", "info"] or not step.get("__children__"):
             return None
         screen = {
             "src": None,
             "rect": [],
             "pos": [],
             "vector": [],
             "confidence": None,
         }
 
         for item in step["__children__"]:
             if item["data"]["name"] == "try_log_screen":
                 snapshot = item["data"].get("ret", None)
-                if isinstance(snapshot, six.text_type):
+                if isinstance(snapshot, str):
                     src = snapshot
                 elif isinstance(snapshot, dict):
-                    src = snapshot['screen']
-                    screen['resolution'] = snapshot['resolution']
+                    src = snapshot["screen"]
+                    screen["resolution"] = snapshot["resolution"]
                 else:
                     continue
                 if self.export_dir:  # all relative path
-                    screen['_filepath'] = os.path.join(DEFAULT_LOG_DIR, src)
+                    screen["_filepath"] = os.path.join(DEFAULT_LOG_DIR, src)
                 else:
-                    screen['_filepath'] = os.path.abspath(os.path.join(self.log_root, src))
-                screen['src'] = screen['_filepath']
+                    screen["_filepath"] = os.path.abspath(
+                        os.path.join(self.log_root, src)
+                    )
+                screen["src"] = screen["_filepath"]
                 self.get_thumbnail(os.path.join(self.log_root, src))
-                screen['thumbnail'] = self.get_small_name(screen['src'])
+                screen["thumbnail"] = self.get_small_name(screen["src"])
                 break
 
         display_pos = None
 
         for item in step["__children__"]:
-            if item["data"]["name"] == "_cv_match" and isinstance(item["data"].get("ret"), dict):
+            if item["data"]["name"] == "_cv_match" and isinstance(
+                item["data"].get("ret"), dict
+            ):
                 cv_result = item["data"]["ret"]
-                pos = cv_result['result']
+                pos = cv_result["result"]
                 if self.is_pos(pos):
                     display_pos = [round(pos[0]), round(pos[1])]
-                rect = self.div_rect(cv_result['rectangle'])
-                screen['rect'].append(rect)
-                screen['confidence'] = cv_result['confidence']
+                rect = self.div_rect(cv_result["rectangle"])
+                screen["rect"].append(rect)
+                screen["confidence"] = cv_result["confidence"]
                 break
 
         if step["data"]["name"] in ["touch", "assert_exists", "wait", "exists"]:
             # 将图像匹配得到的pos修正为最终pos
             if self.is_pos(step["data"].get("ret")):
                 display_pos = step["data"]["ret"]
             elif self.is_pos(step["data"]["call_args"].get("v")):
                 display_pos = step["data"]["call_args"]["v"]
 
         elif step["data"]["name"] == "swipe":
             if "ret" in step["data"]:
                 screen["pos"].append(step["data"]["ret"][0])
                 target_pos = step["data"]["ret"][1]
                 origin_pos = step["data"]["ret"][0]
-                screen["vector"].append([target_pos[0] - origin_pos[0], target_pos[1] - origin_pos[1]])
+                screen["vector"].append(
+                    [target_pos[0] - origin_pos[0], target_pos[1] - origin_pos[1]]
+                )
 
         if display_pos:
             screen["pos"].append(display_pos)
         return screen
 
     @classmethod
     def get_thumbnail(cls, path):
@@ -227,15 +248,15 @@
             return new_path
         else:
             return None
 
     @classmethod
     def get_small_name(cls, filename):
         name, ext = os.path.splitext(filename)
-        return "%s_small%s" % (name, ext)
+        return f"{name}_small{ext}"
 
     def _translate_info(self, step):
         trace_msg, log_msg = "", ""
         if "traceback" in step["data"]:
             # 若包含有traceback内容，将会认定步骤失败
             trace_msg = step["data"]["traceback"]
         if step["tag"] == "info":
@@ -250,123 +271,137 @@
         step_data = step["data"]
         args = []
         code = {
             "name": step_data["name"],
             "args": args,
         }
         for key, value in step_data["call_args"].items():
-            args.append({
-                "key": key,
-                "value": value,
-            })
+            args.append(
+                {
+                    "key": key,
+                    "value": value,
+                }
+            )
         for k, arg in enumerate(args):
             value = arg["value"]
             if isinstance(value, dict) and value.get("__class__") == "Template":
                 if self.export_dir:  # all relative path
-                    image_path = value['filename']
-                    if not os.path.isfile(os.path.join(self.script_root, image_path)) and value['_filepath']:
+                    image_path = value["filename"]
+                    if (
+                        not os.path.isfile(os.path.join(self.script_root, image_path))
+                        and value["_filepath"]
+                    ):
                         # copy image used by using statement
-                        shutil.copyfile(value['_filepath'], os.path.join(self.script_root, value['filename']))
+                        shutil.copyfile(
+                            value["_filepath"],
+                            os.path.join(self.script_root, value["filename"]),
+                        )
                 else:
-                    image_path = os.path.abspath(value['_filepath'] or value['filename'])
+                    image_path = os.path.abspath(
+                        value["_filepath"] or value["filename"]
+                    )
                 arg["image"] = image_path
-                if not value['_filepath'] and not os.path.exists(value['filename']):
-                    crop_img = imread(os.path.join(self.script_root, value['filename']))
+                if not value["_filepath"] and not os.path.exists(value["filename"]):
+                    crop_img = imread(os.path.join(self.script_root, value["filename"]))
                 else:
-                    crop_img = imread(value['_filepath'] or value['filename'])
+                    crop_img = imread(value["_filepath"] or value["filename"])
                 arg["resolution"] = get_resolution(crop_img)
         return code
 
     @staticmethod
     def div_rect(r):
         """count rect for js use"""
         xs = [p[0] for p in r]
         ys = [p[1] for p in r]
         left = min(xs)
         top = min(ys)
         w = max(xs) - left
         h = max(ys) - top
-        return {'left': left, 'top': top, 'width': w, 'height': h}
+        return {"left": left, "top": top, "width": w, "height": h}
 
     def _translate_desc(self, step, code):
-        """ 函数描述 """
-        if step['tag'] != "function":
+        """函数描述"""
+        if step["tag"] != "function":
             return None
-        name = step['data']['name']
-        res = step['data'].get('ret')
+        name = step["data"]["name"]
+        res = step["data"].get("ret")
         args = {i["key"]: i["value"] for i in code["args"]}
 
         desc = {
-            "snapshot": lambda: u"Screenshot description: %s" % args.get("msg"),
-            "touch": lambda: u"Touch %s" % ("target image" if isinstance(args['v'], dict) else "coordinates %s" % args['v']),
-            "swipe": u"Swipe on screen",
-            "wait": u"Wait for target image to appear",
-            "exists": lambda: u"Image %s exists" % ("" if res else "not"),
-            "text": lambda: u"Input text:%s" % args.get('text'),
-            "keyevent": lambda: u"Click [%s] button" % args.get('keyname'),
-            "sleep": lambda: u"Wait for %s seconds" % args.get('secs'),
-            "assert_exists": u"Assert target image exists",
-            "assert_not_exists": u"Assert target image does not exists",
+            "snapshot": lambda: "Screenshot description: %s" % args.get("msg"),
+            "touch": lambda: "Touch %s"
+            % (
+                "target image"
+                if isinstance(args["v"], dict)
+                else "coordinates %s" % args["v"]
+            ),
+            "swipe": "Swipe on screen",
+            "wait": "Wait for target image to appear",
+            "exists": lambda: "Image %s exists" % ("" if res else "not"),
+            "text": lambda: "Input text:%s" % args.get("text"),
+            "keyevent": lambda: "Click [%s] button" % args.get("keyname"),
+            "sleep": lambda: "Wait for %s seconds" % args.get("secs"),
+            "assert_exists": "Assert target image exists",
+            "assert_not_exists": "Assert target image does not exists",
         }
 
         # todo: 最好用js里的多语言实现
         desc_zh = {
-            "snapshot": lambda: u"截图描述: %s" % args.get("msg"),
-            "touch": lambda: u"点击 %s" % (u"目标图片" if isinstance(args['v'], dict) else u"屏幕坐标 %s" % args['v']),
-            "swipe": u"滑动操作",
-            "wait": u"等待目标图片出现",
-            "exists": lambda: u"图片%s存在" % ("" if res else u"不"),
-            "text": lambda: u"输入文字:%s" % args.get('text'),
-            "keyevent": lambda: u"点击[%s]按键" % args.get('keyname'),
-            "sleep": lambda: u"等待%s秒" % args.get('secs'),
-            "assert_exists": u"断言目标图片存在",
-            "assert_not_exists": u"断言目标图片不存在",
+            "snapshot": lambda: "截图描述: %s" % args.get("msg"),
+            "touch": lambda: "点击 %s"
+            % ("目标图片" if isinstance(args["v"], dict) else "屏幕坐标 %s" % args["v"]),
+            "swipe": "滑动操作",
+            "wait": "等待目标图片出现",
+            "exists": lambda: "图片%s存在" % ("" if res else "不"),
+            "text": lambda: "输入文字:%s" % args.get("text"),
+            "keyevent": lambda: "点击[%s]按键" % args.get("keyname"),
+            "sleep": lambda: "等待%s秒" % args.get("secs"),
+            "assert_exists": "断言目标图片存在",
+            "assert_not_exists": "断言目标图片不存在",
         }
 
         if self.lang == "zh":
             desc = desc_zh
 
         ret = desc.get(name)
         if callable(ret):
             ret = ret()
         return ret
 
     def _translate_title(self, name, step):
         title = {
-            "touch": u"Touch",
-            "swipe": u"Swipe",
-            "wait": u"Wait",
-            "exists": u"Exists",
-            "text": u"Text",
-            "keyevent": u"Keyevent",
-            "sleep": u"Sleep",
-            "assert_exists": u"Assert exists",
-            "assert_not_exists": u"Assert not exists",
-            "snapshot": u"Snapshot",
-            "assert_equal": u"Assert equal",
-            "assert_not_equal": u"Assert not equal",
+            "touch": "Touch",
+            "swipe": "Swipe",
+            "wait": "Wait",
+            "exists": "Exists",
+            "text": "Text",
+            "keyevent": "Keyevent",
+            "sleep": "Sleep",
+            "assert_exists": "Assert exists",
+            "assert_not_exists": "Assert not exists",
+            "snapshot": "Snapshot",
+            "assert_equal": "Assert equal",
+            "assert_not_equal": "Assert not equal",
         }
 
         return title.get(name, name)
 
     @staticmethod
     def _render(template_name, output_file=None, **template_vars):
-        """ 用jinja2渲染html"""
+        """用jinja2渲染html"""
         env = jinja2.Environment(
-            loader=jinja2.FileSystemLoader(STATIC_DIR),
-            extensions=(),
-            autoescape=True
+            loader=jinja2.FileSystemLoader(STATIC_DIR), extensions=(), autoescape=True
         )
-        env.filters['nl2br'] = nl2br
-        env.filters['datetime'] = timefmt
+        env.filters["nl2br"] = nl2br
+        env.filters["datetime"] = timefmt
         template = env.get_template(template_name)
         html = template.render(**template_vars)
 
         if output_file:
-            with io.open(output_file, 'w', encoding="utf-8") as f:
+            with open(output_file, "w", encoding="utf-8") as f:
                 f.write(html)
             LOGGING.info(output_file)
 
         return html
 
     def is_pos(self, v):
         return isinstance(v, (list, tuple))
@@ -376,37 +411,45 @@
             shutil.copytree(src, dst, ignore=ignore)
         except:
             LOGGING.error(traceback.format_exc())
 
     def _make_export_dir(self):
         """mkdir & copy /staticfiles/screenshots"""
         # let dirname = <script name>.log
-        dirname = self.script_name.replace(os.path.splitext(self.script_name)[1], ".log")
+        dirname = self.script_name.replace(
+            os.path.splitext(self.script_name)[1], ".log"
+        )
         # mkdir
         dirpath = os.path.join(self.export_dir, dirname)
         if os.path.isdir(dirpath):
             shutil.rmtree(dirpath, ignore_errors=True)
 
         # copy script
         def ignore_export_dir(dirname, filenames):
             # 忽略当前导出的目录，防止递归导出
             if os.path.commonprefix([dirpath, dirname]) == dirpath:
                 return filenames
             return []
+
         self.copy_tree(self.script_root, dirpath, ignore=ignore_export_dir)
         # copy log
         logpath = os.path.join(dirpath, DEFAULT_LOG_DIR)
         if os.path.normpath(logpath) != os.path.normpath(self.log_root):
             if os.path.isdir(logpath):
                 shutil.rmtree(logpath, ignore_errors=True)
-            self.copy_tree(self.log_root, logpath, ignore=shutil.ignore_patterns(dirname))
+            self.copy_tree(
+                self.log_root, logpath, ignore=shutil.ignore_patterns(dirname)
+            )
         # if self.static_root is not a http server address, copy static files from local directory
         if not self.static_root.startswith("http"):
             for subdir in ["css", "fonts", "image", "js"]:
-                self.copy_tree(os.path.join(self.static_root, subdir), os.path.join(dirpath, "static", subdir))
+                self.copy_tree(
+                    os.path.join(self.static_root, subdir),
+                    os.path.join(dirpath, "static", subdir),
+                )
 
         return dirpath, logpath
 
     def get_relative_log(self, output_file):
         """
         Try to get the relative path of log.txt
         :param output_file: output file: log.html
@@ -421,30 +464,34 @@
             return os.path.relpath(os.path.join(self.log_root, self.logfile), html_dir)
         except:
             LOGGING.error(traceback.format_exc())
             return ""
 
     def get_console(self, output_file):
         html_dir = os.path.dirname(output_file)
-        file = os.path.join(html_dir, 'console.txt')
+        file = os.path.join(html_dir, "console.txt")
         content = ""
         if os.path.isfile(file):
             try:
                 content = self.readFile(file)
             except Exception:
                 try:
                     content = self.readFile(file, "gbk")
                 except Exception:
                     content = traceback.format_exc() + content
-                    content = content + "Can not read console.txt. Please check file in:\n" + file
+                    content = (
+                        content
+                        + "Can not read console.txt. Please check file in:\n"
+                        + file
+                    )
         return content
 
-    def readFile(self, filename, code='utf-8'):
+    def readFile(self, filename, code="utf-8"):
         content = ""
-        with io.open(filename, encoding=code) as f:
+        with open(filename, encoding=code) as f:
             for line in f.readlines():
                 content = content + line
         return content
 
     def report_data(self, output_file=None, record_list=None, base_dir=None):
         """
         Generate data for the report page
@@ -459,49 +506,61 @@
         self._load()
         steps = self._analyse()
 
         script_path = os.path.join(self.script_root, self.script_name)
         info = json.loads(get_script_info(script_path))
 
         if record_list:
-            records = [os.path.join(DEFAULT_LOG_DIR, f) if self.export_dir
-                       else os.path.abspath(os.path.join(self.log_root, f)).replace(root, "..\\..\\..") for f in record_list]
+            records = [
+                os.path.join(DEFAULT_LOG_DIR, f)
+                if self.export_dir
+                else os.path.abspath(os.path.join(self.log_root, f)).replace(
+                    root, "..\\..\\.."
+                )
+                for f in record_list
+            ]
         else:
             records = []
 
         if not self.static_root.endswith(os.path.sep):
             self.static_root = self.static_root.replace("\\", "/")
             self.static_root += "/"
 
         if not output_file:
             output_file = HTML_FILE
 
         data = {}
-        data['steps'] = steps
-        data['name'] = self.script_root
-        data['scale'] = self.scale
-        data['test_result'] = self.test_result
-        data['run_end'] = self.run_end
-        data['run_start'] = self.run_start
-        data['static_root'] = self.static_root
-        data['lang'] = self.lang
-        data['records'] = records
-        data['info'] = info
-        data['log'] = self.get_relative_log(output_file)
-        data['console'] = self.get_console(output_file)
+        data["steps"] = steps
+        data["name"] = self.script_root
+        data["scale"] = self.scale
+        data["test_result"] = self.test_result
+        data["run_end"] = self.run_end
+        data["run_start"] = self.run_start
+        data["static_root"] = self.static_root
+        data["lang"] = self.lang
+        data["records"] = records
+        data["info"] = info
+        data["log"] = self.get_relative_log(output_file)
+        data["console"] = self.get_console(output_file)
         # 如果带有<>符号，容易被highlight.js认为是特殊语法，有可能导致页面显示异常，尝试替换成不常用的{}
         info = json.dumps(data).replace("<", "{").replace(">", "}")
-        data['data'] = info
+        data["data"] = info
 
         # 修改路径
 
-        data['data'] = json.dumps(data).replace(root, "..\\\\..\\\\..")
+        data["data"] = json.dumps(data).replace(root, "..\\\\..\\\\..")
         return data
 
-    def report(self, template_name=HTML_TPL, output_file=HTML_FILE, record_list=None, base_dir=None):
+    def report(
+        self,
+        template_name=HTML_TPL,
+        output_file=HTML_FILE,
+        record_list=None,
+        base_dir=None,
+    ):
         """
         Generate the report page, you can add custom data and overload it if needed
 
         :param template_name: default is HTML_TPL
         :param output_file: The file name or full path of the output file, default HTML_FILE
         :param record_list: List of screen recording files
         :param base_dir:
@@ -509,60 +568,92 @@
         """
         if not self.script_name:
             path, self.script_name = script_dir_name(self.script_root)
 
         if self.export_dir:
             self.script_root, self.log_root = self._make_export_dir()
             # output_file可传入文件名，或绝对路径
-            output_file = output_file if output_file and os.path.isabs(output_file) \
+            output_file = (
+                output_file
+                if output_file and os.path.isabs(output_file)
                 else os.path.join(self.script_root, output_file or HTML_FILE)
+            )
             if not self.static_root.startswith("http"):
                 self.static_root = "static/"
 
         if not record_list:
             record_list = [f for f in os.listdir(self.log_root) if f.endswith(".mp4")]
-        data = self.report_data(output_file=output_file, record_list=record_list, base_dir=base_dir)
+        data = self.report_data(
+            output_file=output_file, record_list=record_list, base_dir=base_dir
+        )
         return self._render(template_name, output_file, **data)
 
 
 def simple_report(filepath, logpath=True, logfile=None, output=HTML_FILE):
     path, name = script_dir_name(filepath)
     if logpath is True:
         logpath = os.path.join(path, getattr(ST, "LOG_DIR", DEFAULT_LOG_DIR))
-    rpt = LogToHtml(path, logpath, logfile=logfile or getattr(ST, "LOG_FILE", DEFAULT_LOG_FILE), script_name=name)
+    rpt = LogToHtml(
+        path,
+        logpath,
+        logfile=logfile or getattr(ST, "LOG_FILE", DEFAULT_LOG_FILE),
+        script_name=name,
+    )
     rpt.report(HTML_TPL, output_file=output)
 
 
 def get_parger(ap):
     ap.add_argument("script", help="script filepath")
-    ap.add_argument("--outfile", help="output html filepath, default to be log.html", default=HTML_FILE)
+    ap.add_argument(
+        "--outfile",
+        help="output html filepath, default to be log.html",
+        default=HTML_FILE,
+    )
     ap.add_argument("--static_root", help="static files root dir")
-    ap.add_argument("--log_root", help="log & screen data root dir, logfile should be log_root/log.txt")
+    ap.add_argument(
+        "--log_root",
+        help="log & screen data root dir, logfile should be log_root/log.txt",
+    )
     ap.add_argument("--record", help="custom screen record file path", nargs="+")
-    ap.add_argument("--export", help="export a portable report dir containing all resources")
+    ap.add_argument(
+        "--export", help="export a portable report dir containing all resources"
+    )
     ap.add_argument("--lang", help="report language", default="en")
     ap.add_argument("--plugins", help="load reporter plugins", nargs="+")
-    ap.add_argument("--report", help="placeholder for report cmd", default=True, nargs="?")
+    ap.add_argument(
+        "--report", help="placeholder for report cmd", default=True, nargs="?"
+    )
     return ap
 
 
 def main(args):
     # script filepath
     path, name = script_dir_name(args.script)
     record_list = args.record or []
-    log_root = decode_path(args.log_root) or decode_path(os.path.join(path, DEFAULT_LOG_DIR))
+    log_root = decode_path(args.log_root) or decode_path(
+        os.path.join(path, DEFAULT_LOG_DIR)
+    )
     static_root = args.static_root or STATIC_DIR
     static_root = decode_path(static_root)
     export = decode_path(args.export) if args.export else None
-    lang = args.lang if args.lang in ['zh', 'en'] else 'en'
+    lang = args.lang if args.lang in ["zh", "en"] else "en"
     plugins = args.plugins
 
     # gen html report
-    rpt = LogToHtml(path, log_root, static_root, export_dir=export, script_name=name, lang=lang, plugins=plugins)
+    rpt = LogToHtml(
+        path,
+        log_root,
+        static_root,
+        export_dir=export,
+        script_name=name,
+        lang=lang,
+        plugins=plugins,
+    )
     rpt.report(HTML_TPL, output_file=args.outfile, record_list=record_list)
 
 
 if __name__ == "__main__":
     import argparse
+
     ap = argparse.ArgumentParser()
     args = get_parger(ap).parse_args()
     main(args)
```

### Comparing `utx-1.3.3/utx/core/css/summary_template.html` & `utx-1.3.4/utx/core/css/summary_template.html`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/css/summary_template_pool.html` & `utx-1.3.4/utx/core/css/summary_template_pool.html`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/core/utils/hook.py` & `utx-1.3.4/utx/core/utils/hook.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  9/14/2021 3:36 PM
 @Desc    :  Hook line.
 """
 import logging
 import random
+from logging import getLogger
 
 import allure
 import pytest
-
-from logging import getLogger
 from airtest.core.api import *
-from airtest.core.error import AdbError, DeviceConnectionError
-from airtest.core.helper import device_platform, ST
-from popups.dismiss import popup, UT
-from selenium.webdriver.chrome.options import Options
+from airtest.core.error import AdbError
+from airtest.core.error import DeviceConnectionError
+from airtest.core.helper import device_platform
+from airtest.core.helper import ST
+from popups.dismiss import popup
+from popups.dismiss import UT
 from selenium import webdriver
-from webdriver_manager.chrome import ChromeDriverManager
-from tenacity import Retrying, wait_fixed, stop_after_attempt
+from selenium.webdriver.chrome.options import Options
+from tenacity import Retrying
+from tenacity import stop_after_attempt
+from tenacity import wait_fixed
 from wda import WDAError
+from webdriver_manager.chrome import ChromeDriverManager
+
 from utx.core.css.custom_report import gen_report
+from utx.core.utils.tools import check_network
+from utx.core.utils.tools import check_port
+from utx.core.utils.tools import cleanup
+from utx.core.utils.tools import decryption
+from utx.core.utils.tools import device_udid
 from utx.core.utils.tools import display
-from utx.core.utils.tools import str_to_bool, check_port, decryption, plat, download, device_udid, cleanup, proxy, \
-    check_network
+from utx.core.utils.tools import download
+from utx.core.utils.tools import plat
+from utx.core.utils.tools import proxy
+from utx.core.utils.tools import str_to_bool
 
-os.environ['WDM_SSL_VERIFY'] = '0'
+os.environ["WDM_SSL_VERIFY"] = "0"
 logger = getLogger(__name__)
 
 ST.THRESHOLD = 0.7
 ST.OPDELAY = 0.25
 ST.FIND_TIMEOUT = 10
 ST.FIND_TIMEOUT_TMP = 2
 ST.SNAPSHOT_QUALITY = 10
@@ -39,79 +49,95 @@
 # todo https://github.com/openutx/utx-pypi/issues/4
 # 1.全部都截图，不管成功失败
 # 2.只有失败才截图
 # 3.配置化
 ST.SAVE_IMAGE = True
 
 
-def app_info(cli_platform, cli_device, cli_wda, cli_init, ini_platform, ini_device, ini_wda, ini_init):
+def app_info(
+    cli_platform,
+    cli_device,
+    cli_wda,
+    cli_init,
+    ini_platform,
+    ini_device,
+    ini_wda,
+    ini_init,
+):
     """
 
     :param cli_platform:
     :param cli_device:
     :param cli_wda:
     :param cli_init:
     :param ini_platform:
     :param ini_device:
     :param ini_wda:
     :param ini_init:
     :return: iOS:///127.0.0.1:8100
     """
-    if cli_init in [None, '']:
+    if cli_init in [None, ""]:
         is_init = str_to_bool(ini_init)
     else:
         is_init = str_to_bool(cli_init)
-    if cli_wda in [None, '']:
+    if cli_wda in [None, ""]:
         web_driver_agent = ini_wda
         # web_driver_agent = "*WebDriverAgent*"
     else:
         web_driver_agent = cli_wda
         # web_driver_agent = "*WebDriverAgent*"
     # 改为通配符，避免传入错误 bundle_id 启动失败
 
-    if cli_platform in [None, '']:
+    if cli_platform in [None, ""]:
         platform = ini_platform.lower()
-        if platform in 'android':
-            device_idx = str(ini_device).split(',')
+        if platform in "android":
+            device_idx = str(ini_device).split(",")
             device_uri = []
             for idx in device_idx:
                 device_uri.append(
-                    'Android:///{}?cap_method=MINICAP&&ori_method=MINICAPORI&&touch_method=MAXTOUCH'.format(idx))
+                    f"Android:///{idx}?cap_method=MINICAP&&ori_method=MINICAPORI&&touch_method=MAXTOUCH"
+                )
             return device_uri, device_idx, is_init
-        elif platform in 'ios':
+        elif platform in "ios":
             device_idx = []
             device_uri = []
-            for u in device_udid(types='ios', state=None):
+            for u in device_udid(types="ios", state=None):
                 proxy_port = str(random.randint(50000, 60000) + 1)
                 check_port(port=proxy_port)
-                os.system('{} -u {} wdaproxy -B {} --port {} &'.format(decryption(b'dGlkZXZpY2U='), u, web_driver_agent,
-                                                                       proxy_port))
-                device_idx.append('127.0.0.1:{}'.format(proxy_port))
-                device_uri.append('iOS:///127.0.0.1:{}'.format(proxy_port))
+                os.system(
+                    "{} -u {} wdaproxy -B {} --port {} &".format(
+                        decryption(b"dGlkZXZpY2U="), u, web_driver_agent, proxy_port
+                    )
+                )
+                device_idx.append(f"127.0.0.1:{proxy_port}")
+                device_uri.append(f"iOS:///127.0.0.1:{proxy_port}")
             return device_uri, device_idx, is_init
 
-    elif cli_platform not in [None, '']:
-        if cli_platform.lower() in 'android':
-            device_idx = str(cli_device).split(',')
+    elif cli_platform not in [None, ""]:
+        if cli_platform.lower() in "android":
+            device_idx = str(cli_device).split(",")
             device_uri = []
             for idx in device_idx:
                 device_uri.append(
-                    'Android:///{}?cap_method=MINICAP&&ori_method=MINICAPORI&&touch_method=MAXTOUCH'.format(idx))
+                    f"Android:///{idx}?cap_method=MINICAP&&ori_method=MINICAPORI&&touch_method=MAXTOUCH"
+                )
             return device_uri, device_idx, is_init
-        elif cli_platform.lower() in 'ios':
+        elif cli_platform.lower() in "ios":
             device_idx = []
             device_uri = []
-            for u in device_udid(types='ios', state=None):
+            for u in device_udid(types="ios", state=None):
                 proxy_port = str(random.randint(50000, 60000) + 1)
                 check_port(port=proxy_port)
                 os.system(
-                    '{} -u {} wdaproxy -B {} --port {} &'.format(decryption(b'dGlkZXZpY2U='), u, web_driver_agent,
-                                                                 proxy_port))
-                device_idx.append('127.0.0.1:{}'.format(proxy))
-                device_uri.append('iOS:///127.0.0.1:{}'.format(proxy_port))
+                    "{} -u {} wdaproxy -B {} --port {} &".format(
+                        decryption(b"dGlkZXZpY2U="), u, web_driver_agent, proxy_port
+                    )
+                )
+                device_idx.append(f"127.0.0.1:{proxy}")
+                device_uri.append(f"iOS:///127.0.0.1:{proxy_port}")
             return device_uri, device_idx, is_init
 
 
 def my_before_sleep(retry_state):
     """
 
     :param retry_state:
@@ -120,15 +146,15 @@
     if retry_state.attempt_number < 1:
         loglevel = logging.INFO
     else:
         loglevel = logging.WARNING
 
     logging.log(
         loglevel,
-        'Retrying %s: attempt %s ended with: %s',
+        "Retrying %s: attempt %s ended with: %s",
         retry_state.fn,
         retry_state.attempt_number,
         retry_state.outcome,
     )
 
 
 @allure.step("Try to link the device！")
@@ -140,40 +166,44 @@
     :param sleeps:
     :param max_attempts:
     :return:
     """
     if not whether_retry:
         max_attempts = 1
 
-    r = Retrying(wait=wait_fixed(sleeps), stop=stop_after_attempt(max_attempts), before_sleep=my_before_sleep,
-                 reraise=True)
+    r = Retrying(
+        wait=wait_fixed(sleeps),
+        stop=stop_after_attempt(max_attempts),
+        before_sleep=my_before_sleep,
+        reraise=True,
+    )
     try:
         return r(connect_device, uri)
     except Exception as e:
         if isinstance(e, (WDAError,)):
             logger.info("Can't connect iphone, please check device or wda state!")
-        logger.info("Try connect device {} 3 times per wait 10 sec failed.".format(uri))
+        logger.info(f"Try connect device {uri} 3 times per wait 10 sec failed.")
         raise e
     finally:
-        logger.info("Retry connect statistics: {}".format(str(r.statistics)))
+        logger.info(f"Retry connect statistics: {str(r.statistics)}")
 
 
 @allure.step("Switch to current device！")
 def ensure_current_device(device_idx):
     """
 
     :param device_idx:
     :return:
     """
     idx = device_idx
     try:
         if device().uuid != idx:
             set_current(idx)
     except IndexError:
-        if device().uuid != 'http://{}'.format(idx):
+        if device().uuid != f"http://{idx}":
             set_current(idx)
 
 
 @allure.step("Try to wake up the current device！")
 def wake_device(current_device):
     """
 
@@ -186,15 +216,17 @@
             w, h = display()
             swipe((0.5 * w, 0.8 * h), (0.5 * w, 0.2 * h), duration=0.1)
         current_device.home()
     except AttributeError:
         pass
 
 
-def app_fixture(request, device_uri, app_filepath, app_name, device_idx, init, agent=False):
+def app_fixture(
+    request, device_uri, app_filepath, app_name, device_idx, init, agent=False
+):
     """
 
     :param request: default param
     :param device_uri: device_uri
     :param app_filepath: app_filepath
     :param app_name: app_name
     :param device_idx: device udid
@@ -204,43 +236,57 @@
     """
     with allure.step("Initialize and generate APP object！"):
         logger.info("Session start test.")
 
         try:
             app = None
             if init:
-                logger.info("Detected that the initialization is True and started installing the application！")
-                if str(device_uri[0]).startswith('iOS'):
-                    if 'http' in app_filepath:
-                        app_pkg = download(file_url=app_filepath, types='ipa')
+                logger.info(
+                    "Detected that the initialization is True and started installing the application！"
+                )
+                if str(device_uri[0]).startswith("iOS"):
+                    if "http" in app_filepath:
+                        app_pkg = download(file_url=app_filepath, types="ipa")
                     else:
                         app_pkg = app_filepath
                 else:
-                    if 'http' in app_filepath:
-                        app_pkg = download(file_url=app_filepath, types='apk')
+                    if "http" in app_filepath:
+                        app_pkg = download(file_url=app_filepath, types="apk")
                     else:
                         app_pkg = app_filepath
-            for (uri, idx) in zip(device_uri, device_idx):
+            for uri, idx in zip(device_uri, device_idx):
                 app = my_retry_connect(uri)
                 wake_device(G.DEVICE)
-                if device_platform().lower() in 'android':
+                if device_platform().lower() in "android":
                     if not check_network():
-                        warning_report = os.path.join(app_filepath.split('packages')[0], 'report', 'airtest')
-                        gen_report(results=[{'result': ['warning_report',
-                                                        "Warning: The current device network is abnormal, please check it and run it again!"]}],
-                                   report_path=warning_report)
+                        warning_report = os.path.join(
+                            app_filepath.split("packages")[0], "report", "airtest"
+                        )
+                        gen_report(
+                            results=[
+                                {
+                                    "result": [
+                                        "warning_report",
+                                        "Warning: The current device network is abnormal, please check it and run it again!",
+                                    ]
+                                }
+                            ],
+                            report_path=warning_report,
+                        )
                         # todo: xfail is skip ,fail is fail. Lack of multi-device differentiation.
-                        pytest.xfail(f'The current device {idx} network is abnormal, please check it and run it again!')
+                        pytest.xfail(
+                            f"The current device {idx} network is abnormal, please check it and run it again!"
+                        )
                     if agent:
                         proxy(devices=idx, status=True)
 
                 if init:
-                    if str(uri).startswith('iOS'):
-                        os.system('utx uninstall {}'.format(app_name))
-                        os.system('utx install {}'.format(app_pkg))
+                    if str(uri).startswith("iOS"):
+                        os.system(f"utx uninstall {app_name}")
+                        os.system(f"utx install {app_pkg}")
                         UT.iOS = True
                     else:
                         try:
                             uninstall(app_name)
                         except AdbError:
                             pass
                         install(app_pkg, install_options=["-g"])
@@ -253,57 +299,64 @@
                     popup(devices=uri)
                 else:
                     stop_app(app_name)
                     sleep(2)
                     start_app(app_name)
                     sleep(2)
         except Exception as e:
-
-            if device_platform().lower() in 'ios':
+            if device_platform().lower() in "ios":
                 cleanup()
 
-            if device_platform().lower() in 'android' and agent:
+            if device_platform().lower() in "android" and agent:
                 for _ in device_idx:
                     proxy(devices=_, status=False)
 
-            logger.error("Create app fail: {}".format(e))
-            allure.attach(body='',
-                          name="Create app fail: {}".format(e),
-                          attachment_type=allure.attachment_type.TEXT)
-            warning_report = os.path.join(app_filepath.split('packages')[0], 'report', 'airtest')
-            gen_report(results=[{'result': ['warning_report', "Warning: Create app fail: {}".format(e)]}],
-                       report_path=warning_report)
-            pytest.xfail("Create app fail: {}".format(e))
+            logger.error(f"Create app fail: {e}")
+            allure.attach(
+                body="",
+                name=f"Create app fail: {e}",
+                attachment_type=allure.attachment_type.TEXT,
+            )
+            warning_report = os.path.join(
+                app_filepath.split("packages")[0], "report", "airtest"
+            )
+            gen_report(
+                results=[
+                    {"result": ["warning_report", f"Warning: Create app fail: {e}"]}
+                ],
+                report_path=warning_report,
+            )
+            pytest.xfail(f"Create app fail: {e}")
 
-        assert (app is not None)
+        assert app is not None
 
         ensure_current_device(device_idx[0])
 
-        logger.info("Current test platform: {}".format(device_platform()))
-        logger.info("Start app {0} in {1}:{2}".format(app_name, device_platform(), G.DEVICE.uuid))
+        logger.info(f"Current test platform: {device_platform()}")
+        logger.info(f"Start app {app_name} in {device_platform()}:{G.DEVICE.uuid}")
 
     def teardown_test():
         with allure.step("Teardown session"):
             try:
                 stop_app(app_name)
             except DeviceConnectionError:
                 pass
 
             # todo: Do not uninstall the installation package at the end of the execution
             #  which is convenient for troubleshooting.
 
-            if device_platform().lower() in 'ios':
-                check_port(port=str(device_idx[0]).split(':')[1])
+            if device_platform().lower() in "ios":
+                check_port(port=str(device_idx[0]).split(":")[1])
                 cleanup()
                 logger.info("Cleanup device wda process.")
-            if device_platform().lower() in 'android' and agent:
+            if device_platform().lower() in "android" and agent:
                 for _ in device_idx:
                     proxy(devices=_, status=False)
             try:
-                keyevent('26')
+                keyevent("26")
             except DeviceConnectionError:
                 pass
 
         logger.info("Session stop test.")
 
     request.addfinalizer(teardown_test)
 
@@ -334,47 +387,49 @@
 
     :param request:
     :return:
     """
     with allure.step("Initialize and generate Web object！"):
         logger.info("Session start test.")
     # chrome://version/
-    cache = kwargs.get('cache')
-    headless = kwargs.get('headless')
+    cache = kwargs.get("cache")
+    headless = kwargs.get("headless")
 
     global driver
     if driver is None:
         chrome_options = Options()
-        chrome_options.add_argument('disable-infobars')
+        chrome_options.add_argument("disable-infobars")
         chrome_options.add_experimental_option("excludeSwitches", ["enable-automation"])
-        chrome_options.add_experimental_option('useAutomationExtension', False)
-        if plat() == 'Windows':
+        chrome_options.add_experimental_option("useAutomationExtension", False)
+        if plat() == "Windows":
             chrome_options.add_argument("--remote-debugging-port=9222")
             if headless:
-                chrome_options.add_argument('--headless')
+                chrome_options.add_argument("--headless")
             if cache:
                 chrome_options.add_argument(f"--user-data-dir={cache}")
 
-        elif plat() == 'Linux':
+        elif plat() == "Linux":
             chrome_options.add_argument("--remote-debugging-port=9222")
-            chrome_options.add_argument('--headless')
-            chrome_options.add_argument('--no-sandbox')
-            chrome_options.add_argument('--disable-dev-shm-usage')
+            chrome_options.add_argument("--headless")
+            chrome_options.add_argument("--no-sandbox")
+            chrome_options.add_argument("--disable-dev-shm-usage")
             if cache:
                 chrome_options.add_argument(f"--user-data-dir={cache}")
         else:
             chrome_options.add_argument("--remote-debugging-port=9222")
             if headless:
-                chrome_options.add_argument('--headless')
+                chrome_options.add_argument("--headless")
 
             if cache:
                 chrome_options.add_argument(f"--user-data-dir={cache}")
 
-        driver = webdriver.Chrome(options=chrome_options,
-                                  executable_path=ChromeDriverManager(cache_valid_range=3).install())
+        driver = webdriver.Chrome(
+            options=chrome_options,
+            executable_path=ChromeDriverManager(cache_valid_range=3).install(),
+        )
 
         driver.maximize_window()
         # driver.set_window_size(1920, 1080)
 
     driver.implicitly_wait(30)
 
     def fn():
```

### Comparing `utx-1.3.3/utx/core/utils/runner.py` & `utx-1.3.4/utx/core/utils/runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  8/31/2021 6:42 PM
 @Desc    :  Runner line.
 """
-import time
-import unittest
-import sys
-import six
+import os
 import re
 import shutil
+import sys
+import time
 import traceback
+import unittest
 import warnings
-from io import open
-
-from popups.dismiss import popup, UT
-from airtest.core.api import G, auto_setup, log, stop_app, shell, connect_device
-from airtest.core.helper import device_platform
-from airtest.core.settings import Settings as ST
-from airtest.core.error import DeviceConnectionError
-from airtest.utils.compat import script_dir_name, script_log_dir
-from copy import copy
-
 from argparse import *
+from copy import copy
 
 from airtest.core.android.adb import ADB
-from airtest.core.api import device, start_app
+from airtest.core.api import auto_setup
+from airtest.core.api import connect_device
+from airtest.core.api import device
+from airtest.core.api import log
+from airtest.core.api import shell
+from airtest.core.api import start_app
+from airtest.core.api import stop_app
 from airtest.core.error import AirtestError
-
-from utx.core.utils.tools import ios_device_info, plat, decryption
+from airtest.core.error import DeviceConnectionError
+from airtest.core.helper import device_platform
+from airtest.core.settings import Settings as ST
+from airtest.utils.compat import script_dir_name
+from airtest.utils.compat import script_log_dir
 from poco.exceptions import PocoException
+from popups.dismiss import popup
+from popups.dismiss import UT
 
 from utx.core.css import report
-import os
+from utx.core.utils.tools import decryption
+from utx.core.utils.tools import ios_device_info
+from utx.core.utils.tools import plat
 
 
 class AirtestCase(unittest.TestCase):
     PROJECT_ROOT = "."
     SCRIPTEXT = ".air"
     TPLEXT = ".png"
 
@@ -58,49 +60,55 @@
                 device().start_recording()
             except AirtestError:
                 traceback.print_exc()
 
     def tearDown(self):
         if self.args.log and self.args.recording:
             try:
-                if isinstance(self.args.recording, six.string_types) and self.args.recording.endswith(".mp4"):
+                if isinstance(
+                    self.args.recording, str
+                ) and self.args.recording.endswith(".mp4"):
                     output_name = os.path.basename(self.args.recording)
                     # output_name = dev.serialno + "_" + basename if len(G.DEVICE_LIST) > 1 else basename
                 else:
-                    output_name = "recording_{serialno}.mp4".format(serialno=device().serialno)
+                    output_name = f"recording_{device().serialno}.mp4"
                 output = os.path.join(self.args.log, output_name)
                 device().stop_recording(output)
             except AirtestError:
                 traceback.print_exc()
 
     def runTest(self):
         scriptpath, pyfilename = script_dir_name(self.args.script)
         pyfilepath = os.path.join(scriptpath, pyfilename)
         pyfilepath = os.path.abspath(pyfilepath)
         self.scope["__file__"] = pyfilepath
-        with open(pyfilepath, 'r', encoding="utf8") as f:
+        with open(pyfilepath, encoding="utf8") as f:
             code = f.read()
         pyfilepath = pyfilepath.encode(sys.getfilesystemencoding())
 
         try:
-            exec(compile(code.encode("utf-8"), pyfilepath, 'exec'), self.scope)
+            exec(compile(code.encode("utf-8"), pyfilepath, "exec"), self.scope)
         except Exception as err:
             log(err, desc="Final Error", snapshot=True)
-            six.reraise(*sys.exc_info())
+            raise
 
     @classmethod
     def exec_other_script(cls, scriptpath):
         """run other script in test script"""
 
         warnings.simplefilter("always")
         warnings.warn("please use using() api instead.", PendingDeprecationWarning)
 
         def _sub_dir_name(scriptname):
             dirname = os.path.splitdrive(os.path.normpath(scriptname))[-1]
-            dirname = dirname.strip(os.path.sep).replace(os.path.sep, "_").replace(cls.SCRIPTEXT, "_sub")
+            dirname = (
+                dirname.strip(os.path.sep)
+                .replace(os.path.sep, "_")
+                .replace(cls.SCRIPTEXT, "_sub")
+            )
             return dirname
 
         def _copy_script(src, dst):
             if os.path.isdir(dst):
                 shutil.rmtree(dst, ignore_errors=True)
             os.mkdir(dst)
             for f in os.listdir(src):
@@ -116,19 +124,19 @@
         sub_dir = _sub_dir_name(scriptpath)
         sub_dirpath = os.path.join(cls.args.script, sub_dir)
         _copy_script(scriptpath, sub_dirpath)
         # read code
         pyfilename = os.path.basename(scriptpath).replace(cls.SCRIPTEXT, ".py")
         pyfilepath = os.path.join(scriptpath, pyfilename)
         pyfilepath = os.path.abspath(pyfilepath)
-        with open(pyfilepath, 'r', encoding='utf8') as f:
+        with open(pyfilepath, encoding="utf8") as f:
             code = f.read()
         # replace tpl filepath with filepath in sub_dir
         code = re.sub(r"[\'\"](\w+.png)[\'\"]", r"\"%s/\g<1>\"" % sub_dir, code)
-        exec(compile(code.encode("utf8"), pyfilepath, 'exec'), cls.scope)
+        exec(compile(code.encode("utf8"), pyfilepath, "exec"), cls.scope)
 
 
 def setup_by_args(args):
     # init devices
     if isinstance(args.device, list):
         devices = args.device
     elif args.device:
@@ -180,16 +188,26 @@
     :param sch_resolution:
     :param src_resolution:
     :return: device resolution
     """
     return int(w), int(h)
 
 
-def run_air(devices, case, app_name, log_path, case_path, base_dir,
-            static_dir=decryption('aHR0cHM6Ly9mYXN0bHkuanNkZWxpdnIubmV0L2doL29wZW51dHgvc3RhdGljLw=='), record=None):
+def run_air(
+    devices,
+    case,
+    app_name,
+    log_path,
+    case_path,
+    base_dir,
+    static_dir=decryption(
+        "aHR0cHM6Ly9mYXN0bHkuanNkZWxpdnIubmV0L2doL29wZW51dHgvc3RhdGljLw=="
+    ),
+    record=None,
+):
     """
     //See also: https://www.theiphonewiki.com/wiki/Models
 
     :param devices: read device id
     :param case: case list
     :param record: whether to enable recording
     :param log_path: log_path
@@ -199,125 +217,156 @@
     :param static_dir: use local style file when empty
 
     :return:
     """
 
     connect_device(devices)
 
-    if device_platform().lower() in 'ios':
+    if device_platform().lower() in "ios":
         _device = ios_device_info()
-        model = _device['MarketName']
-        build_version = _device['ProductVersion']
-        dev = model + ' ios {}'.format(build_version).replace('\n', '').replace('\r', '')
+        model = _device["MarketName"]
+        build_version = _device["ProductVersion"]
+        dev = model + f" ios {build_version}".replace("\n", "").replace("\r", "")
 
-    elif device_platform().lower() in 'android':
+    elif device_platform().lower() in "android":
         serialno = device().serialno
         model = ADB(serialno=serialno).get_model()
-        build_version = shell('getprop ro.build.version.release')
-        dev = model + ' Android {}'.format(build_version).replace('\n', '').replace('\r', '')
+        build_version = shell("getprop ro.build.version.release")
+        dev = model + f" Android {build_version}".replace("\n", "").replace("\r", "")
     else:
-        print('{} is unsupported platform on utx!'.format(device_platform()))
-        raise AirtestError('utx unsupported this platform!')
+        print(f"{device_platform()} is unsupported platform on utx!")
+        raise AirtestError("utx unsupported this platform!")
 
     UT.SYS = False
     UT.LOOP = 1
     popup(devices=devices)
 
     if os.path.isdir(log_path):
         pass
     else:
         os.makedirs(log_path)
-        print(str(log_path) + 'is created')
+        print(str(log_path) + "is created")
 
     if str(case).endswith(".air"):
-        if plat() == 'Windows':
-            air_name = str(case).split('\\')[-1]
+        if plat() == "Windows":
+            air_name = str(case).split("\\")[-1]
         else:
-            air_name = str(case).split('/')[-1]
+            air_name = str(case).split("/")[-1]
 
         if record:
-            record = air_name.replace('.air', '.mp4')
+            record = air_name.replace(".air", ".mp4")
 
         print(case)
-        log = os.path.join(log_path + '/' + dev + '/' + air_name.replace('.air', ''))
+        log = os.path.join(log_path + "/" + dev + "/" + air_name.replace(".air", ""))
 
-        run_log = case + '/' + 'log' + '/' + dev
+        run_log = case + "/" + "log" + "/" + dev
         if not os.path.exists(run_log):
             os.makedirs(run_log)
         print(log)
         if os.path.isdir(log):
             pass
         else:
             os.makedirs(log)
-            print(str(log) + 'is created')
-        output_file = log + '/' + 'log.html'
-        args = Namespace(device=devices, log=run_log, recording=record, script=case, compress=20, no_image=False)
+            print(str(log) + "is created")
+        output_file = log + "/" + "log.html"
+        args = Namespace(
+            device=devices,
+            log=run_log,
+            recording=record,
+            script=case,
+            compress=20,
+            no_image=False,
+        )
         try:
             run_script(args, AirtestCase)
         except (AirtestError, PocoException):
             pass
         finally:
-            rpt = report.LogToHtml(case, run_log, script_name=air_name.replace(".air", ".py"), static_root=static_dir,
-                                   plugins=['utx.mod.report.seleniumui', 'utx.mod.report.pocoui'])
+            rpt = report.LogToHtml(
+                case,
+                run_log,
+                script_name=air_name.replace(".air", ".py"),
+                static_root=static_dir,
+                plugins=["utx.mod.report.seleniumui", "utx.mod.report.pocoui"],
+            )
             rpt.report("log_template.html", output_file=output_file, base_dir=base_dir)
-            result = {"name": air_name.replace('.air', ''), "result": rpt.test_result}
+            result = {"name": air_name.replace(".air", ""), "result": rpt.test_result}
         try:
             stop_app(app_name)
             time.sleep(2)
             start_app(app_name)
             time.sleep(2)
         except DeviceConnectionError:
             pass
 
         return result, dev
 
 
-def run_web_air(case, log_path, case_path, base_dir,
-                static_dir=decryption('aHR0cHM6Ly9mYXN0bHkuanNkZWxpdnIubmV0L2doL29wZW51dHgvc3RhdGljLw==')):
+def run_web_air(
+    case,
+    log_path,
+    case_path,
+    base_dir,
+    static_dir=decryption(
+        "aHR0cHM6Ly9mYXN0bHkuanNkZWxpdnIubmV0L2doL29wZW51dHgvc3RhdGljLw=="
+    ),
+):
     """
 
     :param case:
     :param log_path:
     :param case_path:
     :param base_dir:
     :param static_dir:
     :return:
     """
-    dev = 'chrome'
+    dev = "chrome"
     time.sleep(2)
 
     if os.path.isdir(log_path):
         pass
     else:
         os.makedirs(log_path)
-        print(str(log_path) + 'is created')
+        print(str(log_path) + "is created")
 
     if str(case).endswith(".air"):
-        if plat() == 'Windows':
-            air_name = str(case).split('\\')[-1]
+        if plat() == "Windows":
+            air_name = str(case).split("\\")[-1]
         else:
-            air_name = str(case).split('/')[-1]
+            air_name = str(case).split("/")[-1]
         print(case)
-        log = os.path.join(log_path + '/' + dev + '/' + air_name.replace('.air', ''))
+        log = os.path.join(log_path + "/" + dev + "/" + air_name.replace(".air", ""))
 
-        run_log = case + '/' + 'log' + '/' + dev
+        run_log = case + "/" + "log" + "/" + dev
         if not os.path.exists(run_log):
             os.makedirs(run_log)
         print(log)
         if os.path.isdir(log):
             pass
         else:
             os.makedirs(log)
-            print(str(log) + 'is created')
-        output_file = log + '/' + 'log.html'
-        args = Namespace(device=None, log=run_log, recording=None, script=case, compress=20, no_image=False)
+            print(str(log) + "is created")
+        output_file = log + "/" + "log.html"
+        args = Namespace(
+            device=None,
+            log=run_log,
+            recording=None,
+            script=case,
+            compress=20,
+            no_image=False,
+        )
         try:
             run_script(args, AirtestCase)
         except Exception:
             pass
         finally:
-            rpt = report.LogToHtml(case, run_log, script_name=air_name.replace(".air", ".py"), static_root=static_dir,
-                                   plugins=['utx.mod.report.seleniumui', 'utx.mod.report.pocoui'])
+            rpt = report.LogToHtml(
+                case,
+                run_log,
+                script_name=air_name.replace(".air", ".py"),
+                static_root=static_dir,
+                plugins=["utx.mod.report.seleniumui", "utx.mod.report.pocoui"],
+            )
             rpt.report("log_template.html", output_file=output_file, base_dir=base_dir)
-            result = {"name": air_name.replace('.air', ''), "result": rpt.test_result}
+            result = {"name": air_name.replace(".air", ""), "result": rpt.test_result}
 
         return result, dev
```

### Comparing `utx-1.3.3/utx/core/utils/tools.py` & `utx-1.3.4/utx/core/utils/tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  8/31/2021 9:42 PM
 @Desc    :  Tools line.
 """
 import base64
+import configparser
 import platform
+import re
+import smtplib
 import socket
 import subprocess
-import re
-import configparser
+from email.mime.multipart import MIMEMultipart
+from email.mime.text import MIMEText
+from multiprocessing import Process
+
 import pytest
 import requests
 import urllib3
-import smtplib
-from email.mime.text import MIMEText
-from email.mime.multipart import MIMEMultipart
-from multiprocessing import Process
+from airtest.core.android.adb import ADB
 from airtest.core.android.recorder import Recorder
+from airtest.core.api import *
 from airtest.core.error import AdbShellError
+from airtest.utils.logger import get_logger
 from loguru import logger
 from tqdm import tqdm
-from airtest.utils.logger import get_logger
-from airtest.core.api import *
-from airtest.core.android.adb import ADB
+
 from utx.core.css.custom_report import gen_report
 
 LOGGING = get_logger(__name__)
 
 
 @logwrap
 def reboot():
     """
 
     :return:
     """
     serialno = device().serialno
-    ADB(serialno=serialno).cmd(cmds='reboot')
+    ADB(serialno=serialno).cmd(cmds="reboot")
     log(f"Device {serialno} has been restarted!")
 
 
 def allure_report(report_path, report_html):
     """
     Generate allure Report
     :param report_path:
     :param report_html:
     :return:
     """
     # execution allure generate
-    allure_cmd = "allure generate %s -o %s --clean" % (report_path, report_html)
+    allure_cmd = f"allure generate {report_path} -o {report_html} --clean"
     try:
         subprocess.call(allure_cmd, shell=True)
     except Exception:
-        LOGGING.error("The generation of allure report failed. Please check the relevant configuration of the test "
-                      "environment")
+        LOGGING.error(
+            "The generation of allure report failed. Please check the relevant configuration of the test "
+            "environment"
+        )
         raise
 
 
 def plat():
     """
     Check the current script running platform
     :return:'Linux', 'Windows' or 'Darwin'.
@@ -69,46 +71,48 @@
 
 def check_port(port):
     """
     Detect whether the port is occupied and clean up
     :param port:System port
     :return:None
     """
-    if plat() != 'Windows':
+    if plat() != "Windows":
         os.system("lsof -i:%s| grep LISTEN| awk '{print $2}'|xargs kill -9" % port)
     else:
-        port_cmd = 'netstat -ano | findstr {}'.format(port)
+        port_cmd = f"netstat -ano | findstr {port}"
         r = os.popen(port_cmd)
         if len(r.readlines()) == 0:
             return
         else:
             pid_list = []
             for line in r.readlines():
                 line = line.strip()
-                pid = re.findall(r'[1-9]\d*', line)
+                pid = re.findall(r"[1-9]\d*", line)
                 pid_list.append(pid[-1])
             pid_set = list(set(pid_list))[0]
-            pid_cmd = 'taskkill -PID {} -F'.format(pid_set)
+            pid_cmd = f"taskkill -PID {pid_set} -F"
             os.system(pid_cmd)
 
 
 def cleanup():
     """
     cleanup device wda process
     :return:
     """
     pid_list = []
-    cmd = decryption(b'dGlkZXZpY2U=')
-    sub = subprocess.Popen(f'{cmd} ps', shell=True, close_fds=True, stdout=subprocess.PIPE)
+    cmd = decryption(b"dGlkZXZpY2U=")
+    sub = subprocess.Popen(
+        f"{cmd} ps", shell=True, close_fds=True, stdout=subprocess.PIPE
+    )
     sub.wait()
     pid_info = sub.stdout.read().decode().splitlines()
     for u in pid_info:
-        if 'WebDriverAgentRunner' in u:
-            pid_list.append(u.strip().split(' ')[0])
-    [os.system(f'{cmd} kill {pid}') for pid in pid_list]
+        if "WebDriverAgentRunner" in u:
+            pid_list.append(u.strip().split(" ")[0])
+    [os.system(f"{cmd} kill {pid}") for pid in pid_list]
 
 
 def display():
     """
     Gets the length and width of the current device
     :return:
     """
@@ -121,69 +125,75 @@
     Perform `adb devices` command and return the list of adb devices
     Perform `utx list` command and return the list of iphone devices
     :param types: mobile platform
     :param state: optional parameter to filter devices in specific state
     :return: list od android devices or ios devices
     """
     device_list = []
-    if types.lower() == 'android':
-        patten = re.compile(r'^[\w\d.:-]+\t[\w]+$')
+    if types.lower() == "android":
+        patten = re.compile(r"^[\w\d.:-]+\t[\w]+$")
         output = ADB().cmd("devices", device=False)
         for line in output.splitlines():
             line = line.strip()
             if not line or not patten.match(line):
                 continue
-            serialno, cstate = line.split('\t')
+            serialno, cstate = line.split("\t")
             if state and cstate != state:
                 continue
             device_list.append(serialno)
-    elif types.lower() == 'ios':
+    elif types.lower() == "ios":
         # Get the udid list of the connected mobile phone
-        sub = subprocess.Popen('utx list', shell=True, close_fds=True, stdout=subprocess.PIPE)
+        sub = subprocess.Popen(
+            "utx list", shell=True, close_fds=True, stdout=subprocess.PIPE
+        )
         sub.wait()
         udid = sub.stdout.read().decode().splitlines()
         for u in udid:
-            us = u.strip().split(' ')[0]
-            if us != 'UDID':
+            us = u.strip().split(" ")[0]
+            if us != "UDID":
                 device_list.append(us)
     return device_list
 
 
 def ios_device_info():
     """
     Gets device_info of the current device
 
     :return:
     """
-    res = subprocess.run('{} info'.format(decryption(b'dGlkZXZpY2U=')), shell=True, stdout=subprocess.PIPE,
-                         stderr=subprocess.PIPE)
+    res = subprocess.run(
+        "{} info".format(decryption(b"dGlkZXZpY2U=")), shell=True, capture_output=True
+    )
     lines = res.stdout.decode("utf-8", "ignore")
-    device_info = [info for info in lines.split('\n') if info]
+    device_info = [info for info in lines.split("\n") if info]
     _device = {}
     if len(device_info) < 2:
-        LOGGING.error(f'Read device info line error. {lines}')
+        LOGGING.error(f"Read device info line error. {lines}")
     for info in device_info:
-        info_kv = info.split(':')
-        if info_kv[0] == 'ProductVersion':
-            _device['ProductVersion'] = info_kv[1].strip()
-        if info_kv[0] == 'MarketName':
-            _device['MarketName'] = info_kv[1].strip()
-        if info_kv[0] == 'SerialNumber':
-            _device['SerialNumber'] = info_kv[1].strip()
+        info_kv = info.split(":")
+        if info_kv[0] == "ProductVersion":
+            _device["ProductVersion"] = info_kv[1].strip()
+        if info_kv[0] == "MarketName":
+            _device["MarketName"] = info_kv[1].strip()
+        if info_kv[0] == "SerialNumber":
+            _device["SerialNumber"] = info_kv[1].strip()
     return _device
 
 
 def get_report(airtest_report_path):
     """
     Get the latest test report path
     :return: report name and path
     """
     file_lists = os.listdir(airtest_report_path)
-    file_lists.sort(key=lambda fn: os.path.getmtime(airtest_report_path + "/" + fn)
-    if not os.path.isdir(airtest_report_path + "/" + fn) else 0)
+    file_lists.sort(
+        key=lambda fn: os.path.getmtime(airtest_report_path + "/" + fn)
+        if not os.path.isdir(airtest_report_path + "/" + fn)
+        else 0
+    )
     report = os.path.join(airtest_report_path, file_lists[-1])
     print(file_lists[-1])
     return report
 
 
 def encryption(value):
     """
@@ -210,46 +220,46 @@
 
 def str_to_bool(value):
     """
     str convert bool
     :param value:
     :return:
     """
-    return True if value.lower() == 'true' else False
+    return True if value.lower() == "true" else False
 
 
 def find_all_cases(base, status, mark):
     """
 
     :param base:
     :param status:
     :param mark:
     :return:
     """
     for root, ds, fs in os.walk(base, topdown=True):
         if status in ["0", False]:
             for f in ds:
-                if f.endswith('.air') and mark in f:
+                if f.endswith(".air") and mark in f:
                     fullname = os.path.join(root, f)
                     yield fullname
         else:
             for f in ds:
-                if f.endswith('.air'):
+                if f.endswith(".air"):
                     fullname = os.path.join(root, f)
                     yield fullname
 
 
 def get_host_ip():
     """
     Query the local ip address
     :return:
     """
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
-        s.connect(('8.8.8.8', 80))
+        s.connect(("8.8.8.8", 80))
         ip = s.getsockname()[0]
     finally:
         s.close()
 
     return ip
 
 
@@ -259,19 +269,19 @@
     :param devices:
     :param status: on or off
     :return:
     :platforms: Android
     """
     if status:
         proxy_cmd = f"{ADB.builtin_adb_path()} -s {devices} {decryption(b'c2hlbGwgc2V0dGluZ3MgcHV0IGdsb2JhbCBodHRwX3Byb3h5')} {get_host_ip()}:8888"
-        logger.info(f'Successfully enabled {devices} global proxy！')
+        logger.info(f"Successfully enabled {devices} global proxy！")
         os.system(proxy_cmd)
     else:
         proxy_cmd = f"{ADB.builtin_adb_path()} -s {devices} {decryption(b'c2hlbGwgc2V0dGluZ3MgcHV0IGdsb2JhbCBodHRwX3Byb3h5IDow')}"
-        logger.info(f'Close the {devices} global proxy successfully！')
+        logger.info(f"Close the {devices} global proxy successfully！")
         os.system(proxy_cmd)
 
 
 def selector(status, flag, cases_list):
     """
 
     :param status:
@@ -296,31 +306,41 @@
 
 def selector_v2(path, status, mark):
     cases = []
     for i in find_all_cases(path, status, mark):
         print(i)
         cases.append(i)
     if len(cases) == 0:
-        warning_report = os.path.join(path.split('suites')[0], 'report', 'airtest')
-        gen_report(results=[{'result': ['warning_report', "Warning: No test case found, please check the path!"]}], report_path=warning_report)
+        warning_report = os.path.join(path.split("suites")[0], "report", "airtest")
+        gen_report(
+            results=[
+                {
+                    "result": [
+                        "warning_report",
+                        "Warning: No test case found, please check the path!",
+                    ]
+                }
+            ],
+            report_path=warning_report,
+        )
         pytest.xfail("No test case found, please check the path!")
     return sorted(cases)
 
 
 def selector_v3(path: str, status, mark):
     """
 
     :param path:
     :param status:
     :param mark:
     :return:
     """
     cases = []
-    base_path = path.split(path.split('/')[-1])[0]
-    path_list = ''.join(str(path).split()[0].split('/')[-1]).split(',')
+    base_path = path.split(path.split("/")[-1])[0]
+    path_list = "".join(str(path).split()[0].split("/")[-1]).split(",")
     for item in path_list:
         for i in find_all_cases(base_path + item, status, mark):
             print(i)
             cases.append(i)
     if len(cases) == 0:
         pytest.xfail("No test case found, please check the path!")
     return sorted(cases)
@@ -329,28 +349,33 @@
 def download(file_url, types):
     """
 
     :param types:
     :param file_url:
     :return:
     """
-    if 'http' not in file_url:
+    import urllib
+
+    file_url = urllib.parse.unquote(file_url)
+    if "http" not in file_url:
         return
-    download_url = 'http' + file_url.split('http')[-1]
+    download_url = "http" + file_url.split("http")[-1]
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
     r = requests.get(download_url, stream=True, verify=False)
-    total = int(r.headers.get('content-length', 0))
-    filename = "{}utx_download_{}.{}".format(file_url.split('http')[0], int(round(time.time() * 1000)), types)
-
-    with open(filename, 'wb') as file, tqdm(
-            desc=filename,
-            total=total,
-            unit='iB',
-            unit_scale=True,
-            unit_divisor=1024,
+    total = int(r.headers.get("content-length", 0))
+    filename = "{}utx_download_{}.{}".format(
+        file_url.split("http")[0], int(round(time.time() * 1000)), types
+    )
+
+    with open(filename, "wb") as file, tqdm(
+        desc=filename,
+        total=total,
+        unit="iB",
+        unit_scale=True,
+        unit_divisor=1024,
     ) as bar:
         for data in r.iter_content(chunk_size=1024):
             size = file.write(data)
             bar.update(size)
 
     return filename
 
@@ -372,29 +397,31 @@
 
     :param file: __file__
     :param name: mp4 name
     :return: video file
     """
     serialno = device().serialno
     model = ADB(serialno=serialno)
-    build_version = shell('getprop ro.build.version.release')
-    dev = model.get_model() + ' Android {}'.format(build_version).replace('\n', '').replace('\r', '')
+    build_version = shell("getprop ro.build.version.release")
+    dev = model.get_model() + f" Android {build_version}".replace("\n", "").replace(
+        "\r", ""
+    )
     recorder = Recorder(model)
     if not name:
-        name = str(file).split('/')[-1].split('.')[0]
-    output_path = os.path.join(str(file).split('.air')[0] + '.air', 'log', dev, name)
-    recorder.stop_recording(output=f'{output_path}.mp4')
+        name = str(file).split("/")[-1].split(".")[0]
+    output_path = os.path.join(str(file).split(".air")[0] + ".air", "log", dev, name)
+    recorder.stop_recording(output=f"{output_path}.mp4")
 
 
 def check_network():
     """
     :return:
     """
     try:
-        result = shell('ping -c 1 www.baidu.com')
+        result = shell("ping -c 1 www.baidu.com")
         logger.info(result)
         return True
     except AdbShellError as e:
         logger.error(e)
         return False
 
 
@@ -422,19 +449,31 @@
     GetData()
 ]
 """
     create_file(os.path.join("proxy.py"), content)
     try:
         from garbevents.cli.main import mitmweb
         from garbevents.settings import Settings as ST
-        mitmweb(args=["-p", f"{ST.server_port}", "--ssl-insecure", "--web-host", f"{ST.web_host}", "--web-port",
-                      f"{ST.web_port}", "--no-web-open-browser", "-s", "proxy.py"])
+
+        mitmweb(
+            args=[
+                "-p",
+                f"{ST.server_port}",
+                "--ssl-insecure",
+                "--web-host",
+                f"{ST.web_host}",
+                "--web-port",
+                f"{ST.web_port}",
+                "--no-web-open-browser",
+                "-s",
+                "proxy.py",
+            ]
+        )
     except (ImportError, AttributeError):
-        logger.error(
-            "garbevents not installed, please run: pip install -U garbevents")
+        logger.error("garbevents not installed, please run: pip install -U garbevents")
         return
 
 
 def launcher(main, salve):
     """
 
     :param main:
@@ -455,16 +494,18 @@
     configuration file
     """
 
     def __init__(self, ini_path):
         self.ini_path = ini_path
         if not os.path.exists(ini_path):
             raise FileNotFoundError("Profile %s does not exist！" % ini_path)
-        self.config = configparser.RawConfigParser()  # When there are% symbols, use raw to read
-        self.config.read(ini_path, encoding='utf-8')
+        self.config = (
+            configparser.RawConfigParser()
+        )  # When there are% symbols, use raw to read
+        self.config.read(ini_path, encoding="utf-8")
 
     def _get(self, section, option):
         """
 
         :param section:
         :param option:
         :return:
@@ -479,26 +520,34 @@
         :param value:
         :return:
         """
         try:
             self.config.set(section, option, value)
         except configparser.NoSectionError as e:
             logger.error(e)
-        with open(self.ini_path, 'w') as f:
+        with open(self.ini_path, "w") as f:
             self.config.write(f)
 
     def getvalue(self, env, name):
         return self._get(env, name)
 
     def update_value(self, env, name, value):
         return self._set(env, name, str(value).strip())
 
 
 class SendMail:
-    def __init__(self, report_path, receive_address, send_address_name, send_address_pwd, title='', receive=None):
+    def __init__(
+        self,
+        report_path,
+        receive_address,
+        send_address_name,
+        send_address_pwd,
+        title="",
+        receive=None,
+    ):
         """
 
         :param report_path:
         :param receive_address:
         :param send_address_name:
         :param send_address_pwd:
         :param title:
@@ -514,42 +563,44 @@
         self.send_address_pwd = send_address_pwd
         self.title = title
 
     def __get_report(self):
         dirs = os.listdir(self.report_path)
         dirs.sort()
         new_report_name = dirs[-1]
-        print('The new report name: {0}'.format(new_report_name))
+        print(f"The new report name: {new_report_name}")
         return new_report_name
 
     def __take_messages(self):
         new_report = self.__get_report()
         self.msg = MIMEMultipart()
         now = time.strftime("%Y-%m-%d_%H-%M")
-        self.msg['Subject'] = f'UTX自动化{self.title}测试报告_' + now
-        self.msg['date'] = time.strftime("%Y-%m-%d_%H-%M")
+        self.msg["Subject"] = f"UTX自动化{self.title}测试报告_" + now
+        self.msg["date"] = time.strftime("%Y-%m-%d_%H-%M")
 
-        with open(os.path.join(self.report_path, new_report), 'rb') as f:
+        with open(os.path.join(self.report_path, new_report), "rb") as f:
             mail_body = f.read()
-        html = MIMEText(mail_body, _subtype='html', _charset='utf-8')
+        html = MIMEText(mail_body, _subtype="html", _charset="utf-8")
         self.msg.attach(html)
 
-        att1 = MIMEText(mail_body, 'base64', 'gb2312')
-        att1["Content-Type"] = 'application/octet-stream'
+        att1 = MIMEText(mail_body, "base64", "gb2312")
+        att1["Content-Type"] = "application/octet-stream"
         att1["Content-Disposition"] = 'attachment; filename="utx_summary.html"'
         self.msg.attach(att1)
 
     def send(self):
         self.__take_messages()
-        self.msg['from'] = self.send_address_name
+        self.msg["from"] = self.send_address_name
         # ",,,,"
-        self.msg['to'] = self.receive_address
+        self.msg["to"] = self.receive_address
         try:
             port = 465
-            smtp = smtplib.SMTP_SSL('smtp.exmail.qq.com', port)
+            smtp = smtplib.SMTP_SSL("smtp.exmail.qq.com", port)
             smtp.login(self.send_address_name, self.send_address_pwd)
-            smtp.sendmail(self.msg['from'], self.msg['to'].split(","), self.msg.as_string())
+            smtp.sendmail(
+                self.msg["from"], self.msg["to"].split(","), self.msg.as_string()
+            )
             smtp.close()
             print("send success")
         except smtplib.SMTPException as e:
             print(e)
-            print('send fail')
+            print("send fail")
```

### Comparing `utx-1.3.3/utx/mod/load.py` & `utx-1.3.4/utx/mod/load.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  2021/12/8 5:59 下午
 @Desc    :  plugins line.
 """
-
-import traceback
 import importlib
+import traceback
 
 from airtest.utils.logger import get_logger
 
 LOGGING = get_logger(__name__)
 
 
 class TestPlugin:
     @staticmethod
     def show_me():
-        print('plugin_name')
+        print("plugin_name")
 
 
-def plugin(plugin_name: str, sep=':'):
+def plugin(plugin_name: str, sep=":"):
     """
 
     :param plugin_name:
     :param sep:
     :return:
     """
     m, _, c = plugin_name.partition(sep)
@@ -46,10 +43,10 @@
         LOGGING.debug("try loading plugin: %s" % plugin_name)
         try:
             __import__(plugin_name)
         except ImportError:
             LOGGING.error(traceback.format_exc())
 
 
-if __name__ == '__main__':
-    pg = plugin('_load:TestPlugin')
+if __name__ == "__main__":
+    pg = plugin("_load:TestPlugin")
     pg.show_me()
```

### Comparing `utx-1.3.3/utx/mod/platform.py` & `utx-1.3.4/utx/mod/platform.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  2021/12/11 11:11 上午 
 @Desc    :  platform line.
 """
 
 
-class PluginsProcessor(object):
+class PluginsProcessor:
     PLUGINS = {}
 
     def process(self, text, plugins=()):
         if plugins is ():
             for plugin_name in self.PLUGINS.keys():
                 text = self.PLUGINS[plugin_name]().process(text)
         else:
```

### Comparing `utx-1.3.3/utx/mod/report/pocoui.py` & `utx-1.3.4/utx/mod/report/pocoui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  2022/4/15 11:02 上午
 @Desc    :  pocoui report plugin.
 """
 import utx.core.css.report as report
 
@@ -31,19 +29,19 @@
     poco_ui = ""
     if "__children__" in step:
         for item in step["__children__"]:
             if item["data"]["name"] == "record_ui":
                 poco_ui = item["data"]["call_args"]["ui"]
 
     if poco_ui:
-        name = step['data']['name']
+        name = step["data"]["name"]
         desc = {
             "touch": "Touch %s" % poco_ui,
             "swipe": "Swipe from %s" % poco_ui,
-            "set_text": "Set %s of text" % poco_ui
+            "set_text": "Set %s of text" % poco_ui,
         }
 
         ret = desc.get(name)
         if callable(ret):
             ret = ret()
         return ret
 
@@ -58,17 +56,17 @@
     if "__children__" in step:
         for item in step["__children__"]:
             if item["data"]["name"] == "record_ui":
                 poco_title = True
 
     if poco_title:
         title = {
-            "touch": u"Poco Click",
-            "swipe": u"Poco Swipe",
-            "set_text": u"Poco Set Text"
+            "touch": "Poco Click",
+            "swipe": "Poco Swipe",
+            "set_text": "Poco Set Text",
         }
         return title.get(name, name)
     else:
         return title
 
 
 report.LogToHtml._translate_desc = new_translate_desc
```

### Comparing `utx-1.3.3/utx/mod/report/seleniumui.py` & `utx-1.3.4/utx/mod/report/seleniumui.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,62 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  11/02/2021 3:36 PM
 @Desc    :  utx selenium report plugin
 """
-
 import os
+
 import utx.core.css.report as report
 
 LOGDIR = "log"
 
 old_trans_screen = report.LogToHtml._translate_screen
 old_trans_desc = report.LogToHtml._translate_desc
 old_trans_code = report.LogToHtml._translate_code
 
-screen_func = ["find_element_by_xpath", "find_element_by_id", "find_element_by_name", "assert_exist",
-               "back", "forward", "switch_to_new_tab", "switch_to_previous_tab", "get",
-               "click", "send_keys"]
+screen_func = [
+    "find_element_by_xpath",
+    "find_element_by_id",
+    "find_element_by_name",
+    "assert_exist",
+    "back",
+    "forward",
+    "switch_to_new_tab",
+    "switch_to_previous_tab",
+    "get",
+    "click",
+    "send_keys",
+]
 
 second_screen_func = ["click", "send_keys"]
 other_func = []
 
 
 def new_trans_screen(self, step, code):
     trans = old_trans_screen(self, step, code)
-    if "name" in step['data'] and step['data']["name"] in screen_func:
+    if "name" in step["data"] and step["data"]["name"] in screen_func:
         screen = {
             "src": None,
             "rect": [],
             "pos": [],
             "vector": [],
             "confidence": None,
         }
 
         src = ""
         if step["data"]["name"] in second_screen_func:
-            res = step["data"]['ret']
+            res = step["data"]["ret"]
             src = res["screen"]
             if "pos" in res:
                 screen["pos"] = res["pos"]
 
         for item in step["__children__"]:
             if item["data"]["name"] == "_gen_screen_log":
-                res = item["data"]['ret']
+                res = item["data"]["ret"]
                 src = res["screen"]
                 if "pos" in res:
                     screen["pos"] = res["pos"]
                 break
 
         if self.export_dir and src:
             src = os.path.join(LOGDIR, src)
@@ -57,48 +65,52 @@
         return screen
     else:
         return trans
 
 
 def new_translate_desc(self, step, code):
     trans = old_trans_desc(self, step, code)
-    if "name" in step['data'] and (step['data']["name"] in screen_func or step["data"]["name"] in other_func):
+    if "name" in step["data"] and (
+        step["data"]["name"] in screen_func or step["data"]["name"] in other_func
+    ):
         name = step["data"]["name"]
         args = {i["key"]: i["value"] for i in code["args"]}
         desc = {
-            "find_element_by_xpath": lambda: u"Find element by xpath: %s" % args.get("xpath"),
-            "find_element_by_id": lambda: u"Find element by id: %s" % args.get("id"),
-            "find_element_by_name": lambda: u"Find element by name: %s" % args.get("name"),
-            "assert_exist": u"Assert element exists.",
-            "click": u"Click the element that been found.",
-            "send_keys": u"Send some text and keyboard event to the element that been found.",
-            "get": lambda: u"Get the web address: %s" % args.get("address"),
-            "switch_to_last_window": u"Switch to the last tab.",
-            "switch_to_latest_window": u"Switch to the new tab.",
-            "back": u"Back to the last page.",
-            "forward": u"Forward to the next page.",
-            "snapshot": u"Snopshot current page."
+            "find_element_by_xpath": lambda: "Find element by xpath: %s"
+            % args.get("xpath"),
+            "find_element_by_id": lambda: "Find element by id: %s" % args.get("id"),
+            "find_element_by_name": lambda: "Find element by name: %s"
+            % args.get("name"),
+            "assert_exist": "Assert element exists.",
+            "click": "Click the element that been found.",
+            "send_keys": "Send some text and keyboard event to the element that been found.",
+            "get": lambda: "Get the web address: %s" % args.get("address"),
+            "switch_to_last_window": "Switch to the last tab.",
+            "switch_to_latest_window": "Switch to the new tab.",
+            "back": "Back to the last page.",
+            "forward": "Forward to the next page.",
+            "snapshot": "Snopshot current page.",
         }
 
         desc_zh = {
-            "find_element_by_xpath": lambda: u"寻找指定页面元素: \"%s\"" % args.get("xpath"),
-            "find_element_by_id": lambda: u"寻找指定页面元素: \"%s\"" % args.get("id"),
-            "find_element_by_name": lambda: u"寻找指定页面元素: \"%s\"" % args.get("name"),
-            "assert_exist": u"断言页面元素存在.",
-            "click": u"点击找到的页面元素.",
-            "send_keys": u"传送文本\"%s\"到选中文本框." % (args.get("text", "")),
-            "get": lambda: u"访问网络地址: %s" % args.get("address"),
-            "switch_to_last_window": u"切换到上一个标签页.",
-            "switch_to_latest_window": u"切换到最新标签页.",
-            "back": u"后退到上一个页面.",
-            "forward": u"前进到下一个页面.",
-            "snapshot": u"截取当前页面."
+            "find_element_by_xpath": lambda: '寻找指定页面元素: "%s"' % args.get("xpath"),
+            "find_element_by_id": lambda: '寻找指定页面元素: "%s"' % args.get("id"),
+            "find_element_by_name": lambda: '寻找指定页面元素: "%s"' % args.get("name"),
+            "assert_exist": "断言页面元素存在.",
+            "click": "点击找到的页面元素.",
+            "send_keys": '传送文本"%s"到选中文本框.' % (args.get("text", "")),
+            "get": lambda: "访问网络地址: %s" % args.get("address"),
+            "switch_to_last_window": "切换到上一个标签页.",
+            "switch_to_latest_window": "切换到最新标签页.",
+            "back": "后退到上一个页面.",
+            "forward": "前进到下一个页面.",
+            "snapshot": "截取当前页面.",
         }
 
-        if self.lang == 'zh':
+        if self.lang == "zh":
             desc = desc_zh
         ret = desc.get(name)
         if callable(ret):
             ret = ret()
         return ret
     else:
         return trans
```

### Comparing `utx-1.3.3/utx/scripts/ipa_pkg.py` & `utx-1.3.4/utx/scripts/ipa_pkg.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  2022/2/8 10:58 上午
 @Desc    :  ipa_pkg line.
 """
 import os
 import shutil
@@ -27,8 +25,8 @@
     xcodebuild build-for-testing -scheme WebDriverAgentRunner -sdk iphoneos -configuration Release -derivedDataPath {ipa_home}
     cd {ipa_home}/Build/Products/Release-iphoneos
     mkdir Payload && mv *.app Payload
     zip -r UTX-Runner.ipa Payload
     mv *.ipa {os.getcwd()}
     """
     os.system(cmd)
-    os.system('{} parse UTX-Runner.ipa'.format(decryption(b'dGlkZXZpY2U=')))
+    os.system("{} parse UTX-Runner.ipa".format(decryption(b"dGlkZXZpY2U=")))
```

### Comparing `utx-1.3.3/utx/scripts/ipa_sign.sh` & `utx-1.3.4/utx/scripts/ipa_sign.sh`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/scripts/plistdump-tcp-proxy.py` & `utx-1.3.4/utx/scripts/plistdump-tcp-proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 #!/usr/bin/python
 # This is a simple port-forward / proxy, written using only the default python
 # library. If you want to make a suggestion or fix something you can contact-me
 # at voorloop_at_gmail.com
 # Distributed over IDC(I Don't Care) license
-
 # Python3
 # Modified: 2020/05/15 (Fri) shengxiang.ssx
-
 import argparse
 import datetime
 import os
 import plistlib
 import pprint
 import re
 import select
 import socket
 import ssl
-import string
 import struct
 import sys
 import threading
 import time
 import traceback
-from tidevice._hexdump import hexdump
+
 from logzero import logger
+from tidevice._hexdump import hexdump
 
 # Changing the buffer_size and delay, you can improve the speed and bandwidth.
 # But when buffer get to high or delay go too down, you can broke things
 buffer_size = 40960
 delay = 0.0001
 
 _package_index = [0]
@@ -42,17 +40,16 @@
     if isinstance(addr, (tuple, list)):
         return socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     elif isinstance(addr, str):
         return socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
 
 
 def is_ssl_data(data: bytes) -> bool:
-    """ FIXME(ssx): better to change to EnableSSLSession """
-    return len(data) >= 8 and \
-           data[:3] == b'\x16\x03\x01' and data[5:6] == b'\x01'
+    """FIXME(ssx): better to change to EnableSSLSession"""
+    return len(data) >= 8 and data[:3] == b"\x16\x03\x01" and data[5:6] == b"\x01"
 
 
 def recvall(sock: socket.socket, n: int) -> bytearray:
     buf = bytearray()
     while n > len(buf):
         chunk = sock.recv(n - len(buf))
         if not chunk:
@@ -62,49 +59,48 @@
 
 
 class TheServer:
     input_list = []
     channel = {}
     socket_tags = {}
 
-    def __init__(self,
-                 listen_addr: str,
-                 forward_to: str,
-                 parse_ssl: bool = False,
-                 pemfile=None):
+    def __init__(
+        self, listen_addr: str, forward_to: str, parse_ssl: bool = False, pemfile=None
+    ):
         print("Listening on", listen_addr, "forward to", forward_to)
         self.server = create_socket(listen_addr)
         self.server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.server.bind(listen_addr)
         if isinstance(listen_addr, str):
             os.chmod(listen_addr, 0o777)
         self.server.listen(200)
 
         self.ssl_server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.ssl_server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        self.ssl_server.bind(('localhost', 10443))
+        self.ssl_server.bind(("localhost", 10443))
         self.ssl_server.listen(200)
 
         self.forward_to = forward_to
         self.parse_ssl = parse_ssl
         self.pemfile = pemfile
 
         self.__tempsocks = {}  # Store SSLSocket
         self.__tag = 0
-        self._data_directory = "usbmuxd-dumpdata/" + time.strftime(
-            "%Y%m%d-%H-%M-%S")
+        self._data_directory = "usbmuxd-dumpdata/" + time.strftime("%Y%m%d-%H-%M-%S")
 
     def main_loop(self):
         self.input_list.append(self.server)
         self.input_list.append(self.ssl_server)
 
         while True:
             time.sleep(delay)
-            timeout = .5
-            inputready, outputready, exceptready = select.select(self.input_list, [], [], timeout)
+            timeout = 0.5
+            inputready, outputready, exceptready = select.select(
+                self.input_list, [], [], timeout
+            )
             for self.s in inputready:
                 if self.s == self.server:
                     self.on_accept()
                     break
 
                 if self.s == self.ssl_server:
                     self.on_ssl_accept()
@@ -113,20 +109,20 @@
                 try:
                     self.data = self.s.recv(buffer_size)
                     if len(self.data) == 0:
                         self.on_close()
                         break
                     self.on_recv()
                 except ssl.SSLError as e:
-                    logger.warning("SSLError: tag: %d, %s",
-                                   self.socket_tags[self.s], e)
+                    logger.warning("SSLError: tag: %d, %s", self.socket_tags[self.s], e)
 
                     self.on_close()
                 except Exception as e:
                     import traceback
+
                     traceback.print_exc()
                     # logger.warning("Unknown error: %s", e)
 
     def gen_tag(self) -> int:  # return uniq int
         self.__tag += 1
         return self.__tag
 
@@ -160,103 +156,105 @@
 
     def on_accept(self):
         forward = create_socket(self.forward_to)
         forward.connect(self.forward_to)
 
         clientsock, clientaddr = self.server.accept()
         if forward:
-            print('[proxy]', clientaddr, "has connected")
+            print("[proxy]", clientaddr, "has connected")
             self.pipe_socket(clientsock, forward, self.gen_tag())
         else:
-            print("[proxy] Can't establish connection with remote server.", )
+            print(
+                "[proxy] Can't establish connection with remote server.",
+            )
             print("[proxy] Closing connection with client side", clientaddr)
             clientsock.close()
 
     def on_ssl_accept(self):
         sock, addr = self.ssl_server.accept()
 
         header = recvall(sock, 4)  # sock.recv(4)
         (tag,) = struct.unpack("I", header)
         logger.info("on ssl accept: %s, tag: %d", addr, tag)
         ssl_serversock = self.__tempsocks[tag]
 
         def wait_ssl_socket():
-            ssock = ssl.wrap_socket(sock,
-                                    keyfile=self.pemfile,
-                                    certfile=self.pemfile,
-                                    server_side=True)
+            ssock = ssl.wrap_socket(
+                sock, keyfile=self.pemfile, certfile=self.pemfile, server_side=True
+            )
             self.pipe_socket(ssock, ssl_serversock, tag)
 
         th = threading.Thread(target=wait_ssl_socket)
         th.daemon = True
         th.start()
 
     def pretty_format_data(self, data: bytes) -> str:
         try:
-            return '\n'.join(list(self._iter_pretty_format_data(data)))
+            return "\n".join(list(self._iter_pretty_format_data(data)))
         except:
             print(list(self._iter_pretty_format_data(data)))
             raise
 
     def _iter_pretty_format_data(self, data: bytes):
-        if b'<plist version=' in data:
-            lindex = data.find(b'<?xml version=')
-            rindex = data.find(b'</plist>') + len('</plist>')
+        if b"<plist version=" in data:
+            lindex = data.find(b"<?xml version=")
+            rindex = data.find(b"</plist>") + len("</plist>")
             plistdata = data[lindex:rindex]
 
             yield hexdump.hexdump(data[:lindex], "return")
             yield "## Plist-XML"
             try:
                 pdata = plistlib.loads(plistdata)
-                if 'PairRecordData' in pdata:
+                if "PairRecordData" in pdata:
                     yield "... PairRecordData ..."
                 else:
                     yield pprint.pformat(pdata)
                 yield hexdump.hexdump(data[rindex:], "return")
             except:
                 yield hexdump.hexdump(data, "return")
-        elif b'bplist00' in data:
+        elif b"bplist00" in data:
             # parse bplist data
             from tinstruments import bplist
+
             buf = data
             while True:
-                lindex = buf.find(b'bplist00')
+                lindex = buf.find(b"bplist00")
                 # print("bplist00", hex(lindex))
                 if lindex == -1:
                     break
                 m = re.search(b"\x00{6}[\x02\x01]{2}.{24}", buf)
                 if not m:
                     break
                 rindex = m.end()
 
                 yield hexdump.hexdump(buf[:lindex], "return")
                 try:
-                    yield "## NSKeyedArchiver-BINARY: [{}, {}]".format(hex(lindex), hex(rindex))
+                    yield f"## NSKeyedArchiver-BINARY: [{hex(lindex)}, {hex(rindex)}]"
                     pdata = bplist.objc_decode(buf[lindex:rindex])
                     yield pprint.pformat(pdata)
                 except bplist.InvalidNSKeyedArchiverFormat:
-                    yield "## Plist-BINARY: [{}, {}]".format(hex(lindex), hex(rindex))
+                    yield f"## Plist-BINARY: [{hex(lindex)}, {hex(rindex)}]"
                     pdata = bplist.loads(buf[lindex:rindex])
                     yield pprint.pformat(pdata)
                 except Exception as e:
-                    yield "## Parse plist-BINARY error: [{}, {}]".format(hex(lindex), hex(rindex))
+                    yield f"## Parse plist-BINARY error: [{hex(lindex)}, {hex(rindex)}]"
                     yield traceback.format_exc()
                     # BPlistdata failed string indices must be integers
-                    yield "load binary plistdata failed: {}".format(e)
+                    yield f"load binary plistdata failed: {e}"
                     yield hexdump.hexdump(buf[lindex:rindex], "return")
                 finally:
                     buf = buf[rindex:]
             yield hexdump.hexdump(buf, "return")
         else:  # just call hexdump
             yield f"## RAW length={len(data)}"
             max_length = 512
             if len(data) > max_length // 2:
-                yield hexdump.hexdump(data[:max_length // 2], "return")
+                yield hexdump.hexdump(data[: max_length // 2], "return")
                 yield "........ " * 5
-                yield hexdump.hexdump(data[-max_length // 2:], "return")
+                yield hexdump.hexdump(data[-max_length // 2 :], "return")
             else:
                 yield hexdump.hexdump(data, "return")
         # else:
         #     try:
         #         pdata = data.decode('utf-8')
         #         print(pdata)
         #     except UnicodeDecodeError:
@@ -268,62 +266,63 @@
 
         tag = self.socket_tags[self.s]
         direction = ">"
         if tag < 0:
             direction = "<"
         index = abs(tag)
 
-        print(f' {index} '.center(50, direction))
+        print(f" {index} ".center(50, direction))
         if isinstance(self.s, ssl.SSLSocket):  # secure tunnel
-            print('\33[32m', end="")
+            print("\33[32m", end="")
         print(f"Length={len(data)} 0x{len(data):02X}")
-        print("Time:", datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S.%f')[:-3])
+        print("Time:", datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S.%f")[:-3])
 
         # todo
         # if tag < 0:
         #    print("Skip show receving data")
         #    return
         if True:
             os.makedirs(self._data_directory, 0o755, exist_ok=True)
             fpath = os.path.join(self._data_directory, f"{index}.txt")
             with open(fpath, "a") as f:
-                f.write(f'# INDEX: {index} {direction * 5}\n')
+                f.write(f"# INDEX: {index} {direction * 5}\n")
                 f.write(f"Size: oct:{len(data)} hex:0x{len(data):02X}\n")
-                f.write(f"Time: {datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S.%f')[:-3]}\n")
+                f.write(
+                    f"Time: {datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S.%f')[:-3]}\n"
+                )
                 f.write(f"Package index: {next_package_index()}\n")
                 f.write(self.pretty_format_data(data) + "\n")
-                f.write('\n\n')
+                f.write("\n\n")
 
         if True:
             for line in self._iter_pretty_format_data(data):
                 print(line)
 
         # else:
         #    try:
         #        pdata = data.decode('utf-8')
         #        print(pdata)
         #    except UnicodeDecodeError:
         #        hexdump.hexdump(data)
 
         if isinstance(self.s, ssl.SSLSocket):  # secure tunnel
-            print('\33[0m', end="")
+            print("\33[0m", end="")
 
     def man_in_middle_ssl(self, clientsock, ssl_hello_data: bytes):
         serversock = self.channel[clientsock]
         tag = self.unpipe_socket(clientsock)
 
         ssl_serversock = ssl.wrap_socket(
-            serversock,
-            keyfile=self.pemfile,  # iPhoneSE
-            certfile=self.pemfile)
-        print("serversock secure ready, tag: {}".format(tag))
+            serversock, keyfile=self.pemfile, certfile=self.pemfile  # iPhoneSE
+        )
+        print(f"serversock secure ready, tag: {tag}")
 
         self.__tempsocks[tag] = ssl_serversock
 
-        mim_clientsock = socket.create_connection(('localhost', 10443))
+        mim_clientsock = socket.create_connection(("localhost", 10443))
         mim_clientsock.sendall(struct.pack("I", tag))
 
         hexdump.hexdump(ssl_hello_data[:1024])
         mim_clientsock.sendall(ssl_hello_data)
         self.pipe_socket(clientsock, mim_clientsock)
 
     def on_recv(self):
@@ -344,15 +343,15 @@
 
         try:
             self.channel[self.s].send(data)
         except BrokenPipeError:
             print("channel broken pipe")
 
     def on_close(self):
-        print('[proxy]', self.socket_tags.get(self.s), "has disconnected")
+        print("[proxy]", self.socket_tags.get(self.s), "has disconnected")
         # print('[proxy]', self.channel[self.s].getpeername(), "has disconnected, too")
 
         # remove objects from input_list
 
         # self.input_list.remove(self.s)
         # self.input_list.remove(self.channel[self.s])
 
@@ -365,52 +364,52 @@
 
         self.unpipe_socket(self.s)
         # del self.channel[out]
         # del self.channel[self.s]
 
 
 def _parse_addr(addr: str):
-    if ':' in addr:
+    if ":" in addr:
         host, port = addr.split(":", 1)
         return (host, int(port))
     return addr
 
 
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument("-L",
-                        "--listen-addr",
-                        default="/var/run/usbmuxd",
-                        help="listen address, eg :5555 or /tmp/listen.sock")
+    parser.add_argument(
+        "-L",
+        "--listen-addr",
+        default="/var/run/usbmuxd",
+        help="listen address, eg :5555 or /tmp/listen.sock",
+    )
     parser.add_argument(
         "-F",
         "--forward-to",
         default="/var/run/usbmuxx",
-        help="forward to, eg: localhost:5037 or /var/lib/usbmuxd")
-    parser.add_argument("-S",
-                        "--ssl",
-                        action="store_true",
-                        help="parse ssl data")
+        help="forward to, eg: localhost:5037 or /var/lib/usbmuxd",
+    )
+    parser.add_argument("-S", "--ssl", action="store_true", help="parse ssl data")
     parser.add_argument("--pemfile", help="ssl pemfile")
     args = parser.parse_args()
     # print(args)
 
     listen_addr = _parse_addr(args.listen_addr)
     forward_to = _parse_addr(args.forward_to)
 
-    server = TheServer(listen_addr,
-                       forward_to,
-                       parse_ssl=args.ssl,
-                       pemfile=args.pemfile)
+    server = TheServer(
+        listen_addr, forward_to, parse_ssl=args.ssl, pemfile=args.pemfile
+    )
     try:
         server.main_loop()
     except KeyboardInterrupt:
         print("Ctrl C - Stopping server")
         sys.exit(1)
     finally:
         if isinstance(listen_addr, str):
             import os
+
             os.unlink(listen_addr)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `utx-1.3.3/utx/scripts/run-usbmuxd-proxy.sh` & `utx-1.3.4/utx/scripts/run-usbmuxd-proxy.sh`

 * *Files identical despite different names*

### Comparing `utx-1.3.3/utx/scripts/uitest_screenrecord.py` & `utx-1.3.4/utx/scripts/uitest_screenrecord.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# coding: utf-8
 #
 # Run with the following command
 # ::Install
 # pip3 install imageio pytest facebook-wda
 #
 # ::Usage
 # py.test -v scripts/uitest_screenrecord.py -s
-
 import contextlib
 import io
 import socket
 import threading
 
 import imageio
 import pytest
@@ -22,34 +20,34 @@
 def c() -> wda.Client:
     _c = wda.USBClient()
     _c.unlock()
     yield _c
 
 
 class SocketBuffer:
-    """ Since I can't find a lib that can buffer socket read and write, so I write a one """
+    """Since I can't find a lib that can buffer socket read and write, so I write a one"""
 
     def __init__(self, sock: socket.socket):
         self._sock = sock
         self._buf = bytearray()
 
     def _drain(self):
         _data = self._sock.recv(1024)
         if _data is None:
-            raise IOError("socket closed")
+            raise OSError("socket closed")
         self._buf.extend(_data)
         return len(_data)
 
     def read_until(self, delimeter: bytes) -> bytes:
-        """ return without delimeter """
+        """return without delimeter"""
         while True:
             index = self._buf.find(delimeter)
             if index != -1:
                 _return = self._buf[:index]
-                self._buf = self._buf[index + len(delimeter):]
+                self._buf = self._buf[index + len(delimeter) :]
                 return _return
             self._drain()
 
     def read_bytes(self, length: int) -> bytes:
         while length > len(self._buf):
             self._drain()
 
@@ -58,39 +56,39 @@
 
     def write(self, data: bytes):
         return self._sock.sendall(data)
 
 
 @contextlib.contextmanager
 def make_screenrecord(c: wda.Client, t: tidevice.Device, output_video_path: str):
-    _old_fps = c.appium_settings()['mjpegServerFramerate']
+    _old_fps = c.appium_settings()["mjpegServerFramerate"]
     _fps = 10
     c.appium_settings({"mjpegServerFramerate": _fps})
 
     # Read image from WDA mjpeg server
     pconn = t.create_inner_connection(9100)  # default WDA mjpeg server port
     sock = pconn.get_socket()
     buf = SocketBuffer(sock)
     buf.write(b"GET / HTTP/1.0\r\nHost: localhost\r\n\r\n")
-    buf.read_until(b'\r\n\r\n')
+    buf.read_until(b"\r\n\r\n")
     print("screenrecord is ready to begin")
 
     wr = imageio.get_writer(output_video_path, fps=_fps)
 
     def _drain(stop_event, done_event):
         while not stop_event.is_set():
             # read http header
             length = None
             while True:
-                line = buf.read_until(b'\r\n')
+                line = buf.read_until(b"\r\n")
                 if line.startswith(b"Content-Length"):
-                    length = int(line.decode('utf-8').split(": ")[1])
+                    length = int(line.decode("utf-8").split(": ")[1])
                     break
             while True:
-                if buf.read_until(b'\r\n') == b'':
+                if buf.read_until(b"\r\n") == b"":
                     break
 
             imdata = buf.read_bytes(length)
             im = imageio.imread(io.BytesIO(imdata))
             wr.append_data(im)
         done_event.set()
```

### Comparing `utx-1.3.3/utx/selenium/exceptions.py` & `utx-1.3.4/utx/selenium/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,60 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  11/02/2021 8:16 PM
 @Desc    :  exceptions line.
 """
-
-from __future__ import unicode_literals
-
 import utx.selenium.utils.six as six
 
 
 def to_text(val):
-    if not isinstance(val, six.text_type):
-        return val.decode('utf-8')
+    if not isinstance(val, str):
+        return val.decode("utf-8")
     return val
 
 
 class UtxSeleniumException(Exception):
     """
     Base class for errors and exceptions of Airtest-Selenium
     """
 
     def __init__(self, message=None):
-        super(UtxSeleniumException, self).__init__(message)
+        super().__init__(message)
         self.message = message
 
     def __str__(self):
         if six.PY2:
-            if isinstance(self.message, six.text_type):
+            if isinstance(self.message, str):
                 return self.message.encode("utf-8")
             else:
                 return self.message
         else:
             if isinstance(self.message, bytes):
-                return self.message.decode('utf-8')
+                return self.message.decode("utf-8")
             else:
                 return self.message
 
     __repr__ = __str__
 
 
 class IsNotTemplateError(UtxSeleniumException):
     """
     Base class for errors and exceptions of Airtest-Selenium
     """
 
     def __init__(self, message=None):
-        super(IsNotTemplateError, self).__init__(message)
+        super().__init__(message)
 
     def __str__(self):
         if six.PY2:
-            if isinstance(self.message, six.text_type):
+            if isinstance(self.message, str):
                 return self.message.encode("utf-8")
             else:
                 return self.message
         else:
             if isinstance(self.message, bytes):
-                return self.message.decode('utf-8')
+                return self.message.decode("utf-8")
             else:
                 return self.message
 
     __repr__ = __str__
```

### Comparing `utx-1.3.3/utx/selenium/proxy.py` & `utx-1.3.4/utx/selenium/proxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,90 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  11/02/2021 3:36 PM
 @Desc    :  proxy line
 """
+import os
+import sys
+import time
+
 import pyperclip
+from airtest import aircv
+from airtest.aircv import get_resolution
 from airtest.core.api import sleep
+from airtest.core.cv import Template
+from airtest.core.error import TargetNotFoundError
+from airtest.core.helper import log
+from airtest.core.helper import logwrap
+from airtest.core.settings import Settings as ST
 from pykeyboard import PyKeyboard
 from pymouse import PyMouse
-from selenium.webdriver import Chrome, ActionChains, Firefox, Remote
-from selenium.webdriver.remote.webelement import WebElement
+from pynput.mouse import Button
+from pynput.mouse import Controller
 from selenium.common.exceptions import NoSuchElementException
+from selenium.webdriver import ActionChains
+from selenium.webdriver import Chrome
+from selenium.webdriver import Firefox
+from selenium.webdriver import Remote
 from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.remote.webelement import WebElement
 from webdriver_manager.chrome import ChromeDriverManager
-from airtest.core.settings import Settings as ST
-from airtest.core.helper import logwrap, log
-from airtest import aircv
-from airtest.core.cv import Template
 
 from utx.core.utils.tools import plat
+from utx.selenium.exceptions import IsNotTemplateError
+from utx.selenium.exceptions import UtxSeleniumException
 from utx.selenium.utils.airtest_api import loop_find
-from utx.selenium.exceptions import IsNotTemplateError, UtxSeleniumException
-from airtest.aircv import get_resolution
-from pynput.mouse import Controller, Button
-from airtest.core.error import TargetNotFoundError
-
-import os
-import time
-import sys
 
 
 class WebChrome(Chrome):
-    os.environ['WDM_SSL_VERIFY'] = '0'
+    os.environ["WDM_SSL_VERIFY"] = "0"
     chrome_options = Options()
     chrome_options.add_experimental_option("debuggerAddress", "127.0.0.1:9222")
 
-    def __init__(self, executable_path=ChromeDriverManager(cache_valid_range=3).install(), port=0,
-                 options=chrome_options, service_args=None,
-                 desired_capabilities=None, service_log_path=None,
-                 chrome_options=None):
-
+    def __init__(
+        self,
+        executable_path=ChromeDriverManager(cache_valid_range=3).install(),
+        port=0,
+        options=chrome_options,
+        service_args=None,
+        desired_capabilities=None,
+        service_log_path=None,
+        chrome_options=None,
+    ):
         # todo 适配selenium 4.0.0
         # def __init__(self, executable_path="chromedriver", port=0,
         #              options: Options = chrome_options, service_args=None,
         #              desired_capabilities=None, service_log_path=None,
         #              chrome_options=None, service=Service(executable_path=driver_path), keep_alive=None):
 
         if "darwin" in sys.platform:
-            os.environ['PATH'] += ":/Applications/AirtestIDE.app/Contents/Resources/selenium_plugin"
-        super(WebChrome, self).__init__(chrome_options=chrome_options, executable_path=executable_path,
-                                        port=port, options=options, service_args=service_args,
-                                        service_log_path=service_log_path, desired_capabilities=desired_capabilities)
+            os.environ[
+                "PATH"
+            ] += ":/Applications/AirtestIDE.app/Contents/Resources/selenium_plugin"
+        super().__init__(
+            chrome_options=chrome_options,
+            executable_path=executable_path,
+            port=port,
+            options=options,
+            service_args=service_args,
+            service_log_path=service_log_path,
+            desired_capabilities=desired_capabilities,
+        )
         self.father_number = {0: 0}
         self.action_chains = ActionChains(self)
         self.number = 0
         self.mouse = Controller()
-        self.operation_to_func = {"elementsD": self.find_any_element, "xpath": self.find_element_by_xpath,
-                                  "id": self.find_element_by_id,
-                                  "name": self.find_element_by_name, "css": self.find_element_by_css_selector}
+        self.operation_to_func = {
+            "elementsD": self.find_any_element,
+            "xpath": self.find_element_by_xpath,
+            "id": self.find_element_by_id,
+            "name": self.find_element_by_name,
+            "css": self.find_element_by_css_selector,
+        }
 
     def loop_find_element(self, func, text, timeout=10, interval=0.5):
         """
         Loop to find the target web element by func.
 
         Args:
             func: function to find element
@@ -79,15 +100,16 @@
                 element = func(text)
             except NoSuchElementException:
                 print("Element not found!")
                 # 超时则raise，未超时则进行下次循环:
                 if (time.time() - start_time) > timeout:
                     # try_log_screen(screen)
                     raise NoSuchElementException(
-                        'Element %s not found in screen' % text)
+                        "Element %s not found in screen" % text
+                    )
                 else:
                     time.sleep(interval)
             else:
                 return element
 
     def loop_find_element_noExc(self, func, text, timeout=3, interval=0.5):
         """
@@ -110,15 +132,15 @@
                 # 超时则raise，未超时则进行下次循环:
                 if (time.time() - start_time) > timeout:
                     # try_log_screen(screen)
                     return None
                 else:
                     time.sleep(interval)
             else:
-                print('element found')
+                print("element found")
                 return element
 
     @logwrap
     def find_any_element(self, elementsD):
         """
         Find the web element by the indicated parameters.
 
@@ -127,49 +149,65 @@
         Returns:
             Web element of current page.
         """
         web_element = None
         for key in elementsD:
             value = elementsD[key]
             print(value)
-            if key.upper() == 'ID':
-                web_element = self.loop_find_element_noExc(super().find_element_by_id, value)
-            elif key.upper() == 'XPATH':
-                web_element = self.loop_find_element_noExc(super().find_element_by_xpath, value)
-            elif key.upper() == 'CSS':
-                web_element = self.loop_find_element_noExc(super().find_element_by_css_selector, value)
-            elif key.upper() == 'NAME':
-                web_element = self.loop_find_element_noExc(super().find_element_by_name, value)
-            elif key.upper() == 'LINKTEXT':
-                web_element = self.loop_find_element_noExc(super().find_element_by_link_text, value)
-            elif key.upper() == 'CLASSNAME':
-                web_element = self.loop_find_element_noExc(super().find_element_by_class_name, value)
-            elif key.upper() == 'PARTIALLINKTEXT':
-                web_element = self.loop_find_element_noExc(super().find_element_by_partial_link_text, value)
-            elif key.upper() == 'TAGNAME':
-                web_element = self.loop_find_element_noExc(super().find_element_by_tag_name, value)
+            if key.upper() == "ID":
+                web_element = self.loop_find_element_noExc(
+                    super().find_element_by_id, value
+                )
+            elif key.upper() == "XPATH":
+                web_element = self.loop_find_element_noExc(
+                    super().find_element_by_xpath, value
+                )
+            elif key.upper() == "CSS":
+                web_element = self.loop_find_element_noExc(
+                    super().find_element_by_css_selector, value
+                )
+            elif key.upper() == "NAME":
+                web_element = self.loop_find_element_noExc(
+                    super().find_element_by_name, value
+                )
+            elif key.upper() == "LINKTEXT":
+                web_element = self.loop_find_element_noExc(
+                    super().find_element_by_link_text, value
+                )
+            elif key.upper() == "CLASSNAME":
+                web_element = self.loop_find_element_noExc(
+                    super().find_element_by_class_name, value
+                )
+            elif key.upper() == "PARTIALLINKTEXT":
+                web_element = self.loop_find_element_noExc(
+                    super().find_element_by_partial_link_text, value
+                )
+            elif key.upper() == "TAGNAME":
+                web_element = self.loop_find_element_noExc(
+                    super().find_element_by_tag_name, value
+                )
                 # check by position/ picture / visual testing
             if web_element is not None:
                 break
         if web_element is not None:
             log_res = self._gen_screen_log(web_element)
             return Element(web_element, log_res)
-        raise NoSuchElementException('Element not found in screen')
+        raise NoSuchElementException("Element not found in screen")
 
     @logwrap
     def find_element_by_xpath(self, xpath):
         """
         Find the web element by xpath.
 
         Args:
             xpath: find the element by xpath.
         Returns:
             Web element of current page.
         """
-        web_element = self.loop_find_element(super(WebChrome, self).find_element_by_xpath, xpath)
+        web_element = self.loop_find_element(super().find_element_by_xpath, xpath)
         # web_element = super(WebChrome, self).find_element_by_xpath(xpath)
         log_res = self._gen_screen_log(web_element)
         return Element(web_element, log_res)
 
     @logwrap
     def is_element_exist(self, xpath):
         """
@@ -199,97 +237,102 @@
         :return:
         """
 
         def _is_china(name):
             # To determine whether the file name contains Chinese, the official library requires that the file path must be in English,
             # otherwise an exception will be thrown, so a separate layer of judgment is added
             for ch in name:
-                if u'\u4e00' <= ch <= u'\u9fff':
+                if "\u4e00" <= ch <= "\u9fff":
                     return True
             return False
 
         try:
-            if plat() != 'Darwin':
+            if plat() != "Darwin":
                 return False
 
             if _is_china(file) is True:
-                log("Chinese characters are not allowed in the file path! Please change the file name. file path:{0}".format(
-                    file))
+                log(
+                    "Chinese characters are not allowed in the file path! Please change the file name. file path:{}".format(
+                        file
+                    )
+                )
 
             if _is_china(file) is False:
-                log("Start uploading files, file path:{0}".format(file))
+                log(f"Start uploading files, file path:{file}")
 
                 k = PyKeyboard()
 
                 m = PyMouse()
-                filepath = '/'
+                filepath = "/"
                 # Simulate keyboard clicks Command + Shift + G
-                k.press_keys(['Command', 'Shift', 'G'])
+                k.press_keys(["Command", "Shift", "G"])
 
                 # Get current screen size
                 x_dim, y_dim = m.screen_size()
                 m.click(x_dim // 2, y_dim // 2, 1)
 
                 # Copy the slash/at the beginning of the file path. If you don't add a slash, the script will miss the slash at the beginning
                 pyperclip.copy(filepath)
 
                 # Paste slash/
-                k.press_keys(['Command', 'V'])
+                k.press_keys(["Command", "V"])
                 # Enter the full path of the file
                 k.type_string(file)
                 sleep(2)
                 # When the input method is in Chinese, press enter once more
-                k.press_key('Return')
+                k.press_key("Return")
                 sleep(2)
-                k.press_key('Return')
+                k.press_key("Return")
                 sleep(2)
-                k.press_key('Return')
+                k.press_key("Return")
 
         except UtxSeleniumException:
-            log("Upload file failed! File path {0}".format(file), snapshot=True)
+            log(f"Upload file failed! File path {file}", snapshot=True)
 
     @logwrap
     def find_element_by_id(self, id):
         """
         Find the web element by id.
 
         Args:
             id: find the element by attribute id.
         Returns:
             Web element of current page.
         """
-        web_element = self.loop_find_element(super(WebChrome, self).find_element_by_id, id)
+        web_element = self.loop_find_element(super().find_element_by_id, id)
         log_res = self._gen_screen_log(web_element)
         return Element(web_element, log_res)
 
     @logwrap
     def find_element_by_css_selector(self, css_selector):
         """
         Find the web element by css_selector.
 
         Args:
             css_selector: find the element by attribute css_selector.
         Returns:
             Web element of current page.
         """
-        web_element = self.loop_find_element(super(WebChrome, self).find_element_by_css_selector, css_selector)
+        web_element = self.loop_find_element(
+            super().find_element_by_css_selector, css_selector
+        )
         log_res = self._gen_screen_log(web_element)
         return Element(web_element, log_res)
 
     @logwrap
     def find_element_by_name(self, name):
         """
         Find the web element by name.
 
         Args:
             name: find the element by attribute name.
         Returns:
             Web element of current page.
         """
-        web_element = self.loop_find_element(super(WebChrome, self).find_element_by_name, name)
+        web_element = self.loop_find_element(super().find_element_by_name, name)
         log_res = self._gen_screen_log(web_element)
         return Element(web_element, log_res)
 
     @logwrap
     def switch_to_new_tab(self):
         """
         Switch to the new tab.
@@ -384,58 +427,62 @@
     def get(self, address):
         """
         Access the web address.
 
         Args:
             address: the address that to accesss
         """
-        super(WebChrome, self).get(address)
+        super().get(address)
         time.sleep(2)
 
     @logwrap
     def back(self):
         """
         Back to last page.
         """
-        super(WebChrome, self).back()
+        super().back()
         self._gen_screen_log()
         time.sleep(1)
 
     @logwrap
     def forward(self):
         """
         Forward to next page.
         """
-        super(WebChrome, self).forward()
+        super().forward()
         self._gen_screen_log()
         time.sleep(1)
 
     @logwrap
     def snapshot(self, filename=None):
         self._gen_screen_log(filename=filename)
 
     @logwrap
-    def _gen_screen_log(self, element=None, filename=None, ):
+    def _gen_screen_log(
+        self,
+        element=None,
+        filename=None,
+    ):
         if ST.LOG_DIR is None:
             return None
         if filename:
             self.screenshot(filename)
 
         # 忽略警告 .jpg
-        jpg_file_name = str(int(time.time())) + '.png'
+        jpg_file_name = str(int(time.time())) + ".png"
         # 适配utx报告路径
         jpg_path = os.path.join(ST.LOG_DIR, jpg_file_name)
         print("this is jpg path:", jpg_path)
         self.screenshot(jpg_path)
         saved = {"screen": jpg_path}
         if element:
             size = element.size
             location = element.location
-            x = size['width'] / 2 + location['x']
-            y = size['height'] / 2 + location['y']
+            x = size["width"] / 2 + location["x"]
+            y = size["height"] / 2 + location["y"]
             if "darwin" in sys.platform:
                 x, y = x * 2, y * 2
             saved.update({"pos": [[x, y]]})
         return saved
 
     def screenshot(self, file_path=None):
         if file_path:
@@ -451,47 +498,66 @@
 
     def _get_left_up_offset(self):
         window_pos = self.get_window_position()
         window_size = self.get_window_size()
         mouse = Controller()
         screen = self.screenshot()
         screen_size = get_resolution(screen)
-        offset = window_size["width"] - \
-                 screen_size[0], window_size["height"] - screen_size[1]
-        pos = (int(offset[0] / 2 + window_pos['x']),
-               int(offset[1] + window_pos['y'] - offset[0] / 2))
+        offset = (
+            window_size["width"] - screen_size[0],
+            window_size["height"] - screen_size[1],
+        )
+        pos = (
+            int(offset[0] / 2 + window_pos["x"]),
+            int(offset[1] + window_pos["y"] - offset[0] / 2),
+        )
         return pos
 
     def _move_to_pos(self, pos):
         self.mouse.position = pos
 
     def _click_current_pos(self):
         self.mouse.click(Button.left, 1)
 
     def to_json(self):
         # add this method for json encoder in logwrap
         return repr(self)
 
 
 class WebRemote(Remote):
-
-    def __init__(self, command_executor='http://127.0.0.1:4444/wd/hub',
-                 desired_capabilities=None, browser_profile=None, proxy=None,
-                 keep_alive=False, file_detector=None, options=None):
-        super(WebRemote, self).__init__(command_executor=command_executor,
-                                        desired_capabilities=desired_capabilities, browser_profile=browser_profile,
-                                        proxy=proxy,
-                                        keep_alive=keep_alive, file_detector=file_detector, options=options)
+    def __init__(
+        self,
+        command_executor="http://127.0.0.1:4444/wd/hub",
+        desired_capabilities=None,
+        browser_profile=None,
+        proxy=None,
+        keep_alive=False,
+        file_detector=None,
+        options=None,
+    ):
+        super().__init__(
+            command_executor=command_executor,
+            desired_capabilities=desired_capabilities,
+            browser_profile=browser_profile,
+            proxy=proxy,
+            keep_alive=keep_alive,
+            file_detector=file_detector,
+            options=options,
+        )
 
         self.father_number = {0: 0}
         self.action_chains = ActionChains(self)
         self.number = 0
         self.mouse = Controller()
-        self.operation_to_func = {"xpath": self.find_element_by_xpath, "id": self.find_element_by_id,
-                                  "name": self.find_element_by_name, "css": self.find_element_by_css_selector}
+        self.operation_to_func = {
+            "xpath": self.find_element_by_xpath,
+            "id": self.find_element_by_id,
+            "name": self.find_element_by_name,
+            "css": self.find_element_by_css_selector,
+        }
 
     def loop_find_element(self, func, text, timeout=10, interval=0.5):
         """
         Loop to find the target web element by func.
 
         Args:
             func: function to find element
@@ -506,15 +572,17 @@
             try:
                 element = func(text)
             except NoSuchElementException:
                 print("Element not found!")
                 # 超时则raise，未超时则进行下次循环:
                 if (time.time() - start_time) > timeout:
                     # try_log_screen(screen)
-                    raise NoSuchElementException('Element %s not found in screen' % text)
+                    raise NoSuchElementException(
+                        "Element %s not found in screen" % text
+                    )
                 else:
                     time.sleep(interval)
             else:
                 return element
 
     @logwrap
     def find_element_by_xpath(self, xpath):
@@ -522,57 +590,59 @@
         Find the web element by xpath.
 
         Args:
             xpath: find the element by xpath.
         Returns:
             Web element of current page.
         """
-        web_element = self.loop_find_element(super(WebRemote, self).find_element_by_xpath, xpath)
+        web_element = self.loop_find_element(super().find_element_by_xpath, xpath)
         log_res = self._gen_screen_log(web_element)
         return Element(web_element, log_res)
 
     @logwrap
     def find_element_by_id(self, id):
         """
         Find the web element by id.
 
         Args:
             id: find the element by attribute id.
         Returns:
             Web element of current page.
         """
-        web_element = self.loop_find_element(super(WebRemote, self).find_element_by_id, id)
+        web_element = self.loop_find_element(super().find_element_by_id, id)
         log_res = self._gen_screen_log(web_element)
         return Element(web_element, log_res)
 
     @logwrap
     def find_element_by_css_selector(self, css_selector):
         """
         Find the web element by css_selector.
 
         Args:
             css_selector: find the element by attribute css_selector.
         Returns:
             Web element of current page.
         """
-        web_element = self.loop_find_element(super(WebRemote, self).find_element_by_css_selector, css_selector)
+        web_element = self.loop_find_element(
+            super().find_element_by_css_selector, css_selector
+        )
         log_res = self._gen_screen_log(web_element)
         return Element(web_element, log_res)
 
     @logwrap
     def find_element_by_name(self, name):
         """
         Find the web element by name.
 
         Args:
             name: find the element by attribute name.
         Returns:
             Web element of current page.
         """
-        web_element = self.loop_find_element(super(WebRemote, self).find_element_by_name, name)
+        web_element = self.loop_find_element(super().find_element_by_name, name)
         log_res = self._gen_screen_log(web_element)
         return Element(web_element, log_res)
 
     @logwrap
     def switch_to_new_tab(self):
         """
         Switch to the new tab.
@@ -664,55 +734,59 @@
     def get(self, address):
         """
         Access the web address.
 
         Args:
             address: the address that to accesss
         """
-        super(WebRemote, self).get(address)
+        super().get(address)
         time.sleep(2)
 
     @logwrap
     def back(self):
         """
         Back to last page.
         """
-        super(WebRemote, self).back()
+        super().back()
         self._gen_screen_log()
         time.sleep(1)
 
     @logwrap
     def forward(self):
         """
         Forward to next page.
         """
-        super(WebRemote, self).forward()
+        super().forward()
         self._gen_screen_log()
         time.sleep(1)
 
     @logwrap
     def snapshot(self, filename=None):
         self._gen_screen_log(filename=filename)
 
     @logwrap
-    def _gen_screen_log(self, element=None, filename=None, ):
+    def _gen_screen_log(
+        self,
+        element=None,
+        filename=None,
+    ):
         if ST.LOG_DIR is None:
             return None
         if filename:
             self.screenshot(filename)
-        jpg_file_name = str(int(time.time())) + '.png'
+        jpg_file_name = str(int(time.time())) + ".png"
         jpg_path = os.path.join(ST.LOG_DIR, jpg_file_name)
         print("this is jpg path:", jpg_path)
         self.screenshot(jpg_path)
         saved = {"screen": jpg_path}
         if element:
             size = element.size
             location = element.location
-            x = size['width'] / 2 + location['x']
-            y = size['height'] / 2 + location['y']
+            x = size["width"] / 2 + location["x"]
+            y = size["height"] / 2 + location["y"]
             if "darwin" in sys.platform:
                 x, y = x * 2, y * 2
             saved.update({"pos": [[x, y]]})
         return saved
 
     def screenshot(self, file_path=None):
         if file_path:
@@ -728,50 +802,76 @@
 
     def _get_left_up_offset(self):
         window_pos = self.get_window_position()
         window_size = self.get_window_size()
         mouse = Controller()
         screen = self.screenshot()
         screen_size = get_resolution(screen)
-        offset = window_size["width"] - \
-                 screen_size[0], window_size["height"] - screen_size[1]
-        pos = (int(offset[0] / 2 + window_pos['x']),
-               int(offset[1] + window_pos['y'] - offset[0] / 2))
+        offset = (
+            window_size["width"] - screen_size[0],
+            window_size["height"] - screen_size[1],
+        )
+        pos = (
+            int(offset[0] / 2 + window_pos["x"]),
+            int(offset[1] + window_pos["y"] - offset[0] / 2),
+        )
         return pos
 
     def _move_to_pos(self, pos):
         self.mouse.position = pos
 
     def _click_current_pos(self):
         self.mouse.click(Button.left, 1)
 
     def to_json(self):
         # add this method for json encoder in logwrap
         return repr(self)
 
 
 class WebFirefox(Firefox):
-
-    def __init__(self, firefox_profile=None, firefox_binary=None,
-                 timeout=30, capabilities=None, proxy=None,
-                 executable_path="geckodriver", options=None, firefox_options=None,
-                 service_args=None, desired_capabilities=None, log_path=None):
-        print("Please make sure your geckodriver is in your path before proceeding using this driver")
-        super(WebFirefox, self).__init__(firefox_profile=firefox_profile, firefox_binary=firefox_binary,
-                                         timeout=timeout, capabilities=capabilities, proxy=proxy,
-                                         executable_path=executable_path, options=options,
-                                         firefox_options=firefox_options,
-                                         service_args=service_args, desired_capabilities=desired_capabilities,
-                                         log_path=log_path)
+    def __init__(
+        self,
+        firefox_profile=None,
+        firefox_binary=None,
+        timeout=30,
+        capabilities=None,
+        proxy=None,
+        executable_path="geckodriver",
+        options=None,
+        firefox_options=None,
+        service_args=None,
+        desired_capabilities=None,
+        log_path=None,
+    ):
+        print(
+            "Please make sure your geckodriver is in your path before proceeding using this driver"
+        )
+        super().__init__(
+            firefox_profile=firefox_profile,
+            firefox_binary=firefox_binary,
+            timeout=timeout,
+            capabilities=capabilities,
+            proxy=proxy,
+            executable_path=executable_path,
+            options=options,
+            firefox_options=firefox_options,
+            service_args=service_args,
+            desired_capabilities=desired_capabilities,
+            log_path=log_path,
+        )
         self.father_number = {0: 0}
         self.action_chains = ActionChains(self)
         self.number = 0
         self.mouse = Controller()
-        self.operation_to_func = {"xpath": self.find_element_by_xpath, "id": self.find_element_by_id,
-                                  "name": self.find_element_by_name, "css": self.find_element_by_css_selector}
+        self.operation_to_func = {
+            "xpath": self.find_element_by_xpath,
+            "id": self.find_element_by_id,
+            "name": self.find_element_by_name,
+            "css": self.find_element_by_css_selector,
+        }
 
     def loop_find_element(self, func, text, timeout=10, interval=0.5):
         """
         Loop to find the target web element by func.
 
         Args:
             func: function to find element
@@ -786,15 +886,17 @@
             try:
                 element = func(text)
             except NoSuchElementException:
                 print("Element not found!")
                 # 超时则raise，未超时则进行下次循环:
                 if (time.time() - start_time) > timeout:
                     # try_log_screen(screen)
-                    raise NoSuchElementException('Element %s not found in screen' % text)
+                    raise NoSuchElementException(
+                        "Element %s not found in screen" % text
+                    )
                 else:
                     time.sleep(interval)
             else:
                 return element
 
     @logwrap
     def find_element_by_xpath(self, xpath):
@@ -802,57 +904,65 @@
         Find the web element by xpath.
 
         Args:
             xpath: find the element by xpath.
         Returns:
             Web element of current page.
         """
-        web_element = self.loop_find_element(super(Firefox, self).find_element_by_xpath, xpath)
+        web_element = self.loop_find_element(
+            super(Firefox, self).find_element_by_xpath, xpath
+        )
         log_res = self._gen_screen_log(web_element)
         return Element(web_element, log_res)
 
     @logwrap
     def find_element_by_id(self, id):
         """
         Find the web element by id.
 
         Args:
             id: find the element by attribute id.
         Returns:
             Web element of current page.
         """
-        web_element = self.loop_find_element(super(Firefox, self).find_element_by_id, id)
+        web_element = self.loop_find_element(
+            super(Firefox, self).find_element_by_id, id
+        )
         log_res = self._gen_screen_log(web_element)
         return Element(web_element, log_res)
 
     @logwrap
     def find_element_by_css_selector(self, css_selector):
         """
         Find the web element by css_selector.
 
         Args:
             css_selector: find the element by attribute css_selector.
         Returns:
             Web element of current page.
         """
-        web_element = self.loop_find_element(super(Firefox, self).find_element_by_css_selector, css_selector)
+        web_element = self.loop_find_element(
+            super(Firefox, self).find_element_by_css_selector, css_selector
+        )
         log_res = self._gen_screen_log(web_element)
         return Element(web_element, log_res)
 
     @logwrap
     def find_element_by_name(self, name):
         """
         Find the web element by name.
 
         Args:
             name: find the element by attribute name.
         Returns:
             Web element of current page.
         """
-        web_element = self.loop_find_element(super(Firefox, self).find_element_by_name, name)
+        web_element = self.loop_find_element(
+            super(Firefox, self).find_element_by_name, name
+        )
         log_res = self._gen_screen_log(web_element)
         return Element(web_element, log_res)
 
     @logwrap
     def switch_to_new_tab(self):
         """
         Switch to the new tab.
@@ -944,55 +1054,59 @@
     def get(self, address):
         """
         Access the web address.
 
         Args:
             address: the address that to accesss
         """
-        super(WebFirefox, self).get(address)
+        super().get(address)
         time.sleep(2)
 
     @logwrap
     def back(self):
         """
         Back to last page.
         """
-        super(WebFirefox, self).back()
+        super().back()
         self._gen_screen_log()
         time.sleep(1)
 
     @logwrap
     def forward(self):
         """
         Forward to next page.
         """
-        super(WebFirefox, self).forward()
+        super().forward()
         self._gen_screen_log()
         time.sleep(1)
 
     @logwrap
     def snapshot(self, filename=None):
         self._gen_screen_log(filename=filename)
 
     @logwrap
-    def _gen_screen_log(self, element=None, filename=None, ):
+    def _gen_screen_log(
+        self,
+        element=None,
+        filename=None,
+    ):
         if ST.LOG_DIR is None:
             return None
         if filename:
             self.screenshot(filename)
-        jpg_file_name = str(int(time.time())) + '.png'
+        jpg_file_name = str(int(time.time())) + ".png"
         jpg_path = os.path.join(ST.LOG_DIR, jpg_file_name)
         print("this is jpg path:", jpg_path)
         self.screenshot(jpg_path)
         saved = {"screen": jpg_path}
         if element:
             size = element.size
             location = element.location
-            x = size['width'] / 2 + location['x']
-            y = size['height'] / 2 + location['y']
+            x = size["width"] / 2 + location["x"]
+            y = size["height"] / 2 + location["y"]
             if "darwin" in sys.platform:
                 x, y = x * 2, y * 2
             saved.update({"pos": [[x, y]]})
         return saved
 
     def screenshot(self, file_path=None):
         if file_path:
@@ -1008,43 +1122,45 @@
 
     def _get_left_up_offset(self):
         window_pos = self.get_window_position()
         window_size = self.get_window_size()
         mouse = Controller()
         screen = self.screenshot()
         screen_size = get_resolution(screen)
-        offset = window_size["width"] - \
-                 screen_size[0], window_size["height"] - screen_size[1]
-        pos = (int(offset[0] / 2 + window_pos['x']),
-               int(offset[1] + window_pos['y'] - offset[0] / 2))
+        offset = (
+            window_size["width"] - screen_size[0],
+            window_size["height"] - screen_size[1],
+        )
+        pos = (
+            int(offset[0] / 2 + window_pos["x"]),
+            int(offset[1] + window_pos["y"] - offset[0] / 2),
+        )
         return pos
 
     def _move_to_pos(self, pos):
         self.mouse.position = pos
 
     def _click_current_pos(self):
         self.mouse.click(Button.left, 1)
 
     def to_json(self):
         # add this method for json encoder in logwrap
         return repr(self)
 
 
 class Element(WebElement):
-
     def __init__(self, _obj, log):
-        super(Element, self).__init__(
-            parent=_obj._parent, id_=_obj._id, w3c=_obj._w3c)
+        super().__init__(parent=_obj._parent, id_=_obj._id, w3c=_obj._w3c)
         self.res_log = log
 
     def click(self):
-        super(Element, self).click()
+        super().click()
         time.sleep(0.5)
         return self.res_log
 
     def send_keys(self, text, keyborad=None):
         if keyborad:
-            super(Element, self).send_keys(text, keyborad)
+            super().send_keys(text, keyborad)
         else:
-            super(Element, self).send_keys(text)
+            super().send_keys(text)
         time.sleep(0.5)
         return self.res_log
```

### Comparing `utx-1.3.3/utx/selenium/utils/airtest_api.py` & `utx-1.3.4/utx/selenium/utils/airtest_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 #!/usr/bin/python
-# encoding=utf-8
-
 """
 @Author  :  Lijiawei
 @Date    :  11/02/2021 3:36 PM
 @Desc    :  airtest_api line.
 """
-import time
 import os
-from airtest.core.helper import G, logwrap
+import time
+
 from airtest import aircv
 from airtest.aircv import get_resolution
 from airtest.core.error import TargetNotFoundError
+from airtest.core.helper import G
+from airtest.core.helper import logwrap
 from airtest.core.settings import Settings as ST
 
 
 @logwrap
-def loop_find(query, driver=None, timeout=10, threshold=None, interval=0.5, intervalfunc=None):
+def loop_find(
+    query, driver=None, timeout=10, threshold=None, interval=0.5, intervalfunc=None
+):
     """
     Search for image template in the screen until timeout
 
     Args:
         query: image template to be found in screenshot
         timeout: time interval how long to look for the image template
         threshold: default is None
@@ -51,15 +53,15 @@
 
         if intervalfunc is not None:
             intervalfunc()
 
         # 超时则raise，未超时则进行下次循环:
         if (time.time() - start_time) > timeout:
             try_log_screen(screen)
-            raise TargetNotFoundError('Picture %s not found in screen' % query)
+            raise TargetNotFoundError("Picture %s not found in screen" % query)
         else:
             time.sleep(interval)
 
 
 @logwrap
 def try_log_screen(screen=None):
     """
@@ -72,11 +74,11 @@
         None
 
     """
     if not ST.LOG_DIR:
         return
     if screen is None:
         screen = G.DEVICE.snapshot()
-    filename = "%(time)d.jpg" % {'time': time.time() * 1000}
+    filename = "%(time)d.jpg" % {"time": time.time() * 1000}
     filepath = os.path.join(ST.LOG_DIR, filename)
     aircv.imwrite(filepath, screen)
     return filename
```

### Comparing `utx-1.3.3/utx/selenium/utils/six.py` & `utx-1.3.4/utx/selenium/utils/six.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Utilities for writing code that runs on Python 2 and 3"""
-
 # Copyright (c) 2010-2015 Benjamin Peterson
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
@@ -15,17 +14,14 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
-from __future__ import absolute_import
-
 import functools
 import itertools
 import operator
 import sys
 import types
 
 __author__ = "Benjamin Peterson <benjamin@python.org>"
@@ -34,37 +30,37 @@
 
 # Useful for very coarse version differentiation.
 PY2 = sys.version_info[0] == 2
 PY3 = sys.version_info[0] == 3
 PY34 = sys.version_info[0:2] >= (3, 4)
 
 if PY3:
-    string_types = str,
-    integer_types = int,
-    class_types = type,
+    string_types = (str,)
+    integer_types = (int,)
+    class_types = (type,)
     text_type = str
     binary_type = bytes
 
     MAXSIZE = sys.maxsize
 else:
-    string_types = basestring,
+    string_types = (basestring,)
     integer_types = (int, long)
     class_types = (type, types.ClassType)
     text_type = unicode
     binary_type = str
 
     if sys.platform.startswith("java"):
         # Jython always uses 32 bits.
         MAXSIZE = int((1 << 31) - 1)
     else:
         # It's possible to have sizeof(long) != sizeof(Py_ssize_t).
-        class X(object):
-
+        class X:
             def __len__(self):
                 return 1 << 31
+
         try:
             len(X())
         except OverflowError:
             # 32-bit
             MAXSIZE = int((1 << 31) - 1)
         else:
             # 64-bit
@@ -79,16 +75,15 @@
 
 def _import_module(name):
     """Import module, returning the module after the last dot."""
     __import__(name)
     return sys.modules[name]
 
 
-class _LazyDescr(object):
-
+class _LazyDescr:
     def __init__(self, name):
         self.name = name
 
     def __get__(self, obj, tp):
         result = self._resolve()
         setattr(obj, self.name, result)  # Invokes __set__.
         try:
@@ -97,17 +92,16 @@
             delattr(obj.__class__, self.name)
         except AttributeError:
             pass
         return result
 
 
 class MovedModule(_LazyDescr):
-
     def __init__(self, name, old, new=None):
-        super(MovedModule, self).__init__(name)
+        super().__init__(name)
         if PY3:
             if new is None:
                 new = name
             self.mod = new
         else:
             self.mod = old
 
@@ -118,32 +112,30 @@
         _module = self._resolve()
         value = getattr(_module, attr)
         setattr(self, attr, value)
         return value
 
 
 class _LazyModule(types.ModuleType):
-
     def __init__(self, name):
-        super(_LazyModule, self).__init__(name)
+        super().__init__(name)
         self.__doc__ = self.__class__.__doc__
 
     def __dir__(self):
         attrs = ["__doc__", "__name__"]
         attrs += [attr.name for attr in self._moved_attributes]
         return attrs
 
     # Subclasses should override this
     _moved_attributes = []
 
 
 class MovedAttribute(_LazyDescr):
-
     def __init__(self, name, old_mod, new_mod, old_attr=None, new_attr=None):
-        super(MovedAttribute, self).__init__(name)
+        super().__init__(name)
         if PY3:
             if new_mod is None:
                 new_mod = name
             self.mod = new_mod
             if new_attr is None:
                 if old_attr is None:
                     new_attr = name
@@ -157,15 +149,15 @@
             self.attr = old_attr
 
     def _resolve(self):
         module = _import_module(self.mod)
         return getattr(module, self.attr)
 
 
-class _SixMetaPathImporter(object):
+class _SixMetaPathImporter:
 
     """
     A meta path importer to import six.moves and its submodules.
 
     This class implements a PEP302 finder and loader. It should be compatible
     with Python 2.5 and all existing versions of Python3
     """
@@ -217,57 +209,68 @@
 
     def get_code(self, fullname):
         """Return None
 
         Required, if is_package is implemented"""
         self.__get_module(fullname)  # eventually raises ImportError
         return None
+
     get_source = get_code  # same as get_code
 
+
 _importer = _SixMetaPathImporter(__name__)
 
 
 class _MovedItems(_LazyModule):
 
     """Lazy loading of moved objects"""
+
     __path__ = []  # mark as package
 
 
 _moved_attributes = [
     MovedAttribute("cStringIO", "cStringIO", "io", "StringIO"),
     MovedAttribute("filter", "itertools", "builtins", "ifilter", "filter"),
-    MovedAttribute("filterfalse", "itertools", "itertools", "ifilterfalse", "filterfalse"),
+    MovedAttribute(
+        "filterfalse", "itertools", "itertools", "ifilterfalse", "filterfalse"
+    ),
     MovedAttribute("input", "__builtin__", "builtins", "raw_input", "input"),
     MovedAttribute("intern", "__builtin__", "sys"),
     MovedAttribute("map", "itertools", "builtins", "imap", "map"),
     MovedAttribute("getcwd", "os", "os", "getcwdu", "getcwd"),
     MovedAttribute("getcwdb", "os", "os", "getcwd", "getcwdb"),
     MovedAttribute("range", "__builtin__", "builtins", "xrange", "range"),
-    MovedAttribute("reload_module", "__builtin__", "importlib" if PY34 else "imp", "reload"),
+    MovedAttribute(
+        "reload_module", "__builtin__", "importlib" if PY34 else "imp", "reload"
+    ),
     MovedAttribute("reduce", "__builtin__", "functools"),
     MovedAttribute("shlex_quote", "pipes", "shlex", "quote"),
     MovedAttribute("StringIO", "StringIO", "io"),
     MovedAttribute("UserDict", "UserDict", "collections"),
     MovedAttribute("UserList", "UserList", "collections"),
     MovedAttribute("UserString", "UserString", "collections"),
     MovedAttribute("xrange", "__builtin__", "builtins", "xrange", "range"),
     MovedAttribute("zip", "itertools", "builtins", "izip", "zip"),
-    MovedAttribute("zip_longest", "itertools", "itertools", "izip_longest", "zip_longest"),
+    MovedAttribute(
+        "zip_longest", "itertools", "itertools", "izip_longest", "zip_longest"
+    ),
     MovedModule("builtins", "__builtin__"),
     MovedModule("configparser", "ConfigParser"),
     MovedModule("copyreg", "copy_reg"),
     MovedModule("dbm_gnu", "gdbm", "dbm.gnu"),
     MovedModule("_dummy_thread", "dummy_thread", "_dummy_thread"),
     MovedModule("http_cookiejar", "cookielib", "http.cookiejar"),
     MovedModule("http_cookies", "Cookie", "http.cookies"),
     MovedModule("html_entities", "htmlentitydefs", "html.entities"),
     MovedModule("html_parser", "HTMLParser", "html.parser"),
     MovedModule("http_client", "httplib", "http.client"),
     MovedModule("email_mime_multipart", "email.MIMEMultipart", "email.mime.multipart"),
-    MovedModule("email_mime_nonmultipart", "email.MIMENonMultipart", "email.mime.nonmultipart"),
+    MovedModule(
+        "email_mime_nonmultipart", "email.MIMENonMultipart", "email.mime.nonmultipart"
+    ),
     MovedModule("email_mime_text", "email.MIMEText", "email.mime.text"),
     MovedModule("email_mime_base", "email.MIMEBase", "email.mime.base"),
     MovedModule("BaseHTTPServer", "BaseHTTPServer", "http.server"),
     MovedModule("CGIHTTPServer", "CGIHTTPServer", "http.server"),
     MovedModule("SimpleHTTPServer", "SimpleHTTPServer", "http.server"),
     MovedModule("cPickle", "cPickle", "pickle"),
     MovedModule("queue", "Queue"),
@@ -279,23 +282,20 @@
     MovedModule("tkinter_filedialog", "FileDialog", "tkinter.filedialog"),
     MovedModule("tkinter_scrolledtext", "ScrolledText", "tkinter.scrolledtext"),
     MovedModule("tkinter_simpledialog", "SimpleDialog", "tkinter.simpledialog"),
     MovedModule("tkinter_tix", "Tix", "tkinter.tix"),
     MovedModule("tkinter_ttk", "ttk", "tkinter.ttk"),
     MovedModule("tkinter_constants", "Tkconstants", "tkinter.constants"),
     MovedModule("tkinter_dnd", "Tkdnd", "tkinter.dnd"),
-    MovedModule("tkinter_colorchooser", "tkColorChooser",
-                "tkinter.colorchooser"),
-    MovedModule("tkinter_commondialog", "tkCommonDialog",
-                "tkinter.commondialog"),
+    MovedModule("tkinter_colorchooser", "tkColorChooser", "tkinter.colorchooser"),
+    MovedModule("tkinter_commondialog", "tkCommonDialog", "tkinter.commondialog"),
     MovedModule("tkinter_tkfiledialog", "tkFileDialog", "tkinter.filedialog"),
     MovedModule("tkinter_font", "tkFont", "tkinter.font"),
     MovedModule("tkinter_messagebox", "tkMessageBox", "tkinter.messagebox"),
-    MovedModule("tkinter_tksimpledialog", "tkSimpleDialog",
-                "tkinter.simpledialog"),
+    MovedModule("tkinter_tksimpledialog", "tkSimpleDialog", "tkinter.simpledialog"),
     MovedModule("urllib_parse", __name__ + ".moves.urllib_parse", "urllib.parse"),
     MovedModule("urllib_error", __name__ + ".moves.urllib_error", "urllib.error"),
     MovedModule("urllib", __name__ + ".moves.urllib", __name__ + ".moves.urllib"),
     MovedModule("urllib_robotparser", "robotparser", "urllib.robotparser"),
     MovedModule("xmlrpc_client", "xmlrpclib", "xmlrpc.client"),
     MovedModule("xmlrpc_server", "SimpleXMLRPCServer", "xmlrpc.server"),
 ]
@@ -349,16 +349,19 @@
 ]
 for attr in _urllib_parse_moved_attributes:
     setattr(Module_six_moves_urllib_parse, attr.name, attr)
 del attr
 
 Module_six_moves_urllib_parse._moved_attributes = _urllib_parse_moved_attributes
 
-_importer._add_module(Module_six_moves_urllib_parse(__name__ + ".moves.urllib_parse"),
-                      "moves.urllib_parse", "moves.urllib.parse")
+_importer._add_module(
+    Module_six_moves_urllib_parse(__name__ + ".moves.urllib_parse"),
+    "moves.urllib_parse",
+    "moves.urllib.parse",
+)
 
 
 class Module_six_moves_urllib_error(_LazyModule):
 
     """Lazy loading of moved objects in six.moves.urllib_error"""
 
 
@@ -369,16 +372,19 @@
 ]
 for attr in _urllib_error_moved_attributes:
     setattr(Module_six_moves_urllib_error, attr.name, attr)
 del attr
 
 Module_six_moves_urllib_error._moved_attributes = _urllib_error_moved_attributes
 
-_importer._add_module(Module_six_moves_urllib_error(__name__ + ".moves.urllib.error"),
-                      "moves.urllib_error", "moves.urllib.error")
+_importer._add_module(
+    Module_six_moves_urllib_error(__name__ + ".moves.urllib.error"),
+    "moves.urllib_error",
+    "moves.urllib.error",
+)
 
 
 class Module_six_moves_urllib_request(_LazyModule):
 
     """Lazy loading of moved objects in six.moves.urllib_request"""
 
 
@@ -419,16 +425,19 @@
 ]
 for attr in _urllib_request_moved_attributes:
     setattr(Module_six_moves_urllib_request, attr.name, attr)
 del attr
 
 Module_six_moves_urllib_request._moved_attributes = _urllib_request_moved_attributes
 
-_importer._add_module(Module_six_moves_urllib_request(__name__ + ".moves.urllib.request"),
-                      "moves.urllib_request", "moves.urllib.request")
+_importer._add_module(
+    Module_six_moves_urllib_request(__name__ + ".moves.urllib.request"),
+    "moves.urllib_request",
+    "moves.urllib.request",
+)
 
 
 class Module_six_moves_urllib_response(_LazyModule):
 
     """Lazy loading of moved objects in six.moves.urllib_response"""
 
 
@@ -440,51 +449,62 @@
 ]
 for attr in _urllib_response_moved_attributes:
     setattr(Module_six_moves_urllib_response, attr.name, attr)
 del attr
 
 Module_six_moves_urllib_response._moved_attributes = _urllib_response_moved_attributes
 
-_importer._add_module(Module_six_moves_urllib_response(__name__ + ".moves.urllib.response"),
-                      "moves.urllib_response", "moves.urllib.response")
+_importer._add_module(
+    Module_six_moves_urllib_response(__name__ + ".moves.urllib.response"),
+    "moves.urllib_response",
+    "moves.urllib.response",
+)
 
 
 class Module_six_moves_urllib_robotparser(_LazyModule):
 
     """Lazy loading of moved objects in six.moves.urllib_robotparser"""
 
 
 _urllib_robotparser_moved_attributes = [
     MovedAttribute("RobotFileParser", "robotparser", "urllib.robotparser"),
 ]
 for attr in _urllib_robotparser_moved_attributes:
     setattr(Module_six_moves_urllib_robotparser, attr.name, attr)
 del attr
 
-Module_six_moves_urllib_robotparser._moved_attributes = _urllib_robotparser_moved_attributes
-
-_importer._add_module(Module_six_moves_urllib_robotparser(__name__ + ".moves.urllib.robotparser"),
-                      "moves.urllib_robotparser", "moves.urllib.robotparser")
+Module_six_moves_urllib_robotparser._moved_attributes = (
+    _urllib_robotparser_moved_attributes
+)
+
+_importer._add_module(
+    Module_six_moves_urllib_robotparser(__name__ + ".moves.urllib.robotparser"),
+    "moves.urllib_robotparser",
+    "moves.urllib.robotparser",
+)
 
 
 class Module_six_moves_urllib(types.ModuleType):
 
     """Create a six.moves.urllib namespace that resembles the Python 3 namespace"""
+
     __path__ = []  # mark as package
     parse = _importer._get_module("moves.urllib_parse")
     error = _importer._get_module("moves.urllib_error")
     request = _importer._get_module("moves.urllib_request")
     response = _importer._get_module("moves.urllib_response")
     robotparser = _importer._get_module("moves.urllib_robotparser")
 
     def __dir__(self):
-        return ['parse', 'error', 'request', 'response', 'robotparser']
+        return ["parse", "error", "request", "response", "robotparser"]
+
 
-_importer._add_module(Module_six_moves_urllib(__name__ + ".moves.urllib"),
-                      "moves.urllib")
+_importer._add_module(
+    Module_six_moves_urllib(__name__ + ".moves.urllib"), "moves.urllib"
+)
 
 
 def add_move(move):
     """Add an item to six.moves."""
     setattr(_MovedItems, move.name, move)
 
 
@@ -492,15 +512,15 @@
     """Remove item from six.moves."""
     try:
         delattr(_MovedItems, name)
     except AttributeError:
         try:
             del moves.__dict__[name]
         except KeyError:
-            raise AttributeError("no such move, %r" % (name,))
+            raise AttributeError(f"no such move, {name!r}")
 
 
 if PY3:
     _meth_func = "__func__"
     _meth_self = "__self__"
 
     _func_closure = "__closure__"
@@ -516,65 +536,72 @@
     _func_defaults = "func_defaults"
     _func_globals = "func_globals"
 
 
 try:
     advance_iterator = next
 except NameError:
+
     def advance_iterator(it):
         return it.next()
+
+
 next = advance_iterator
 
 
 try:
     callable = callable
 except NameError:
+
     def callable(obj):
         return any("__call__" in klass.__dict__ for klass in type(obj).__mro__)
 
 
 if PY3:
+
     def get_unbound_function(unbound):
         return unbound
 
     create_bound_method = types.MethodType
 
     def create_unbound_method(func, cls):
         return func
 
     Iterator = object
 else:
+
     def get_unbound_function(unbound):
         return unbound.im_func
 
     def create_bound_method(func, obj):
         return types.MethodType(func, obj, obj.__class__)
 
     def create_unbound_method(func, cls):
         return types.MethodType(func, None, cls)
 
-    class Iterator(object):
-
+    class Iterator:
         def next(self):
             return type(self).__next__(self)
 
     callable = callable
-_add_doc(get_unbound_function,
-         """Get the function out of a possibly unbound function""")
+_add_doc(
+    get_unbound_function, """Get the function out of a possibly unbound function"""
+)
 
 
 get_method_function = operator.attrgetter(_meth_func)
 get_method_self = operator.attrgetter(_meth_self)
 get_function_closure = operator.attrgetter(_func_closure)
 get_function_code = operator.attrgetter(_func_code)
 get_function_defaults = operator.attrgetter(_func_defaults)
 get_function_globals = operator.attrgetter(_func_globals)
 
 
 if PY3:
+
     def iterkeys(d, **kw):
         return iter(d.keys(**kw))
 
     def itervalues(d, **kw):
         return iter(d.values(**kw))
 
     def iteritems(d, **kw):
@@ -585,14 +612,15 @@
 
     viewkeys = operator.methodcaller("keys")
 
     viewvalues = operator.methodcaller("values")
 
     viewitems = operator.methodcaller("items")
 else:
+
     def iterkeys(d, **kw):
         return d.iterkeys(**kw)
 
     def itervalues(d, **kw):
         return d.itervalues(**kw)
 
     def iteritems(d, **kw):
@@ -605,60 +633,69 @@
 
     viewvalues = operator.methodcaller("viewvalues")
 
     viewitems = operator.methodcaller("viewitems")
 
 _add_doc(iterkeys, "Return an iterator over the keys of a dictionary.")
 _add_doc(itervalues, "Return an iterator over the values of a dictionary.")
-_add_doc(iteritems,
-         "Return an iterator over the (key, value) pairs of a dictionary.")
-_add_doc(iterlists,
-         "Return an iterator over the (key, [values]) pairs of a dictionary.")
+_add_doc(iteritems, "Return an iterator over the (key, value) pairs of a dictionary.")
+_add_doc(
+    iterlists, "Return an iterator over the (key, [values]) pairs of a dictionary."
+)
 
 
 if PY3:
+
     def b(s):
         return s.encode("latin-1")
 
     def u(s):
         return s
+
     unichr = chr
     import struct
+
     int2byte = struct.Struct(">B").pack
     del struct
     byte2int = operator.itemgetter(0)
     indexbytes = operator.getitem
     iterbytes = iter
     import io
+
     StringIO = io.StringIO
     BytesIO = io.BytesIO
     _assertCountEqual = "assertCountEqual"
     if sys.version_info[1] <= 1:
         _assertRaisesRegex = "assertRaisesRegexp"
         _assertRegex = "assertRegexpMatches"
     else:
         _assertRaisesRegex = "assertRaisesRegex"
         _assertRegex = "assertRegex"
 else:
+
     def b(s):
         return s
+
     # Workaround for standalone backslash
 
     def u(s):
-        return unicode(s.replace(r'\\', r'\\\\'), "unicode_escape")
+        return unicode(s.replace(r"\\", r"\\\\"), "unicode_escape")
+
     unichr = unichr
     int2byte = chr
 
     def byte2int(bs):
         return ord(bs[0])
 
     def indexbytes(buf, i):
         return ord(buf[i])
+
     iterbytes = functools.partial(itertools.imap, ord)
     import StringIO
+
     StringIO = BytesIO = StringIO.StringIO
     _assertCountEqual = "assertItemsEqual"
     _assertRaisesRegex = "assertRaisesRegexp"
     _assertRegex = "assertRegexpMatches"
 _add_doc(b, """Byte literal""")
 _add_doc(u, """Text literal""")
 
@@ -682,66 +719,78 @@
         if value is None:
             value = tp()
         if value.__traceback__ is not tb:
             raise value.with_traceback(tb)
         raise value
 
 else:
+
     def exec_(_code_, _globs_=None, _locs_=None):
         """Execute code in a namespace."""
         if _globs_ is None:
             frame = sys._getframe(1)
             _globs_ = frame.f_globals
             if _locs_ is None:
                 _locs_ = frame.f_locals
             del frame
         elif _locs_ is None:
             _locs_ = _globs_
         exec("""exec _code_ in _globs_, _locs_""")
 
-    exec_("""def reraise(tp, value, tb=None):
+    exec_(
+        """def reraise(tp, value, tb=None):
     raise tp, value, tb
-""")
+"""
+    )
 
 
 if sys.version_info[:2] == (3, 2):
-    exec_("""def raise_from(value, from_value):
+    exec_(
+        """def raise_from(value, from_value):
     if from_value is None:
         raise value
     raise value from from_value
-""")
+"""
+    )
 elif sys.version_info[:2] > (3, 2):
-    exec_("""def raise_from(value, from_value):
+    exec_(
+        """def raise_from(value, from_value):
     raise value from from_value
-""")
+"""
+    )
 else:
+
     def raise_from(value, from_value):
         raise value
 
 
 print_ = getattr(moves.builtins, "print", None)
 if print_ is None:
+
     def print_(*args, **kwargs):
         """The new-style print function for Python 2.4 and 2.5."""
         fp = kwargs.pop("file", sys.stdout)
         if fp is None:
             return
 
         def write(data):
             if not isinstance(data, basestring):
                 data = str(data)
             # If the file has an encoding, encode unicode with it.
-            if (isinstance(fp, file) and
-                    isinstance(data, unicode) and
-                    fp.encoding is not None):
+            if (
+                isinstance(fp, file)
+                and isinstance(data, unicode)
+                and fp.encoding is not None
+            ):
                 errors = getattr(fp, "errors", None)
                 if errors is None:
                     errors = "strict"
                 data = data.encode(fp.encoding, errors)
             fp.write(data)
+
         want_unicode = False
         sep = kwargs.pop("sep", None)
         if sep is not None:
             if isinstance(sep, unicode):
                 want_unicode = True
             elif not isinstance(sep, str):
                 raise TypeError("sep must be None or a string")
@@ -769,81 +818,94 @@
         if end is None:
             end = newline
         for i, arg in enumerate(args):
             if i:
                 write(sep)
             write(arg)
         write(end)
+
+
 if sys.version_info[:2] < (3, 3):
     _print = print_
 
     def print_(*args, **kwargs):
         fp = kwargs.get("file", sys.stdout)
         flush = kwargs.pop("flush", False)
         _print(*args, **kwargs)
         if flush and fp is not None:
             fp.flush()
 
+
 _add_doc(reraise, """Reraise an exception.""")
 
 if sys.version_info[0:2] < (3, 4):
-    def wraps(wrapped, assigned=functools.WRAPPER_ASSIGNMENTS,
-              updated=functools.WRAPPER_UPDATES):
+
+    def wraps(
+        wrapped,
+        assigned=functools.WRAPPER_ASSIGNMENTS,
+        updated=functools.WRAPPER_UPDATES,
+    ):
         def wrapper(f):
             f = functools.wraps(wrapped, assigned, updated)(f)
             f.__wrapped__ = wrapped
             return f
+
         return wrapper
+
 else:
     wraps = functools.wraps
 
 
 def with_metaclass(meta, *bases):
     """Create a base class with a metaclass."""
+
     # This requires a bit of explanation: the basic idea is to make a dummy
     # metaclass for one level of class instantiation that replaces itself with
     # the actual metaclass.
     class metaclass(meta):
-
         def __new__(cls, name, this_bases, d):
             return meta(name, bases, d)
-    return type.__new__(metaclass, 'temporary_class', (), {})
+
+    return type.__new__(metaclass, "temporary_class", (), {})
 
 
 def add_metaclass(metaclass):
     """Class decorator for creating a class with a metaclass."""
+
     def wrapper(cls):
         orig_vars = cls.__dict__.copy()
-        slots = orig_vars.get('__slots__')
+        slots = orig_vars.get("__slots__")
         if slots is not None:
             if isinstance(slots, str):
                 slots = [slots]
             for slots_var in slots:
                 orig_vars.pop(slots_var)
-        orig_vars.pop('__dict__', None)
-        orig_vars.pop('__weakref__', None)
+        orig_vars.pop("__dict__", None)
+        orig_vars.pop("__weakref__", None)
         return metaclass(cls.__name__, cls.__bases__, orig_vars)
+
     return wrapper
 
 
 def python_2_unicode_compatible(klass):
     """
     A decorator that defines __unicode__ and __str__ methods under Python 2.
     Under Python 3 it does nothing.
 
     To support Python 2 and 3 with a single code base, define a __str__ method
     returning text and apply this decorator to the class.
     """
     if PY2:
-        if '__str__' not in klass.__dict__:
-            raise ValueError("@python_2_unicode_compatible cannot be applied "
-                             "to %s because it doesn't define __str__()." %
-                             klass.__name__)
+        if "__str__" not in klass.__dict__:
+            raise ValueError(
+                "@python_2_unicode_compatible cannot be applied "
+                "to %s because it doesn't define __str__()." % klass.__name__
+            )
         klass.__unicode__ = klass.__str__
-        klass.__str__ = lambda self: self.__unicode__().encode('utf-8')
+        klass.__str__ = lambda self: self.__unicode__().encode("utf-8")
     return klass
 
 
 # Complete the moves implementation.
 # This code is at the end of this module to speed up module loading.
 # Turn this module into a package.
 __path__ = []  # required for PEP 302 and PEP 451
@@ -855,14 +917,16 @@
 # this for some reason.)
 if sys.meta_path:
     for i, importer in enumerate(sys.meta_path):
         # Here's some real nastiness: Another "instance" of the six module might
         # be floating around. Therefore, we can't use isinstance() to check for
         # the six meta path importer, since the other six instance will have
         # inserted an importer with different class.
-        if (type(importer).__name__ == "_SixMetaPathImporter" and
-                importer.name == __name__):
+        if (
+            type(importer).__name__ == "_SixMetaPathImporter"
+            and importer.name == __name__
+        ):
             del sys.meta_path[i]
             break
     del i, importer
 # Finally, add the importer to the meta path import hook.
 sys.meta_path.append(_importer)
```

### Comparing `utx-1.3.3/utx.egg-info/PKG-INFO` & `utx-1.3.4/utx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utx
-Version: 1.3.3
+Version: 1.3.4
 Summary: UTX will help you write ui automated tests more easily!
 Home-page: https://github.com/openutx
 Author: lijiawei
 Author-email: jiawei.li2@qq.com
 License: Apache License 2.0
 Keywords: utx,airtest,pytest,selenium,ui,tools
 Platform: any
```

### Comparing `utx-1.3.3/utx.egg-info/SOURCES.txt` & `utx-1.3.4/utx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

