# Comparing `tmp/acconeer-exptool-6.0.5.tar.gz` & `tmp/acconeer-exptool-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acconeer-exptool-6.0.5.tar", last modified: Thu May  4 12:03:06 2023, max compression
+gzip compressed data, was "acconeer-exptool-7.0.0.tar", last modified: Mon May 15 11:16:23 2023, max compression
```

## Comparing `acconeer-exptool-6.0.5.tar` & `acconeer-exptool-7.0.0.tar`

### file list

```diff
@@ -1,607 +1,608 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.426633 acconeer-exptool-6.0.5/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/.gitattributes
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.378632 acconeer-exptool-6.0.5/.github/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.382632 acconeer-exptool-6.0.5/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      877 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      368 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/.gitignore
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      158 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/.readthedocs.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13506 2023-05-04 11:32:49.000000 acconeer-exptool-6.0.5/CHANGELOG.md
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13663 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/Jenkinsfile
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1881 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/LICENSE.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      217 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/MANIFEST.in
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-05-04 12:03:06.426633 acconeer-exptool-6.0.5/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7948 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/README.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       73 2023-05-04 11:32:49.000000 acconeer-exptool-6.0.5/UNRELEASED_CHANGELOG.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.382632 acconeer-exptool-6.0.5/docker/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1865 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/docker/Dockerfile
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/docker/requirements-dev.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1604 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/dodo.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.378632 acconeer-exptool-6.0.5/examples/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.382632 acconeer-exptool-6.0.5/examples/a111/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3247 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/basic.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1819 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/basic_continuous.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2657 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/load_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1273 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/load_record_h5.m
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.382632 acconeer-exptool-6.0.5/examples/a111/plotting/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1999 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/plotting/plot_with_matplotlib.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/plotting/plot_with_pyqtgraph.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a111/record_data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1156 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/record_data/barebones.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2541 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/record_data/long_duration_split_files.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1958 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/record_data/with_cli.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a111/services/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2251 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/services/envelope.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3013 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/services/iq.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2277 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/services/power_bins.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2861 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/services/sparse.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a111/utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      802 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/utils/ping.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      805 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/utils/test_throughput.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1222 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/basic.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/bilateration/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8174 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/bilateration/bilaterator.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/breathing/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6340 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/breathing/breathing.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/distance/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4522 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/distance/detector.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/distance/processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      776 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/extended_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a121/load_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1405 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a121/load_record_h5.m
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/phase_tracking/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5808 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/phase_tracking/phase_tracking.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4538 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/plot.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/presence/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11241 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/presence/detector.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11026 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/presence/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/record_data/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      921 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/record_data/barebones.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1092 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/record_data/with_cli.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1140 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/reuse_calibration.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/smart_presence/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10430 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/smart_presence/processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9497 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/smart_presence/ref_app.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4253 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/stress.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      946 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/subsweeps.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/surface_velocity/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8515 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/surface_velocity/example_app.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8864 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/surface_velocity/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/touchless_button/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3927 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/touchless_button/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/vibration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4410 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/examples/a121/vibration/vibration.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/gui/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1254 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/gui/main.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7005 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/noxfile.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/portable/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       27 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/portable/.gitignore
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1571 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/portable/make.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/portable/package/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/portable/package/cmd_with_path.bat
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      346 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/portable/package/run_app.bat
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/portable/package/tools/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/portable/package/tools/update.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      168 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/portable/package/update.bat
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2515 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/pyproject.toml
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2433 2023-05-04 12:03:06.426633 acconeer-exptool-6.0.5/setup.cfg
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.382632 acconeer-exptool-6.0.5/src/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.378632 acconeer-exptool-6.0.5/src/acconeer/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/src/acconeer/exptool/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      295 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3212 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_bs_thread.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/src/acconeer/exptool/_pyusb/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      100 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_pyusb/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5890 2023-01-24 10:54:24.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_pyusb/pyusbcomm.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/_structs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_structs/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15542 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_structs/configbase.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15673 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_structs/qtpidgets.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/_tests/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_tests/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4259 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_tests/test_rig.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       22 2023-05-04 12:03:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_version.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1071 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/LICENSE
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      190 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2847 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6837 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/usb_cdc.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2021 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusb.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3466 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusbclasses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      231 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusberror.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10029 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusbpy.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12307 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusbutils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      438 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      119 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7940 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5916 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5513 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/client_factory.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      517 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/common.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/json/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/json/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18330 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/json/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14209 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/links.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/mock/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/mock/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7621 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/mock/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1496 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/multiwrap.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24884 2023-05-04 11:25:32.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/data/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8068 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6351 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/protocol.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9853 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/regmap.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7176 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_conf_to_rss_sdk.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28007 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      587 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_modes.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3710 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      242 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/_base/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2708 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/_base/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      860 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/_base/module_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1695 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/_standalone_main.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      538 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7469 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4554 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      618 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6054 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5308 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11319 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4931 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      948 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21416 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2204 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6126 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      862 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3943 2022-12-29 10:02:50.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5280 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      565 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1985 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3928 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      939 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27784 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9166 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16847 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9162 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8503 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      576 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2599 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4172 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      612 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1400 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15250 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13885 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14079 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10519 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      615 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10381 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4623 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5079 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1341 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4454 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      557 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5185 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5472 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      824 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12380 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      186 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7812 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10409 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3125 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/ui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2560 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      545 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4662 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6099 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9009 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/recording.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1136 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1790 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_cli.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      989 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      671 2023-05-04 10:56:45.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2023-02-08 08:58:10.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4195 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    22033 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10267 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/session_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11137 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1035 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      592 2023-05-04 10:56:45.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8821 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/client_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4798 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/metadata.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4585 2023-05-04 10:56:45.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2192 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/result.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2906 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/server_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/server_log_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1675 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      144 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/dtypes.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/mediators/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      130 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/mediators/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      931 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/mediators/link.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      822 2023-05-04 11:00:03.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/mediators/recorder.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      401 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      439 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6962 2023-05-03 13:30:39.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4129 2023-05-04 11:00:03.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1324 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15712 2023-05-03 13:30:39.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      403 2023-02-13 09:23:57.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1023 2023-02-13 09:23:57.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6512 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      985 2023-02-13 09:23:57.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1037 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      521 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      687 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1150 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       96 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/parse_error.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4314 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1123 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      752 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2836 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1045 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      791 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       97 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/server_error.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1998 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/links.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      643 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11468 2023-05-03 13:30:39.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3996 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      229 2023-05-04 11:00:03.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7651 2023-05-04 11:00:03.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2820 2023-05-04 11:00:03.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11206 2023-05-04 11:00:03.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      928 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/im_record/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/im_record/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3854 2023-05-04 10:56:45.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18035 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core_ext/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core_ext/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4082 2023-05-03 13:30:39.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core_ext/_replaying_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_h5_utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4840 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_perf_calc.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2516 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_rate_calc.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      646 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4086 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_base.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      367 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7322 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/_a121.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      434 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      617 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3783 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      446 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8225 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1276 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6492 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7327 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/bilateration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-06 10:51:29.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/bilateration/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      395 2023-03-28 07:00:16.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/bilateration/_configs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    24882 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/bilateration/_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    17474 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/bilateration/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      192 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/breathing/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      376 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8723 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/breathing/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7401 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/breathing/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      507 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      855 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5471 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_aggregator.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      307 2023-03-28 07:00:16.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    59249 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24069 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    30450 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_processors.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15812 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7575 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7141 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      213 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2175 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14290 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_detector.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25641 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18288 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_processors.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4717 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      182 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2223 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6607 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7165 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21666 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6835 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2023-02-06 16:11:19.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8167 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3116 2023-02-06 16:11:19.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7245 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      130 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11412 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21651 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14090 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      219 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1658 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25992 2023-04-26 11:57:07.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7290 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6265 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4229 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_serializer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      306 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      486 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1100 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1738 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7687 2023-03-31 08:16:11.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14570 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2896 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/vibration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/vibration/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/vibration/__main__,py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8514 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/vibration/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7398 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/vibration/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/py.typed
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/app/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      333 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4475 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/launcher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.414633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      959 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      994 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/_argument_parser.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1718 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/_enums.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/_exceptions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      983 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/_version_checker.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2698 2022-12-29 10:02:50.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.414633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      239 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    27938 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/app_model.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/app_model_listener.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      981 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/file_detective.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      428 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/plugin_protocols.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2074 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/port_updater.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.414633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      452 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2840 2023-05-03 13:30:39.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_application_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_backend.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1610 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_backend_logger.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1857 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_backend_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1559 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_message.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4896 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_model.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1558 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/plugin_loader.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.414633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      241 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      973 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1024 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2222 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/py.typed
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      470 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/qt_subclasses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      804 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/storage.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.414633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      495 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2141 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/app_model_viewer.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2641 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/device_comboboxes.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.414633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/flash_tab/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       94 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/flash_tab/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14023 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4635 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/flash_tab/threads.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15274 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1802 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/help_tab.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2052 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/icons.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3600 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/main_window.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1968 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/misc.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      783 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6615 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1290 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1026 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6166 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1432 2023-03-27 09:23:51.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3557 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      769 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      499 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/common.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3814 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2082 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25494 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2004 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12975 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6474 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7963 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1887 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      294 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/types.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      865 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/utils.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9480 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/status_bar.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       98 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10441 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5853 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/hints.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12245 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4551 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2636 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1382 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    84006 2023-05-04 11:26:07.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4735 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/data_processing.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8476 2022-12-29 10:02:50.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/helper.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2346 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/modules.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10745 2023-05-04 11:25:32.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/qt_subclasses.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    90184 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/a111_gui.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    57036 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/a121_gui.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4162 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/icon-black.svg
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35706 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/icon.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3208 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/loader.gif
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.382632 acconeer-exptool-6.0.5/src/acconeer/exptool/data/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1245 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/LICENSE.txt
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/aarch64/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   513305 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/amd64/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   209008 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   314552 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/armv6/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   484176 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/armv7/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   399731 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/i386/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   160256 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   271672 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/x86_64/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   504389 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      338 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5844 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_bin_fetcher.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3625 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_dev_license.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4284 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_dev_license_tui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_device_flasher_base.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12868 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_flasher.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      828 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_products.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_stm32uart/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_stm32uart/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      274 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_stm32uart/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6665 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_xc120/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_xc120/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9147 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9417 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      224 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_xc120/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11051 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/libft4222.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3338 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/mpl_process.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3185 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/pg_process.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/__main__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      244 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/platform_install.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      980 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/prompts.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/setup_group.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/setup_step.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/cli/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/cli/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      684 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/cli/argument_parser.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/platforms/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/platforms/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/platforms/how_to.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1867 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/platforms/linux.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/py.typed
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21469 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.426633 acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-05-04 12:03:06.000000 acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25411 2023-05-04 12:03:06.000000 acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-04 12:03:06.000000 acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-04 12:03:05.000000 acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      475 2023-05-04 12:03:06.000000 acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2023-05-04 12:03:06.000000 acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.426633 acconeer-exptool-6.0.5/tools/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3715 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/tools/check_changelog.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12005 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/tools/check_copyright.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/tools/check_line_length.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1495 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/tools/check_permissions.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4237 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/tools/check_sdk_mentions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1801 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/tools/check_whitespace.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2064 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/tools/update_regmap.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.426633 acconeer-exptool-6.0.5/utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14756 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/utils/convert_to_csv.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.404196 acconeer-exptool-7.0.0/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/.gitattributes
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.356195 acconeer-exptool-7.0.0/.github/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      877 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      368 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/.gitignore
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      158 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/.readthedocs.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14227 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/CHANGELOG.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13663 2023-04-04 07:09:09.000000 acconeer-exptool-7.0.0/Jenkinsfile
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1881 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/LICENSE.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      217 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-05-15 11:16:23.404196 acconeer-exptool-7.0.0/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7948 2023-04-04 08:06:20.000000 acconeer-exptool-7.0.0/README.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       73 2023-05-12 21:00:22.000000 acconeer-exptool-7.0.0/UNRELEASED_CHANGELOG.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/docker/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1865 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/docker/Dockerfile
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/docker/requirements-dev.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1604 2023-03-28 13:52:52.000000 acconeer-exptool-7.0.0/dodo.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.356195 acconeer-exptool-7.0.0/examples/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a111/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3247 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/basic.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1819 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/basic_continuous.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2657 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/load_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1273 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/load_record_h5.m
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a111/plotting/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1999 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/plotting/plot_with_matplotlib.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/plotting/plot_with_pyqtgraph.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a111/record_data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1156 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/record_data/barebones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2541 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/record_data/long_duration_split_files.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1958 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/record_data/with_cli.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a111/services/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2251 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/services/envelope.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3013 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/services/iq.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2277 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/services/power_bins.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2861 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/services/sparse.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a111/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      802 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/utils/ping.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      805 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a111/utils/test_throughput.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a121/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1222 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/examples/a121/basic.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a121/bilateration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8174 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/examples/a121/bilateration/bilaterator.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a121/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6340 2023-05-12 21:00:22.000000 acconeer-exptool-7.0.0/examples/a121/breathing/breathing.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a121/distance/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4522 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/examples/a121/distance/detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/examples/a121/distance/processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      776 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/examples/a121/extended_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a121/load_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1405 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/examples/a121/load_record_h5.m
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a121/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5808 2023-04-11 14:12:51.000000 acconeer-exptool-7.0.0/examples/a121/phase_tracking/phase_tracking.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4538 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/examples/a121/plot.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a121/presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11241 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/examples/a121/presence/detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11026 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/examples/a121/presence/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a121/record_data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      975 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/examples/a121/record_data/barebones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1017 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/examples/a121/record_data/with_cli.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1140 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/examples/a121/reuse_calibration.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a121/smart_presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10430 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/examples/a121/smart_presence/processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9497 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/examples/a121/smart_presence/ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4253 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/examples/a121/stress.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      946 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/examples/a121/subsweeps.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a121/surface_velocity/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8515 2023-04-17 09:00:21.000000 acconeer-exptool-7.0.0/examples/a121/surface_velocity/example_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8864 2023-04-17 09:00:21.000000 acconeer-exptool-7.0.0/examples/a121/surface_velocity/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a121/touchless_button/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3927 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/examples/a121/touchless_button/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/examples/a121/vibration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4410 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.0/examples/a121/vibration/vibration.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/gui/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1254 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/gui/main.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7005 2023-04-17 09:00:21.000000 acconeer-exptool-7.0.0/noxfile.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/portable/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       27 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/portable/.gitignore
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1571 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/portable/make.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/portable/package/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/portable/package/cmd_with_path.bat
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      346 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/portable/package/run_app.bat
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.364195 acconeer-exptool-7.0.0/portable/package/tools/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/portable/package/tools/update.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      168 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/portable/package/update.bat
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2515 2023-04-04 07:09:09.000000 acconeer-exptool-7.0.0/pyproject.toml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2433 2023-05-15 11:16:23.404196 acconeer-exptool-7.0.0/setup.cfg
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.360195 acconeer-exptool-7.0.0/src/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.356195 acconeer-exptool-7.0.0/src/acconeer/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.368195 acconeer-exptool-7.0.0/src/acconeer/exptool/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      295 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3212 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_bs_thread.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.368195 acconeer-exptool-7.0.0/src/acconeer/exptool/_pyusb/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      100 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_pyusb/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5890 2023-01-16 13:15:52.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_pyusb/pyusbcomm.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.368195 acconeer-exptool-7.0.0/src/acconeer/exptool/_structs/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_structs/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15542 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_structs/configbase.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15673 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_structs/qtpidgets.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.368195 acconeer-exptool-7.0.0/src/acconeer/exptool/_tests/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_tests/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4259 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_tests/test_rig.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       22 2023-05-15 11:16:23.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_version.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.368195 acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1071 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/LICENSE
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      190 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2847 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6837 2023-01-18 08:37:12.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/usb_cdc.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2021 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/winusb.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3466 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/winusbclasses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      231 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/winusberror.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10029 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/winusbpy.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12307 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/winusbutils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.368195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      438 2023-04-04 07:09:09.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.368195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      119 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7940 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5916 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5513 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/client_factory.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      517 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/common.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.368195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/json/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/json/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18330 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/json/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14209 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/links.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.368195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/mock/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/mock/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7621 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/mock/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1496 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/multiwrap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.368195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/reg/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/reg/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24884 2023-05-12 21:00:22.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/reg/client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.368195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/reg/data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/reg/data/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8068 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6351 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/reg/protocol.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9853 2023-04-04 07:09:09.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/reg/regmap.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7176 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_conf_to_rss_sdk.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28007 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      587 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_modes.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3710 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.368195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      242 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.372195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/_base/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2708 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/_base/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      860 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/_base/module_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1695 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/_standalone_main.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.372195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      538 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/breathing/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7469 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4554 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/breathing/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.372195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      618 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6054 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5308 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.372195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11319 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press_sparse/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4931 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.372195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/distance_detector/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/distance_detector/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/distance_detector/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      948 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/distance_detector/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21416 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/distance_detector/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2204 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/distance_detector/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6126 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/distance_detector/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.372195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/envelope/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/envelope/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/envelope/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      862 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/envelope/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3943 2023-01-02 07:40:17.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/envelope/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/envelope/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5280 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/envelope/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.372195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/iq/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/iq/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/iq/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      565 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/iq/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1985 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/iq/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3928 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/iq/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.372195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/obstacle_detection/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/obstacle_detection/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/obstacle_detection/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      939 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27784 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9166 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/obstacle_detection/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16847 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.372195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/parking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/parking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/parking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/parking/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9162 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/parking/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8503 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/parking/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.376195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/phase_tracking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/phase_tracking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      576 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2599 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4172 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/phase_tracking/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.376195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/power_bins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/power_bins/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/power_bins/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      612 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/power_bins/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/power_bins/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1400 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/power_bins/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.376195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-13 14:33:08.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-13 14:33:08.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-13 14:33:08.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15250 2023-02-13 14:33:08.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13885 2023-02-13 14:33:08.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.376195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14079 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10519 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.376195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sleep_breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sleep_breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sleep_breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      615 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10381 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4623 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.376195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5079 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.376195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_fft/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_fft/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_fft/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1341 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4454 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_fft/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.376195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      557 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5185 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5472 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.376195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/speed_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/speed_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/speed_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      824 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12380 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      186 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/speed_sparse/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7812 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/speed_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.380195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/tank_level_short/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/tank_level_short/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/tank_level_short/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10409 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3125 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/tank_level_short/ui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2560 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.380195 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/wave_to_exit/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/wave_to_exit/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/wave_to_exit/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      545 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4662 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6099 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9009 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a111/recording.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.380195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1136 2023-03-31 13:21:19.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1790 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_cli.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.380195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.380195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.380195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/configs/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2023-02-07 10:50:48.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/configs/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4195 2023-03-29 14:55:09.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    22033 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10267 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/configs/session_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11137 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1035 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.380195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      607 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8821 2023-04-17 12:38:00.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/client_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4798 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/metadata.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8216 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2192 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/result.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2906 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/server_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/server_log_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1675 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      144 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/dtypes.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.380195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/mediators/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/mediators/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      931 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/mediators/link.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1265 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/mediators/recorder.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.380195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      401 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.380195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      439 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7119 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1324 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15568 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.384195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      403 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1023 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6512 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      985 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1037 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.384195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      521 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      687 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1150 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       96 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/parse_error.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4314 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1123 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      752 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2836 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1045 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      791 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       97 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/server_error.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1998 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/links.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      643 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11369 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3996 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.384195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      276 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8225 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3012 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12719 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      928 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.384195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/im_record/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/im_record/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3543 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18035 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.384195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core_ext/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core_ext/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4903 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core_ext/_replaying_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_h5_utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4840 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_perf_calc.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2516 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_rate_calc.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.384195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      646 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4086 2023-04-17 12:38:00.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_base.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.384195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      367 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7322 2023-04-19 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/_a121.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      434 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      617 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3783 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.384195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/processor/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      446 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/processor/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8308 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1276 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6492 2023-04-26 12:00:23.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7327 2023-05-15 10:00:18.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.384195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/bilateration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-03 12:56:53.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/bilateration/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      395 2023-03-28 07:00:16.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/bilateration/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24956 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/bilateration/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17474 2023-03-29 14:55:09.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/bilateration/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.384195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      192 2023-05-12 21:00:22.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2023-05-12 21:00:22.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8723 2023-05-12 21:00:22.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/breathing/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7401 2023-05-12 21:00:22.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/breathing/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.388195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      507 2023-03-29 14:55:09.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      855 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5471 2023-03-29 14:55:09.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/_aggregator.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      307 2023-03-28 07:00:16.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    59292 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24143 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    30450 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/_processors.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15812 2023-03-29 14:55:09.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.388195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7575 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7141 2023-03-31 11:49:16.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.388195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      213 2023-03-22 15:48:42.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/presence/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2175 2023-03-22 15:48:42.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/presence/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14333 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/presence/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25715 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18288 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/presence/_processors.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4717 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/presence/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.388195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/smart_presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      182 2023-02-16 12:21:41.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/smart_presence/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2223 2023-03-22 15:48:42.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/smart_presence/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6607 2023-03-23 12:16:45.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/smart_presence/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7165 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21740 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6835 2023-03-22 15:48:42.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.388195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/sparse_iq/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2023-02-03 12:56:53.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8167 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3116 2023-02-03 12:56:53.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7245 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.388195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/surface_velocity/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      130 2023-03-27 10:18:02.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11455 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21725 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14090 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.388195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/tank_level/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      219 2023-03-22 21:29:48.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/tank_level/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1658 2023-03-29 14:55:09.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/tank_level/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27271 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/tank_level/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7290 2023-03-22 15:48:42.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/tank_level/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6265 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4229 2023-03-22 21:29:48.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/tank_level/_serializer.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.388195 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/touchless_button/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      306 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/touchless_button/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      486 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/touchless_button/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1100 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1738 2023-01-18 08:37:12.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/touchless_button/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7687 2023-03-31 08:35:45.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14570 2023-04-11 12:00:20.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/touchless_button/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2896 2023-03-29 14:55:09.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.392196 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/vibration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/vibration/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/vibration/__main__,py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8514 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/vibration/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7398 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/vibration/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/a121/py.typed
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.392196 acconeer-exptool-7.0.0/src/acconeer/exptool/app/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      333 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4475 2023-03-31 11:49:16.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/launcher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.392196 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      959 2023-04-26 12:00:23.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      994 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/_argument_parser.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1718 2023-02-16 12:21:41.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/_enums.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/_exceptions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      983 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/_version_checker.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2698 2023-01-02 07:40:17.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/app.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.392196 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/app_model/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      239 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/app_model/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27938 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/app_model/app_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/app_model/app_model_listener.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      981 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/app_model/file_detective.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      428 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/app_model/plugin_protocols.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2074 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/app_model/port_updater.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.392196 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/backend/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      452 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/backend/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2737 2023-05-15 11:15:55.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/backend/_application_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5135 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/backend/_backend.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1610 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/backend/_backend_logger.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1857 2023-04-19 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/backend/_backend_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1559 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/backend/_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4896 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/backend/_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1558 2023-05-12 21:00:22.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/plugin_loader.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.392196 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/pluginbase/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      241 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/pluginbase/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      973 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1024 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2222 2023-04-19 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/py.typed
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      470 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/qt_subclasses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      804 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/storage.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.392196 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      495 2023-04-26 12:00:23.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2141 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/app_model_viewer.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2641 2023-04-11 13:26:34.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/device_comboboxes.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.392196 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/flash_tab/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       94 2023-04-21 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/flash_tab/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14023 2023-04-21 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4635 2023-04-19 08:17:48.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/flash_tab/threads.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15274 2023-04-21 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1802 2023-04-21 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/help_tab.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2052 2023-04-21 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/icons.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3600 2023-04-21 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/main_window.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1968 2023-04-11 13:29:49.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/misc.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.396196 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      783 2023-04-26 12:00:23.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6615 2023-04-19 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1290 2023-03-22 15:48:42.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1026 2023-04-19 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6166 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1432 2023-03-27 09:27:37.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3557 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.396196 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      769 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      499 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/common.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3814 2023-04-19 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2082 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25494 2023-04-19 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2004 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12975 2023-04-19 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6474 2023-04-26 12:00:23.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7963 2023-04-19 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1887 2023-04-19 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      294 2023-04-19 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/types.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      865 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9480 2023-04-11 13:26:34.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/status_bar.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.396196 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/stream_tab/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       98 2023-04-11 13:34:25.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10441 2023-04-11 13:34:25.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5853 2023-04-11 13:34:25.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/stream_tab/hints.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12245 2023-04-11 13:34:25.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4551 2023-04-11 13:34:25.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2636 2023-04-21 07:00:24.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1382 2023-04-26 12:00:23.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.396196 acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    84006 2023-05-12 21:00:22.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4735 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/data_processing.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.396196 acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/elements/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/elements/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8476 2022-12-28 08:17:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/elements/helper.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2346 2023-02-13 14:33:08.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/elements/modules.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10745 2023-05-12 21:00:22.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/elements/qt_subclasses.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.396196 acconeer-exptool-7.0.0/src/acconeer/exptool/app/resources/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/resources/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    90184 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/resources/a111_gui.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    57036 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/resources/a121_gui.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4162 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/resources/icon-black.svg
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35706 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/resources/icon.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3208 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/app/resources/loader.gif
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.360195 acconeer-exptool-7.0.0/src/acconeer/exptool/data/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.396196 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1245 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/LICENSE.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.396196 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/aarch64/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   513305 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.400195 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/amd64/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   209008 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   314552 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.400195 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/armv6/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   484176 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.400195 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/armv7/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   399731 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.400195 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/i386/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   160256 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   271672 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.400195 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/x86_64/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   504389 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.404196 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      338 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5844 2023-04-03 11:06:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_bin_fetcher.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3625 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_dev_license.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4284 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_dev_license_tui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_device_flasher_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12868 2023-04-04 08:00:22.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_flasher.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      828 2023-01-18 08:37:12.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_products.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.404196 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_stm32uart/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_stm32uart/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      274 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_stm32uart/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6665 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.404196 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_xc120/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2023-01-18 08:37:12.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_xc120/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9147 2023-01-18 08:37:12.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9417 2023-04-19 13:00:22.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      224 2023-01-18 08:37:12.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_xc120/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11051 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/libft4222.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3338 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/mpl_process.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3185 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/pg_process.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.404196 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/__main__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.404196 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/base/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      244 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/base/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/base/platform_install.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      980 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/base/prompts.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/base/setup_group.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/base/setup_step.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/base/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.404196 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/cli/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/cli/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      684 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/cli/argument_parser.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.404196 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/platforms/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/platforms/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/platforms/how_to.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1867 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/platforms/linux.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/setup/py.typed
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21469 2023-03-22 21:29:48.000000 acconeer-exptool-7.0.0/src/acconeer/exptool/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.404196 acconeer-exptool-7.0.0/src/acconeer_exptool.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-05-15 11:16:23.000000 acconeer-exptool-7.0.0/src/acconeer_exptool.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25483 2023-05-15 11:16:23.000000 acconeer-exptool-7.0.0/src/acconeer_exptool.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-15 11:16:23.000000 acconeer-exptool-7.0.0/src/acconeer_exptool.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-15 11:16:22.000000 acconeer-exptool-7.0.0/src/acconeer_exptool.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      475 2023-05-15 11:16:23.000000 acconeer-exptool-7.0.0/src/acconeer_exptool.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2023-05-15 11:16:23.000000 acconeer-exptool-7.0.0/src/acconeer_exptool.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.404196 acconeer-exptool-7.0.0/tools/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3715 2023-05-04 12:49:42.000000 acconeer-exptool-7.0.0/tools/check_changelog.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12005 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/tools/check_copyright.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/tools/check_line_length.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1495 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/tools/check_permissions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4237 2023-04-04 07:09:09.000000 acconeer-exptool-7.0.0/tools/check_sdk_mentions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1801 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/tools/check_whitespace.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2064 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/tools/update_regmap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 11:16:23.404196 acconeer-exptool-7.0.0/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14756 2022-12-27 09:08:13.000000 acconeer-exptool-7.0.0/utils/convert_to_csv.py
```

### Comparing `acconeer-exptool-6.0.5/.github/ISSUE_TEMPLATE/bug_report.md` & `acconeer-exptool-7.0.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/CHANGELOG.md` & `acconeer-exptool-7.0.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,37 @@
 # Changelog
 
+## v7.0.0
+This release is not fully backwards compatibility,
+which calls for a *major bump* (`v6 -> v7`).
+
+### Changed
+`Client` & `H5Recorder` classes have been changed (and upgraded).
+`H5Recorder` is now able to record multiple `Client` sessions in a single file.
+Recommended usage can be seen below.
+Detectors and Reference Applications have gotten no changes.
+
+```
+client = a121.Client.open()
+
+with a121.H5Recorder("filename.h5", client):
+    for number_of_sessions in range(10):
+        client.setup_session(a121.SessionConfig())
+        client.start_session()
+
+        for _ in range(10):
+            client.get_next()
+
+        client.stop_session()
+
+client.close()
+```
+
+All examples have been updated accordingly.
+
 ## v6.0.5
 
 ### Added
 - A121: Surface velocity: Validation added to check that start point is
   larger than the surface distance
 - Tabs in the A121 Application
```

### Comparing `acconeer-exptool-6.0.5/Jenkinsfile` & `acconeer-exptool-7.0.0/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/LICENSE.md` & `acconeer-exptool-7.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/PKG-INFO` & `acconeer-exptool-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acconeer-exptool
-Version: 6.0.5
+Version: 7.0.0
 Summary: Acconeer Exploration Tool
 Home-page: https://github.com/acconeer/acconeer-python-exploration
 Author: Acconeer AB
 Author-email: tools@acconeer.com
 License: BSD 3-Clause Clear License
 Project-URL: Tracker, https://github.com/acconeer/acconeer-python-exploration/issues
 Project-URL: Documentation, https://acconeer-python-exploration.readthedocs.io
```

### Comparing `acconeer-exptool-6.0.5/README.md` & `acconeer-exptool-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/docker/Dockerfile` & `acconeer-exptool-7.0.0/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/dodo.py` & `acconeer-exptool-7.0.0/dodo.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/basic.py` & `acconeer-exptool-7.0.0/examples/a111/basic.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/basic_continuous.py` & `acconeer-exptool-7.0.0/examples/a111/basic_continuous.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/load_record.py` & `acconeer-exptool-7.0.0/examples/a111/load_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/load_record_h5.m` & `acconeer-exptool-7.0.0/examples/a111/load_record_h5.m`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/plotting/plot_with_matplotlib.py` & `acconeer-exptool-7.0.0/examples/a111/plotting/plot_with_matplotlib.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/plotting/plot_with_pyqtgraph.py` & `acconeer-exptool-7.0.0/examples/a111/plotting/plot_with_pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/record_data/barebones.py` & `acconeer-exptool-7.0.0/examples/a111/record_data/barebones.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/record_data/long_duration_split_files.py` & `acconeer-exptool-7.0.0/examples/a111/record_data/long_duration_split_files.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/record_data/with_cli.py` & `acconeer-exptool-7.0.0/examples/a111/record_data/with_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/services/envelope.py` & `acconeer-exptool-7.0.0/examples/a111/services/envelope.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/services/iq.py` & `acconeer-exptool-7.0.0/examples/a111/services/iq.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/services/power_bins.py` & `acconeer-exptool-7.0.0/examples/a111/services/power_bins.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/services/sparse.py` & `acconeer-exptool-7.0.0/examples/a111/services/sparse.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/utils/ping.py` & `acconeer-exptool-7.0.0/examples/a111/utils/ping.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a111/utils/test_throughput.py` & `acconeer-exptool-7.0.0/examples/a111/utils/test_throughput.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/basic.py` & `acconeer-exptool-7.0.0/examples/a121/basic.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/bilateration/bilaterator.py` & `acconeer-exptool-7.0.0/examples/a121/bilateration/bilaterator.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/breathing/breathing.py` & `acconeer-exptool-7.0.0/examples/a121/breathing/breathing.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/distance/detector.py` & `acconeer-exptool-7.0.0/examples/a121/distance/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/distance/processor.py` & `acconeer-exptool-7.0.0/examples/a121/distance/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/extended_config.py` & `acconeer-exptool-7.0.0/examples/a121/extended_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/load_record.py` & `acconeer-exptool-7.0.0/examples/a121/load_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/load_record_h5.m` & `acconeer-exptool-7.0.0/examples/a121/load_record_h5.m`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/phase_tracking/phase_tracking.py` & `acconeer-exptool-7.0.0/examples/a121/phase_tracking/phase_tracking.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/plot.py` & `acconeer-exptool-7.0.0/examples/a121/plot.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/presence/detector.py` & `acconeer-exptool-7.0.0/examples/a121/presence/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/presence/processor.py` & `acconeer-exptool-7.0.0/examples/a121/presence/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/record_data/barebones.py` & `acconeer-exptool-7.0.0/examples/a121/record_data/barebones.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,29 +7,31 @@
 # Client creation
 client = a121.Client.open(ip_address="192.168.0.1")
 
 # Session setup, just like the other examples.
 config = a121.SessionConfig()
 client.setup_session(config)
 
-# Here we create a H5Recorder.
+
+# Here we specify the file name for the H5Recorder.
 # The H5Recorder is an object that saves frames directly to a H5-file.
 filename = "data.h5"
-h5_recorder = a121.H5Recorder(filename)
 
-# Here we send the H5Recorder to the Client.
-# After this call, the client is responsible for the H5Recorder.
-# The Client will automatically close the file when
-# "stop_session" is called.
-client.start_session(recorder=h5_recorder)
-
-n = 10
-for i in range(n):
-    # Client will send its Results to the H5Recorder.
-    client.get_next()
-    print(f"Result {i + 1}/{n} was sampled")
+# Here we create and attach a H5Recorder to the Client.
+# The H5Recorder will sample all frames retrieved in the client.
+# Once the "with"-block have been exited, the H5Recorder will
+# wrap up and close the file.
+with a121.H5Recorder(filename, client):
+    client.start_session()
+
+    n = 10
+    for i in range(n):
+        # Client will send its Results to the H5Recorder.
+        client.get_next()
+        print(f"Result {i + 1}/{n} was sampled")
+
+    client.stop_session()
 
-client.stop_session()
 client.close()
 
 with a121.open_record(filename) as record:
     print(record)
```

### Comparing `acconeer-exptool-6.0.5/examples/a121/record_data/with_cli.py` & `acconeer-exptool-7.0.0/examples/a121/record_data/with_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,30 +7,28 @@
 
 parser = a121.ExampleArgumentParser()
 parser.add_argument("--output-file", required=True)
 parser.add_argument("--num-frames", required=True, type=int)
 args = parser.parse_args()
 et.utils.config_logging(args)
 
-# Here we create a H5Recorder.
-# The H5Recorder is an object that saves frames directly to a H5-file.
-h5_recorder = a121.H5Recorder(args.output_file)
-
 client = a121.Client.open(**a121.get_client_args(args))
 
 # Session setup, just like the other examples.
 config = a121.SessionConfig()
 client.setup_session(config)
 
-# Here we send the H5Recorder to the Client.
-# After this call, the client is responsible for the H5Recorder.
-# The Client will automatically close the file when
-# "stop_session" is called.
-client.start_session(recorder=h5_recorder)
-
-for i in range(args.num_frames):
-    # Client will send its Results to the H5Recorder.
-    client.get_next()
-    print(f"Result {i + 1}/{args.num_frames} was sampled")
+# Here we create and attach a H5Recorder to the Client.
+# The H5Recorder will sample all frames retrieved in the client.
+# Once the "with"-block have been exited, the H5Recorder will
+# wrap up and close the file.
+with a121.H5Recorder(args.output_file, client):
+    client.start_session()
+
+    for i in range(args.num_frames):
+        # Client will send its Results to the H5Recorder.
+        client.get_next()
+        print(f"Result {i + 1}/{args.num_frames} was sampled")
+
+    client.stop_session()
 
-client.stop_session()
 client.close()
```

### Comparing `acconeer-exptool-6.0.5/examples/a121/reuse_calibration.py` & `acconeer-exptool-7.0.0/examples/a121/reuse_calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/smart_presence/processor.py` & `acconeer-exptool-7.0.0/examples/a121/smart_presence/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/smart_presence/ref_app.py` & `acconeer-exptool-7.0.0/examples/a121/smart_presence/ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/stress.py` & `acconeer-exptool-7.0.0/examples/a121/stress.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/subsweeps.py` & `acconeer-exptool-7.0.0/examples/a121/subsweeps.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/surface_velocity/example_app.py` & `acconeer-exptool-7.0.0/examples/a121/surface_velocity/example_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/surface_velocity/processor.py` & `acconeer-exptool-7.0.0/examples/a121/surface_velocity/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/touchless_button/processor.py` & `acconeer-exptool-7.0.0/examples/a121/touchless_button/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/examples/a121/vibration/vibration.py` & `acconeer-exptool-7.0.0/examples/a121/vibration/vibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/gui/main.py` & `acconeer-exptool-7.0.0/gui/main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/noxfile.py` & `acconeer-exptool-7.0.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/portable/make.py` & `acconeer-exptool-7.0.0/portable/make.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/portable/package/tools/update.py` & `acconeer-exptool-7.0.0/portable/package/tools/update.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/pyproject.toml` & `acconeer-exptool-7.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/setup.cfg` & `acconeer-exptool-7.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/_bs_thread.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/_bs_thread.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/_pyusb/pyusbcomm.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/_pyusb/pyusbcomm.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/_structs/configbase.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/_structs/configbase.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/_structs/qtpidgets.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/_structs/qtpidgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/_tests/test_rig.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/_tests/test_rig.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/LICENSE` & `acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/LICENSE`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/__main__.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/usb_cdc.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/usb_cdc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusb.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/winusb.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusbclasses.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/winusbclasses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusbpy.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/winusbpy.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusbutils.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/_winusbcdc/winusbutils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/base.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/client.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/client_factory.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/client_factory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/common.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/common.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/json/client.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/json/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/links.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/links.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/mock/client.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/mock/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/multiwrap.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/multiwrap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/client.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/reg/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/protocol.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/reg/protocol.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/regmap.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_clients/reg/regmap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_conf_to_rss_sdk.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_conf_to_rss_sdk.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_configs.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_modes.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_modes.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_utils.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/_utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/_base/calibration.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/_base/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/_base/module_info.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/_base/module_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/_standalone_main.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/_standalone_main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/breathing/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/breathing/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/distance_detector/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/distance_detector/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/calibration.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/distance_detector/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/distance_detector/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/envelope/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/envelope/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/calibration.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/envelope/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/envelope/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/iq/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/iq/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/iq/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/parking/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/parking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/parking/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/phase_tracking/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/power_bins/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/power_bins/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_fft/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/speed_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/tank_level_short/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/utils.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/recording.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a111/recording.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/__init__.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_cli.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/__init__.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/__init__.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     Result,
     ResultContext,
     SensorCalibration,
     SensorInfo,
     SerialInfo,
     ServerInfo,
     ServerLogMessage,
+    SessionRecord,
     SocketInfo,
     StackedResults,
     USBInfo,
     complex_array_to_int16_complex,
     int16_complex_array_to_complex,
 )
 from .dtypes import INT_16_COMPLEX
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/session_config.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/configs/session_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/__init__.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from .client_info import ClientInfo, MockInfo, SerialInfo, SocketInfo, USBInfo
 from .metadata import Metadata
-from .record import PersistentRecord, Record, RecordException
+from .record import PersistentRecord, Record, RecordException, SessionRecord
 from .result import Result, ResultContext
 from .sensor_calibration import SensorCalibration
 from .server_info import SensorInfo, ServerInfo
 from .server_log_message import ServerLogMessage
 from .stacked_results import StackedResults
 from .utils import (
     complex_array_to_int16_complex,
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/client_info.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/client_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/metadata.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/metadata.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/result.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/result.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/server_info.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/server_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/utils.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/entities/containers/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/mediators/link.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/mediators/link.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/client.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         :returns:
             ``Metadata`` if ``config.extended is False``,
             ``list[dict[int, Metadata]]`` otherwise.
         """
         ...
 
     @abc.abstractmethod
-    def start_session(self, recorder: Optional[Recorder] = None) -> None:
+    def start_session(self) -> None:
         """Starts the already set up session.
 
         After this call, the server starts streaming data to the client.
 
         :param recorder:
             An optional ``Recorder``, which samples every ``get_next()``
         :raises: ``ClientError`` if ``Client``'s  session is not set up.
@@ -135,27 +135,35 @@
             ``list[dict[int, Result]]`` otherwise.
         :raises:
             ``ClientError`` if ``Client``'s session is not started.
         """
         ...
 
     @abc.abstractmethod
-    def stop_session(self) -> Any:
+    def stop_session(self) -> None:
         """Stops an on-going session
 
-        :returns:
-            The return value of the passed ``Recorder.stop()`` passed in ``start_session``.
         :raises:
             ``ClientError`` if ``Client``'s session is not started.
         """
         ...
 
     @abc.abstractmethod
+    def attach_recorder(self, recorder: Recorder) -> None:
+        """Attaches a recorder to this client."""
+        ...
+
+    @abc.abstractmethod
+    def detach_recorder(self) -> Optional[Recorder]:
+        """Detaches and returns the attached recorder (if present)."""
+        ...
+
+    @abc.abstractmethod
     def close(self) -> None:
-        """Disconnects the client from the host."""
+        """Closes the connection to the host"""
         ...
 
     @property
     @abc.abstractmethod
     def connected(self) -> bool:
         """Whether this Client is connected."""
         ...
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
-from typing import Any, Optional, Union
+from typing import Optional, Union
 
 from acconeer.exptool.a121._core.entities import (
     ClientInfo,
     Metadata,
     Result,
     SensorCalibration,
     SessionConfig,
@@ -46,40 +46,66 @@
         self._calibrations_provided = {}
         self._metadata = None
         self._recorder = None
         self._sensor_calibrations = None
         self._session_is_started = False
         self._session_config = None
 
-    def _recorder_start(self, recorder: Optional[Recorder]) -> None:
-        if recorder is not None:
+    def attach_recorder(self, recorder: Recorder) -> None:
+        if self.session_is_started:
+            raise ClientError("Cannot attach a recorder when session is started.")
+
+        if not self.connected:
+            raise ClientError("Cannot attach a recorder to a closed client")
+
+        if self._recorder is not None:
+            raise ClientError(
+                "Client already has a recorder attached. "
+                + "Try detaching the current recorder before attaching a new recorder."
+            )
+
+        self._recorder = recorder
+        self._recorder._start(
+            client_info=self.client_info,
+            server_info=self.server_info,
+        )
+
+    def detach_recorder(self) -> Optional[Recorder]:
+        if self.session_is_started:
+            raise ClientError("Cannot detach a recorder when session is started.")
+
+        if not self.connected:
+            raise ClientError("Cannot detach a recorder from a closed client")
+
+        if self._recorder is None:
+            return None
+        else:
+            previously_attached_recorder = self._recorder
+            self._recorder = None
+            return previously_attached_recorder
+
+    def _recorder_start_session(self) -> None:
+        if self._recorder is not None:
             calibrations_provided: Optional[dict[int, bool]] = self.calibrations_provided
             try:
                 calibrations = self.calibrations
             except ClientError:
                 calibrations = None
                 calibrations_provided = None
 
-            self._recorder = recorder
-            self._recorder._start(
-                client_info=self.client_info,
-                extended_metadata=self.extended_metadata,
-                server_info=self.server_info,
+            self._recorder._start_session(
                 session_config=self.session_config,
+                extended_metadata=self.extended_metadata,
                 calibrations=calibrations,
                 calibrations_provided=calibrations_provided,
             )
 
-    def _recorder_stop(self) -> Any:
-        if self._recorder is None:
-            recorder_result = None
-        else:
-            recorder_result = self._recorder._stop()
-            self._recorder = None
-        return recorder_result
+    def _recorder_stop_session(self) -> None:
+        if self._recorder is not None:
+            self._recorder._stop_session()
 
     def _recorder_sample(self, extended_results: list[dict[int, Result]]) -> None:
         if self._recorder is not None:
             self._recorder._sample(extended_results)
 
     def _return_results(
         self, extended_results: list[dict[int, Result]]
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     SensorCalibration,
     SensorConfig,
     SensorInfo,
     ServerInfo,
     ServerLogMessage,
     SessionConfig,
 )
-from acconeer.exptool.a121._core.mediators import Recorder
 from acconeer.exptool.a121._core.utils import (
     create_extended_structure,
     iterate_extended_structure,
     unextend,
     unwrap_ticks,
 )
 from acconeer.exptool.a121._perf_calc import _SessionPerformanceCalc
@@ -317,21 +316,21 @@
         self._link.timeout = self._link_timeout
 
         if self.session_config.extended:
             return self._metadata
         else:
             return unextend(self._metadata)
 
-    def start_session(self, recorder: Optional[Recorder] = None) -> None:
+    def start_session(self) -> None:
         self._assert_session_setup()
 
         if self.session_is_started:
             raise ClientError("Session is already started.")
 
-        self._recorder_start(recorder)
+        self._recorder_start_session()
         self._session_is_started = True
 
         self._link.timeout = self._link_timeout
         self._link.send(self._protocol.start_streaming_command())
         self._apply_messages_until_message_type_encountered(messages.StartStreamingResponse)
 
     def get_next(self) -> Union[Result, list[dict[int, Result]]]:
@@ -357,42 +356,41 @@
         )
 
         extended_results = self._tick_unwrapper.unwrap_ticks(extended_results)
 
         self._recorder_sample(extended_results)
         return self._return_results(extended_results)
 
-    def stop_session(self) -> Any:
+    def stop_session(self) -> None:
         self._assert_session_started()
 
         self._link.send(self._protocol.stop_streaming_command())
 
         try:
             self._apply_messages_until_message_type_encountered(
                 messages.StopStreamingResponse, timeout_s=self._link.timeout + 1
             )
             self._session_is_started = False
         except Exception:
             raise
         finally:
             self._link.timeout = self._default_link_timeout
-            self._tick_unwrapper = TickUnwrapper()
 
-        recorder_result = self._recorder_stop()
-        self._log_queue.clear()
+        self._recorder_stop_session()
 
-        return recorder_result
+        self._log_queue.clear()
 
     def close(self) -> None:
         # TODO: Make sure this cleans up corner-cases (like lost connection)
         #       to not hog resources.
 
         if self.session_is_started:
-            _ = self.stop_session()
+            self.stop_session()
 
+        self._tick_unwrapper = TickUnwrapper()
         self._system_info = None
         self._sensor_infos = {}
         self._message_stream = iter([])
         self._metadata = None
         self._log_queue.clear()
         self._link.disconnect()
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/links.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/links.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/message.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     SensorCalibration,
     SensorConfig,
     SensorInfo,
     ServerInfo,
     SessionConfig,
     SubsweepConfig,
 )
-from acconeer.exptool.a121._core.mediators import Recorder
 from acconeer.exptool.a121._core.utils import unextend
 from acconeer.exptool.a121._perf_calc import _SessionPerformanceCalc
 
 from .client import Client, ClientCreationError, ClientError
 from .common_client import CommonClient
 from .communication_protocol import CommunicationProtocol
 from .utils import get_calibrations_provided
@@ -258,21 +257,21 @@
         self._mock_update_rate = max(self._mock_update_rate, self.MIN_MOCK_UPDATE_RATE_HZ)
 
         if self.session_config.extended:
             return self._metadata
         else:
             return unextend(self._metadata)
 
-    def start_session(self, recorder: Optional[Recorder] = None) -> None:
+    def start_session(self) -> None:
         self._assert_session_setup()
 
         if self.session_is_started:
             raise ClientError("Session is already started.")
 
-        self._recorder_start(recorder)
+        self._recorder_start_session()
         self._session_is_started = True
         self._start_time = time.perf_counter()
         self._mock_next_data_time = self._start_time
 
     def get_next(self) -> Union[Result, list[dict[int, Result]]]:
         self._assert_session_started()
 
@@ -289,26 +288,25 @@
             time.sleep(delta)
 
         self._mock_next_data_time += 1 / self._mock_update_rate
 
         self._recorder_sample(extended_results)
         return self._return_results(extended_results)
 
-    def stop_session(self) -> Any:
+    def stop_session(self) -> None:
         self._assert_session_started()
+        self._recorder_stop_session()
         self._session_is_started = False
 
-        return self._recorder_stop()
-
     def close(self) -> None:
         if not self._connected:
             raise ClientError("Client is already closed")
 
         if self.session_is_started:
-            _ = self.stop_session()
+            self.stop_session()
 
         self._metadata = None
         self._connected = False
 
     @property
     def connected(self) -> bool:
         return self._connected
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,72 +19,80 @@
     PersistentRecord,
     RecordException,
     Result,
     ResultContext,
     SensorCalibration,
     ServerInfo,
     SessionConfig,
+    SessionRecord,
     StackedResults,
 )
 from acconeer.exptool.utils import get_module_version  # type: ignore[import]
 
+from .session_schema import SessionSchema
+
 
 T = TypeVar("T")
 
 
 class H5RecordException(RecordException):
     pass
 
 
-class H5Record(PersistentRecord):
-    file: h5py.File
-
-    def __init__(self, file: h5py.File) -> None:
-        self.file = file
-
-        try:
-            version_of_record = Version(self.lib_version)
-        except KeyError:
-            pass
-        else:
-            installed_version = Version(get_module_version(acconeer.exptool))
-            if installed_version < version_of_record:
-                warnings.warn(
-                    f"The loaded file {str(self.file.name)!r} was recorded "
-                    + f"with a newer version of Exploration Tool ({version_of_record}) "
-                    + f"than is installed ({installed_version})."
-                )
-
-    @property
-    def client_info(self) -> ClientInfo:
-        return ClientInfo.from_json(self.file["client_info"][()])
+class H5SessionRecord(SessionRecord):
+    def __init__(self, group: h5py.Group, ticks_per_second: int) -> None:
+        self._group = group
+        self._ticks_per_second = ticks_per_second
 
     @property
     def extended_metadata(self) -> list[dict[int, Metadata]]:
         return self._map_over_entries(self._get_metadata_for_entry_group)
 
     @property
+    def extended_results(self) -> Iterator[list[dict[int, Result]]]:
+        for frame_no in range(self.num_frames):
+            yield self._get_result_for_all_entries(frame_no)
+
+    @property
     def extended_stacked_results(self) -> list[dict[int, StackedResults]]:
         return self._map_over_entries(self._entry_group_to_stacked_results)
 
-    def _entry_group_to_stacked_results(self, entry_group: h5py.Group) -> StackedResults:
-        return StackedResults(
-            data_saturated=entry_group["result/data_saturated"][()],
-            calibration_needed=entry_group["result/calibration_needed"][()],
-            temperature=entry_group["result/temperature"][()],
-            tick=entry_group["result/tick"][()],
-            frame_delayed=entry_group["result/frame_delayed"][()],
-            frame=entry_group["result/frame"][()],
-            context=self._get_result_context_for_entry_group(entry_group),
-        )
+    @property
+    def num_frames(self) -> int:
+        (num_frames,) = {len(entry["result/frame"]) for _, _, entry in self._iterate_entries()}
+        return num_frames
 
     @property
-    def extended_results(self) -> Iterator[list[dict[int, Result]]]:
-        for frame_no in range(self.num_frames):
-            yield self._get_result_for_all_entries(frame_no)
+    def session_config(self) -> SessionConfig:
+        return SessionConfig.from_json(self._group["session_config"][()])
+
+    @property
+    def sensor_id(self) -> int:
+        entry_group = utils.unextend(self._get_entries())
+        return int(entry_group["sensor_id"][()])
+
+    @property
+    def calibrations(self) -> dict[int, SensorCalibration]:
+        sensor_calibrations_dict = {}
+        for sensor_id, group in self._iterate_calibrations():
+            sensor_calibrations_dict[sensor_id] = SensorCalibration.from_h5(group)
+
+        return sensor_calibrations_dict
+
+    @property
+    def calibrations_provided(self) -> dict[int, bool]:
+        calibrations_provided = {}
+        for sensor_id, group in self._iterate_calibrations():
+            calibrations_provided[sensor_id] = group["provided"][()] > 0
+
+        return calibrations_provided
+
+    @staticmethod
+    def _get_metadata_for_entry_group(g: h5py.Group) -> Metadata:
+        return Metadata.from_json(g["metadata"][()])
 
     def _get_result_for_all_entries(self, frame_no: int) -> list[dict[int, Result]]:
         def entry_group_to_result(entry_group: h5py.Group) -> Result:
             return Result(
                 data_saturated=entry_group["result/data_saturated"][frame_no],
                 frame_delayed=entry_group["result/frame_delayed"][frame_no],
                 calibration_needed=entry_group["result/calibration_needed"][frame_no],
@@ -92,105 +100,61 @@
                 tick=entry_group["result/tick"][frame_no],
                 frame=np.array(entry_group["result/frame"][frame_no]),
                 context=self._get_result_context_for_entry_group(entry_group),
             )
 
         return self._map_over_entries(entry_group_to_result)
 
+    def _entry_group_to_stacked_results(self, entry_group: h5py.Group) -> StackedResults:
+        return StackedResults(
+            data_saturated=entry_group["result/data_saturated"][()],
+            calibration_needed=entry_group["result/calibration_needed"][()],
+            temperature=entry_group["result/temperature"][()],
+            tick=entry_group["result/tick"][()],
+            frame_delayed=entry_group["result/frame_delayed"][()],
+            frame=entry_group["result/frame"][()],
+            context=self._get_result_context_for_entry_group(entry_group),
+        )
+
     def _get_result_context_for_entry_group(self, entry_group: h5py.Group) -> ResultContext:
         return ResultContext(
             metadata=self._get_metadata_for_entry_group(entry_group),
-            ticks_per_second=self.server_info.ticks_per_second,
+            ticks_per_second=self._ticks_per_second,
         )
 
-    @property
-    def lib_version(self) -> str:
-        return self._h5py_dataset_to_str(self.file["lib_version"])
-
-    @property
-    def num_frames(self) -> int:
-        (num_frames,) = {len(entry["result/frame"]) for _, _, entry in self._iterate_entries()}
-        return num_frames
-
-    @property
-    def server_info(self) -> ServerInfo:
-        return ServerInfo.from_json(self.file["server_info"][()])
-
-    @property
-    def session_config(self) -> SessionConfig:
-        return SessionConfig.from_json(self.file["session/session_config"][()])
-
-    @property
-    def sensor_id(self) -> int:
-        entry_group = utils.unextend(self._get_entries())
-        return int(entry_group["sensor_id"][()])
-
-    @property
-    def timestamp(self) -> str:
-        return self._h5py_dataset_to_str(self.file["timestamp"])
-
-    @property
-    def uuid(self) -> str:
-        return self._h5py_dataset_to_str(self.file["uuid"])
-
-    def close(self) -> None:
-        self.file.close()
-
     def _get_entries(self) -> list[dict[int, h5py.Group]]:
         structure: dict[int, dict[int, h5py.Group]] = {}
 
-        for k, v in self.file["session"].items():
+        for k, v in self._group.items():
             m = re.fullmatch(r"group_(\d+)", k)
 
             if not m:
                 continue
 
             group_index = int(m.group(1))
             structure[group_index] = {}
 
             for vv in v.values():
                 sensor_id = vv["sensor_id"][()]
                 structure[group_index][sensor_id] = vv
 
         return [structure[i] for i in range(len(structure))]
 
-    def _map_over_entries(self, func: Callable[[h5py.Group], T]) -> list[dict[int, T]]:
-        return utils.map_over_extended_structure(func, self._get_entries())
-
     def _iterate_entries(self) -> Iterator[Tuple[int, int, h5py.Group]]:
         """Iterates over "Entry" items in this record.
 
         :returns: An iterable of <group_id>, <sensor_id>, <"EntryGroup">
         """
         for group_id, group_dict in enumerate(self._get_entries()):
             for sensor_id, entry_group in group_dict.items():
                 yield (group_id, sensor_id, entry_group)
 
-    @staticmethod
-    def _get_metadata_for_entry_group(g: h5py.Group) -> Metadata:
-        return Metadata.from_json(g["metadata"][()])
-
-    @staticmethod
-    def _h5py_dataset_to_str(dataset: h5py.Dataset) -> str:
-        return bytes(dataset[()]).decode()
-
-    def get_algo_group(self, key: str) -> h5py.Group:
-        group = self.file["algo"]  # Raises KeyError if the "algo" group doesn't exist
-
-        existing_key = self._h5py_dataset_to_str(group["key"])
-        if existing_key != key:
-            raise KeyError
-
-        return group
-
     def _get_calibrations_group(self) -> h5py.Group:
-        session_group = self.file["session"]
-
-        if "calibrations" in session_group.keys():
-            return session_group["calibrations"]
+        if "calibrations" in self._group.keys():
+            return self._group["calibrations"]
         raise H5RecordException("No calibration in h5 file")
 
     def _iterate_calibrations(self) -> Iterator[Tuple[int, h5py.Group]]:
         """Iterates over "Calibration" items in this record.
 
         :returns: An iterable of <sensor_id>, <"CalibrationGroup">
         """
@@ -200,22 +164,77 @@
 
             if not m:
                 continue
 
             sensor_id = int(m.group(1))
             yield (sensor_id, group)
 
+    def _map_over_entries(self, func: Callable[[h5py.Group], T]) -> list[dict[int, T]]:
+        return utils.map_over_extended_structure(func, self._get_entries())
+
+
+class H5Record(PersistentRecord):
+    _schema = SessionSchema
+
+    file: h5py.File
+
+    def __init__(self, file: h5py.File) -> None:
+        self.file = file
+
+        try:
+            version_of_record = Version(self.lib_version)
+        except KeyError:
+            pass
+        else:
+            installed_version = Version(get_module_version(acconeer.exptool))
+            if installed_version < version_of_record:
+                warnings.warn(
+                    f"The loaded file {str(self.file.name)!r} was recorded "
+                    + f"with a newer version of Exploration Tool ({version_of_record}) "
+                    + f"than is installed ({installed_version})."
+                )
+
     @property
-    def calibrations(self) -> dict[int, SensorCalibration]:
-        sensor_calibrations_dict = {}
-        for sensor_id, group in self._iterate_calibrations():
-            sensor_calibrations_dict[sensor_id] = SensorCalibration.from_h5(group)
+    def client_info(self) -> ClientInfo:
+        return ClientInfo.from_json(self.file["client_info"][()])
 
-        return sensor_calibrations_dict
+    @property
+    def lib_version(self) -> str:
+        return self._h5py_dataset_to_str(self.file["lib_version"])
 
     @property
-    def calibrations_provided(self) -> dict[int, bool]:
-        calibrations_provided = {}
-        for sensor_id, group in self._iterate_calibrations():
-            calibrations_provided[sensor_id] = group["provided"][()] > 0
+    def server_info(self) -> ServerInfo:
+        return ServerInfo.from_json(self.file["server_info"][()])
 
-        return calibrations_provided
+    @property
+    def timestamp(self) -> str:
+        return self._h5py_dataset_to_str(self.file["timestamp"])
+
+    @property
+    def uuid(self) -> str:
+        return self._h5py_dataset_to_str(self.file["uuid"])
+
+    def close(self) -> None:
+        self.file.close()
+
+    @staticmethod
+    def _h5py_dataset_to_str(dataset: h5py.Dataset) -> str:
+        return bytes(dataset[()]).decode()
+
+    def get_algo_group(self, key: str) -> h5py.Group:
+        group = self.file["algo"]  # Raises KeyError if the "algo" group doesn't exist
+
+        existing_key = self._h5py_dataset_to_str(group["key"])
+        if existing_key != key:
+            raise KeyError
+
+        return group
+
+    def session(self, session_index: int) -> H5SessionRecord:
+        return H5SessionRecord(
+            group=self._schema.session_groups_on_disk(self.file)[session_index],
+            ticks_per_second=self.server_info.ticks_per_second,
+        )
+
+    @property
+    def num_sessions(self) -> int:
+        return len(self._schema.session_groups_on_disk(self.file))
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 from acconeer.exptool.a121._core.entities import PersistentRecord, Record
 from acconeer.exptool.a121._core.peripherals.im_record import InMemoryRecord
 
@@ -71,22 +71,24 @@
 
     return save_record_to_h5(path_or_file, record)
 
 
 def save_record_to_h5(path_or_file: PathOrH5File, record: Record) -> None:
     """Save a record to a HDF5 file"""
 
-    recorder = H5Recorder(path_or_file)
+    with H5Recorder(path_or_file) as r:
+        r._start(
+            client_info=record.client_info,
+            server_info=record.server_info,
+        )
+        for session in (record.session(i) for i in range(record.num_sessions)):
+            r._start_session(
+                session_config=session.session_config,
+                extended_metadata=session.extended_metadata,
+                calibrations=session.calibrations,
+                calibrations_provided=session.calibrations_provided,
+            )
 
-    recorder._start(
-        client_info=record.client_info,
-        extended_metadata=record.extended_metadata,
-        server_info=record.server_info,
-        session_config=record.session_config,
-        calibrations=record.calibrations,
-        calibrations_provided=record.calibrations_provided,
-    )
-
-    for extended_result in record.extended_results:
-        recorder._sample(extended_result)
+            for extended_result in session.extended_results:
+                r._sample(extended_result)
 
-    recorder._stop()
+            r._stop_session()
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,17 +20,18 @@
     ClientInfo,
     Metadata,
     Result,
     SensorCalibration,
     ServerInfo,
     SessionConfig,
 )
-from acconeer.exptool.a121._core.mediators import Recorder
+from acconeer.exptool.a121._core.mediators import Recorder, RecorderAttachable
 from acconeer.exptool.utils import get_module_version  # type: ignore[import]
 
+from .session_schema import SessionSchema
 from .utils import PathOrH5File, h5_file_factory
 
 
 T = TypeVar("T")
 
 
 def get_h5py_str_dtype() -> Any:
@@ -53,14 +54,17 @@
 
     :param path_or_file:
         If a path-like object, by default (depending on ``mode`` below) an HDF5 file is created at
         that path. When stopping, the file is closed.
 
         If an ``h5py.File``, that file is used as-is. In this case, the file is not closed when
         stopping.
+    :param attachable:
+        A ``Client`` that the recorder will be attached to. When a recorder is attached to a
+        ``Client``, all metadata and data frames will be recorded.
     :param mode:
         The file mode to use if a path-like object was given for ``path_or_file``. Default value is
         'x', meaning that we open for exclusive creation, failing if the file already exists.
     :param _chunk_size:
         If given, data will be written to file every ``_chunk_size`` samples.
 
         If not given, data will be written at least every 512:th sample, or at least once per
@@ -69,44 +73,53 @@
         Setting a small chunk size (e.g. 1) may degrade performance for high sample rates.
 
         Internal parameter, subject to change.
     """
 
     _AUTO_CHUNK_MAX_SIZE = 512
     _AUTO_CHUNK_MAX_TIME = 1.0
+    _schema = SessionSchema
 
     path: Optional[os.PathLike[Any]]
     """The file path, if a path-like object was given for ``path_or_file``."""
     file: h5py.File
     """The ``h5py.File``."""
     owns_file: bool
     """Whether :class:`H5Recorder` opened and owns the file, i.e., if a path-like object was given
     for ``path_or_file``. If it does, the file is closed when stopping.
     """
-    _num_frames: int
+    _num_frames_current_session: int
     _chunk_size: Optional[int]
     _chunk_buffer: list[list[dict[int, Result]]]
     _last_write_time: float
 
     def __init__(
         self,
         path_or_file: PathOrH5File,
+        attachable: Optional[RecorderAttachable] = None,
         mode: str = "x",
         *,
         _chunk_size: Optional[int] = None,
         _lib_version: Optional[str] = None,
         _timestamp: Optional[str] = None,
         _uuid: Optional[str] = None,
     ) -> None:
         self.file, self.owns_file = h5_file_factory(path_or_file, h5_file_mode=mode)
         self.path = Path(self.file.filename) if self.owns_file else None
         self._chunk_size = _chunk_size
         self._chunk_buffer = []
-        self._num_frames = 0
+        self._num_frames_current_session = 0
         self._last_write_time = 0.0
+        self._current_session_group: Optional[h5py.Group] = None
+
+        if attachable is None:
+            self._attachable = None
+        else:
+            self._attachable = attachable
+            attachable.attach_recorder(self)
 
         if _lib_version is None:
             _lib_version = get_module_version(acconeer.exptool)
 
         if _timestamp is None:
             _timestamp = get_timestamp()
 
@@ -138,44 +151,52 @@
             track_times=False,
         )
 
     def _start(
         self,
         *,
         client_info: ClientInfo,
-        extended_metadata: list[dict[int, Metadata]],
         server_info: ServerInfo,
-        session_config: SessionConfig,
-        calibrations: Optional[dict[int, SensorCalibration]],
-        calibrations_provided: Optional[dict[int, bool]],
     ) -> None:
+        if "client_info" in self.file or "server_info" in self.file:
+            raise RuntimeError("It's not allowed to call '_start' once.")
+
         self.file.create_dataset(
             "client_info",
             data=client_info.to_json(),
             dtype=_H5PY_STR_DTYPE,
             track_times=False,
         )
         self.file.create_dataset(
             "server_info",
             data=server_info.to_json(),
             dtype=_H5PY_STR_DTYPE,
             track_times=False,
         )
+        self._last_write_time = time()
 
-        session_group = self.file.create_group("session")
+    def _start_session(
+        self,
+        *,
+        session_config: SessionConfig,
+        extended_metadata: list[dict[int, Metadata]],
+        calibrations: Optional[dict[int, SensorCalibration]],
+        calibrations_provided: Optional[dict[int, bool]],
+    ) -> None:
+        self._current_session_group = self._schema.create_next_session_group(self.file)
 
-        session_group.create_dataset(
+        self._current_session_group.create_dataset(
             "session_config",
             data=session_config.to_json(),
             dtype=_H5PY_STR_DTYPE,
             track_times=False,
         )
 
         for i, metadata_group_dict in enumerate(extended_metadata):
-            group_group = session_group.create_group(f"group_{i}")
+            group_group = self._current_session_group.create_group(f"group_{i}")
 
             for entry_id, (sensor_id, metadata) in enumerate(metadata_group_dict.items()):
                 entry_group = group_group.create_group(f"entry_{entry_id}")
                 entry_group.create_dataset("sensor_id", data=sensor_id, track_times=False)
 
                 entry_group.create_dataset(
                     "metadata",
@@ -189,15 +210,15 @@
 
         if (calibrations is None) != (calibrations_provided is None):
             raise ValueError(
                 "'calibrations_provided' must be provided if 'calibrations' is provided"
             )
 
         if calibrations is not None and calibrations_provided is not None:
-            calibrations_group = session_group.create_group("calibrations")
+            calibrations_group = self._current_session_group.create_group("calibrations")
             for sensor_id, calibration in calibrations.items():
                 sensor_calibration_group = calibrations_group.create_group(f"sensor_{sensor_id}")
 
                 calibration.to_h5(sensor_calibration_group)
 
                 sensor_calibration_group.create_dataset(
                     "provided", data=calibrations_provided[sensor_id], track_times=False
@@ -206,23 +227,25 @@
         self._last_write_time = time()
 
     def _write_chunk_buffer_to_file(self, start_idx: int) -> int:
         """Saves the contents of ``self.chunk_buffer`` to file.
 
         :returns: the number of extended results saved.
         """
-
         if len(self._chunk_buffer) == 0:
             return 0
 
+        if self._current_session_group is None:
+            raise RuntimeError("No session group selected yet. This should not happen.")
+
         for group_idx, entry_idx, results in utils.iterate_extended_structure_as_entry_list(
             utils.transpose_extended_structures(self._chunk_buffer)
         ):
             self._write_results(
-                g=self.file[f"session/group_{group_idx}/entry_{entry_idx}/result"],
+                g=self._current_session_group[f"group_{group_idx}/entry_{entry_idx}/result"],
                 start_index=start_idx,
                 results=results,
             )
 
         return len(self._chunk_buffer)
 
     def _sample(self, extended_result: list[dict[int, Result]]) -> None:
@@ -232,24 +255,36 @@
             reached_size_limit = len(self._chunk_buffer) >= self._AUTO_CHUNK_MAX_SIZE
             reached_time_limit = (time() - self._last_write_time) >= self._AUTO_CHUNK_MAX_TIME
             write = reached_size_limit or reached_time_limit
         else:
             write = len(self._chunk_buffer) == self._chunk_size
 
         if write:
-            self._num_frames += self._write_chunk_buffer_to_file(start_idx=self._num_frames)
+            self._num_frames_current_session += self._write_chunk_buffer_to_file(
+                start_idx=self._num_frames_current_session
+            )
             self._chunk_buffer = []
             self._last_write_time = time()
 
-    def _stop(self) -> Any:
-        self._num_frames += self._write_chunk_buffer_to_file(start_idx=self._num_frames)
-        self._chunk_buffer = []
+    def _stop_session(self) -> None:
+        if len(self._chunk_buffer) > 0:
+            _ = self._write_chunk_buffer_to_file(start_idx=self._num_frames_current_session)
+            self._chunk_buffer = []
+        self._num_frames_current_session = 0
 
-        if self.owns_file:
-            self.file.close()
+    def close(self) -> Any:
+        try:
+            self._stop_session()
+
+            # If the client has self as an attached recorder, make sure to detatch it.
+            if self._attachable is not None:
+                _ = self._attachable.detach_recorder()
+        finally:
+            if self.owns_file:
+                self.file.close()
 
     @staticmethod
     def _create_result_datasets(g: h5py.Group, metadata: Metadata) -> None:
         g.create_dataset(
             "data_saturated",
             shape=(0,),
             maxshape=(None,),
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,114 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
-from typing import Iterator, Optional
+from typing import Iterator, Optional, Sequence
 
 import attrs
 
 from acconeer.exptool.a121._core import utils
 from acconeer.exptool.a121._core.entities import (
     ClientInfo,
     Metadata,
     Record,
     RecordException,
     Result,
     SensorCalibration,
     ServerInfo,
     SessionConfig,
+    SessionRecord,
     StackedResults,
 )
 
 
 class InMemoryRecordException(Exception):
     pass
 
 
 @attrs.frozen(kw_only=True)
-class InMemoryRecord(Record):
-    _client_info: ClientInfo = attrs.field()
-    _extended_metadata: list[dict[int, Metadata]] = attrs.field()
-    _extended_stacked_results: list[dict[int, StackedResults]] = attrs.field()
-    _lib_version: str = attrs.field()
-    _num_frames: int = attrs.field()
-    _server_info: ServerInfo = attrs.field()
-    _session_config: SessionConfig = attrs.field()
-    _timestamp: str = attrs.field()
-    _uuid: str = attrs.field()
-    _calibrations: Optional[dict[int, SensorCalibration]] = attrs.field()
-    _calibrations_provided: Optional[dict[int, bool]] = attrs.field()
-
-    @property
-    def client_info(self) -> ClientInfo:
-        return self._client_info
-
-    @property
-    def extended_metadata(self) -> list[dict[int, Metadata]]:
-        return self._extended_metadata
+class InMemorySessionRecord(SessionRecord):
+    extended_metadata: list[dict[int, Metadata]]
+    extended_stacked_results: list[dict[int, StackedResults]]
+    num_frames: int
+    session_config: SessionConfig
+    _calibrations: Optional[dict[int, SensorCalibration]]
+    _calibrations_provided: Optional[dict[int, bool]]
 
     @property
     def extended_results(self) -> Iterator[list[dict[int, Result]]]:
         for frame_no in range(self.num_frames):
             yield self._get_result_for_all_entries(frame_no)
 
-    def _get_result_for_all_entries(self, frame_no: int) -> list[dict[int, Result]]:
-        def stacked_results_to_result(stacked_results: StackedResults) -> Result:
-            return stacked_results[frame_no]
-
-        return utils.map_over_extended_structure(
-            stacked_results_to_result, self._extended_stacked_results
-        )
-
-    @property
-    def extended_stacked_results(self) -> list[dict[int, StackedResults]]:
-        return self._extended_stacked_results
-
-    @property
-    def lib_version(self) -> str:
-        return self._lib_version
-
-    @property
-    def num_frames(self) -> int:
-        return self._num_frames
-
-    @property
-    def server_info(self) -> ServerInfo:
-        return self._server_info
-
-    @property
-    def session_config(self) -> SessionConfig:
-        return self._session_config
-
     @property
     def sensor_id(self) -> int:
-        return self._session_config.sensor_id
-
-    @property
-    def timestamp(self) -> str:
-        return self._timestamp
-
-    @property
-    def uuid(self) -> str:
-        return self._uuid
+        return self.session_config.sensor_id
 
     @property
     def calibrations(self) -> dict[int, SensorCalibration]:
         if self._calibrations is None:
             raise InMemoryRecordException("No calibration in record")
         return self._calibrations
 
     @property
     def calibrations_provided(self) -> dict[int, bool]:
         if self._calibrations_provided is None:
             raise InMemoryRecordException("No calibration in record")
         return self._calibrations_provided
 
+    def _get_result_for_all_entries(self, frame_no: int) -> list[dict[int, Result]]:
+        def stacked_results_to_result(stacked_results: StackedResults) -> Result:
+            return stacked_results[frame_no]
+
+        return utils.map_over_extended_structure(
+            stacked_results_to_result, self.extended_stacked_results
+        )
+
     @classmethod
-    def from_record(cls, record: Record) -> InMemoryRecord:
+    def from_session_record(cls, session_record: SessionRecord) -> InMemorySessionRecord:
         try:
-            calibrations = record.calibrations
-            calibrations_provided = record.calibrations_provided
+            calibrations = session_record.calibrations
+            calibrations_provided = session_record.calibrations_provided
         except RecordException:
             calibrations = None
             calibrations_provided = None
 
         return cls(
+            extended_metadata=session_record.extended_metadata,
+            extended_stacked_results=session_record.extended_stacked_results,
+            num_frames=session_record.num_frames,
+            session_config=session_record.session_config,
+            calibrations=calibrations,
+            calibrations_provided=calibrations_provided,
+        )
+
+
+@attrs.frozen(kw_only=True)
+class InMemoryRecord(Record):
+    client_info: ClientInfo
+    lib_version: str
+    server_info: ServerInfo
+    timestamp: str
+    uuid: str
+    _sessions: Sequence[InMemorySessionRecord]
+
+    def session(self, session_index: int) -> InMemorySessionRecord:
+        return self._sessions[session_index]
+
+    @property
+    def num_sessions(self) -> int:
+        return len(self._sessions)
+
+    @classmethod
+    def from_record(cls, record: Record) -> InMemoryRecord:
+        return cls(
             client_info=record.client_info,
-            extended_metadata=record.extended_metadata,
-            extended_stacked_results=record.extended_stacked_results,
             lib_version=record.lib_version,
-            num_frames=record.num_frames,
             server_info=record.server_info,
-            session_config=record.session_config,
             timestamp=record.timestamp,
             uuid=record.uuid,
-            calibrations=calibrations,
-            calibrations_provided=calibrations_provided,
+            sessions=tuple(
+                InMemorySessionRecord.from_session_record(record.session(i))
+                for i in range(record.num_sessions)
+            ),
         )
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/utils.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_core/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core_ext/_replaying_client.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,152 +1,139 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
-import time
-from typing import Any, Dict, Iterator, List, Optional, Union, cast
+import abc
+import enum
+import json
+import warnings
+from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 
-from acconeer.exptool.a121 import (
-    Client,
-    ClientError,
-    ClientInfo,
-    Metadata,
-    Record,
-    Recorder,
-    Result,
-    SensorCalibration,
-    SensorConfig,
-    ServerInfo,
-    SessionConfig,
-)
-
-
-class _StopReplay(Exception):
-    pass
-
-
-class _ReplayingClient(Client):
-    def __init__(self, record: Record):
-        self._record = record
-        self._is_started: bool = False
-        self._result_iterator: Optional[
-            Union[Iterator[Result], Iterator[list[dict[int, Result]]]]
-        ] = None
-        self._origin_time: Optional[float] = None
-
-    def _assert_connected(self) -> None:
-        if not self.connected:
-            raise ClientError("Client is not connected.")
-
-    def _assert_session_setup(self) -> None:
-        self._assert_connected()
-        if not self.session_is_setup:
-            raise ClientError("Session is not set up.")
-
-    def _assert_session_started(self) -> None:
-        self._assert_session_setup()
-        if not self.session_is_started:
-            raise ClientError("Session is not started.")
+import attrs
 
-    def _open(self) -> None:
-        pass
-
-    def setup_session(
-        self,
-        config: Union[SensorConfig, SessionConfig],
-        calibrations: Optional[dict[int, SensorCalibration]] = None,
-    ) -> Union[Metadata, list[dict[int, Metadata]]]:
-        if isinstance(config, SensorConfig):
-            config = SessionConfig(config)
-
-        if config != self._record.session_config:
-            raise ValueError
-
-        if self.session_config.extended:
-            return self._record.extended_metadata
-        else:
-            return self._record.metadata
-
-    def start_session(self, recorder: Optional[Recorder] = None) -> None:
-        if recorder is not None:
-            raise ValueError(f"{type(self).__name__} can not record")
-
-        if self.session_config.extended:
-            self._result_iterator = self._record.extended_results
-        else:
-            self._result_iterator = self._record.results
+from acconeer.exptool import a121
+from acconeer.exptool.a121._core.utils import EntityJSONEncoder
 
-        self._is_started = True
-        self._origin_time = None
 
-    def get_next(self) -> Union[Result, list[dict[int, Result]]]:
-        if not self.session_is_setup:
-            raise ClientError("Session is not set up.")
+AlgoBaseT = TypeVar("AlgoBaseT", bound="AlgoBase")
+InputT = TypeVar("InputT", a121.Result, List[Dict[int, a121.Result]])
+MetadataT = TypeVar("MetadataT", a121.Metadata, List[Dict[int, a121.Metadata]])
+ConfigT = TypeVar("ConfigT", bound="AlgoConfigBase")
+ProcessorConfigT = TypeVar("ProcessorConfigT", bound="AlgoProcessorConfigBase")
+ParamEnumT = TypeVar("ParamEnumT", bound="AlgoParamEnum")
+ResultT = TypeVar("ResultT")
 
-        assert self._result_iterator is not None
 
-        try:
-            result_ = next(self._result_iterator)
-            result = cast(Union[Result, List[Dict[int, Result]]], result_)
-        except StopIteration:
-            raise _StopReplay
-
-        if isinstance(result, Result):
-            some_result = result
-        else:
-            some_result = next(iter(next(iter(result)).values()))
-
-        now = time.monotonic() - some_result.tick_time
+class GenericProcessorBase(abc.ABC, Generic[InputT, ProcessorConfigT, ResultT, MetadataT]):
+    def __init__(
+        self,
+        *,
+        sensor_config: a121.SensorConfig,
+        metadata: MetadataT,
+        processor_config: ProcessorConfigT,
+    ) -> None:
+        self.sensor_config = sensor_config
+        self.metadata: MetadataT = metadata
+        self.processor_config = processor_config
+
+    @abc.abstractmethod
+    def process(self, result: InputT) -> ResultT:
+        ...
+
+    @abc.abstractmethod
+    def update_config(self, config: ProcessorConfigT) -> None:
+        ...
+
+
+ProcessorBase = GenericProcessorBase[a121.Result, ProcessorConfigT, ResultT, a121.Metadata]
+ExtendedProcessorBase = GenericProcessorBase[
+    List[Dict[int, a121.Result]], ProcessorConfigT, ResultT, List[Dict[int, a121.Metadata]]
+]
+
+
+class Controller(abc.ABC, Generic[ConfigT, ResultT]):
+    def __init__(self, *, client: a121.Client, config: ConfigT):
+        self.client = client
+        self.config = config
+
+    @abc.abstractmethod
+    def start(self, recorder: Optional[a121.Recorder] = None) -> None:
+        ...
+
+    @abc.abstractmethod
+    def get_next(self) -> ResultT:
+        ...
+
+    @abc.abstractmethod
+    def stop(self) -> Any:
+        ...
+
+
+@attrs.mutable(slots=False)
+class AlgoBase:
+    def to_dict(self) -> dict[str, Any]:
+        return attrs.asdict(self)
+
+    @classmethod
+    def from_dict(cls: type[AlgoBaseT], d: dict[str, Any]) -> AlgoBaseT:
+        return cls(**d)
+
+    def to_json(self) -> str:
+        return json.dumps(self.to_dict(), cls=EntityJSONEncoder)
+
+    @classmethod
+    def from_json(cls: type[AlgoBaseT], json_str: str) -> AlgoBaseT:
+        return cls.from_dict(json.loads(json_str))
+
+
+@attrs.mutable(slots=False)
+class AlgoConfigBase(AlgoBase, abc.ABC):
+    def validate(self) -> None:
+        """Performs self-validation
+
+        :raises ValidationError: If anything is invalid.
+        """
+        for validation_result in self._collect_validation_results():
+            try:
+                raise validation_result
+            except a121.ValidationWarning as vw:
+                warnings.warn(vw.message)
 
-        if self._origin_time is None:
-            self._origin_time = now
+    @abc.abstractmethod
+    def _collect_validation_results(self) -> list[a121.ValidationResult]:
+        pass
 
-        delta = now - self._origin_time
 
-        if delta < 0:
-            time.sleep(-delta)
+@attrs.mutable(slots=False)
+class AlgoProcessorConfigBase(AlgoBase, abc.ABC):
+    def validate(self, config: Union[a121.SensorConfig, a121.SessionConfig]) -> None:
+        """Performs self-validation and validation of its session config
+
+        :raises ValidationError: If anything is invalid.
+        """
+        if isinstance(config, a121.SensorConfig):
+            config = a121.SessionConfig(config)
+
+        for validation_result in self._collect_validation_results(config):
+            try:
+                raise validation_result
+            except a121.ValidationWarning as vw:
+                warnings.warn(vw.message)
+
+    @abc.abstractmethod
+    def _collect_validation_results(
+        self, config: a121.SessionConfig
+    ) -> list[a121.ValidationResult]:
+        pass
 
-        return result
 
-    def stop_session(self) -> Any:
-        self._result_iterator = None
-        self._is_started = False
+class AlgoParamEnum(enum.Enum):
+    # TODO: Share with config_enums.py (?)
 
-    def close(self) -> None:
-        pass
+    @classmethod
+    def _missing_(cls: type[ParamEnumT], value: object) -> Optional[ParamEnumT]:
+        for member in cls:
+            if member.name == value:
+                return member
 
-    @property
-    def connected(self) -> bool:
-        return True
-
-    @property
-    def session_is_setup(self) -> bool:
-        return True
-
-    @property
-    def session_is_started(self) -> bool:
-        return self._is_started
-
-    @property
-    def server_info(self) -> ServerInfo:
-        return self._record.server_info
-
-    @property
-    def client_info(self) -> ClientInfo:
-        return self._record.client_info
-
-    @property
-    def session_config(self) -> SessionConfig:
-        return self._record.session_config
-
-    @property
-    def extended_metadata(self) -> list[dict[int, Metadata]]:
-        return self._record.extended_metadata
-
-    @property
-    def calibrations(self) -> dict[int, SensorCalibration]:
-        return self._record.calibrations
-
-    @property
-    def calibrations_provided(self) -> dict[int, bool]:
-        return self._record.calibrations_provided
+        return None
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_perf_calc.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_perf_calc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_rate_calc.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/_rate_calc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/__init__.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/_a121.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/_a121.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,14 @@
     PLUGIN_PRESETS: Mapping[int, Callable[[], ProcessorPluginPreset[ProcessorConfigT]]] = {}
 
     def __init__(
         self, callback: Callable[[Message], None], generation: PluginGeneration, key: str
     ):
         super().__init__(callback=callback, generation=generation, key=key)
         self._processor_instance = None
-        self._recorder = None
         self._log = BackendLogger.getLogger(__name__)
         self.restore_defaults()
 
     def _load_from_cache(self, file: h5py.File) -> None:
         self.shared_state.session_config = a121.SessionConfig.from_json(file["session_config"][()])
         self.shared_state.processor_config = self.get_processor_config_cls().from_json(
             file["processor_config"][()]
@@ -129,46 +128,52 @@
         """Hook for validating session configs."""
         pass
 
     def _start_session(self, recorder: Optional[a121.H5Recorder]) -> None:
         session_config = self.shared_state.session_config
         self._validate_session_config(session_config)
 
+        assert self.client
         if recorder:
             algo_group = recorder.require_algo_group(self.key)  # noqa: F841
 
             # TODO: break out saving (?)
             _create_h5_string_dataset(
                 algo_group, "processor_config", self.shared_state.processor_config.to_json()
             )
-        assert self.client
+
+            self.client.attach_recorder(recorder)
+
         metadata = self.client.setup_session(session_config)
         the_first_sensor_config = next(
             _core.utils.iterate_extended_structure_values(session_config.groups)
         )
         self._processor_instance = self.get_processor_cls()(
             sensor_config=the_first_sensor_config,  # FIXME: a bit scuffed but wth
             metadata=metadata,  # type: ignore[arg-type]
             processor_config=self.shared_state.processor_config,
         )
 
         self.shared_state.metadata = metadata  # type: ignore[assignment]
-        self.client.start_session(self._recorder)
+        self.client.start_session()
 
         self.callback(
             GeneralMessage(
                 name="setup",
                 kwargs=dict(metadata=metadata, sensor_config=the_first_sensor_config),
                 recipient="plot_plugin",
             )
         )
 
     def end_session(self) -> None:
         if self.client is None:
             raise RuntimeError("Client is not attached. Can not 'stop'.")
+
+        if self._recorder is not None:
+            self._recorder.close()
         self.client.stop_session()
 
     @classmethod
     @abc.abstractmethod
     def get_processor_cls(
         cls,
     ) -> Type[GenericProcessorBase[InputT, ProcessorConfigT, ResultT, MetadataT]]:
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_utils.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/_utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/bilateration/_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/bilateration/_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,16 @@
                 recipient="plot_plugin",
             )
         )
 
     def end_session(self) -> None:
         if self._detector_instance is None:
             raise RuntimeError
+        if self._recorder is not None:
+            self._recorder.close()
         self._detector_instance.stop()
 
     def get_next(self) -> None:
         if self._detector_instance is None:
             raise RuntimeError
         detector_result = self._detector_instance.get_next()
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/bilateration/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/bilateration/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/breathing/_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/breathing/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/breathing/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/__main__.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_aggregator.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/_aggregator.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_detector.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -893,15 +893,17 @@
                     self.config,
                     self.context,
                 )
             else:
                 # Should never happen as we currently only have the H5Recorder
                 warnings.warn("Will not save algo data")
 
-        self.client.start_session(recorder)
+            self.client.attach_recorder(recorder)
+
+        self.client.start_session()
         self.started = True
 
     def get_next(self) -> Dict[int, DetectorResult]:
         """Called from host to get next measurement."""
         if not self.started:
             raise RuntimeError("Not started")
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,16 @@
                 kwargs=dict(num_curves=len(self._detector_instance.processor_specs)),
                 recipient="plot_plugin",
             )
         )
 
     def end_session(self) -> None:
         assert self._detector_instance
+        if self._recorder is not None:
+            self._recorder.close()
         self._detector_instance.stop()
 
     def get_next(self) -> None:
         if self._detector_instance is None:
             raise RuntimeError
 
         assert self.client
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_processors.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_serializers.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/distance/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_configs.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/presence/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_detector.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/presence/_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,17 @@
                     self.sensor_id,
                     self.config,
                 )
             else:
                 # Should never happen as we currently only have the H5Recorder
                 warnings.warn("Will not save algo data")
 
-        self.client.start_session(recorder)
+            self.client.attach_recorder(recorder)
+
+        self.client.start_session()
 
         self.started = True
 
     @classmethod
     def _get_sensor_config(cls, config: DetectorConfig) -> a121.SensorConfig:
         start_point = int(np.floor(config.start_m / Processor.APPROX_BASE_STEP_LENGTH_M))
         if config.profile is not None:
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,16 @@
                 recipient="plot_plugin",
             )
         )
 
     def end_session(self) -> None:
         if self._detector_instance is None:
             raise RuntimeError
+        if self._recorder is not None:
+            self._recorder.close()
         self._detector_instance.stop()
 
     def get_next(self) -> None:
         assert self.client
         if self._detector_instance is None:
             raise RuntimeError
         result = self._detector_instance.get_next()
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_processors.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/presence/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_serializers.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/presence/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_configs.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/smart_presence/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/smart_presence/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,16 @@
                 recipient="plot_plugin",
             )
         )
 
     def end_session(self) -> None:
         if self._ref_app_instance is None:
             raise RuntimeError
+        if self._recorder is not None:
+            self._recorder.close()
         self._ref_app_instance.stop()
 
     def get_next(self) -> None:
         assert self.client
         if self._ref_app_instance is None:
             raise RuntimeError
         result = self._ref_app_instance.get_next()
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,17 @@
                     self.sensor_id,
                     self.config,
                 )
             else:
                 # Should never happen as we currently only have the H5Recorder
                 warnings.warn("Will not save algo data")
 
-        self.client.start_session(recorder)
+            self.client.attach_recorder(recorder)
+
+        self.client.start_session()
 
         self.started = True
 
     @classmethod
     def _get_sensor_config(cls, config: ExampleAppConfig) -> a121.SensorConfig:
         optimal_distance = config.surface_distance / np.cos(np.radians(config.sensor_angle))
         optimal_point = int(np.ceil(optimal_distance / APPROX_BASE_STEP_LENGTH_M))
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,16 @@
                 recipient="plot_plugin",
             )
         )
 
     def end_session(self) -> None:
         if self._example_app_instance is None:
             raise RuntimeError
+        if self._recorder is not None:
+            self._recorder.close()
         self._example_app_instance.stop()
 
     def get_next(self) -> None:
         assert self.client
         if self._example_app_instance is None:
             raise RuntimeError
         result = self._example_app_instance.get_next()
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_configs.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/tank_level/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/tank_level/_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,18 @@
                 recipient="plot_plugin",
             )
         )
 
     def end_session(self) -> None:
         if self._ref_app_instance is None:
             raise RuntimeError
+
+        if self._recorder is not None:
+            self._recorder.close()
+
         self._ref_app_instance.stop()
 
     def get_next(self) -> None:
         assert self.client is not None
         if self._ref_app_instance is None:
             raise RuntimeError
         result = self._ref_app_instance.get_next()
@@ -410,51 +414,72 @@
             and result.peak_detected is not None
             and result.peak_status is not None
         ):
             current_level = result.level
             peak_detected = result.peak_detected
             peak_status = result.peak_status
 
-            level_text = self.STATUS_MSG_MAP[peak_status]
-            if peak_status == ProcessorLevelStatus.OVERFLOW:
-                for rect in self.rects:
-                    rect.setBrush(et.utils.pg_brush_cycler(0))
-            elif peak_detected and (peak_status == ProcessorLevelStatus.IN_RANGE):
-                self.bar_loc = round(current_level / (self.end_m - self.start_m) * self.num_rects)
-                for rect in self.rects[: self.bar_loc]:
-                    rect.setBrush(et.utils.pg_brush_cycler(0))
-
-                for rect in self.rects[self.bar_loc :]:
-                    rect.setBrush(et.utils.pg_brush_cycler(1))
-
-                level_text = "Level: {:.1f} cm, {:.0f} %".format(
-                    current_level * 100,
-                    current_level / (self.end_m - self.start_m) * 100,
-                )
-                self.counter = 0
-            elif peak_detected and (peak_status == ProcessorLevelStatus.OUT_OF_RANGE):
+            # Show the percentage level plot if the plot width is greater than 600 pixels,
+            # otherwise display the level as text.
+            if self.plot_layout.width() >= 600:
+                level_text = self.STATUS_MSG_MAP[peak_status]
+                if peak_status == ProcessorLevelStatus.OVERFLOW:
+                    for rect in self.rects:
+                        rect.setBrush(et.utils.pg_brush_cycler(0))
+                elif peak_detected and (peak_status == ProcessorLevelStatus.IN_RANGE):
+                    self.bar_loc = round(
+                        current_level / (self.end_m - self.start_m) * self.num_rects
+                    )
+                    for rect in self.rects[: self.bar_loc]:
+                        rect.setBrush(et.utils.pg_brush_cycler(0))
+
+                    for rect in self.rects[self.bar_loc :]:
+                        rect.setBrush(et.utils.pg_brush_cycler(1))
+
+                    level_text = "Level: {:.1f} cm, {:.0f} %".format(
+                        current_level * 100,
+                        current_level / (self.end_m - self.start_m) * 100,
+                    )
+                    self.counter = 0
+                elif peak_detected and (peak_status == ProcessorLevelStatus.OUT_OF_RANGE):
+                    for rect in self.rects:
+                        rect.setBrush(et.utils.pg_brush_cycler(1))
+                elif ~peak_detected and (self.counter <= NO_DETECTION_TIMEOUT):
+                    for rect in self.rects[: self.bar_loc]:
+                        rect.setBrush(et.utils.pg_brush_cycler(0))
+
+                    for rect in self.rects[self.bar_loc :]:
+                        rect.setBrush(et.utils.pg_brush_cycler(1))
+
+                    self.counter += 1
+                else:
+                    for rect in self.rects:
+                        rect.setBrush(et.utils.pg_brush_cycler(1))
+                        self.bar_loc = 0
                 for rect in self.rects:
-                    rect.setBrush(et.utils.pg_brush_cycler(1))
-            elif ~peak_detected and (self.counter <= NO_DETECTION_TIMEOUT):
-                for rect in self.rects[: self.bar_loc]:
-                    rect.setBrush(et.utils.pg_brush_cycler(0))
+                    rect.setVisible(True)
 
-                for rect in self.rects[self.bar_loc :]:
-                    rect.setBrush(et.utils.pg_brush_cycler(1))
-
-                self.counter += 1
+                level_html = self.level_html_format.format(level_text)
+                self.level_text_item.setHtml(level_html)
+                self.level_text_item.setPos(self.num_rects / 4.0, self.num_rects + 4.0)
+                self.level_text_item.show()
             else:
+                level_text = self.STATUS_MSG_MAP[peak_status]
+                if peak_detected and (peak_status == ProcessorLevelStatus.IN_RANGE):
+                    level_text = "Level: {:.1f} cm, {:.0f} %".format(
+                        current_level * 100,
+                        current_level / (self.end_m - self.start_m) * 100,
+                    )
+                    self.counter = 0
+                level_html = self.level_html_format.format(level_text)
+                self.level_text_item.setHtml(level_html)
+                self.level_text_item.setPos(self.num_rects / 4.0, self.num_rects + 4.0)
+                self.level_text_item.show()
                 for rect in self.rects:
-                    rect.setBrush(et.utils.pg_brush_cycler(1))
-                    self.bar_loc = 0
-
-            level_html = self.level_html_format.format(level_text)
-            self.level_text_item.setHtml(level_html)
-            self.level_text_item.setPos(self.num_rects / 4.0, self.num_rects + 4.0)
-            self.level_text_item.show()
+                    rect.setVisible(False)
 
 
 class ViewPlugin(DetectorViewPluginBase):
 
     TEXT_MSG_MAP = {
         DetailedStatus.OK: "Ready to start.",
         DetailedStatus.CONTEXT_MISSING: "Run detector calibration.",
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/tank_level/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_serializer.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/tank_level/_serializer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_configs.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/touchless_button/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/touchless_button/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/vibration/_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/vibration/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/vibration/_processor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/a121/algo/vibration/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/launcher.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/launcher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/__init__.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/_argument_parser.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/_argument_parser.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/_enums.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/_enums.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/_version_checker.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/_version_checker.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/app_model.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/app_model/app_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/app_model_listener.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/app_model/app_model_listener.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/file_detective.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/app_model/file_detective.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/port_updater.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/app_model/port_updater.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_application_client.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/backend/_application_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from __future__ import annotations
 
 from typing import Any, Callable, Optional, TypeVar, Union, cast
 
 from acconeer.exptool.a121 import Client, Result, _RateCalculator
 from acconeer.exptool.a121._core import utils
-from acconeer.exptool.a121._core.mediators import Recorder
 
 from ._message import GeneralMessage, Message
 
 
 ClientT = TypeVar("ClientT", bound=Client)
 
 
@@ -41,16 +40,16 @@
         typing perspective.
 
         The cast is necessary as we are dealing with magic here, but should hold
         up so long any overriden functions have the same type as the overriders.
         """
         return cast(ClientT, cls(wrapped_client, callback))
 
-    def start_session(self, recorder: Optional[Recorder] = None) -> None:
-        self._wrapped_client.start_session(recorder)
+    def start_session(self) -> None:
+        self._wrapped_client.start_session()
         assert self._wrapped_client.session_config is not None
         assert self._wrapped_client.extended_metadata is not None
 
         if self._wrapped_client.session_config.extended:
             self._rate_stats_calc = _RateCalculator(
                 self._wrapped_client.session_config, self._wrapped_client.extended_metadata
             )
@@ -63,13 +62,13 @@
         assert self._rate_stats_calc is not None
         self._rate_stats_calc.update(results)
         self.callback(GeneralMessage(name="rate_stats", data=self._rate_stats_calc.stats))
         self._frame_count += 1
         self.callback(GeneralMessage(name="frame_count", data=self._frame_count))
         return results
 
-    def stop_session(self) -> Any:
+    def stop_session(self) -> None:
         result = self._wrapped_client.stop_session()
         self._frame_count = 0
         self.callback(GeneralMessage(name="rate_stats", data=None))
         self.callback(GeneralMessage(name="frame_count", data=None))
         return result
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_backend.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/backend/_backend.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_backend_logger.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/backend/_backend_logger.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_backend_plugin.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/backend/_backend_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_message.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/backend/_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_model.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/backend/_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/plugin_loader.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/storage.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/storage.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/app_model_viewer.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/app_model_viewer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/device_comboboxes.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/device_comboboxes.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/flash_tab/threads.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/flash_tab/threads.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/help_tab.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/help_tab.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/icons.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/icons.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/main_window.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/misc.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/misc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/utils.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/plugin_components/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/status_bar.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/status_bar.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/hints.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/stream_tab/hints.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/utils.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/new/ui/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/app.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/data_processing.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/data_processing.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/helper.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/elements/helper.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/modules.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/elements/modules.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/qt_subclasses.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/old/elements/qt_subclasses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/a111_gui.png` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/resources/a111_gui.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/a121_gui.png` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/resources/a121_gui.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/icon-black.svg` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/resources/icon-black.svg`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/icon.png` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/resources/icon.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/loader.gif` & `acconeer-exptool-7.0.0/src/acconeer/exptool/app/resources/loader.gif`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/LICENSE.txt` & `acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44` & `acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll` & `acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll` & `acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44` & `acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44` & `acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll` & `acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll` & `acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44` & `acconeer-exptool-7.0.0/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_bin_fetcher.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_bin_fetcher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_dev_license.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_dev_license.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_dev_license_tui.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_dev_license_tui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_flasher.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_flasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_products.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_products.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/libft4222.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/libft4222.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/mpl_process.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/mpl_process.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/pg_process.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/pg_process.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/__main__.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/setup/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/platform_install.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/setup/base/platform_install.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/prompts.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/setup/base/prompts.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/setup_group.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/setup/base/setup_group.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/setup_step.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/setup/base/setup_step.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/utils.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/setup/base/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/cli/argument_parser.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/setup/cli/argument_parser.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/platforms/linux.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/setup/platforms/linux.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer/exptool/utils.py` & `acconeer-exptool-7.0.0/src/acconeer/exptool/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/PKG-INFO` & `acconeer-exptool-7.0.0/src/acconeer_exptool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acconeer-exptool
-Version: 6.0.5
+Version: 7.0.0
 Summary: Acconeer Exploration Tool
 Home-page: https://github.com/acconeer/acconeer-python-exploration
 Author: Acconeer AB
 Author-email: tools@acconeer.com
 License: BSD 3-Clause Clear License
 Project-URL: Tracker, https://github.com/acconeer/acconeer-python-exploration/issues
 Project-URL: Documentation, https://acconeer-python-exploration.readthedocs.io
```

### Comparing `acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/SOURCES.txt` & `acconeer-exptool-7.0.0/src/acconeer_exptool.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,15 @@
 src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py
 src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py
 src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py
 src/acconeer/exptool/a121/_core/peripherals/h5_record/__init__.py
 src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py
 src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py
 src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py
+src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py
 src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py
 src/acconeer/exptool/a121/_core/peripherals/im_record/__init__.py
 src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py
 src/acconeer/exptool/a121/_core_ext/__init__.py
 src/acconeer/exptool/a121/_core_ext/_replaying_client.py
 src/acconeer/exptool/a121/algo/__init__.py
 src/acconeer/exptool/a121/algo/_base.py
```

### Comparing `acconeer-exptool-6.0.5/tools/check_changelog.py` & `acconeer-exptool-7.0.0/tools/check_changelog.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/tools/check_copyright.py` & `acconeer-exptool-7.0.0/tools/check_copyright.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/tools/check_line_length.py` & `acconeer-exptool-7.0.0/tools/check_line_length.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/tools/check_permissions.py` & `acconeer-exptool-7.0.0/tools/check_permissions.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/tools/check_sdk_mentions.py` & `acconeer-exptool-7.0.0/tools/check_sdk_mentions.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/tools/check_whitespace.py` & `acconeer-exptool-7.0.0/tools/check_whitespace.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/tools/update_regmap.py` & `acconeer-exptool-7.0.0/tools/update_regmap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.5/utils/convert_to_csv.py` & `acconeer-exptool-7.0.0/utils/convert_to_csv.py`

 * *Files identical despite different names*

