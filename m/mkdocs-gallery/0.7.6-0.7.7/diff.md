# Comparing `tmp/mkdocs-gallery-0.7.6.tar.gz` & `tmp/mkdocs-gallery-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mkdocs-gallery-0.7.6.tar", last modified: Sat May  7 14:58:16 2022, max compression
+gzip compressed data, was "mkdocs-gallery-0.7.7.tar", last modified: Mon Apr 24 09:27:50 2023, max compression
```

## Comparing `mkdocs-gallery-0.7.6.tar` & `mkdocs-gallery-0.7.7.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     5877 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/.github/workflows/base.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3379 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6960 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/ci_tools/
--rw-r--r--   0 runner    (1001) docker     (121)    17413 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/ci_tools/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/ci_tools/check_python_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/ci_tools/flake8-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5754 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/ci_tools/github_release.py
--rw-r--r--   0 runner    (1001) docker     (121)    29255 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/ci_tools/nox_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)   230273 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/_static/demo.png
--rw-r--r--   0 runner    (1001) docker     (121)    15415 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/_static/plotly_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/docs/binder_cfg/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/binder_cfg/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4389 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/local_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/docs/examples/no_output/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/no_output/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/no_output/just_code.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/no_output/plot_raise.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/no_output/plot_strings.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/no_output/plot_syntaxerror.py
--rw-r--r--   0 runner    (1001) docker     (121)     4098 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/plot_0_sin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/plot_1_exp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/plot_2_seaborn.py
--rw-r--r--   0 runner    (1001) docker     (121)     4882 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/plot_3_capture_repr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/plot_4_choose_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/plot_4b_provide_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/plot_5_unicode_everywhere.py
--rw-r--r--   0 runner    (1001) docker     (121)     2071 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/plot_6_function_identifier.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/plot_7_sys_argv.py
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/plot_8_animations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2881 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/examples/plot_9_plotly.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/gallery_conf.py
--rw-r--r--   0 runner    (1001) docker     (121)    11844 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)     2385 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/long_description.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/tutorials/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3176 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/docs/tutorials/plot_parse.py
--rw-r--r--   0 runner    (1001) docker     (121)     2849 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/noxfile-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13315 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2239 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-05-07 14:58:15.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    13751 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/backreferences.py
--rw-r--r--   0 runner    (1001) docker     (121)     9667 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/binder.py
--rw-r--r--   0 runner    (1001) docker     (121)    18336 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/docs_resolv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/downloads.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    33737 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/gen_data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    37963 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/gen_gallery.py
--rw-r--r--   0 runner    (1001) docker     (121)    43653 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/gen_single.py
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/mkdocs_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)    10453 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/notebook.py
--rw-r--r--   0 runner    (1001) docker     (121)    19945 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     7374 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/py_source_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    19903 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/scrapers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4212 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/sorting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/
--rw-r--r--   0 runner    (1001) docker     (121)     3380 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/binder_badge_logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)    21404 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/broken_example.png
--rw-r--r--   0 runner    (1001) docker     (121)    53268 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/broken_stamp.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4315 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/no_image.png
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/sg_gallery-binder.css
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/sg_gallery-dataframe.css
--rw-r--r--   0 runner    (1001) docker     (121)     3714 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/sg_gallery-rendered-html.css
--rw-r--r--   0 runner    (1001) docker     (121)     4426 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/sg_gallery.css
--rw-r--r--   0 runner    (1001) docker     (121)    11127 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3379 2022-05-07 14:58:15.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2494 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-07 14:58:15.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-05-07 14:58:15.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-07 14:58:15.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-05-07 14:58:15.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/src/mkdocs_gallery.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 14:58:16.000000 mkdocs-gallery-0.7.6/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3715 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/tests/reference_parse.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    33070 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/tests/test_gen_md.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/tests/test_packaging.py
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-05-07 14:57:19.000000 mkdocs-gallery-0.7.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.713727 mkdocs-gallery-0.7.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.701727 mkdocs-gallery-0.7.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.701727 mkdocs-gallery-0.7.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/.github/workflows/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-24 09:27:50.713727 mkdocs-gallery-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.705727 mkdocs-gallery-0.7.7/ci_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/ci_tools/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/ci_tools/check_python_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/ci_tools/flake8-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/ci_tools/github_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29340 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/ci_tools/nox_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.705727 mkdocs-gallery-0.7.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.705727 mkdocs-gallery-0.7.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   230273 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/_static/demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/_static/plotly_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.705727 mkdocs-gallery-0.7.7/docs/binder_cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/binder_cfg/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.705727 mkdocs-gallery-0.7.7/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/local_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.709727 mkdocs-gallery-0.7.7/docs/examples/no_output/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/no_output/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/no_output/just_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/no_output/plot_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/no_output/plot_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/no_output/plot_syntaxerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/plot_0_sin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/plot_1_exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/plot_2_seaborn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/plot_3_capture_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/plot_4_choose_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/plot_4b_provide_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/plot_5_unicode_everywhere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/plot_6_function_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/plot_7_sys_argv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/plot_8_animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/examples/plot_9_plotly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/gallery_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/long_description.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.709727 mkdocs-gallery-0.7.7/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/tutorials/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/docs/tutorials/plot_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/noxfile-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-24 09:27:50.717727 mkdocs-gallery-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.701727 mkdocs-gallery-0.7.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.709727 mkdocs-gallery-0.7.7/src/mkdocs_gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 09:27:50.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/backreferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/binder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18336 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/docs_resolv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33737 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/gen_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37963 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/gen_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43653 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/gen_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/mkdocs_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21112 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/py_source_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19903 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/scrapers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/sorting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.713727 mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/binder_badge_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21404 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/broken_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53268 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/broken_stamp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/no_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/sg_gallery-binder.css
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/sg_gallery-dataframe.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/sg_gallery-rendered-html.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/sg_gallery.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.713727 mkdocs-gallery-0.7.7/src/mkdocs_gallery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-24 09:27:50.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-24 09:27:50.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:27:50.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 09:27:50.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:27:35.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 09:27:50.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 09:27:50.000000 mkdocs-gallery-0.7.7/src/mkdocs_gallery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:50.713727 mkdocs-gallery-0.7.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/tests/reference_parse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33070 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/tests/test_gen_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/tests/test_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-24 09:26:56.000000 mkdocs-gallery-0.7.7/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mkdocs-gallery-0.7.6/.github/workflows/base.yml` & `mkdocs-gallery-0.7.7/.github/workflows/base.yml`

 * *Files 22% similar despite different names*

```diff
@@ -8,130 +8,145 @@
     tags:
       - '*'
     branches:
       - main
   pull_request:
     branches:
       - main
+
+defaults:
+  run:
+    shell: bash -l {0}
+
 jobs:
   # pre-job to read nox tests matrix - see https://stackoverflow.com/q/66747359/7262247
   list_nox_test_sessions:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v1
+      - name: Checkout
+        uses: actions/checkout@v2
+
+      - name: Install python 3.9
+        uses: actions/setup-python@v4
         with:
-          python-version: 3.7
+          python-version: 3.9
           architecture: x64
 
       - name: Install noxfile requirements
-        shell: bash -l {0}
         run: pip install -r noxfile-requirements.txt
 
-      - name: List 'tests' nox sessions
+      - name: List 'tests' nox sessions and required python versions
         id: set-matrix
-        run: echo "::set-output name=matrix::$(nox -s gha_list -- tests)"
+        run: echo "::set-output name=matrix::$(nox -s gha_list -- -s tests -v)"
+
     outputs:
       matrix: ${{ steps.set-matrix.outputs.matrix }}  # save nox sessions list to outputs
 
   run_all_tests:
     needs: list_nox_test_sessions
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu-latest, windows-latest ]  # , macos-latest, windows-latest]
         # all nox sessions: manually > dynamically from previous job
         # nox_session: ["tests-2.7", "tests-3.7"]
         nox_session: ${{ fromJson(needs.list_nox_test_sessions.outputs.matrix) }}
 
-    name: ${{ matrix.os }} ${{ matrix.nox_session }} # ${{ matrix.name_suffix }}
+    name: ${{ matrix.os }} ${{ matrix.nox_session.python }} ${{ matrix.nox_session.session }} # ${{ matrix.name_suffix }}
     runs-on: ${{ matrix.os }}
     steps:
-      - uses: actions/checkout@v2
+      - name: Checkout
+        uses: actions/checkout@v2
 
-      # Conda install
-      - name: Install conda v3.7
-        uses: conda-incubator/setup-miniconda@v2
-        with:
-          # auto-update-conda: true
-          python-version: 3.7
-          activate-environment: noxenv
-      - run: conda info
-        shell: bash -l {0}  # so that conda works
-      - run: conda list
-        shell: bash -l {0}  # so that conda works
+      - name: Install python ${{ matrix.nox_session.python }} for tests
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.nox_session.python }}
+          architecture: x64
+
+      - name: Install python 3.9 for nox
+        uses: actions/setup-python@v4
+        with:
+          python-version: 3.9
+          architecture: x64
 
-      # Nox install + run
       - name: Install noxfile requirements
-        shell: bash -l {0}  # so that conda works
         run: pip install -r noxfile-requirements.txt
-      - run: conda list
-        shell: bash -l {0}  # so that conda works
-      - run: nox -s "${{ matrix.nox_session }}"
-        shell: bash -l {0}  # so that conda works
+
+      - name: Run nox session ${{ matrix.nox_session.session }}
+        run: nox -s "${{ matrix.nox_session.session }}"
 
       # Share ./docs/reports so that they can be deployed with doc in next job
       - name: Share reports with other jobs
         # if: matrix.nox_session == '...': not needed, if empty wont be shared
         uses: actions/upload-artifact@master
         with:
           name: reports_dir
           path: ./docs/reports
 
+#  build_doc: useless in our case since own doc is part of the tests session
+#    runs-on: ubuntu-latest
+#    if: github.event_name == 'pull_request'
+#    steps:
+#      - name: Checkout
+#        uses: actions/checkout@v2
+#
+#      - name: Install python 3.9 for nox
+#        uses: actions/setup-python@v4
+#        with:
+#          python-version: 3.9
+#          architecture: x64
+#
+#      - name: Install noxfile requirements
+#        run: pip install -r noxfile-requirements.txt
+#
+#      - name: Build the doc including example gallery
+#        run: nox -s docs -- build
+
   publish_release:
     needs: run_all_tests
     runs-on: ubuntu-latest
     if: github.event_name == 'push'
     steps:
       - name: GitHub context to debug conditional steps
         env:
           GITHUB_CONTEXT: ${{ toJSON(github) }}
         run: echo "$GITHUB_CONTEXT"
 
-      - uses: actions/checkout@v2
+      - name: Checkout with no depth
+        uses: actions/checkout@v2
         with:
           fetch-depth: 0  # so that gh-deploy works
 
+      - name: Install python 3.9 for nox
+        uses: actions/setup-python@v4
+        with:
+          python-version: 3.9
+          architecture: x64
+
       # 1) retrieve the reports generated previously
       - name: Retrieve reports
         uses: actions/download-artifact@master
         with:
           name: reports_dir
           path: ./docs/reports
 
-      # Conda install
-      - name: Install conda v3.7
-        uses: conda-incubator/setup-miniconda@v2
-        with:
-          # auto-update-conda: true
-          python-version: 3.7
-          activate-environment: noxenv
-      - run: conda info
-        shell: bash -l {0}  # so that conda works
-      - run: conda list
-        shell: bash -l {0}  # so that conda works
-
       # Nox install
       - name: Install noxfile requirements
-        shell: bash -l {0}  # so that conda works
         run: pip install -r noxfile-requirements.txt
-      - run: conda list
-        shell: bash -l {0}  # so that conda works
 
       # 5) Run the flake8 report and badge
       - name: Run flake8 analysis and generate corresponding badge
-        shell: bash -l {0}  # so that conda works
         run: nox -s flake8
 
       # -------------- only on Ubuntu + MAIN PUSH (no pull request, no tag) -----------
 
       # 5) Publish the doc and test reports
       - name: \[not on TAG\] Publish documentation, tests and coverage reports
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/heads')  # startsWith(matrix.os,'ubuntu')
-        shell: bash -l {0}  # so that conda works
         run: nox -s publish
 
       # 6) Publish coverage report
       - name: \[not on TAG\] Create codecov.yaml with correct paths
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/heads')
         shell: bash
         run: |
@@ -147,15 +162,14 @@
           files: ./docs/reports/coverage/coverage.xml
 
       # -------------- only on Ubuntu + TAG PUSH (no pull request) -----------
 
       # 7) Create github release and build the wheel
       - name: \[TAG only\] Build wheel and create github release
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
-        shell: bash -l {0}  # so that conda works
         run: nox -s release -- ${{ secrets.GITHUB_TOKEN }}
 
       # 8) Publish the wheel on PyPi
       - name: \[TAG only\] Deploy on PyPi
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
```

### Comparing `mkdocs-gallery-0.7.6/.gitignore` & `mkdocs-gallery-0.7.7/.gitignore`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/.zenodo.json` & `mkdocs-gallery-0.7.7/.zenodo.json`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/LICENSE` & `mkdocs-gallery-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/PKG-INFO` & `mkdocs-gallery-0.7.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: mkdocs-gallery
-Version: 0.7.6
+Version: 0.7.7
 Summary: a `mkdocs` plugin to generate example galleries from python scripts, similar to `sphinx-gallery`.
 Home-page: https://github.com/smarie/mkdocs-gallery
-Download-URL: https://github.com/smarie/mkdocs-gallery/tarball/0.7.6
+Download-URL: https://github.com/smarie/mkdocs-gallery/tarball/0.7.7
 Author: Sylvain MARIE <sylvain.marie@se.com>
 License: BSD 3-Clause
 Keywords: gallery web page generator figure jupyter notebook binder example code latex mkdocs sphinx
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: Topic :: Documentation
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mkdocs-gallery
 
 *[Sphinx-Gallery](https://sphinx-gallery.github.io/) features for [mkdocs](https://www.mkdocs.org/) (no [Sphinx](sphinx-doc.org/) dependency !).*
 
@@ -32,9 +33,7 @@
 Do you love [Sphinx-Gallery](https://sphinx-gallery.github.io/) but prefer [mkdocs](https://www.mkdocs.org/) over [Sphinx](sphinx-doc.org/) for your documentation ? `mkdocs-gallery` was written for you ;) 
 
 It relies on [mkdocs-material](https://squidfunk.github.io/mkdocs-material) to get the most of mkdocs, so that your galleries look nice!
 
 The documentation for users is available here: [https://smarie.github.io/mkdocs-gallery/](https://smarie.github.io/mkdocs-gallery/)
 
 A readme for developers is available here: [https://github.com/smarie/mkdocs-gallery](https://github.com/smarie/mkdocs-gallery)
-
-
```

### Comparing `mkdocs-gallery-0.7.6/README.md` & `mkdocs-gallery-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/ci_tools/.pylintrc` & `mkdocs-gallery-0.7.7/ci_tools/.pylintrc`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/ci_tools/check_python_version.py` & `mkdocs-gallery-0.7.7/ci_tools/check_python_version.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/ci_tools/github_release.py` & `mkdocs-gallery-0.7.7/ci_tools/github_release.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/ci_tools/nox_utils.py` & `mkdocs-gallery-0.7.7/ci_tools/nox_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import nox
 from nox.sessions import Session
 
 
 nox_logger = logging.getLogger("nox")
 
 
-PY27, PY35, PY36, PY37, PY38, PY39, PY310 = "2.7", "3.5", "3.6", "3.7", "3.8", "3.9", "3.10"
+PY27, PY35, PY36, PY37, PY38, PY39, PY310, PY311 = "2.7", "3.5", "3.6", "3.7", "3.8", "3.9", "3.10", "3.11"
 DONT_INSTALL = "dont_install"
 
 
 def power_session(
         func=None,
         envs=None,
         grid_param_name="env",
@@ -318,15 +318,18 @@
      - sub-list of these requirements that should be installed with conda, from [tool.my_conda] conda_packages
     """
     if os.path.exists("pyproject.toml"):
         import toml
         nox_logger.debug("\nA `pyproject.toml` file exists. Loading it.")
         pyproject = toml.load("pyproject.toml")
         requires = pyproject['build-system']['requires']
-        conda_pkgs = pyproject['tool']['conda']['conda_packages']
+        try:
+            conda_pkgs = pyproject['tool']['conda']['conda_packages']
+        except KeyError:
+            conda_pkgs = ()
         return requires, conda_pkgs
     else:
         raise FileNotFoundError("No `pyproject.toml` file exists. No dependency will be installed ...")
 
 
 SetupCfg = namedtuple('SetupCfg', ('setup_requires', 'install_requires', 'tests_requires', 'extras_require'))
```

### Comparing `mkdocs-gallery-0.7.6/docs/_static/demo.png` & `mkdocs-gallery-0.7.7/docs/_static/demo.png`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/_static/plotly_logo.png` & `mkdocs-gallery-0.7.7/docs/_static/plotly_logo.png`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/changelog.md` & `mkdocs-gallery-0.7.7/docs/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+### 0.7.7 - Bugfixes and new python versions
+
+ - Official support for python 3.10 and 3.11. PR [#52](https://github.com/smarie/mkdocs-gallery/pull/52) by [GenevieveBuckley](https://github.com/GenevieveBuckley)
+ - Fixed `AttributeError: MySubConfig has no '_pre_validate'` with `mkdocs` version `1.4` or greater. Fixes [#57](https://github.com/smarie/mkdocs-gallery/issues/57)
+
 ### 0.7.6 - Bugfixes
 
  - Fixed incorrect img `srcset` paths leading to figures not being displayed in gallery examples. Fixes [#47](https://github.com/smarie/mkdocs-gallery/issues/47)
  - Fixed `TypeError: startswith first arg must be str or a tuple of str, not WindowsPath` when running with `mkdocs serve`. Fixes [#45](https://github.com/smarie/mkdocs-gallery/isues/45). PR [#46](https://github.com/smarie/mkdocs-gallery/pull/46) by [mchaaler](https://github.com/mchaaler).
 
 ### 0.7.5 - Bugfixes
```

### Comparing `mkdocs-gallery-0.7.6/docs/examples/README.md` & `mkdocs-gallery-0.7.7/docs/examples/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/examples/no_output/just_code.py` & `mkdocs-gallery-0.7.7/docs/examples/no_output/just_code.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/examples/no_output/plot_raise.py` & `mkdocs-gallery-0.7.7/docs/examples/no_output/plot_raise.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/examples/plot_0_sin.py` & `mkdocs-gallery-0.7.7/docs/examples/plot_0_sin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/examples/plot_1_exp.py` & `mkdocs-gallery-0.7.7/docs/examples/plot_1_exp.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/examples/plot_2_seaborn.py` & `mkdocs-gallery-0.7.7/docs/examples/plot_2_seaborn.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/examples/plot_3_capture_repr.py` & `mkdocs-gallery-0.7.7/docs/examples/plot_3_capture_repr.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/examples/plot_4_choose_thumbnail.py` & `mkdocs-gallery-0.7.7/docs/examples/plot_4_choose_thumbnail.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/examples/plot_4b_provide_thumbnail.py` & `mkdocs-gallery-0.7.7/docs/examples/plot_4b_provide_thumbnail.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/examples/plot_5_unicode_everywhere.py` & `mkdocs-gallery-0.7.7/docs/examples/plot_5_unicode_everywhere.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/examples/plot_6_function_identifier.py` & `mkdocs-gallery-0.7.7/docs/examples/plot_6_function_identifier.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/examples/plot_7_sys_argv.py` & `mkdocs-gallery-0.7.7/docs/examples/plot_7_sys_argv.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/examples/plot_8_animations.py` & `mkdocs-gallery-0.7.7/docs/examples/plot_8_animations.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/examples/plot_9_plotly.py` & `mkdocs-gallery-0.7.7/docs/examples/plot_9_plotly.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/index.md` & `mkdocs-gallery-0.7.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/long_description.md` & `mkdocs-gallery-0.7.7/docs/long_description.md`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/docs/tutorials/plot_parse.py` & `mkdocs-gallery-0.7.7/docs/tutorials/plot_parse.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/mkdocs.yml` & `mkdocs-gallery-0.7.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/noxfile.py` & `mkdocs-gallery-0.7.7/noxfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,42 @@
+import argparse
 from itertools import product
 from json import dumps
 import logging
 
 import nox  # noqa
 from pathlib import Path  # noqa
 import sys
 
 # add parent folder to python path so that we can import noxfile_utils.py
 # note that you need to "pip install -r noxfile-requiterements.txt" for this file to work.
 sys.path.append(str(Path(__file__).parent / "ci_tools"))
-from nox_utils import PY27, PY37, PY36, PY35, PY38, PY39, PY310, power_session, rm_folder, rm_file, PowerSession  # noqa
+from nox_utils import PY27, PY37, PY36, PY35, PY38, PY39, PY310, PY311, power_session, rm_folder, rm_file, PowerSession  # noqa
 
 
 pkg_name = "mkdocs_gallery"
 gh_org = "smarie"
 gh_repo = "mkdocs-gallery"
 
 ENVS = {
-    # python 3.10 is not available on conda yet
-    # PY310: {"coverage": False, "pkg_specs": {"pip": ">19"}},
+    PY311: {"coverage": False, "pkg_specs": {"pip": ">19"}},
+    PY310: {"coverage": False, "pkg_specs": {"pip": ">19"}},
     PY39: {"coverage": False, "pkg_specs": {"pip": ">19"}},
-    PY38: {"coverage": False, "pkg_specs": {"pip": ">19"}},
-    PY37: {"coverage": True, "pkg_specs": {"pip": ">19"}},  # , "pytest-html": "1.9.0"
+    PY37: {"coverage": False, "pkg_specs": {"pip": ">19"}},
+    # IMPORTANT: this should be last so that the folder docs/reports is not deleted afterwards
+    PY38: {"coverage": True, "pkg_specs": {"pip": ">19"}},
 }
 
 
 # set the default activated sessions, minimal for CI
 nox.options.sessions = ["tests", "flake8", "docs"]  # , "docs", "gh_pages"
+nox.options.error_on_missing_interpreters = True
 nox.options.reuse_existing_virtualenvs = True  # this can be done using -r
 # if platform.system() == "Windows":  >> always use this for better control
-nox.options.default_venv_backend = "conda"
+nox.options.default_venv_backend = "virtualenv"
 # os.environ["NO_COLOR"] = "True"  # nox.options.nocolor = True does not work
 # nox.options.verbose = True
 
 nox_logger = logging.getLogger("nox")
 # nox_logger.setLevel(logging.INFO)  NO !!!! this prevents the "verbose" nox flag to work !
 
 
@@ -90,18 +93,18 @@
 
     # install CI-only dependencies
     # if install_ci_deps:
     #     session.install2("keyrings.alt")
 
     # list all (conda list alone does not work correctly on github actions)
     # session.run2("conda list")
-    conda_prefix = Path(session.bin)
-    if conda_prefix.name == "bin":
-        conda_prefix = conda_prefix.parent
-    session.run2("conda list", env={"CONDA_PREFIX": str(conda_prefix), "CONDA_DEFAULT_ENV": session.get_session_id()})
+    # conda_prefix = Path(session.bin)
+    # if conda_prefix.name == "bin":
+    #     conda_prefix = conda_prefix.parent
+    # session.run2("conda list", env={"CONDA_PREFIX": str(conda_prefix), "CONDA_DEFAULT_ENV": session.get_session_id()})
 
     # Fail if the assumed python version is not the actual one
     session.run2("python ci_tools/check_python_version.py %s" % session.python)
 
     # finally run all tests
     if not coverage:
         # install self so that it is recognized by pytest
@@ -144,15 +147,15 @@
         # --generates the badge for the test results and fail build if less than x% tests pass
         nox_logger.info("Generating badge for tests coverage")
         # Use our own package to generate the badge
         session.run2("genbadge tests -i '%s' -o '%s' -t 100" % (Folders.test_xml, Folders.test_badge))
         session.run2("genbadge coverage -i '%s' -o '%s'" % (Folders.coverage_xml, Folders.coverage_badge))
 
 
-@power_session(python=PY38, logsdir=Folders.runlogs)
+@power_session(python=PY39, logsdir=Folders.runlogs)
 def flake8(session: PowerSession):
     """Launch flake8 qualimetry."""
 
     session.install("-r", str(Folders.ci_tools / "flake8-requirements.txt"))
     session.install("genbadge[flake8]")
     session.install2('.')
 
@@ -176,15 +179,15 @@
     "statsmodels",
     "plotly",
     # "memory_profiler",
     "pillow"  # PIL, required for image rescaling
 ]
 
 
-@power_session(python=[PY37])
+@power_session(python=[PY39])
 def docs(session: PowerSession):
     """Generates the doc and serves it on a local http server. Pass '-- build' to build statically instead."""
 
     session.install_reqs(phase="docs", phase_reqs=["mkdocs"] + MKDOCS_GALLERY_EXAMPLES_REQS)
 
     # Install the plugin
     session.install2('.')
@@ -192,15 +195,15 @@
     if session.posargs:
         # use posargs instead of "serve"
         session.run2("mkdocs %s" % " ".join(session.posargs))
     else:
         session.run2("mkdocs serve")
 
 
-@power_session(python=[PY37])
+@power_session(python=[PY39])
 def publish(session: PowerSession):
     """Deploy the docs+reports on github pages. Note: this rebuilds the docs"""
 
     session.install_reqs(
         phase="mkdocs",
         phase_reqs=["mkdocs"] + MKDOCS_GALLERY_EXAMPLES_REQS
     )
@@ -223,15 +226,15 @@
     # # keyring set https://app.codecov.io/gh/<org>/<repo> token
     # import keyring  # (note that this import is not from the session env but the main nox env)
     # codecov_token = keyring.get_password("https://app.codecov.io/gh/<org>/<repo>>", "token")
     # # note: do not use --root nor -f ! otherwise "There was an error processing coverage reports"
     # session.run2('codecov -t %s -f %s' % (codecov_token, Folders.coverage_xml))
 
 
-@power_session(python=[PY37])
+@power_session(python=[PY39])
 def release(session: PowerSession):
     """Create a release on github corresponding to the latest tag"""
 
     # Get current tag using setuptools_scm and make sure this is not a dirty/dev one
     from setuptools_scm import get_version  # (note that this import is not from the session env but the main nox env)
     from setuptools_scm.version import guess_next_dev_version
     version = []
@@ -284,27 +287,44 @@
 
 @nox.session(python=False)
 def gha_list(session):
     """(mandatory arg: <base_session_name>) Prints all sessions available for <base_session_name>, for GithubActions."""
 
     # see https://stackoverflow.com/q/66747359/7262247
 
+    # The options
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-s", "--session", help="The nox base session name")
+    parser.add_argument(
+        "-v",
+        "--with_version",
+        action="store_true",
+        default=False,
+        help="Return a list of lists where the first element is the python version and the second the nox session.",
+    )
+    additional_args = parser.parse_args(session.posargs)
+
     # get the desired base session to generate the list for
-    if len(session.posargs) != 1:
-        raise ValueError("This session has a mandatory argument: <base_session_name>")
-    session_func = globals()[session.posargs[0]]
+    session_func = globals()[additional_args.session]
 
     # list all sessions for this base session
     try:
         session_func.parametrize
     except AttributeError:
-        sessions_list = ["%s-%s" % (session_func.__name__, py) for py in session_func.python]
+        if additional_args.with_version:
+            sessions_list = [{"python": py, "session": "%s-%s" % (session_func.__name__, py)} for py in session_func.python]
+        else:
+            sessions_list = ["%s-%s" % (session_func.__name__, py) for py in session_func.python]
     else:
-        sessions_list = ["%s-%s(%s)" % (session_func.__name__, py, param)
-                         for py, param in product(session_func.python, session_func.parametrize)]
+        if additional_args.with_version:
+            sessions_list = [{"python": py, "session": "%s-%s(%s)" % (session_func.__name__, py, param)}
+                             for py, param in product(session_func.python, session_func.parametrize)]
+        else:
+            sessions_list = ["%s-%s(%s)" % (session_func.__name__, py, param)
+                             for py, param in product(session_func.python, session_func.parametrize)]
 
     # print the list so that it can be caught by GHA.
     # Note that json.dumps is optional since this is a list of string.
     # However it is to remind us that GHA expects a well-formatted json list of strings.
     print(dumps(sessions_list))
```

### Comparing `mkdocs-gallery-0.7.6/pyproject.toml` & `mkdocs-gallery-0.7.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [build-system]
 requires = [
     "setuptools>=39.2",
     "setuptools_scm",
-    "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 # pip: no ! does not work in old python 2.7 and not recommended here
 # https://setuptools.readthedocs.io/en/latest/userguide/quickstart.html#basic-use
 
-[tool.conda]
+# [tool.conda]
 # Declare that the following packages should be installed with conda instead of pip
 # Note: this includes packages declared everywhere, here and in setup.cfg
-conda_packages = [
-    "setuptools",
-    "wheel",
-    "pip",
-    "numpy",
-    "pandas",
-    "scikit-learn",
-    "matplotlib",
-    "statsmodels",
-    "plotly",
-]
+# conda_packages = [
+#     "setuptools",
+#     "wheel",
+#     "pip",
+#     "numpy",
+#     "pandas",
+#     "scikit-learn",
+#     "matplotlib",
+#     "statsmodels",
+#     "plotly",
+# ]
 # pytest: not with conda ! does not work in old python 2.7 and 3.5
```

### Comparing `mkdocs-gallery-0.7.6/setup.cfg` & `mkdocs-gallery-0.7.7/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 	Environment :: Plugins
 	Environment :: Web Environment
 	Topic :: Documentation
 	Programming Language :: Python
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 setup_requires = 
 	setuptools_scm
 	pytest-runner
 install_requires = 
 	mkdocs>=1,<2
```

### Comparing `mkdocs-gallery-0.7.6/setup.py` & `mkdocs-gallery-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/__init__.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/backreferences.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/backreferences.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/binder.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/binder.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/docs_resolv.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/docs_resolv.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/downloads.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/downloads.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/errors.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/errors.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/gen_data_model.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/gen_data_model.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/gen_gallery.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/gen_gallery.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/gen_single.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/gen_single.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/mkdocs_compatibility.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/mkdocs_compatibility.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/notebook.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/notebook.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/plugin.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 #  License: 3-clause BSD, <https://github.com/smarie/mkdocs-gallery/blob/master/LICENSE>
 """
 The mkdocs plugin entry point
 """
 import re
 
 from pathlib import Path
+from packaging import version
 
+from mkdocs import __version__ as mkdocs_version_str
 from mkdocs.config.base import ValidationError, Config
 from mkdocs.config import config_options as co
 from mkdocs.exceptions import ConfigurationError
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.files import Files
 from mkdocs.structure.pages import Page
 
@@ -24,14 +26,18 @@
 from . import glr_path_static
 from .binder import copy_binder_files
 # from .docs_resolv import embed_code_links
 from .gen_gallery import parse_config, generate_gallery_md, summarize_failing_examples, fill_mkdocs_nav
 from .utils import is_relative_to
 
 
+mkdocs_version = version.parse(mkdocs_version_str)
+is_mkdocs_14_or_greater = mkdocs_version >= version.parse("1.4")
+
+
 class ConfigList(co.OptionallyRequired):
     """A list or single element of configuration matching a specific ConfigOption"""
 
     def __init__(self, item_config: co.BaseConfigOption, single_elt_allowed: bool = True, **kwargs):
         super().__init__(**kwargs)
         self.single_elt_allowed = single_elt_allowed
         self.item_config = item_config
@@ -50,50 +56,83 @@
             try:
                 result.append(self.item_config.validate(v))
             except ValidationError as e:
                 raise ValidationError(f"Error validating config item #{i+1}: {e}")
         return result
 
 
-class MySubConfig(co.SubConfig):
-    """Same as SubConfig except that it will be an empty dict when nothing is provided by user,
-    instead of a dict with all options containing their default values."""
-
-    def validate(self, value):
-        if value is None or len(value) == 0:
-            return None
-        else:
-            return super(MySubConfig, self).validate(value)
-
-    def run_validation(self, value):
-        """Fix SubConfig: errors and warnings were not caught
-
-        See https://github.com/mkdocs/mkdocs/pull/2710
-        """
-        failed, self.warnings = Config.validate(self)
-        if len(failed) > 0:
-            # get the first failing one
-            key, err = failed[0]
-            raise ConfigurationError(f"Sub-option {key!r} configuration error: {err}")
-
-        return self
-
-
 class Dir(co.Dir):
     """mkdocs.config.config_options.Dir replacement: returns a pathlib object instead of a string"""
     def run_validation(self, value):
         return Path(co.Dir.run_validation(self, value))
 
 
 class File(co.File):
     """mkdocs.config.config_options.File replacement: returns a pathlib object instead of a string"""
     def run_validation(self, value):
         return Path(co.File.run_validation(self, value))
 
 
+# Binder configuration is a "sub config". This has changed in mkdocs 1.4, handling both here.
+if is_mkdocs_14_or_greater:
+    # Construct a class where class attributes are the config options
+    class _BinderOptions(co.Config):
+        # Required keys
+        org = co.Type(str)
+        repo = co.Type(str)
+        dependencies = ConfigList(File(exists=True))
+        # Optional keys
+        branch = co.Type(str, default="gh-pages")
+        binderhub_url = co.URL(default="https://mybinder.org")
+        filepath_prefix = co.Optional(co.Type(str))  # default is None
+        notebooks_dir = co.Optional(co.Type(str))  # default is "notebooks"
+        use_jupyter_lab = co.Optional(co.Type(bool))  # default is False
+
+    def create_binder_config():
+        return co.SubConfig(_BinderOptions)
+else:
+    # Use MySubConfig
+    class MySubConfig(co.SubConfig):
+        """Same as SubConfig except that it will be an empty dict when nothing is provided by user,
+        instead of a dict with all options containing their default values."""
+
+        def validate(self, value):
+            if value is None or len(value) == 0:
+                return None
+            else:
+                return super(MySubConfig, self).validate(value)
+
+        def run_validation(self, value):
+            """Fix SubConfig: errors and warnings were not caught
+
+            See https://github.com/mkdocs/mkdocs/pull/2710
+            """
+            failed, self.warnings = Config.validate(self)
+            if len(failed) > 0:
+                # get the first failing one
+                key, err = failed[0]
+                raise ConfigurationError(f"Sub-option {key!r} configuration error: {err}")
+
+            return self
+
+    def create_binder_config():
+        return MySubConfig(
+            # Required keys
+            ('org', co.Type(str, required=True)),
+            ('repo', co.Type(str, required=True)),
+            ('dependencies', ConfigList(File(exists=True), required=True)),
+            # Optional keys
+            ('branch', co.Type(str, required=True, default="gh-pages")),
+            ('binderhub_url', co.URL(required=True, default="https://mybinder.org")),
+            ('filepath_prefix', co.Type(str)),  # default is None
+            ('notebooks_dir', co.Type(str)),  # default is "notebooks"
+            ('use_jupyter_lab', co.Type(bool)),  # default is False
+        )
+
+
 class GalleryPlugin(BasePlugin):
     #     # Mandatory to display plotly graph within the site
     #     import plotly.io as pio
     #     pio.renderers.default = "sphinx_gallery"
 
     config_scheme = (
         ('conf_script', File(exists=True)),
@@ -118,26 +157,15 @@
         # 'failing_examples': {},  # type: Set[str]
         # 'passing_examples': [],
         # 'stale_examples': [],
         ('run_stale_examples', co.Type(bool)),
         ('expected_failing_examples', ConfigList(File(exists=True))),
         ('thumbnail_size', ConfigList(co.Type(int), single_elt_allowed=False)),
         ('min_reported_time', co.Type(int)),
-        ('binder', MySubConfig(
-            # Required keys
-            ('org', co.Type(str, required=True)),
-            ('repo', co.Type(str, required=True)),
-            ('dependencies', ConfigList(File(exists=True), required=True)),
-            # Optional keys
-            ('branch', co.Type(str, required=True, default="gh-pages")),
-            ('binderhub_url', co.URL(required=True, default="https://mybinder.org")),
-            ('filepath_prefix', co.Type(str)),  # default is None
-            ('notebooks_dir', co.Type(str)),  # default is "notebooks"
-            ('use_jupyter_lab', co.Type(bool)),  # default is False
-        )),
+        ('binder', create_binder_config()),
         ('image_scrapers', ConfigList(co.Type(str))),
         ('compress_images', ConfigList(co.Type(str))),
         ('reset_modules', ConfigList(co.Type(str))),
         ('first_notebook_cell', co.Type(str)),
         ('last_notebook_cell', co.Type(str)),
         ('notebook_images', co.Type(bool)),
         # # 'pypandoc': False,
```

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/py_source_parser.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/py_source_parser.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/scrapers.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/scrapers.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/sorting.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/sorting.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/binder_badge_logo.svg` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/binder_badge_logo.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/broken_example.png` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/broken_example.png`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/broken_stamp.svg` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/broken_stamp.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/no_image.png` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/no_image.png`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/sg_gallery-dataframe.css` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/sg_gallery-dataframe.css`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/sg_gallery-rendered-html.css` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/sg_gallery-rendered-html.css`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/static/sg_gallery.css` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/static/sg_gallery.css`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery/utils.py` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery.egg-info/PKG-INFO` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: mkdocs-gallery
-Version: 0.7.6
+Version: 0.7.7
 Summary: a `mkdocs` plugin to generate example galleries from python scripts, similar to `sphinx-gallery`.
 Home-page: https://github.com/smarie/mkdocs-gallery
-Download-URL: https://github.com/smarie/mkdocs-gallery/tarball/0.7.6
+Download-URL: https://github.com/smarie/mkdocs-gallery/tarball/0.7.7
 Author: Sylvain MARIE <sylvain.marie@se.com>
 License: BSD 3-Clause
 Keywords: gallery web page generator figure jupyter notebook binder example code latex mkdocs sphinx
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: Topic :: Documentation
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mkdocs-gallery
 
 *[Sphinx-Gallery](https://sphinx-gallery.github.io/) features for [mkdocs](https://www.mkdocs.org/) (no [Sphinx](sphinx-doc.org/) dependency !).*
 
@@ -32,9 +33,7 @@
 Do you love [Sphinx-Gallery](https://sphinx-gallery.github.io/) but prefer [mkdocs](https://www.mkdocs.org/) over [Sphinx](sphinx-doc.org/) for your documentation ? `mkdocs-gallery` was written for you ;) 
 
 It relies on [mkdocs-material](https://squidfunk.github.io/mkdocs-material) to get the most of mkdocs, so that your galleries look nice!
 
 The documentation for users is available here: [https://smarie.github.io/mkdocs-gallery/](https://smarie.github.io/mkdocs-gallery/)
 
 A readme for developers is available here: [https://github.com/smarie/mkdocs-gallery](https://github.com/smarie/mkdocs-gallery)
-
-
```

### Comparing `mkdocs-gallery-0.7.6/src/mkdocs_gallery.egg-info/SOURCES.txt` & `mkdocs-gallery-0.7.7/src/mkdocs_gallery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/tests/reference_parse.txt` & `mkdocs-gallery-0.7.7/tests/reference_parse.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/tests/test_config.py` & `mkdocs-gallery-0.7.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/tests/test_gen_md.py` & `mkdocs-gallery-0.7.7/tests/test_gen_md.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/tests/test_packaging.py` & `mkdocs-gallery-0.7.7/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `mkdocs-gallery-0.7.6/tests/test_utils.py` & `mkdocs-gallery-0.7.7/tests/test_utils.py`

 * *Files identical despite different names*

