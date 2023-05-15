# Comparing `tmp/pglive-0.6.3.tar.gz` & `tmp/pglive-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pglive-0.6.3.tar", max compression
+gzip compressed data, was "pglive-0.6.4.tar", max compression
```

## Comparing `pglive-0.6.3.tar` & `pglive-0.6.4.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rwxr-xr-x   0        0        0     1067 2022-07-09 17:29:11.350000 pglive-0.6.3/LICENSE
--rw-r--r--   0        0        0     4832 2023-04-14 17:18:13.360265 pglive-0.6.3/README.md
--rw-r--r--   0        0        0        0 2022-08-12 14:14:02.223971 pglive-0.6.3/pglive/__init__.py
--rw-r--r--   0        0        0     2631 2023-03-25 07:41:59.485596 pglive-0.6.3/pglive/examples_pyqt5/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-14 16:57:54.239777 pglive-0.6.3/pglive/examples_pyqt5/all_plot_types.py
--rw-r--r--   0        0        0     1992 2023-04-14 16:58:27.839960 pglive-0.6.3/pglive/examples_pyqt5/axis.py
--rw-r--r--   0        0        0      685 2023-04-14 16:59:03.904220 pglive-0.6.3/pglive/examples_pyqt5/candlestick_plot.py
--rw-r--r--   0        0        0     1416 2023-04-14 16:59:03.892220 pglive-0.6.3/pglive/examples_pyqt5/categorized_bar_plot.py
--rw-r--r--   0        0        0     2957 2023-04-14 17:00:55.641092 pglive-0.6.3/pglive/examples_pyqt5/crop_offset_to_data.py
--rw-r--r--   0        0        0     2650 2023-04-14 17:01:32.765324 pglive-0.6.3/pglive/examples_pyqt5/crosshair.py
--rw-r--r--   0        0        0        0 2022-08-12 14:14:02.227972 pglive-0.6.3/pglive/examples_pyqt5/designer_example/__init__.py
--rw-r--r--   0        0        0      813 2022-08-12 14:14:02.227972 pglive-0.6.3/pglive/examples_pyqt5/designer_example/main_example.py
--rw-r--r--   0        0        0     2203 2022-08-12 14:14:02.227972 pglive-0.6.3/pglive/examples_pyqt5/designer_example/win_template.py
--rw-r--r--   0        0        0     1489 2022-08-12 14:14:02.227972 pglive-0.6.3/pglive/examples_pyqt5/designer_example/win_template.ui
--rw-r--r--   0        0        0      610 2023-04-14 17:01:53.765447 pglive-0.6.3/pglive/examples_pyqt5/horizontal_bar_plot.py
--rw-r--r--   0        0        0     2498 2023-04-14 17:02:17.081578 pglive-0.6.3/pglive/examples_pyqt5/leading_line.py
--rw-r--r--   0        0        0      630 2023-04-14 17:02:55.533785 pglive-0.6.3/pglive/examples_pyqt5/line_plot.py
--rw-r--r--   0        0        0     6533 2023-04-14 17:02:55.545785 pglive-0.6.3/pglive/examples_pyqt5/live_plot_range.py
--rw-r--r--   0        0        0     2061 2023-04-14 17:03:31.953971 pglive-0.6.3/pglive/examples_pyqt5/one_plot_multiple_plot_rates.py
--rw-r--r--   0        0        0     1767 2023-04-14 17:11:38.123162 pglive-0.6.3/pglive/examples_pyqt5/pause_resume.py
--rw-r--r--   0        0        0      999 2023-04-14 17:04:45.710330 pglive-0.6.3/pglive/examples_pyqt5/plot_rate.py
--rw-r--r--   0        0        0      642 2023-04-14 17:05:01.810406 pglive-0.6.3/pglive/examples_pyqt5/scatter_plot.py
--rw-r--r--   0        0        0     1248 2023-04-14 17:05:38.346576 pglive-0.6.3/pglive/examples_pyqt5/update_rate.py
--rw-r--r--   0        0        0      683 2023-04-14 17:05:38.358576 pglive-0.6.3/pglive/examples_pyqt5/vertical_bar_plot.py
--rw-r--r--   0        0        0     1143 2023-04-14 17:12:56.975330 pglive-0.6.3/pglive/examples_pyqt5/vertical_bar_plot_color.py
--rw-r--r--   0        0        0     2631 2022-11-24 13:54:15.682940 pglive-0.6.3/pglive/examples_pyqt6/__init__.py
--rw-r--r--   0        0        0     1091 2023-04-14 17:17:10.096057 pglive-0.6.3/pglive/examples_pyqt6/all_plot_types.py
--rw-r--r--   0        0        0     1992 2023-04-14 17:08:29.834979 pglive-0.6.3/pglive/examples_pyqt6/axis.py
--rw-r--r--   0        0        0      685 2023-04-14 17:08:48.934979 pglive-0.6.3/pglive/examples_pyqt6/candlestick_plot.py
--rw-r--r--   0        0        0     1416 2023-04-14 17:09:04.442982 pglive-0.6.3/pglive/examples_pyqt6/categorized_bar_plot.py
--rw-r--r--   0        0        0     2955 2023-04-14 17:21:40.620984 pglive-0.6.3/pglive/examples_pyqt6/crop_offset_to_data.py
--rw-r--r--   0        0        0     2650 2023-04-14 17:09:54.127013 pglive-0.6.3/pglive/examples_pyqt6/crosshair.py
--rw-r--r--   0        0        0        0 2022-08-12 14:14:02.227972 pglive-0.6.3/pglive/examples_pyqt6/designer_example/__init__.py
--rw-r--r--   0        0        0      813 2022-11-24 15:39:08.017064 pglive-0.6.3/pglive/examples_pyqt6/designer_example/main_example.py
--rw-r--r--   0        0        0     2191 2022-11-24 15:39:08.017064 pglive-0.6.3/pglive/examples_pyqt6/designer_example/win_template.py
--rw-r--r--   0        0        0     1489 2022-11-24 15:39:08.021064 pglive-0.6.3/pglive/examples_pyqt6/designer_example/win_template.ui
--rw-r--r--   0        0        0      610 2023-04-14 17:10:09.555029 pglive-0.6.3/pglive/examples_pyqt6/horizontal_bar_plot.py
--rw-r--r--   0        0        0     2498 2023-04-14 17:10:33.699058 pglive-0.6.3/pglive/examples_pyqt6/leading_line.py
--rw-r--r--   0        0        0      630 2023-04-14 17:10:50.079081 pglive-0.6.3/pglive/examples_pyqt6/line_plot.py
--rw-r--r--   0        0        0     6546 2023-04-14 17:11:03.675102 pglive-0.6.3/pglive/examples_pyqt6/live_plot_range.py
--rw-r--r--   0        0        0     2061 2023-04-14 17:11:23.751136 pglive-0.6.3/pglive/examples_pyqt6/one_plot_multiple_plot_rates.py
--rw-r--r--   0        0        0     1767 2023-04-14 17:11:41.735169 pglive-0.6.3/pglive/examples_pyqt6/pause_resume.py
--rw-r--r--   0        0        0     1002 2023-04-14 17:11:55.499195 pglive-0.6.3/pglive/examples_pyqt6/plot_rate.py
--rw-r--r--   0        0        0      642 2023-04-14 17:12:12.039229 pglive-0.6.3/pglive/examples_pyqt6/scatter_plot.py
--rw-r--r--   0        0        0     1249 2023-04-14 17:12:23.487254 pglive-0.6.3/pglive/examples_pyqt6/update_rate.py
--rw-r--r--   0        0        0      683 2023-04-14 17:12:38.967288 pglive-0.6.3/pglive/examples_pyqt6/vertical_bar_plot.py
--rw-r--r--   0        0        0     1143 2023-04-14 17:12:56.979330 pglive-0.6.3/pglive/examples_pyqt6/vertical_bar_plot_color.py
--rw-r--r--   0        0        0     2635 2022-10-05 10:08:23.688683 pglive-0.6.3/pglive/examples_pyside2/__init__.py
--rw-r--r--   0        0        0     1090 2023-04-14 17:17:00.544026 pglive-0.6.3/pglive/examples_pyside2/all_plot_types.py
--rw-r--r--   0        0        0     1995 2023-04-14 17:18:13.344265 pglive-0.6.3/pglive/examples_pyside2/axis.py
--rw-r--r--   0        0        0      688 2023-04-14 17:20:19.060696 pglive-0.6.3/pglive/examples_pyside2/candlestick_plot.py
--rw-r--r--   0        0        0     1419 2023-04-14 17:21:00.912843 pglive-0.6.3/pglive/examples_pyside2/categorized_bar_plot.py
--rw-r--r--   0        0        0     2959 2023-04-14 17:21:40.908985 pglive-0.6.3/pglive/examples_pyside2/crop_offset_to_data.py
--rw-r--r--   0        0        0     2657 2023-04-14 17:21:55.837039 pglive-0.6.3/pglive/examples_pyside2/crosshair.py
--rw-r--r--   0        0        0      613 2023-04-14 17:22:09.325087 pglive-0.6.3/pglive/examples_pyside2/horizontal_bar_plot.py
--rw-r--r--   0        0        0     2501 2023-04-14 17:22:31.713167 pglive-0.6.3/pglive/examples_pyside2/leading_line.py
--rw-r--r--   0        0        0      633 2023-04-14 17:18:13.360265 pglive-0.6.3/pglive/examples_pyside2/line_plot.py
--rw-r--r--   0        0        0     6615 2023-04-14 17:22:51.313238 pglive-0.6.3/pglive/examples_pyside2/live_plot_range.py
--rw-r--r--   0        0        0     2064 2023-04-14 17:23:07.897298 pglive-0.6.3/pglive/examples_pyside2/one_plot_multiple_plot_rates.py
--rw-r--r--   0        0        0     1772 2023-04-14 17:23:28.477373 pglive-0.6.3/pglive/examples_pyside2/pause_resume.py
--rw-r--r--   0        0        0     1043 2023-04-14 17:23:43.229426 pglive-0.6.3/pglive/examples_pyside2/plot_rate.py
--rw-r--r--   0        0        0      645 2023-04-14 17:23:56.865476 pglive-0.6.3/pglive/examples_pyside2/scatter_plot.py
--rw-r--r--   0        0        0     1251 2023-04-14 17:24:11.373529 pglive-0.6.3/pglive/examples_pyside2/update_rate.py
--rw-r--r--   0        0        0      686 2023-04-14 17:24:22.181568 pglive-0.6.3/pglive/examples_pyside2/vertical_bar_plot.py
--rw-r--r--   0        0        0     1146 2023-04-14 17:24:22.181568 pglive-0.6.3/pglive/examples_pyside2/vertical_bar_plot_color.py
--rw-r--r--   0        0        0     2635 2022-10-05 10:08:23.684683 pglive-0.6.3/pglive/examples_pyside6/__init__.py
--rw-r--r--   0        0        0     1089 2023-04-14 17:17:00.536026 pglive-0.6.3/pglive/examples_pyside6/all_plot_types.py
--rw-r--r--   0        0        0     1994 2023-04-14 17:18:13.356265 pglive-0.6.3/pglive/examples_pyside6/axis.py
--rw-r--r--   0        0        0      687 2023-04-14 17:20:23.324711 pglive-0.6.3/pglive/examples_pyside6/candlestick_plot.py
--rw-r--r--   0        0        0     1418 2023-04-14 17:21:00.920843 pglive-0.6.3/pglive/examples_pyside6/categorized_bar_plot.py
--rw-r--r--   0        0        0     2958 2023-04-14 17:21:40.916985 pglive-0.6.3/pglive/examples_pyside6/crop_offset_to_data.py
--rw-r--r--   0        0        0     2656 2023-04-14 17:21:55.825039 pglive-0.6.3/pglive/examples_pyside6/crosshair.py
--rw-r--r--   0        0        0      612 2023-04-14 17:22:09.329087 pglive-0.6.3/pglive/examples_pyside6/horizontal_bar_plot.py
--rw-r--r--   0        0        0     2500 2023-04-14 17:22:31.721167 pglive-0.6.3/pglive/examples_pyside6/leading_line.py
--rw-r--r--   0        0        0      632 2023-04-14 17:18:13.356265 pglive-0.6.3/pglive/examples_pyside6/line_plot.py
--rw-r--r--   0        0        0     6614 2023-04-14 17:22:51.301238 pglive-0.6.3/pglive/examples_pyside6/live_plot_range.py
--rw-r--r--   0        0        0     2063 2023-04-14 17:23:07.897298 pglive-0.6.3/pglive/examples_pyside6/one_plot_multiple_plot_rates.py
--rw-r--r--   0        0        0     1771 2023-04-14 17:23:28.485373 pglive-0.6.3/pglive/examples_pyside6/pause_resume.py
--rw-r--r--   0        0        0      999 2023-04-14 17:23:43.217426 pglive-0.6.3/pglive/examples_pyside6/plot_rate.py
--rw-r--r--   0        0        0      644 2023-04-14 17:23:56.857476 pglive-0.6.3/pglive/examples_pyside6/scatter_plot.py
--rw-r--r--   0        0        0     1250 2023-04-14 17:24:11.361528 pglive-0.6.3/pglive/examples_pyside6/update_rate.py
--rw-r--r--   0        0        0      685 2023-04-14 17:24:22.177568 pglive-0.6.3/pglive/examples_pyside6/vertical_bar_plot.py
--rw-r--r--   0        0        0     1145 2023-04-14 17:24:22.169568 pglive-0.6.3/pglive/examples_pyside6/vertical_bar_plot_color.py
--rw-r--r--   0        0        0      967 2022-10-05 06:34:53.511344 pglive-0.6.3/pglive/kwargs.py
--rw-r--r--   0        0        0        0 2022-08-12 14:14:02.235972 pglive-0.6.3/pglive/sources/__init__.py
--rw-r--r--   0        0        0     6859 2023-03-10 13:02:08.227569 pglive-0.6.3/pglive/sources/data_connector.py
--rw-r--r--   0        0        0     4694 2023-02-22 17:37:04.246169 pglive-0.6.3/pglive/sources/live_axis.py
--rw-r--r--   0        0        0     7701 2023-03-10 12:02:20.144602 pglive-0.6.3/pglive/sources/live_axis_range.py
--rw-r--r--   0        0        0     3256 2023-04-14 16:55:56.062555 pglive-0.6.3/pglive/sources/live_candleStickPlot.py
--rw-r--r--   0        0        0     4510 2023-02-22 17:37:04.246169 pglive-0.6.3/pglive/sources/live_categorized_bar_plot.py
--rw-r--r--   0        0        0     5883 2023-02-22 17:37:04.246169 pglive-0.6.3/pglive/sources/live_mixins.py
--rw-r--r--   0        0        0     5274 2023-04-14 17:54:49.990162 pglive-0.6.3/pglive/sources/live_plot.py
--rw-r--r--   0        0        0    11010 2023-04-14 17:48:11.264140 pglive-0.6.3/pglive/sources/live_plot_widget.py
--rw-r--r--   0        0        0     1599 2023-02-25 08:15:41.220788 pglive-0.6.3/pglive/sources/utils.py
--rw-r--r--   0        0        0      973 2023-04-19 05:43:29.658908 pglive-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     5854 1970-01-01 00:00:00.000000 pglive-0.6.3/setup.py
--rw-r--r--   0        0        0     5808 1970-01-01 00:00:00.000000 pglive-0.6.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1067 2022-07-09 17:29:11.350000 pglive-0.6.4/LICENSE
+-rw-r--r--   0        0        0     4832 2023-04-14 17:18:13.360265 pglive-0.6.4/README.md
+-rw-r--r--   0        0        0        0 2022-08-12 14:14:02.223971 pglive-0.6.4/pglive/__init__.py
+-rw-r--r--   0        0        0     2631 2023-03-25 07:41:59.485596 pglive-0.6.4/pglive/examples_pyqt5/__init__.py
+-rw-r--r--   0        0        0     1093 2023-04-14 16:57:54.239777 pglive-0.6.4/pglive/examples_pyqt5/all_plot_types.py
+-rw-r--r--   0        0        0     1992 2023-04-14 16:58:27.839960 pglive-0.6.4/pglive/examples_pyqt5/axis.py
+-rw-r--r--   0        0        0      685 2023-04-14 16:59:03.904220 pglive-0.6.4/pglive/examples_pyqt5/candlestick_plot.py
+-rw-r--r--   0        0        0     1416 2023-04-14 16:59:03.892220 pglive-0.6.4/pglive/examples_pyqt5/categorized_bar_plot.py
+-rw-r--r--   0        0        0     2957 2023-04-14 17:00:55.641092 pglive-0.6.4/pglive/examples_pyqt5/crop_offset_to_data.py
+-rw-r--r--   0        0        0     2650 2023-04-14 17:01:32.765324 pglive-0.6.4/pglive/examples_pyqt5/crosshair.py
+-rw-r--r--   0        0        0        0 2022-08-12 14:14:02.227972 pglive-0.6.4/pglive/examples_pyqt5/designer_example/__init__.py
+-rw-r--r--   0        0        0      813 2022-08-12 14:14:02.227972 pglive-0.6.4/pglive/examples_pyqt5/designer_example/main_example.py
+-rw-r--r--   0        0        0     2203 2022-08-12 14:14:02.227972 pglive-0.6.4/pglive/examples_pyqt5/designer_example/win_template.py
+-rw-r--r--   0        0        0     1489 2022-08-12 14:14:02.227972 pglive-0.6.4/pglive/examples_pyqt5/designer_example/win_template.ui
+-rw-r--r--   0        0        0      610 2023-04-14 17:01:53.765447 pglive-0.6.4/pglive/examples_pyqt5/horizontal_bar_plot.py
+-rw-r--r--   0        0        0     2498 2023-04-14 17:02:17.081578 pglive-0.6.4/pglive/examples_pyqt5/leading_line.py
+-rw-r--r--   0        0        0      630 2023-04-14 17:02:55.533785 pglive-0.6.4/pglive/examples_pyqt5/line_plot.py
+-rw-r--r--   0        0        0     6533 2023-04-14 17:02:55.545785 pglive-0.6.4/pglive/examples_pyqt5/live_plot_range.py
+-rw-r--r--   0        0        0     2061 2023-04-14 17:03:31.953971 pglive-0.6.4/pglive/examples_pyqt5/one_plot_multiple_plot_rates.py
+-rw-r--r--   0        0        0     1767 2023-04-14 17:11:38.123162 pglive-0.6.4/pglive/examples_pyqt5/pause_resume.py
+-rw-r--r--   0        0        0      999 2023-04-14 17:04:45.710330 pglive-0.6.4/pglive/examples_pyqt5/plot_rate.py
+-rw-r--r--   0        0        0      642 2023-04-14 17:05:01.810406 pglive-0.6.4/pglive/examples_pyqt5/scatter_plot.py
+-rw-r--r--   0        0        0     1248 2023-04-14 17:05:38.346576 pglive-0.6.4/pglive/examples_pyqt5/update_rate.py
+-rw-r--r--   0        0        0      683 2023-04-14 17:05:38.358576 pglive-0.6.4/pglive/examples_pyqt5/vertical_bar_plot.py
+-rw-r--r--   0        0        0     1143 2023-04-14 17:12:56.975330 pglive-0.6.4/pglive/examples_pyqt5/vertical_bar_plot_color.py
+-rw-r--r--   0        0        0     2631 2023-05-15 08:42:42.442534 pglive-0.6.4/pglive/examples_pyqt6/__init__.py
+-rw-r--r--   0        0        0     1091 2023-04-14 17:17:10.096057 pglive-0.6.4/pglive/examples_pyqt6/all_plot_types.py
+-rw-r--r--   0        0        0     1992 2023-04-14 17:08:29.834979 pglive-0.6.4/pglive/examples_pyqt6/axis.py
+-rw-r--r--   0        0        0      685 2023-04-14 17:08:48.934979 pglive-0.6.4/pglive/examples_pyqt6/candlestick_plot.py
+-rw-r--r--   0        0        0     1416 2023-04-14 17:09:04.442982 pglive-0.6.4/pglive/examples_pyqt6/categorized_bar_plot.py
+-rw-r--r--   0        0        0     2955 2023-05-15 08:52:40.650072 pglive-0.6.4/pglive/examples_pyqt6/crop_offset_to_data.py
+-rw-r--r--   0        0        0     2650 2023-04-14 17:09:54.127013 pglive-0.6.4/pglive/examples_pyqt6/crosshair.py
+-rw-r--r--   0        0        0        0 2022-08-12 14:14:02.227972 pglive-0.6.4/pglive/examples_pyqt6/designer_example/__init__.py
+-rw-r--r--   0        0        0      813 2022-11-24 15:39:08.017064 pglive-0.6.4/pglive/examples_pyqt6/designer_example/main_example.py
+-rw-r--r--   0        0        0     2191 2022-11-24 15:39:08.017064 pglive-0.6.4/pglive/examples_pyqt6/designer_example/win_template.py
+-rw-r--r--   0        0        0     1489 2022-11-24 15:39:08.021064 pglive-0.6.4/pglive/examples_pyqt6/designer_example/win_template.ui
+-rw-r--r--   0        0        0      610 2023-04-14 17:10:09.555029 pglive-0.6.4/pglive/examples_pyqt6/horizontal_bar_plot.py
+-rw-r--r--   0        0        0     2498 2023-04-14 17:10:33.699058 pglive-0.6.4/pglive/examples_pyqt6/leading_line.py
+-rw-r--r--   0        0        0      630 2023-04-14 17:10:50.079081 pglive-0.6.4/pglive/examples_pyqt6/line_plot.py
+-rw-r--r--   0        0        0     6546 2023-04-14 17:11:03.675102 pglive-0.6.4/pglive/examples_pyqt6/live_plot_range.py
+-rw-r--r--   0        0        0     2061 2023-04-14 17:11:23.751136 pglive-0.6.4/pglive/examples_pyqt6/one_plot_multiple_plot_rates.py
+-rw-r--r--   0        0        0     1767 2023-04-14 17:11:41.735169 pglive-0.6.4/pglive/examples_pyqt6/pause_resume.py
+-rw-r--r--   0        0        0     1002 2023-04-14 17:11:55.499195 pglive-0.6.4/pglive/examples_pyqt6/plot_rate.py
+-rw-r--r--   0        0        0      642 2023-04-14 17:12:12.039229 pglive-0.6.4/pglive/examples_pyqt6/scatter_plot.py
+-rw-r--r--   0        0        0     1249 2023-04-14 17:12:23.487254 pglive-0.6.4/pglive/examples_pyqt6/update_rate.py
+-rw-r--r--   0        0        0      683 2023-04-14 17:12:38.967288 pglive-0.6.4/pglive/examples_pyqt6/vertical_bar_plot.py
+-rw-r--r--   0        0        0     1143 2023-04-14 17:12:56.979330 pglive-0.6.4/pglive/examples_pyqt6/vertical_bar_plot_color.py
+-rw-r--r--   0        0        0     2635 2022-10-05 10:08:23.688683 pglive-0.6.4/pglive/examples_pyside2/__init__.py
+-rw-r--r--   0        0        0     1090 2023-04-14 17:17:00.544026 pglive-0.6.4/pglive/examples_pyside2/all_plot_types.py
+-rw-r--r--   0        0        0     1995 2023-04-14 17:18:13.344265 pglive-0.6.4/pglive/examples_pyside2/axis.py
+-rw-r--r--   0        0        0      688 2023-04-14 17:20:19.060696 pglive-0.6.4/pglive/examples_pyside2/candlestick_plot.py
+-rw-r--r--   0        0        0     1419 2023-04-14 17:21:00.912843 pglive-0.6.4/pglive/examples_pyside2/categorized_bar_plot.py
+-rw-r--r--   0        0        0     2959 2023-04-14 17:21:40.908985 pglive-0.6.4/pglive/examples_pyside2/crop_offset_to_data.py
+-rw-r--r--   0        0        0     2657 2023-04-14 17:21:55.837039 pglive-0.6.4/pglive/examples_pyside2/crosshair.py
+-rw-r--r--   0        0        0      613 2023-04-14 17:22:09.325087 pglive-0.6.4/pglive/examples_pyside2/horizontal_bar_plot.py
+-rw-r--r--   0        0        0     2501 2023-04-14 17:22:31.713167 pglive-0.6.4/pglive/examples_pyside2/leading_line.py
+-rw-r--r--   0        0        0      633 2023-04-14 17:18:13.360265 pglive-0.6.4/pglive/examples_pyside2/line_plot.py
+-rw-r--r--   0        0        0     6615 2023-04-14 17:22:51.313238 pglive-0.6.4/pglive/examples_pyside2/live_plot_range.py
+-rw-r--r--   0        0        0     2064 2023-04-14 17:23:07.897298 pglive-0.6.4/pglive/examples_pyside2/one_plot_multiple_plot_rates.py
+-rw-r--r--   0        0        0     1772 2023-04-14 17:23:28.477373 pglive-0.6.4/pglive/examples_pyside2/pause_resume.py
+-rw-r--r--   0        0        0     1043 2023-04-14 17:23:43.229426 pglive-0.6.4/pglive/examples_pyside2/plot_rate.py
+-rw-r--r--   0        0        0      645 2023-04-14 17:23:56.865476 pglive-0.6.4/pglive/examples_pyside2/scatter_plot.py
+-rw-r--r--   0        0        0     1251 2023-04-14 17:24:11.373529 pglive-0.6.4/pglive/examples_pyside2/update_rate.py
+-rw-r--r--   0        0        0      686 2023-04-14 17:24:22.181568 pglive-0.6.4/pglive/examples_pyside2/vertical_bar_plot.py
+-rw-r--r--   0        0        0     1146 2023-04-14 17:24:22.181568 pglive-0.6.4/pglive/examples_pyside2/vertical_bar_plot_color.py
+-rw-r--r--   0        0        0     2635 2022-10-05 10:08:23.684683 pglive-0.6.4/pglive/examples_pyside6/__init__.py
+-rw-r--r--   0        0        0     1089 2023-04-14 17:17:00.536026 pglive-0.6.4/pglive/examples_pyside6/all_plot_types.py
+-rw-r--r--   0        0        0     1994 2023-04-14 17:18:13.356265 pglive-0.6.4/pglive/examples_pyside6/axis.py
+-rw-r--r--   0        0        0      687 2023-04-14 17:20:23.324711 pglive-0.6.4/pglive/examples_pyside6/candlestick_plot.py
+-rw-r--r--   0        0        0     1418 2023-04-14 17:21:00.920843 pglive-0.6.4/pglive/examples_pyside6/categorized_bar_plot.py
+-rw-r--r--   0        0        0     2958 2023-04-14 17:21:40.916985 pglive-0.6.4/pglive/examples_pyside6/crop_offset_to_data.py
+-rw-r--r--   0        0        0     2656 2023-04-14 17:21:55.825039 pglive-0.6.4/pglive/examples_pyside6/crosshair.py
+-rw-r--r--   0        0        0      612 2023-04-14 17:22:09.329087 pglive-0.6.4/pglive/examples_pyside6/horizontal_bar_plot.py
+-rw-r--r--   0        0        0     2500 2023-04-14 17:22:31.721167 pglive-0.6.4/pglive/examples_pyside6/leading_line.py
+-rw-r--r--   0        0        0      632 2023-04-14 17:18:13.356265 pglive-0.6.4/pglive/examples_pyside6/line_plot.py
+-rw-r--r--   0        0        0     6614 2023-04-14 17:22:51.301238 pglive-0.6.4/pglive/examples_pyside6/live_plot_range.py
+-rw-r--r--   0        0        0     2063 2023-04-14 17:23:07.897298 pglive-0.6.4/pglive/examples_pyside6/one_plot_multiple_plot_rates.py
+-rw-r--r--   0        0        0     1771 2023-04-14 17:23:28.485373 pglive-0.6.4/pglive/examples_pyside6/pause_resume.py
+-rw-r--r--   0        0        0      999 2023-04-14 17:23:43.217426 pglive-0.6.4/pglive/examples_pyside6/plot_rate.py
+-rw-r--r--   0        0        0      644 2023-04-14 17:23:56.857476 pglive-0.6.4/pglive/examples_pyside6/scatter_plot.py
+-rw-r--r--   0        0        0     1250 2023-04-14 17:24:11.361528 pglive-0.6.4/pglive/examples_pyside6/update_rate.py
+-rw-r--r--   0        0        0      685 2023-04-14 17:24:22.177568 pglive-0.6.4/pglive/examples_pyside6/vertical_bar_plot.py
+-rw-r--r--   0        0        0     1145 2023-04-14 17:24:22.169568 pglive-0.6.4/pglive/examples_pyside6/vertical_bar_plot_color.py
+-rw-r--r--   0        0        0      967 2022-10-05 06:34:53.511344 pglive-0.6.4/pglive/kwargs.py
+-rw-r--r--   0        0        0        0 2022-08-12 14:14:02.235972 pglive-0.6.4/pglive/sources/__init__.py
+-rw-r--r--   0        0        0     6859 2023-03-10 13:02:08.227569 pglive-0.6.4/pglive/sources/data_connector.py
+-rw-r--r--   0        0        0     4694 2023-02-22 17:37:04.246169 pglive-0.6.4/pglive/sources/live_axis.py
+-rw-r--r--   0        0        0     8419 2023-05-15 08:48:47.936700 pglive-0.6.4/pglive/sources/live_axis_range.py
+-rw-r--r--   0        0        0     3256 2023-04-14 16:55:56.062555 pglive-0.6.4/pglive/sources/live_candleStickPlot.py
+-rw-r--r--   0        0        0     4510 2023-02-22 17:37:04.246169 pglive-0.6.4/pglive/sources/live_categorized_bar_plot.py
+-rw-r--r--   0        0        0     5883 2023-02-22 17:37:04.246169 pglive-0.6.4/pglive/sources/live_mixins.py
+-rw-r--r--   0        0        0     5274 2023-04-14 17:54:49.990162 pglive-0.6.4/pglive/sources/live_plot.py
+-rw-r--r--   0        0        0    11010 2023-04-14 17:48:11.264140 pglive-0.6.4/pglive/sources/live_plot_widget.py
+-rw-r--r--   0        0        0     1599 2023-02-25 08:15:41.220788 pglive-0.6.4/pglive/sources/utils.py
+-rw-r--r--   0        0        0      973 2023-05-15 08:50:42.821378 pglive-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     5854 1970-01-01 00:00:00.000000 pglive-0.6.4/setup.py
+-rw-r--r--   0        0        0     5808 1970-01-01 00:00:00.000000 pglive-0.6.4/PKG-INFO
```

### Comparing `pglive-0.6.3/LICENSE` & `pglive-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/README.md` & `pglive-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/__init__.py` & `pglive-0.6.4/pglive/examples_pyqt5/__init__.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/all_plot_types.py` & `pglive-0.6.4/pglive/examples_pyqt5/all_plot_types.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/axis.py` & `pglive-0.6.4/pglive/examples_pyqt5/axis.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/candlestick_plot.py` & `pglive-0.6.4/pglive/examples_pyqt5/candlestick_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/categorized_bar_plot.py` & `pglive-0.6.4/pglive/examples_pyqt5/categorized_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/crop_offset_to_data.py` & `pglive-0.6.4/pglive/examples_pyqt5/crop_offset_to_data.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/crosshair.py` & `pglive-0.6.4/pglive/examples_pyqt5/crosshair.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/designer_example/main_example.py` & `pglive-0.6.4/pglive/examples_pyqt5/designer_example/main_example.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/designer_example/win_template.py` & `pglive-0.6.4/pglive/examples_pyqt5/designer_example/win_template.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/designer_example/win_template.ui` & `pglive-0.6.4/pglive/examples_pyqt5/designer_example/win_template.ui`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/horizontal_bar_plot.py` & `pglive-0.6.4/pglive/examples_pyqt5/horizontal_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/leading_line.py` & `pglive-0.6.4/pglive/examples_pyqt5/leading_line.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/line_plot.py` & `pglive-0.6.4/pglive/examples_pyqt5/line_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/live_plot_range.py` & `pglive-0.6.4/pglive/examples_pyqt5/live_plot_range.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/one_plot_multiple_plot_rates.py` & `pglive-0.6.4/pglive/examples_pyqt5/one_plot_multiple_plot_rates.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/pause_resume.py` & `pglive-0.6.4/pglive/examples_pyqt5/pause_resume.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/plot_rate.py` & `pglive-0.6.4/pglive/examples_pyqt5/plot_rate.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/scatter_plot.py` & `pglive-0.6.4/pglive/examples_pyqt5/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/update_rate.py` & `pglive-0.6.4/pglive/examples_pyqt5/update_rate.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/vertical_bar_plot.py` & `pglive-0.6.4/pglive/examples_pyqt5/vertical_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt5/vertical_bar_plot_color.py` & `pglive-0.6.4/pglive/examples_pyqt5/vertical_bar_plot_color.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/__init__.py` & `pglive-0.6.4/pglive/examples_pyqt6/__init__.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/all_plot_types.py` & `pglive-0.6.4/pglive/examples_pyqt6/all_plot_types.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/axis.py` & `pglive-0.6.4/pglive/examples_pyqt6/axis.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/candlestick_plot.py` & `pglive-0.6.4/pglive/examples_pyqt6/candlestick_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/categorized_bar_plot.py` & `pglive-0.6.4/pglive/examples_pyqt6/categorized_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/crop_offset_to_data.py` & `pglive-0.6.4/pglive/examples_pyqt6/crop_offset_to_data.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/crosshair.py` & `pglive-0.6.4/pglive/examples_pyqt6/crosshair.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/designer_example/main_example.py` & `pglive-0.6.4/pglive/examples_pyqt6/designer_example/main_example.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/designer_example/win_template.py` & `pglive-0.6.4/pglive/examples_pyqt6/designer_example/win_template.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/designer_example/win_template.ui` & `pglive-0.6.4/pglive/examples_pyqt6/designer_example/win_template.ui`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/horizontal_bar_plot.py` & `pglive-0.6.4/pglive/examples_pyqt6/horizontal_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/leading_line.py` & `pglive-0.6.4/pglive/examples_pyqt6/leading_line.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/line_plot.py` & `pglive-0.6.4/pglive/examples_pyqt6/line_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/live_plot_range.py` & `pglive-0.6.4/pglive/examples_pyqt6/live_plot_range.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/one_plot_multiple_plot_rates.py` & `pglive-0.6.4/pglive/examples_pyqt6/one_plot_multiple_plot_rates.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/pause_resume.py` & `pglive-0.6.4/pglive/examples_pyqt6/pause_resume.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/plot_rate.py` & `pglive-0.6.4/pglive/examples_pyqt6/plot_rate.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/scatter_plot.py` & `pglive-0.6.4/pglive/examples_pyqt6/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/update_rate.py` & `pglive-0.6.4/pglive/examples_pyqt6/update_rate.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/vertical_bar_plot.py` & `pglive-0.6.4/pglive/examples_pyqt6/vertical_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyqt6/vertical_bar_plot_color.py` & `pglive-0.6.4/pglive/examples_pyqt6/vertical_bar_plot_color.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/__init__.py` & `pglive-0.6.4/pglive/examples_pyside2/__init__.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/all_plot_types.py` & `pglive-0.6.4/pglive/examples_pyside2/all_plot_types.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/axis.py` & `pglive-0.6.4/pglive/examples_pyside2/axis.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/candlestick_plot.py` & `pglive-0.6.4/pglive/examples_pyside2/candlestick_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/categorized_bar_plot.py` & `pglive-0.6.4/pglive/examples_pyside2/categorized_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/crop_offset_to_data.py` & `pglive-0.6.4/pglive/examples_pyside2/crop_offset_to_data.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/crosshair.py` & `pglive-0.6.4/pglive/examples_pyside2/crosshair.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/horizontal_bar_plot.py` & `pglive-0.6.4/pglive/examples_pyside2/horizontal_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/leading_line.py` & `pglive-0.6.4/pglive/examples_pyside2/leading_line.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/line_plot.py` & `pglive-0.6.4/pglive/examples_pyside2/line_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/live_plot_range.py` & `pglive-0.6.4/pglive/examples_pyside2/live_plot_range.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/one_plot_multiple_plot_rates.py` & `pglive-0.6.4/pglive/examples_pyside2/one_plot_multiple_plot_rates.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/pause_resume.py` & `pglive-0.6.4/pglive/examples_pyside2/pause_resume.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/plot_rate.py` & `pglive-0.6.4/pglive/examples_pyside2/plot_rate.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/scatter_plot.py` & `pglive-0.6.4/pglive/examples_pyside2/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/update_rate.py` & `pglive-0.6.4/pglive/examples_pyside2/update_rate.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/vertical_bar_plot.py` & `pglive-0.6.4/pglive/examples_pyside2/vertical_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside2/vertical_bar_plot_color.py` & `pglive-0.6.4/pglive/examples_pyside2/vertical_bar_plot_color.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/__init__.py` & `pglive-0.6.4/pglive/examples_pyside6/__init__.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/all_plot_types.py` & `pglive-0.6.4/pglive/examples_pyside6/all_plot_types.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/axis.py` & `pglive-0.6.4/pglive/examples_pyside6/axis.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/candlestick_plot.py` & `pglive-0.6.4/pglive/examples_pyside6/candlestick_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/categorized_bar_plot.py` & `pglive-0.6.4/pglive/examples_pyside6/categorized_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/crop_offset_to_data.py` & `pglive-0.6.4/pglive/examples_pyside6/crop_offset_to_data.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/crosshair.py` & `pglive-0.6.4/pglive/examples_pyside6/crosshair.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/horizontal_bar_plot.py` & `pglive-0.6.4/pglive/examples_pyside6/horizontal_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/leading_line.py` & `pglive-0.6.4/pglive/examples_pyside6/leading_line.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/line_plot.py` & `pglive-0.6.4/pglive/examples_pyside6/line_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/live_plot_range.py` & `pglive-0.6.4/pglive/examples_pyside6/live_plot_range.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/one_plot_multiple_plot_rates.py` & `pglive-0.6.4/pglive/examples_pyside6/one_plot_multiple_plot_rates.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/pause_resume.py` & `pglive-0.6.4/pglive/examples_pyside6/pause_resume.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/plot_rate.py` & `pglive-0.6.4/pglive/examples_pyside6/plot_rate.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/scatter_plot.py` & `pglive-0.6.4/pglive/examples_pyside6/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/update_rate.py` & `pglive-0.6.4/pglive/examples_pyside6/update_rate.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/vertical_bar_plot.py` & `pglive-0.6.4/pglive/examples_pyside6/vertical_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/examples_pyside6/vertical_bar_plot_color.py` & `pglive-0.6.4/pglive/examples_pyside6/vertical_bar_plot_color.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/kwargs.py` & `pglive-0.6.4/pglive/kwargs.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/sources/data_connector.py` & `pglive-0.6.4/pglive/sources/data_connector.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/sources/live_axis.py` & `pglive-0.6.4/pglive/sources/live_axis.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/sources/live_axis_range.py` & `pglive-0.6.4/pglive/sources/live_axis_range.py`

 * *Files 8% similar despite different names*

```diff
@@ -130,18 +130,31 @@
         if self.final_y_range != final_range:
             self.final_y_range = final_range
         return self.final_y_range
 
     def _get_range(self, axis_range: Tuple[float, float], tick: int, offsets: Tuple[float, float]) -> Optional[
         List[float]]:
         if self.fixed_range is not None:
+            # Return fixed defined range
             return self.fixed_range
         elif self.roll_on_tick == 1:
-            return [axis_range[0], axis_range[1]]
+            # Rolling on every tick
+            if offsets[0] + offsets[1] == 0:
+                # Return full range if there are no offsets
+                return [axis_range[0], axis_range[1]]
+            elif tick > 0:
+                # Return range of width specified by offsets
+                range_width = (abs(axis_range[1] - axis_range[0])) / tick
+                return [axis_range[1] - range_width * offsets[0], (axis_range[1] + range_width) + (
+                        range_width * offsets[1])]
+            else:
+                # Just return axis ranges subtracted by offsets
+                return [axis_range[0] - offsets[0], axis_range[1] + offsets[1]]
         elif tick % self.roll_on_tick == 0 or tick < 2:
+            # Rolling when tick % self.roll_on_tick == 0
             range_width = abs(axis_range[1] - axis_range[0])
             if tick < 2:
                 range_width = range_width * (self.roll_on_tick - (tick + 1))
                 return [axis_range[1], axis_range[1] + range_width]
             else:
                 return [axis_range[1] - range_width * offsets[0], (axis_range[1] + range_width) + (
                         range_width * offsets[1])]
```

### Comparing `pglive-0.6.3/pglive/sources/live_candleStickPlot.py` & `pglive-0.6.4/pglive/sources/live_candleStickPlot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/sources/live_categorized_bar_plot.py` & `pglive-0.6.4/pglive/sources/live_categorized_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/sources/live_mixins.py` & `pglive-0.6.4/pglive/sources/live_mixins.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/sources/live_plot.py` & `pglive-0.6.4/pglive/sources/live_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/sources/live_plot_widget.py` & `pglive-0.6.4/pglive/sources/live_plot_widget.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pglive/sources/utils.py` & `pglive-0.6.4/pglive/sources/utils.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.3/pyproject.toml` & `pglive-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pglive"
-version = "0.6.3"
+version = "0.6.4"
 description = "Pyqtgraph live plot"
 authors = ["Martin Domaracky <domarm@comat.sk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/domarm-comat/pglive"
 repository = "https://github.com/domarm-comat/pglive"
 keywords = ["pyqtgraph", "realtime", "live", "plotting", "pyqt5", "pyqt6", "pyside2", "pyside6"]
```

### Comparing `pglive-0.6.3/setup.py` & `pglive-0.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.24.2,<2.0.0', 'pyqtgraph>=0.13.3,<0.14.0']
 
 setup_kwargs = {
     'name': 'pglive',
-    'version': '0.6.3',
+    'version': '0.6.4',
     'description': 'Pyqtgraph live plot',
     'long_description': '# Live pyqtgraph plot\n\nPglive package adds support for thread-safe live plotting to pyqtgraph.  \nIt supports PyQt5, PyQt6, PySide2 and PySide6.\n\n# Description #\n\nBy default, pyqtgraph doesn\'t support live plotting. Aim of this package is to provide easy implementation of Line,\nScatter and Bar Live plot. Every plot is connected with it\'s DataConnector, which sole purpose is to consume data points\nand manage data re-plotting. DataConnector interface provides Pause and Resume method, update rate and maximum number of\nplotted points. Each time data point is collected, call `DataConnector.cb_set_data`\nor `DataConnector.cb_append_data_point` callback. That\'s all You need to update plot with new data. Callbacks are Thread\nsafe, so it works nicely in applications with multiple data collection Threads.\n\n**Focus on data collection and leave plotting to pglive.**\n\nTo make firsts steps easy, package comes with many examples implemented in PyQt5 or PyQt6.\nSupport for PySide2 and PySide6 was added in version 0.3.0.\n\n# Code examples #\n\n```python\nimport sys\nfrom math import sin\nfrom threading import Thread\nfrom time import sleep\n\nfrom PyQt6.QtWidgets import QApplication\n\nfrom pglive.sources.data_connector import DataConnector\nfrom pglive.sources.live_plot import LiveLinePlot\nfrom pglive.sources.live_plot_widget import LivePlotWidget\n\n"""\nLine plot is displayed in this example.\n"""\napp = QApplication(sys.argv)\nrunning = True\n\nplot_widget = LivePlotWidget(title="Line Plot @ 100Hz")\nplot_curve = LiveLinePlot()\nplot_widget.addItem(plot_curve)\n# DataConnector holding 600 points and plots @ 100Hz\ndata_connector = DataConnector(plot_curve, max_points=600, update_rate=100)\n\n\ndef sin_wave_generator(connector):\n    """Sine wave generator"""\n    x = 0\n    while running:\n        x += 1\n        data_point = sin(x * 0.01)\n        # Callback to plot new data point\n        connector.cb_append_data_point(data_point, x)\n\n        sleep(0.01)\n\n\nplot_widget.show()\nThread(target=sin_wave_generator, args=(data_connector,)).start()\napp.exec()\nrunning = False\n```\n\nOutput:\n\n![Plot example](https://i.postimg.cc/RFYGfNS6/pglive.gif)\n\nTo run built-in examples, use python3 -m parameter like:  \n`python3 -m pglive.examples_pyqt6.all_plot_types`  \n`python3 -m pglive.examples_pyqt6.crosshair`\n\n# Using PyQt5/6 designer #\n\n1. Add QWidget to Your layout\n2. Promote QWidget to `LivePlotWidget` and set header file to `pglive.sources.live_plot_widget`\n3. Click `Add` and `Promote` button\n\n![All plot types](https://i.postimg.cc/m25NVJZm/designer-promotion.png)\n\n# Available plot types #\n\nPglive supports four plot types: `LiveLinePlot`, `LiveScatterPlot`, `LiveHBarPlot` (horizontal bar plot),\n`LiveVBarPlot` (vertical bar plot) and `LiveCandleStickPlot`.\n\n![All plot types](https://i.postimg.cc/637CsKRC/pglive-allplots.gif)\n![CandleStick plot](https://i.postimg.cc/0QcmMMb0/plot-candlestick.gif)\n![live-categorized-bar.gif](https://i.postimg.cc/xqrwXXjY/live-categorized-bar.gif)\n\n# Plot speed optimizations  #\n\nScaling plot view to plotted data has a huge impact on plotting performance.\nRe-plotting might be laggy when using high update frequencies and multiple plots.    \nTo increase plotting performance, pglive introduces `LiveAxisRange`, that can be used in `LivePlotWidget`.\nUser can now specify when and how is new view of plotted data calculated.\n\nHave a look in the `live_plot_range.py` example, to see how it can be used.\n\n![Range_optimization](https://i.postimg.cc/3wrMbbTY/a.gif)\n\nIn case you want to plot wider area with LiveAxisRange you can use crop_offset_to_data flag.\nFor example, you want to store 60 seconds, display 30 seconds in a view and move view every 1 second.\nYou will have big empty space to the left without setting flag to True.\nHave a look into crop_offset_to_data example.\n\n![crop_offset_to_data](https://i.postimg.cc/90X40Ng7/Peek-2022-09-24-15-20.gif)\n\nIntroduced in *v0.4.0*\n\n# Crosshair #\n\nPglive comes with built-in Crosshair as well.\n\n![Crosshair](https://i.postimg.cc/1z75GZLV/pglive-crosshair.gif)\n\n# Leading lines #\n\nLeading line displays horizontal or vertical line (or both) at the last plotted point.  \nYou can choose it\'s color and which axis value is displayed along with it.  \n\n![Leading lines](https://i.postimg.cc/bYKQGBNp/leading-line.gif)\n\n# Axis #\n\nTo make life easier, pglive includes few axis improvements:\n\n- Colored axis line using new `axisPen` attribute\n- Time and DateTime tick format, converting timestamp into human-readable format\n\n![Crosshair](https://i.postimg.cc/8kr0L2YJ/pglive-axis.gif)\n\n# Summary #\n\n- With Pglive You\'ve got easy Thread-safe implementation of fast Live plots\n- You can use all `kwargs` specified in pyqtgraph\n- Use your pyqtgraph plots with `DataConnector` directly, no need to use specific `LivePlot` class \n- **Focus on Data Handling, not Data Plotting**',
     'author': 'Martin Domaracky',
     'author_email': 'domarm@comat.sk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/domarm-comat/pglive',
```

### Comparing `pglive-0.6.3/PKG-INFO` & `pglive-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pglive
-Version: 0.6.3
+Version: 0.6.4
 Summary: Pyqtgraph live plot
 Home-page: https://github.com/domarm-comat/pglive
 License: MIT
 Keywords: pyqtgraph,realtime,live,plotting,pyqt5,pyqt6,pyside2,pyside6
 Author: Martin Domaracky
 Author-email: domarm@comat.sk
 Requires-Python: >=3.8,<3.11
```

