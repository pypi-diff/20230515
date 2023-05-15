# Comparing `tmp/restoreio-0.3.0.tar.gz` & `tmp/restoreio-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restoreio-0.3.0.tar", last modified: Mon May 15 04:56:04 2023, max compression
+gzip compressed data, was "restoreio-0.3.1.tar", last modified: Mon May 15 05:17:09 2023, max compression
```

## Comparing `restoreio-0.3.0.tar` & `restoreio-0.3.1.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.964348 restoreio-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-15 04:55:49.000000 restoreio-0.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 04:55:49.000000 restoreio-0.3.0/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-15 04:55:49.000000 restoreio-0.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-15 04:55:49.000000 restoreio-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-15 04:55:49.000000 restoreio-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-15 04:56:04.964348 restoreio-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-15 04:55:49.000000 restoreio-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.948348 restoreio-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.948348 restoreio-0.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.944348 restoreio-0.3.0/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.944348 restoreio-0.3.0/docs/source/_static/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.948348 restoreio-0.3.0/docs/source/_static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/assets/fonts/synconew.regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/assets/fonts/syncopate.bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/assets/fonts/syncopate.regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.948348 restoreio-0.3.0/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/css/custom-anaconda-doc.css
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/css/custom-pydata.css
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.944348 restoreio-0.3.0/docs/source/_static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.948348 restoreio-0.3.0/docs/source/_static/images/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-anaconda.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-anaconda.png
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-anaconda.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-pypi.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-pypi.png
--rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-pypi.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/docs/source/_static/images/plots/
--rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/cor_cov.png
--rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/deviation.png
--rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/ensembles.png
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/ensembles_js_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/gdop_coverage.png
--rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/js_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/kl_eigenvalues.png
--rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/kl_eigenvectors.png
--rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/orig_vel_and_error.png
--rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/rbf_kernel_2d.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/docs/source/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/js/custom-pydata.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/autosummary/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/autosummary/method.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/autosummary/ndarray_subclass.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/autosummary/property.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/version.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/cite.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/contents.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/generated/restoreio.restore.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   151486 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/notebooks/quick_start.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/recursive_glob.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 04:55:49.000000 restoreio-0.3.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.944348 restoreio-0.3.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/examples/restore/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/restore/main_VaryingNumModes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/restore/plot_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/restore/plot_fixed_size_artificial_mask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/restore/plot_variable_d_artificial_masks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21770 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/restore/plot_variable_size_artificial_masks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/examples/uncertainty_quant/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/uncertainty_quant/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/uncertainty_quant/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/uncertainty_quant/_plot_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/uncertainty_quant/plot_gdop_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/uncertainty_quant/plot_js_divergence.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 04:55:49.000000 restoreio-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-15 04:55:49.000000 restoreio-0.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/restoreio/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio/_file_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_file_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_file_utilities/file_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio/_geography/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_geography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_geography/_find_alpha_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_geography/create_mask_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_geography/detect_land_ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_geography/locate_missing_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio/_inpaint/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_inpaint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_inpaint/_cast_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_inpaint/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_inpaint/_plot_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_inpaint/inpaint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio/_input_output/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_input_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_input_output/get_datetime_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_input_output/load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_input_output/load_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_input_output/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio/_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_parser/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_parser/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_parser/parse_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio/_plots/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/_plot_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/_plot_quiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/_plot_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/_plot_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/_plot_velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/plot_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio/_plots_uq/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/_refine_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/_shifted_colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/plot_auto_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/plot_convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/plot_cor_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/plot_ensembles_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/plot_kl_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/plot_rbf_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.964348 restoreio-0.3.0/restoreio/_restore/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_restore/_make_array_masked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_restore/refine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_restore/restore_generated_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_restore/restore_main_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.964348 restoreio-0.3.0/restoreio/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34694 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_scripts/scan_netcdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.964348 restoreio-0.3.0/restoreio/_subset/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_subset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_subset/_array_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_subset/subset_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_subset/subset_domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.964348 restoreio-0.3.0/restoreio/_uncertainty_quant/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_uncertainty_quant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_uncertainty_quant/_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_uncertainty_quant/_statistical_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_uncertainty_quant/generate_image_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_uncertainty_quant/get_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-15 04:56:04.000000 restoreio-0.3.0/restoreio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-15 04:56:04.000000 restoreio-0.3.0/restoreio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 04:56:04.000000 restoreio-0.3.0/restoreio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 04:56:04.000000 restoreio-0.3.0/restoreio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 04:56:04.000000 restoreio-0.3.0/restoreio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-15 04:56:04.000000 restoreio-0.3.0/restoreio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 04:56:04.000000 restoreio-0.3.0/restoreio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-15 04:56:04.964348 restoreio-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-15 04:55:49.000000 restoreio-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.964348 restoreio-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-15 04:55:49.000000 restoreio-0.3.0/tests/test_restore_local_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-15 04:55:49.000000 restoreio-0.3.0/tests/test_restore_remote_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-15 04:55:49.000000 restoreio-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.567025 restoreio-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-15 05:16:50.000000 restoreio-0.3.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 05:16:50.000000 restoreio-0.3.1/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-15 05:16:50.000000 restoreio-0.3.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-15 05:16:50.000000 restoreio-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-15 05:16:50.000000 restoreio-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-15 05:17:09.567025 restoreio-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-15 05:16:50.000000 restoreio-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.551024 restoreio-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.551024 restoreio-0.3.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.547024 restoreio-0.3.1/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.547024 restoreio-0.3.1/docs/source/_static/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.551024 restoreio-0.3.1/docs/source/_static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/assets/fonts/synconew.regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/assets/fonts/syncopate.bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/assets/fonts/syncopate.regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.551024 restoreio-0.3.1/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/css/custom-anaconda-doc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/css/custom-pydata.css
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.547024 restoreio-0.3.1/docs/source/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.555024 restoreio-0.3.1/docs/source/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-anaconda.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-anaconda.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-anaconda.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-pypi.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-pypi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-pypi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/docs/source/_static/images/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/cor_cov.png
+-rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/deviation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/ensembles.png
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/ensembles_js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/gdop_coverage.png
+-rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/kl_eigenvalues.png
+-rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/kl_eigenvectors.png
+-rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/orig_vel_and_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/rbf_kernel_2d.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/docs/source/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/js/custom-pydata.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/autosummary/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/autosummary/method.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/autosummary/ndarray_subclass.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/autosummary/property.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/version.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/cite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/generated/restoreio.restore.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   151486 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/notebooks/quick_start.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/recursive_glob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 05:16:50.000000 restoreio-0.3.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.547024 restoreio-0.3.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/examples/restore/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/restore/main_VaryingNumModes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/restore/plot_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/restore/plot_fixed_size_artificial_mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/restore/plot_variable_d_artificial_masks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21770 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/restore/plot_variable_size_artificial_masks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/examples/uncertainty_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/uncertainty_quant/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/uncertainty_quant/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/uncertainty_quant/_plot_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/uncertainty_quant/plot_gdop_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/uncertainty_quant/plot_js_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 05:16:50.000000 restoreio-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-15 05:16:50.000000 restoreio-0.3.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio/_file_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_file_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_file_utilities/file_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio/_geography/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_geography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_geography/_find_alpha_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_geography/create_mask_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_geography/detect_land_ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_geography/locate_missing_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio/_inpaint/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_inpaint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_inpaint/_cast_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_inpaint/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_inpaint/_plot_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_inpaint/inpaint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio/_input_output/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_input_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_input_output/get_datetime_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_input_output/load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_input_output/load_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_input_output/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio/_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_parser/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_parser/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_parser/parse_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio/_plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/_plot_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/_plot_quiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/_plot_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/_plot_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/_plot_velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/plot_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.567025 restoreio-0.3.1/restoreio/_plots_uq/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/_refine_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/_shifted_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/plot_auto_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/plot_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/plot_cor_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/plot_ensembles_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/plot_kl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/plot_rbf_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.567025 restoreio-0.3.1/restoreio/_restore/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_restore/_make_array_masked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_restore/refine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_restore/restore_generated_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_restore/restore_main_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.567025 restoreio-0.3.1/restoreio/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34694 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_scripts/scan_netcdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.567025 restoreio-0.3.1/restoreio/_subset/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_subset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_subset/_array_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_subset/subset_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_subset/subset_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.567025 restoreio-0.3.1/restoreio/_uncertainty_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_uncertainty_quant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_uncertainty_quant/_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_uncertainty_quant/_statistical_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_uncertainty_quant/generate_image_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_uncertainty_quant/get_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-15 05:17:09.000000 restoreio-0.3.1/restoreio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-15 05:17:09.000000 restoreio-0.3.1/restoreio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 05:17:09.000000 restoreio-0.3.1/restoreio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 05:17:09.000000 restoreio-0.3.1/restoreio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 05:17:09.000000 restoreio-0.3.1/restoreio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-15 05:17:09.000000 restoreio-0.3.1/restoreio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 05:17:09.000000 restoreio-0.3.1/restoreio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-15 05:17:09.567025 restoreio-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-15 05:16:50.000000 restoreio-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.567025 restoreio-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-15 05:16:50.000000 restoreio-0.3.1/tests/test_restore_local_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-15 05:16:50.000000 restoreio-0.3.1/tests/test_restore_remote_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-15 05:16:50.000000 restoreio-0.3.1/tox.ini
```

### Comparing `restoreio-0.3.0/LICENSE.txt` & `restoreio-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/MANIFEST.in` & `restoreio-0.3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/PKG-INFO` & `restoreio-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.3.0
+Version: 0.3.1
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
```

### Comparing `restoreio-0.3.0/README.rst` & `restoreio-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/Makefile` & `restoreio-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/make.bat` & `restoreio-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_inspect.py` & `restoreio-0.3.1/docs/source/_inspect.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/assets/fonts/synconew.regular.ttf` & `restoreio-0.3.1/docs/source/_static/assets/fonts/synconew.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/assets/fonts/syncopate.bold.ttf` & `restoreio-0.3.1/docs/source/_static/assets/fonts/syncopate.bold.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/assets/fonts/syncopate.regular.ttf` & `restoreio-0.3.1/docs/source/_static/assets/fonts/syncopate.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/css/custom-anaconda-doc.css` & `restoreio-0.3.1/docs/source/_static/css/custom-anaconda-doc.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/css/custom-pydata.css` & `restoreio-0.3.1/docs/source/_static/css/custom-pydata.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/css/custom.css` & `restoreio-0.3.1/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/icons/favicon.ico` & `restoreio-0.3.1/docs/source/_static/images/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/icons/logo-anaconda.ico` & `restoreio-0.3.1/docs/source/_static/images/icons/logo-anaconda.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/icons/logo-anaconda.png` & `restoreio-0.3.1/docs/source/_static/images/icons/logo-anaconda.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/icons/logo-anaconda.svg` & `restoreio-0.3.1/docs/source/_static/images/icons/logo-anaconda.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/icons/logo-pypi.ico` & `restoreio-0.3.1/docs/source/_static/images/icons/logo-pypi.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/icons/logo-pypi.png` & `restoreio-0.3.1/docs/source/_static/images/icons/logo-pypi.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/icons/logo-pypi.svg` & `restoreio-0.3.1/docs/source/_static/images/icons/logo-pypi.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-dark.png` & `restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-dark.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-dark.svg` & `restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-dark.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-light.png` & `restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-light.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-light.svg` & `restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-light.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/plots/cor_cov.png` & `restoreio-0.3.1/docs/source/_static/images/plots/cor_cov.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/plots/deviation.png` & `restoreio-0.3.1/docs/source/_static/images/plots/deviation.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/plots/ensembles.png` & `restoreio-0.3.1/docs/source/_static/images/plots/ensembles.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/plots/ensembles_js_distance.png` & `restoreio-0.3.1/docs/source/_static/images/plots/ensembles_js_distance.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/plots/gdop_coverage.png` & `restoreio-0.3.1/docs/source/_static/images/plots/gdop_coverage.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/plots/js_distance.png` & `restoreio-0.3.1/docs/source/_static/images/plots/js_distance.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/plots/kl_eigenvalues.png` & `restoreio-0.3.1/docs/source/_static/images/plots/kl_eigenvalues.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/plots/kl_eigenvectors.png` & `restoreio-0.3.1/docs/source/_static/images/plots/kl_eigenvectors.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/plots/orig_vel_and_error.png` & `restoreio-0.3.1/docs/source/_static/images/plots/orig_vel_and_error.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/images/plots/rbf_kernel_2d.png` & `restoreio-0.3.1/docs/source/_static/images/plots/rbf_kernel_2d.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_static/js/custom-pydata.js` & `restoreio-0.3.1/docs/source/_static/js/custom-pydata.js`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_templates/autosummary/class.rst` & `restoreio-0.3.1/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_templates/layout.html` & `restoreio-0.3.1/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/_templates/version.html` & `restoreio-0.3.1/docs/source/_templates/version.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/cite.rst` & `restoreio-0.3.1/docs/source/cite.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/conf.py` & `restoreio-0.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/custom_domain.py` & `restoreio-0.3.1/docs/source/custom_domain.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/examples.rst` & `restoreio-0.3.1/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/index.rst` & `restoreio-0.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/install.rst` & `restoreio-0.3.1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/notebooks/quick_start.ipynb` & `restoreio-0.3.1/docs/source/notebooks/quick_start.ipynb`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/docs/source/recursive_glob.py` & `restoreio-0.3.1/docs/source/recursive_glob.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/examples/restore/main_VaryingNumModes.py` & `restoreio-0.3.1/examples/restore/main_VaryingNumModes.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/examples/restore/plot_coverage.py` & `restoreio-0.3.1/examples/restore/plot_coverage.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/examples/restore/plot_fixed_size_artificial_mask.py` & `restoreio-0.3.1/examples/restore/plot_fixed_size_artificial_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/examples/restore/plot_variable_d_artificial_masks.py` & `restoreio-0.3.1/examples/restore/plot_variable_d_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/examples/restore/plot_variable_size_artificial_masks.py` & `restoreio-0.3.1/examples/restore/plot_variable_size_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/examples/uncertainty_quant/_display_utilities.py` & `restoreio-0.3.1/examples/uncertainty_quant/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/examples/uncertainty_quant/_draw_map.py` & `restoreio-0.3.1/examples/uncertainty_quant/_draw_map.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/examples/uncertainty_quant/_plot_utilities.py` & `restoreio-0.3.1/examples/uncertainty_quant/_plot_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/examples/uncertainty_quant/plot_gdop_coverage.py` & `restoreio-0.3.1/examples/uncertainty_quant/plot_gdop_coverage.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/examples/uncertainty_quant/plot_js_divergence.py` & `restoreio-0.3.1/examples/uncertainty_quant/plot_js_divergence.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/__main__.py` & `restoreio-0.3.1/restoreio/__main__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_file_utilities/__init__.py` & `restoreio-0.3.1/restoreio/_file_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_file_utilities/file_utilities.py` & `restoreio-0.3.1/restoreio/_file_utilities/file_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_geography/__init__.py` & `restoreio-0.3.1/restoreio/_geography/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_geography/_find_alpha_shapes.py` & `restoreio-0.3.1/restoreio/_geography/_find_alpha_shapes.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_geography/create_mask_info.py` & `restoreio-0.3.1/restoreio/_geography/create_mask_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_geography/detect_land_ocean.py` & `restoreio-0.3.1/restoreio/_geography/detect_land_ocean.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_geography/locate_missing_data.py` & `restoreio-0.3.1/restoreio/_geography/locate_missing_data.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_inpaint/_cast_types.py` & `restoreio-0.3.1/restoreio/_inpaint/_cast_types.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_inpaint/_image.py` & `restoreio-0.3.1/restoreio/_inpaint/_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_inpaint/_plot_image.py` & `restoreio-0.3.1/restoreio/_inpaint/_plot_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_inpaint/inpaint.py` & `restoreio-0.3.1/restoreio/_inpaint/inpaint.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_input_output/__init__.py` & `restoreio-0.3.1/restoreio/_input_output/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_input_output/get_datetime_info.py` & `restoreio-0.3.1/restoreio/_input_output/get_datetime_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_input_output/load_dataset.py` & `restoreio-0.3.1/restoreio/_input_output/load_dataset.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_input_output/load_variables.py` & `restoreio-0.3.1/restoreio/_input_output/load_variables.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_input_output/writer.py` & `restoreio-0.3.1/restoreio/_input_output/writer.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_parser/examples.py` & `restoreio-0.3.1/restoreio/_parser/examples.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_parser/formatter.py` & `restoreio-0.3.1/restoreio/_parser/formatter.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_parser/parse_arguments.py` & `restoreio-0.3.1/restoreio/_parser/parse_arguments.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots/_display_utilities.py` & `restoreio-0.3.1/restoreio/_plots/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots/_draw_map.py` & `restoreio-0.3.1/restoreio/_plots/_draw_map.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots/_plot_grid.py` & `restoreio-0.3.1/restoreio/_plots/_plot_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots/_plot_quiver.py` & `restoreio-0.3.1/restoreio/_plots/_plot_quiver.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots/_plot_streamlines.py` & `restoreio-0.3.1/restoreio/_plots/_plot_streamlines.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots/_plot_utilities.py` & `restoreio-0.3.1/restoreio/_plots/_plot_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots/_plot_velocities.py` & `restoreio-0.3.1/restoreio/_plots/_plot_velocities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots/plot_results.py` & `restoreio-0.3.1/restoreio/_plots/plot_results.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots_uq/__init__.py` & `restoreio-0.3.1/restoreio/_plots_uq/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots_uq/_refine_mask.py` & `restoreio-0.3.1/restoreio/_plots_uq/_refine_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots_uq/_shifted_colormap.py` & `restoreio-0.3.1/restoreio/_plots_uq/_shifted_colormap.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots_uq/plot_auto_correlation.py` & `restoreio-0.3.1/restoreio/_plots_uq/plot_auto_correlation.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots_uq/plot_convergence.py` & `restoreio-0.3.1/restoreio/_plots_uq/plot_convergence.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots_uq/plot_cor_cov.py` & `restoreio-0.3.1/restoreio/_plots_uq/plot_cor_cov.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots_uq/plot_ensembles_stat.py` & `restoreio-0.3.1/restoreio/_plots_uq/plot_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots_uq/plot_kl_transform.py` & `restoreio-0.3.1/restoreio/_plots_uq/plot_kl_transform.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots_uq/plot_rbf_kernel.py` & `restoreio-0.3.1/restoreio/_plots_uq/plot_rbf_kernel.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py` & `restoreio-0.3.1/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_restore/__init__.py` & `restoreio-0.3.1/restoreio/_restore/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_restore/_make_array_masked.py` & `restoreio-0.3.1/restoreio/_restore/_make_array_masked.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_restore/refine_grid.py` & `restoreio-0.3.1/restoreio/_restore/refine_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_restore/restore_generated_ensembles.py` & `restoreio-0.3.1/restoreio/_restore/restore_generated_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_restore/restore_main_ensemble.py` & `restoreio-0.3.1/restoreio/_restore/restore_main_ensemble.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_scripts/scan_netcdf.py` & `restoreio-0.3.1/restoreio/_scripts/scan_netcdf.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_subset/_array_utilities.py` & `restoreio-0.3.1/restoreio/_subset/_array_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_subset/subset_datetime.py` & `restoreio-0.3.1/restoreio/_subset/subset_datetime.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_subset/subset_domain.py` & `restoreio-0.3.1/restoreio/_subset/subset_domain.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_uncertainty_quant/_compute_correlation_matrix.py` & `restoreio-0.3.1/restoreio/_uncertainty_quant/_compute_correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py` & `restoreio-0.3.1/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_uncertainty_quant/_image_utils.py` & `restoreio-0.3.1/restoreio/_uncertainty_quant/_image_utils.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_uncertainty_quant/_statistical_distances.py` & `restoreio-0.3.1/restoreio/_uncertainty_quant/_statistical_distances.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_uncertainty_quant/generate_image_ensembles.py` & `restoreio-0.3.1/restoreio/_uncertainty_quant/generate_image_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio/_uncertainty_quant/get_ensembles_stat.py` & `restoreio-0.3.1/restoreio/_uncertainty_quant/get_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/restoreio.egg-info/PKG-INFO` & `restoreio-0.3.1/restoreio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.3.0
+Version: 0.3.1
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
```

### Comparing `restoreio-0.3.0/restoreio.egg-info/SOURCES.txt` & `restoreio-0.3.1/restoreio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/setup.py` & `restoreio-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/tests/test_restore_local_data.py` & `restoreio-0.3.1/tests/test_restore_local_data.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.0/tests/test_restore_remote_data.py` & `restoreio-0.3.1/tests/test_restore_remote_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,30 +45,30 @@
 
 def test_restore():
     """
     Test for `restore` function.
     """
 
     # Monterey Bay data
-    input = 'http://hfrnet-tds.ucsd.edu/thredds/dodsC/HFR/USWC/2km/hourly/' + \
-            'RTV/HFRADAR_US_West_Coast_2km_Resolution_Hourly_RTV_best.ncd'
-    min_lon = -122.344
-    max_lon = -121.781
-    min_lat = 36.507
-    max_lat = 36.9925
-    time = '2017-01-25T03:00:00'
+    # input = 'http://hfrnet-tds.ucsd.edu/thredds/dodsC/HFR/USWC/2km/hourly/' + \
+    #         'RTV/HFRADAR_US_West_Coast_2km_Resolution_Hourly_RTV_best.ncd'
+    # min_lon = -122.344
+    # max_lon = -121.781
+    # min_lat = 36.507
+    # max_lat = 36.9925
+    # time = '2017-01-25T03:00:00'
 
     # Martha's Vineyard
-    # input = 'http://transport.me.berkeley.edu/thredds/dodsC/root/' + \
-    #         'WHOI-HFR/WHOI_HFR_2014_original.nc'
-    # min_lon = None
-    # max_lon = None
-    # min_lat = None
-    # max_lat = None
-    # time = '2017-08-17T20:00:00'
+    input = 'http://transport.me.berkeley.edu/thredds/dodsC/root/' + \
+            'WHOI-HFR/WHOI_HFR_2014_original.nc'
+    min_lon = None
+    max_lon = None
+    min_lat = None
+    max_lat = None
+    time = '2017-08-17T20:00:00'
 
     # Output
     output = 'output_remote_data.nc'
 
     # Absolute path
     dir = os.path.dirname(os.path.realpath(__file__))
     output = os.path.join(dir, output)
```

### Comparing `restoreio-0.3.0/tox.ini` & `restoreio-0.3.1/tox.ini`

 * *Files identical despite different names*

