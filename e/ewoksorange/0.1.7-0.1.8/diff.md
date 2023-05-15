# Comparing `tmp/ewoksorange-0.1.7.tar.gz` & `tmp/ewoksorange-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksorange-0.1.7.tar", last modified: Fri Mar 31 15:02:36 2023, max compression
+gzip compressed data, was "dist/ewoksorange-0.1.8.tar", last modified: Mon May 15 16:51:31 2023, max compression
```

## Comparing `ewoksorange-0.1.7.tar` & `ewoksorange-0.1.8.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2878 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2128 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2021 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/
--rw-rw-rw-   0 root         (0) root         (0)      357 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4498 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/bindings.py
--rw-rw-rw-   0 root         (0) root         (0)      959 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/events.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/invalid_data.py
--rw-rw-rw-   0 root         (0) root         (0)    16499 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/owsconvert.py
--rw-rw-rw-   0 root         (0) root         (0)      362 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/owsettings.py
--rw-rw-rw-   0 root         (0) root         (0)     7939 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/owsignal_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     8602 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/owsignals.py
--rw-rw-rw-   0 root         (0) root         (0)    23568 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/owwidgets.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     4639 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/qtapp.py
--rw-rw-rw-   0 root         (0) root         (0)     1962 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/taskexecutor.py
--rw-rw-rw-   0 root         (0) root         (0)     2649 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/taskexecutor_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     7999 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/bindings/taskwrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/canvas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/canvas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/canvas/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      796 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/canvas/config.py
--rw-rw-rw-   0 root         (0) root         (0)     6705 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/canvas/handler.py
--rw-rw-rw-   0 root         (0) root         (0)     3130 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/canvas/main.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/canvas/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/gui/orange_imports.py
--rw-rw-rw-   0 root         (0) root         (0)    21108 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/gui/parameterform.py
--rw-rw-rw-   0 root         (0) root         (0)     2640 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/gui/simpletypesmixin.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/orange_version.py
--rw-rw-rw-   0 root         (0) root         (0)     9630 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/registration.py
--rw-rw-rw-   0 root         (0) root         (0)     6751 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/setuptools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2157 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/ewoks_example_1_addon/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/ewoks_example_1_addon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/ewoks_example_1_addon/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/adder1.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/adder2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/icons/category.svg
--rw-rw-rw-   0 root         (0) root         (0)     3070 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/icons/sum.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/tutorials/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2527 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/tutorials/sumtask_tutorial2.ows
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/adder1.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/adder2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/icons/category.svg
--rw-rw-rw-   0 root         (0) root         (0)     3070 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/icons/sum.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/tutorials/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1532 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/tutorials/mixed_tutorial1.ows
--rw-rw-rw-   0 root         (0) root         (0)     2462 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/tutorials/sumtask_tutorial1.ows
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/
--rw-rw-rw-   0 root         (0) root         (0)      947 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/
--rw-rw-rw-   0 root         (0) root         (0)      574 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      896 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/adder1.py
--rw-rw-rw-   0 root         (0) root         (0)      896 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/adder2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/icons/category.svg
--rw-rw-rw-   0 root         (0) root         (0)     3070 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/icons/sum.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/tutorials/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2662 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/tutorials/sumtask_tutorial3.ows
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/ewoks_example_2_addon/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/ewoks_example_2_addon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/ewoks_example_2_addon/widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/icons/category.svg
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/icons/mywidget.svg
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/listgenerator.py
--rw-rw-rw-   0 root         (0) root         (0)      374 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/print_sum.py
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/sumlist_one_thread.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/sumlist_several_thread.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/sumlist_stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/tutorials/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2916 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/tutorials/sumlist_tutorial.ows
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      912 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/listoperations.py
--rw-rw-rw-   0 root         (0) root         (0)     1364 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_default_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     2061 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_ows_conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     5245 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_parameterform.py
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_register_addon.py
--rw-rw-rw-   0 root         (0) root         (0)     2148 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_task_executor.py
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     6254 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_tutorials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_widgets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_widgets/ewoks_example_1_addon/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_widgets/ewoks_example_1_addon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1891 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_widgets/ewoks_example_1_addon/test_adder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_widgets/ewoks_example_2_addon/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_widgets/ewoks_example_2_addon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1459 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_widgets/ewoks_example_2_addon/test_listoperations.py
--rw-rw-rw-   0 root         (0) root         (0)     3772 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/test_workflow_events.py
--rw-rw-rw-   0 root         (0) root         (0)      734 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/ewoksorange/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2878 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7952 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      489 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      254 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/ewoksorange.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/orangecontrib/
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/orangecontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksdemo/
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksdemo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksdemo/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksdemo/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksdemo/icons/category.svg
--rw-rw-rw-   0 root         (0) root         (0)     3070 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksdemo/icons/sum.png
--rw-rw-rw-   0 root         (0) root         (0)      885 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksdemo/sumtask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksdemo/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksdemo/tutorials/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3489 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksdemo/tutorials/ewoksdemo_acyclic1.ows
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksnowidget/
--rw-rw-rw-   0 root         (0) root         (0)     2374 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksnowidget/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:02:36.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksnowidget/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 15:02:30.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksnowidget/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksnowidget/icons/category.svg
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksnowidget/icons/mywidget.svg
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-03-31 14:55:31.000000 ewoksorange-0.1.7/src/orangecontrib/ewoksnowidget/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2878 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2128 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1924 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2023-05-15 16:43:15.000000 ewoksorange-0.1.8/src/ewoksorange/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4498 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/bindings.py
+-rw-rw-rw-   0 root         (0) root         (0)      959 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/events.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/invalid_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    16499 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/owsconvert.py
+-rw-rw-rw-   0 root         (0) root         (0)      362 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/owsettings.py
+-rw-rw-rw-   0 root         (0) root         (0)     7939 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/owsignal_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     8602 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/owsignals.py
+-rw-rw-rw-   0 root         (0) root         (0)    23568 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/owwidgets.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     4639 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/qtapp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1962 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/taskexecutor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2649 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/taskexecutor_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     8011 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/bindings/taskwrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/canvas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/canvas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/canvas/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      796 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/canvas/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6705 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/canvas/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     3130 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/canvas/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/canvas/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/gui/orange_imports.py
+-rw-rw-rw-   0 root         (0) root         (0)    21108 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/gui/parameterform.py
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/gui/simpletypesmixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/orange_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     9630 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/registration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6751 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/setuptools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/ewoks_example_1_addon/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/ewoks_example_1_addon/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/ewoks_example_1_addon/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/adder1.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/adder2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/icons/category.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3070 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/icons/sum.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/tutorials/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2527 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/tutorials/sumtask_tutorial2.ows
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/adder1.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/adder2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/icons/category.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3070 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/icons/sum.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/tutorials/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1532 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/tutorials/mixed_tutorial1.ows
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/tutorials/sumtask_tutorial1.ows
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/
+-rw-rw-rw-   0 root         (0) root         (0)      947 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      896 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/adder1.py
+-rw-rw-rw-   0 root         (0) root         (0)      896 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/adder2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/icons/category.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3070 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/icons/sum.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/tutorials/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2662 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/tutorials/sumtask_tutorial3.ows
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/ewoks_example_2_addon/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/ewoks_example_2_addon/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/ewoks_example_2_addon/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/icons/category.svg
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/icons/mywidget.svg
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/listgenerator.py
+-rw-rw-rw-   0 root         (0) root         (0)      374 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/print_sum.py
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/sumlist_one_thread.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/sumlist_several_thread.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/sumlist_stack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/tutorials/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2916 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/tutorials/sumlist_tutorial.ows
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/listoperations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_default_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_ows_conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     5245 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_parameterform.py
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_register_addon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2148 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_task_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     6278 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_tutorials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_widgets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_widgets/ewoks_example_1_addon/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_widgets/ewoks_example_1_addon/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_widgets/ewoks_example_1_addon/test_adder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_widgets/ewoks_example_2_addon/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_widgets/ewoks_example_2_addon/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_widgets/ewoks_example_2_addon/test_listoperations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3772 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/test_workflow_events.py
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/ewoksorange/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2878 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7952 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      254 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/ewoksorange.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/orangecontrib/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/orangecontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksdemo/
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksdemo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksdemo/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksdemo/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksdemo/icons/category.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3070 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksdemo/icons/sum.png
+-rw-rw-rw-   0 root         (0) root         (0)      885 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksdemo/sumtask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksdemo/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksdemo/tutorials/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3489 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksdemo/tutorials/ewoksdemo_acyclic1.ows
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksnowidget/
+-rw-rw-rw-   0 root         (0) root         (0)     2374 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksnowidget/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:31.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksnowidget/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:25.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksnowidget/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksnowidget/icons/category.svg
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksnowidget/icons/mywidget.svg
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-05-15 15:49:58.000000 ewoksorange-0.1.8/src/orangecontrib/ewoksnowidget/widgets.py
```

### Comparing `ewoksorange-0.1.7/LICENSE.md` & `ewoksorange-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/PKG-INFO` & `ewoksorange-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksorange
-Version: 0.1.7
+Version: 0.1.8
 Summary: Orange binding for Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksorange/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksorange/
 Project-URL: Documentation, https://ewoksorange.readthedocs.io/
```

### Comparing `ewoksorange-0.1.7/README.md` & `ewoksorange-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/setup.cfg` & `ewoksorange-0.1.8/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	ewokscore >=0.3.1
+	ewokscore >=0.4.1
 	PyQt5
 	orange-canvas-core
 	orange-widget-base
 namespace_packages = 
 	orangecontrib
 
 [options.packages.find]
@@ -71,19 +71,14 @@
 ignore = E501, E203, W503
 max-line-length = 88
 exclude = 
 	.eggs
 	src/ewoksorange/tests/examples/ewoks_example_1_addon/doc/conf.py
 	src/ewoksorange/tests/examples/ewoks_example_2_addon/doc/conf.py
 
-[build_sphinx]
-project = ewoksorange
-version = attr: ewoksorange.__version__
-source-dir = ./doc
-
 [coverage:run]
 omit = 
 	setup.py
 	src/ewoksorange/tests/*
 
 [egg_info]
 tag_build =
```

### Comparing `ewoksorange-0.1.7/src/ewoksorange/bindings/bindings.py` & `ewoksorange-0.1.8/src/ewoksorange/bindings/bindings.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/bindings/events.py` & `ewoksorange-0.1.8/src/ewoksorange/bindings/events.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/bindings/invalid_data.py` & `ewoksorange-0.1.8/src/ewoksorange/bindings/invalid_data.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/bindings/owsconvert.py` & `ewoksorange-0.1.8/src/ewoksorange/bindings/owsconvert.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/bindings/owsignal_manager.py` & `ewoksorange-0.1.8/src/ewoksorange/bindings/owsignal_manager.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/bindings/owsignals.py` & `ewoksorange-0.1.8/src/ewoksorange/bindings/owsignals.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/bindings/owwidgets.py` & `ewoksorange-0.1.8/src/ewoksorange/bindings/owwidgets.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/bindings/progress.py` & `ewoksorange-0.1.8/src/ewoksorange/bindings/progress.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/bindings/qtapp.py` & `ewoksorange-0.1.8/src/ewoksorange/bindings/qtapp.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/bindings/taskexecutor.py` & `ewoksorange-0.1.8/src/ewoksorange/bindings/taskexecutor.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/bindings/taskexecutor_queue.py` & `ewoksorange-0.1.8/src/ewoksorange/bindings/taskexecutor_queue.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/bindings/taskwrapper.py` & `ewoksorange-0.1.8/src/ewoksorange/bindings/taskwrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         input_names=input_names,
         optional_input_names=optional_input_names,
         output_names=output_names,
         registry_name=registry_name,
     ):
         def run(self):
             output_values = execute_ewoks_owwidget(
-                widget_class, inputs=self.input_values
+                widget_class, inputs=self.get_input_values()
             )
             for k, v in output_values.items():
                 self.output_variables[k].value = v
 
     return WrapperTask
 
 
@@ -88,15 +88,15 @@
         input_names=input_names,
         optional_input_names=optional_input_names,
         output_names=output_names,
         registry_name=registry_name,
     ):
         def run(self):
             output_values = execute_native_owwidget(
-                widget_class, inputs=self.input_values
+                widget_class, inputs=self.get_input_values()
             )
             for k, v in output_values.items():
                 self.output_variables[k].value = v
 
     return WrapperTask
```

### Comparing `ewoksorange-0.1.7/src/ewoksorange/canvas/config.py` & `ewoksorange-0.1.8/src/ewoksorange/canvas/config.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/canvas/handler.py` & `ewoksorange-0.1.8/src/ewoksorange/canvas/handler.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/canvas/main.py` & `ewoksorange-0.1.8/src/ewoksorange/canvas/main.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/canvas/utils.py` & `ewoksorange-0.1.8/src/ewoksorange/canvas/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/gui/orange_imports.py` & `ewoksorange-0.1.8/src/ewoksorange/gui/orange_imports.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/gui/parameterform.py` & `ewoksorange-0.1.8/src/ewoksorange/gui/parameterform.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/gui/simpletypesmixin.py` & `ewoksorange-0.1.8/src/ewoksorange/gui/simpletypesmixin.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/registration.py` & `ewoksorange-0.1.8/src/ewoksorange/registration.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/setuptools.py` & `ewoksorange-0.1.8/src/ewoksorange/setuptools.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/conftest.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/__init__.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/adder1.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/adder1.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/adder2.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/adder2.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/icons/sum.png` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/icons/sum.png`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/tutorials/sumtask_tutorial2.ows` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/evaluate/ewoks_example_submodule/tutorials/sumtask_tutorial2.ows`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/__init__.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/adder1.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/adder1.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/adder2.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/adder2.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/icons/sum.png` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/icons/sum.png`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/tutorials/mixed_tutorial1.ows` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/tutorials/mixed_tutorial1.ows`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/tutorials/sumtask_tutorial1.ows` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_category/tutorials/sumtask_tutorial1.ows`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/__init__.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/__init__.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/adder1.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/adder1.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/adder2.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/adder2.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/icons/sum.png` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/icons/sum.png`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/tutorials/sumtask_tutorial3.ows` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_1_addon/orangecontrib/ewoks_example_supercategory/ewoks_example_subcategory/tutorials/sumtask_tutorial3.ows`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/ewoks_example_2_addon/widgets.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/ewoks_example_2_addon/widgets.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/__init__.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/icons/mywidget.svg` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/icons/mywidget.svg`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/sumlist_one_thread.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/sumlist_one_thread.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/sumlist_several_thread.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/sumlist_several_thread.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/sumlist_stack.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/sumlist_stack.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/tutorials/sumlist_tutorial.ows` & `ewoksorange-0.1.8/src/ewoksorange/tests/examples/ewoks_example_2_addon/orangecontrib/list_operations/tutorials/sumlist_tutorial.ows`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/listoperations.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/listoperations.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/test_default_widget.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/test_default_widget.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/test_examples.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/test_ows_conversion.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/test_ows_conversion.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/test_parameterform.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/test_parameterform.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/test_register_addon.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/test_register_addon.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/test_task_executor.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/test_task_executor.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/test_tutorials.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/test_tutorials.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     assert results == {"result": 16}
 
 
 def assert_sumtask_tutorial_without_qt(filename):
     """Execute workflow after converting it to an ewoks workflow"""
     graph = ows_to_ewoks(filename)
     results = execute_graph(graph, output_tasks=True)
-    assert results["5"].output_values == {"result": 16}
+    assert results["5"].get_output_values() == {"result": 16}
 
 
 def assert_sumlist_tutorial_with_qt(ewoks_orange_canvas, filename):
     """Execute workflow using the Qt widgets and signals"""
     ewoks_orange_canvas.load_ows(str(filename))
 
     # Remove artificial delay for this test
@@ -140,17 +140,17 @@
     # Remove artificial delay for this test
     for attrs in graph.graph.nodes.values():
         for adict in attrs.get("default_inputs", list()):
             if adict["name"] == "delay":
                 adict["value"] = 0
 
     results = execute_graph(graph, output_tasks=True)
-    listsum = sum(results["0"].output_values["list"])
+    listsum = sum(results["0"].get_output_values()["list"])
     for i in [4, 5, 6]:
-        assert results[str(i)].input_values == {"sum": listsum}
+        assert results[str(i)].get_input_values() == {"sum": listsum}
 
 
 def assert_mixed_tutorial_with_qt(ewoks_orange_canvas, filename):
     """Execute workflow using the Qt widgets and signals"""
     ewoks_orange_canvas.load_ows(str(filename))
     ewoks_orange_canvas.start_workflow()
     ewoks_orange_canvas.wait_widgets(timeout=10)
@@ -159,8 +159,8 @@
     assert results == {"result": 3}
 
 
 def assert_mixed_tutorial_without_qt(filename):
     """Execute workflow after converting it to an ewoks workflow"""
     graph = ows_to_ewoks(filename)
     results = execute_graph(graph, output_tasks=True)
-    assert results["1"].output_values == {"result": 3}
+    assert results["1"].get_output_values() == {"result": 3}
```

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/test_widgets/ewoks_example_1_addon/test_adder.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/test_widgets/ewoks_example_1_addon/test_adder.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     node_attrs = {
         "task_type": "generated",
         "task_identifier": widget_qualname,
         "task_generator": OWWIDGET_TASKS_GENERATOR,
     }
     task = instantiate_task("node_id", node_attrs, inputs={"a": 1, "b": 2})
     task.execute()
-    assert task.output_values == {"result": 3}
+    assert task.get_output_values() == {"result": 3}
 
 
 @pytest.mark.parametrize("widget_qualname", _WIDGETS)
 def test_adder_missing_inputs(widget_qualname, register_ewoks_example_1_addon):
     node_attrs = {
         "task_type": "generated",
         "task_identifier": widget_qualname,
```

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/test_widgets/ewoks_example_2_addon/test_listoperations.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/test_widgets/ewoks_example_2_addon/test_listoperations.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/test_workflow_events.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/test_workflow_events.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/ewoksorange/tests/utils.py` & `ewoksorange-0.1.8/src/ewoksorange/tests/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 ) -> dict:
     """Execute the task (use the orange widget or ewoks task class) and return the results"""
     if issubclass(task_cls, OWEwoksBaseWidget):
         return execute_ewoks_owwidget(task_cls, inputs=inputs, timeout=timeout)
     if issubclass(task_cls, Task):
         task = task_cls(inputs=inputs)
         task.execute()
-        return task.output_values
+        return task.get_output_values()
     raise TypeError("task")
```

### Comparing `ewoksorange-0.1.7/src/ewoksorange.egg-info/PKG-INFO` & `ewoksorange-0.1.8/src/ewoksorange.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksorange
-Version: 0.1.7
+Version: 0.1.8
 Summary: Orange binding for Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksorange/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksorange/
 Project-URL: Documentation, https://ewoksorange.readthedocs.io/
```

### Comparing `ewoksorange-0.1.7/src/ewoksorange.egg-info/SOURCES.txt` & `ewoksorange-0.1.8/src/ewoksorange.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/orangecontrib/ewoksdemo/icons/sum.png` & `ewoksorange-0.1.8/src/orangecontrib/ewoksdemo/icons/sum.png`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/orangecontrib/ewoksdemo/sumtask.py` & `ewoksorange-0.1.8/src/orangecontrib/ewoksdemo/sumtask.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/orangecontrib/ewoksdemo/tutorials/ewoksdemo_acyclic1.ows` & `ewoksorange-0.1.8/src/orangecontrib/ewoksdemo/tutorials/ewoksdemo_acyclic1.ows`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/orangecontrib/ewoksnowidget/__init__.py` & `ewoksorange-0.1.8/src/orangecontrib/ewoksnowidget/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksorange-0.1.7/src/orangecontrib/ewoksnowidget/icons/mywidget.svg` & `ewoksorange-0.1.8/src/orangecontrib/ewoksnowidget/icons/mywidget.svg`

 * *Files identical despite different names*

