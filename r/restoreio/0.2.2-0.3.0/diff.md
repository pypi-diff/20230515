# Comparing `tmp/restoreio-0.2.2.tar.gz` & `tmp/restoreio-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restoreio-0.2.2.tar", last modified: Sat Mar 11 05:49:53 2023, max compression
+gzip compressed data, was "restoreio-0.3.0.tar", last modified: Mon May 15 04:56:04 2023, max compression
```

## Comparing `restoreio-0.2.2.tar` & `restoreio-0.3.0.tar`

### file list

```diff
@@ -1,152 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.134241 restoreio-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-11 05:49:38.000000 restoreio-0.2.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-11 05:49:38.000000 restoreio-0.2.2/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-11 05:49:38.000000 restoreio-0.2.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-11 05:49:38.000000 restoreio-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-11 05:49:38.000000 restoreio-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-03-11 05:49:53.134241 restoreio-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-03-11 05:49:38.000000 restoreio-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.126241 restoreio-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.126241 restoreio-0.2.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.122241 restoreio-0.2.2/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.122241 restoreio-0.2.2/docs/source/_static/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.126241 restoreio-0.2.2/docs/source/_static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/assets/fonts/synconew.regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/assets/fonts/syncopate.bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/assets/fonts/syncopate.regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.126241 restoreio-0.2.2/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/css/custom-anaconda-doc.css
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/css/custom-pydata.css
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.122241 restoreio-0.2.2/docs/source/_static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.126241 restoreio-0.2.2/docs/source/_static/images/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/images/icons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/images/icons/logo-anaconda.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/images/icons/logo-anaconda.png
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/images/icons/logo-anaconda.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/images/icons/logo-pypi.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/images/icons/logo-pypi.png
--rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/images/icons/logo-pypi.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/images/icons/logo-restoreio-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/images/icons/logo-restoreio-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/images/icons/logo-restoreio-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/images/icons/logo-restoreio-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.126241 restoreio-0.2.2/docs/source/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_static/js/custom-pydata.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.126241 restoreio-0.2.2/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.130241 restoreio-0.2.2/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_templates/autosummary/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_templates/autosummary/method.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_templates/autosummary/ndarray_subclass.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_templates/autosummary/property.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/_templates/version.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/cite.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/contents.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.130241 restoreio-0.2.2/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/generated/restoreio.restore.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.130241 restoreio-0.2.2/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   151486 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/notebooks/quick_start.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-03-11 05:49:38.000000 restoreio-0.2.2/docs/source/recursive_glob.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-11 05:49:38.000000 restoreio-0.2.2/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.130241 restoreio-0.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    30256 2023-03-11 05:49:38.000000 restoreio-0.2.2/examples/main_VaryingNumModes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-03-11 05:49:38.000000 restoreio-0.2.2/examples/plot_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-03-11 05:49:38.000000 restoreio-0.2.2/examples/plot_fixed_size_artificial_mask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-03-11 05:49:38.000000 restoreio-0.2.2/examples/plot_variable_d_artificial_masks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21770 2023-03-11 05:49:38.000000 restoreio-0.2.2/examples/plot_variable_size_artificial_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-11 05:49:38.000000 restoreio-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-11 05:49:38.000000 restoreio-0.2.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.130241 restoreio-0.2.2/restoreio/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.130241 restoreio-0.2.2/restoreio/_file_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_file_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_file_utilities/file_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.130241 restoreio-0.2.2/restoreio/_geography/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_geography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_geography/_find_alpha_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_geography/create_mask_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_geography/detect_land_ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_geography/locate_missing_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.130241 restoreio-0.2.2/restoreio/_inpaint/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_inpaint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_inpaint/_cast_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_inpaint/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_inpaint/_plot_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_inpaint/inpaint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.130241 restoreio-0.2.2/restoreio/_input_output/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_input_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_input_output/load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_input_output/load_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_input_output/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.130241 restoreio-0.2.2/restoreio/_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_parser/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_parser/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_parser/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.134241 restoreio-0.2.2/restoreio/_plots/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots/_plot_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots/_plot_quiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots/_plot_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots/_plot_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots/_plot_velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots/plot_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.134241 restoreio-0.2.2/restoreio/_plots_uq/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots_uq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots_uq/_refine_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots_uq/_shifted_colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots_uq/plot_auto_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots_uq/plot_convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots_uq/plot_cor_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    26501 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots_uq/plot_ensembles_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots_uq/plot_kl_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots_uq/plot_rbf_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.134241 restoreio-0.2.2/restoreio/_restore/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_restore/_make_array_masked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_restore/refine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_restore/restore_generated_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_restore/restore_main_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.134241 restoreio-0.2.2/restoreio/_uncertainty_quant/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_uncertainty_quant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_uncertainty_quant/_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_uncertainty_quant/_statistical_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_uncertainty_quant/generate_image_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/_uncertainty_quant/get_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.134241 restoreio-0.2.2/restoreio/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32461 2023-03-11 05:49:38.000000 restoreio-0.2.2/restoreio/scripts/scan_netcdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.130241 restoreio-0.2.2/restoreio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-03-11 05:49:53.000000 restoreio-0.2.2/restoreio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-03-11 05:49:53.000000 restoreio-0.2.2/restoreio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 05:49:53.000000 restoreio-0.2.2/restoreio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-11 05:49:53.000000 restoreio-0.2.2/restoreio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 05:49:53.000000 restoreio-0.2.2/restoreio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-11 05:49:53.000000 restoreio-0.2.2/restoreio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-11 05:49:53.000000 restoreio-0.2.2/restoreio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-11 05:49:53.134241 restoreio-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-03-11 05:49:38.000000 restoreio-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 05:49:53.134241 restoreio-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-03-11 05:49:38.000000 restoreio-0.2.2/tests/test_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-11 05:49:38.000000 restoreio-0.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.964348 restoreio-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-15 04:55:49.000000 restoreio-0.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 04:55:49.000000 restoreio-0.3.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-15 04:55:49.000000 restoreio-0.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-15 04:55:49.000000 restoreio-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-15 04:55:49.000000 restoreio-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-15 04:56:04.964348 restoreio-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-15 04:55:49.000000 restoreio-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.948348 restoreio-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.948348 restoreio-0.3.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.944348 restoreio-0.3.0/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.944348 restoreio-0.3.0/docs/source/_static/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.948348 restoreio-0.3.0/docs/source/_static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/assets/fonts/synconew.regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/assets/fonts/syncopate.bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/assets/fonts/syncopate.regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.948348 restoreio-0.3.0/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/css/custom-anaconda-doc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/css/custom-pydata.css
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.944348 restoreio-0.3.0/docs/source/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.948348 restoreio-0.3.0/docs/source/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-anaconda.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-anaconda.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-anaconda.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-pypi.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-pypi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-pypi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/docs/source/_static/images/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/cor_cov.png
+-rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/deviation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/ensembles.png
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/ensembles_js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/gdop_coverage.png
+-rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/kl_eigenvalues.png
+-rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/kl_eigenvectors.png
+-rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/orig_vel_and_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/images/plots/rbf_kernel_2d.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/docs/source/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_static/js/custom-pydata.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/autosummary/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/autosummary/method.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/autosummary/ndarray_subclass.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/autosummary/property.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/_templates/version.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/cite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/generated/restoreio.restore.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   151486 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/notebooks/quick_start.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-15 04:55:49.000000 restoreio-0.3.0/docs/source/recursive_glob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 04:55:49.000000 restoreio-0.3.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.944348 restoreio-0.3.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/examples/restore/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/restore/main_VaryingNumModes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/restore/plot_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/restore/plot_fixed_size_artificial_mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/restore/plot_variable_d_artificial_masks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21770 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/restore/plot_variable_size_artificial_masks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/examples/uncertainty_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/uncertainty_quant/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/uncertainty_quant/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/uncertainty_quant/_plot_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/uncertainty_quant/plot_gdop_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-05-15 04:55:49.000000 restoreio-0.3.0/examples/uncertainty_quant/plot_js_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 04:55:49.000000 restoreio-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-15 04:55:49.000000 restoreio-0.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.956348 restoreio-0.3.0/restoreio/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio/_file_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_file_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_file_utilities/file_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio/_geography/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_geography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_geography/_find_alpha_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_geography/create_mask_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_geography/detect_land_ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_geography/locate_missing_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio/_inpaint/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_inpaint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_inpaint/_cast_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_inpaint/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_inpaint/_plot_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_inpaint/inpaint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio/_input_output/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_input_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_input_output/get_datetime_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_input_output/load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_input_output/load_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_input_output/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio/_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_parser/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_parser/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_parser/parse_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio/_plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/_plot_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/_plot_quiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/_plot_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/_plot_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/_plot_velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots/plot_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio/_plots_uq/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/_refine_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/_shifted_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/plot_auto_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/plot_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/plot_cor_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/plot_ensembles_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/plot_kl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/plot_rbf_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.964348 restoreio-0.3.0/restoreio/_restore/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_restore/_make_array_masked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_restore/refine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_restore/restore_generated_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_restore/restore_main_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.964348 restoreio-0.3.0/restoreio/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34694 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_scripts/scan_netcdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.964348 restoreio-0.3.0/restoreio/_subset/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_subset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_subset/_array_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_subset/subset_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_subset/subset_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.964348 restoreio-0.3.0/restoreio/_uncertainty_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_uncertainty_quant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_uncertainty_quant/_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_uncertainty_quant/_statistical_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_uncertainty_quant/generate_image_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-05-15 04:55:49.000000 restoreio-0.3.0/restoreio/_uncertainty_quant/get_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.960348 restoreio-0.3.0/restoreio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-15 04:56:04.000000 restoreio-0.3.0/restoreio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-15 04:56:04.000000 restoreio-0.3.0/restoreio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 04:56:04.000000 restoreio-0.3.0/restoreio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 04:56:04.000000 restoreio-0.3.0/restoreio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 04:56:04.000000 restoreio-0.3.0/restoreio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-15 04:56:04.000000 restoreio-0.3.0/restoreio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 04:56:04.000000 restoreio-0.3.0/restoreio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-15 04:56:04.964348 restoreio-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-15 04:55:49.000000 restoreio-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:56:04.964348 restoreio-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-15 04:55:49.000000 restoreio-0.3.0/tests/test_restore_local_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-15 04:55:49.000000 restoreio-0.3.0/tests/test_restore_remote_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-15 04:55:49.000000 restoreio-0.3.0/tox.ini
```

### Comparing `restoreio-0.2.2/LICENSE.txt` & `restoreio-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/MANIFEST.in` & `restoreio-0.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/PKG-INFO` & `restoreio-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.2.2
+Version: 0.3.0
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
```

### Comparing `restoreio-0.2.2/README.rst` & `restoreio-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/Makefile` & `restoreio-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/make.bat` & `restoreio-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_inspect.py` & `restoreio-0.3.0/docs/source/_inspect.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/assets/fonts/synconew.regular.ttf` & `restoreio-0.3.0/docs/source/_static/assets/fonts/synconew.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/assets/fonts/syncopate.bold.ttf` & `restoreio-0.3.0/docs/source/_static/assets/fonts/syncopate.bold.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/assets/fonts/syncopate.regular.ttf` & `restoreio-0.3.0/docs/source/_static/assets/fonts/syncopate.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/css/custom-anaconda-doc.css` & `restoreio-0.3.0/docs/source/_static/css/custom-anaconda-doc.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/css/custom-pydata.css` & `restoreio-0.3.0/docs/source/_static/css/custom-pydata.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/css/custom.css` & `restoreio-0.3.0/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/images/icons/favicon.ico` & `restoreio-0.3.0/docs/source/_static/images/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/images/icons/logo-anaconda.ico` & `restoreio-0.3.0/docs/source/_static/images/icons/logo-anaconda.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/images/icons/logo-anaconda.png` & `restoreio-0.3.0/docs/source/_static/images/icons/logo-anaconda.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/images/icons/logo-anaconda.svg` & `restoreio-0.3.0/docs/source/_static/images/icons/logo-anaconda.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/images/icons/logo-pypi.ico` & `restoreio-0.3.0/docs/source/_static/images/icons/logo-pypi.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/images/icons/logo-pypi.png` & `restoreio-0.3.0/docs/source/_static/images/icons/logo-pypi.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/images/icons/logo-pypi.svg` & `restoreio-0.3.0/docs/source/_static/images/icons/logo-pypi.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/images/icons/logo-restoreio-dark.png` & `restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-dark.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/images/icons/logo-restoreio-dark.svg` & `restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-dark.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/images/icons/logo-restoreio-light.png` & `restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-light.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/images/icons/logo-restoreio-light.svg` & `restoreio-0.3.0/docs/source/_static/images/icons/logo-restoreio-light.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_static/js/custom-pydata.js` & `restoreio-0.3.0/docs/source/_static/js/custom-pydata.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -67,14 +67,18 @@
 }
 
 document.addEventListener("adobe_dc_view_sdk.ready", function() {
 
     document.getElementById("showPDF-jgr").addEventListener("click", function() {
         showPDF("https://arxiv.org/pdf/1808.07965.pdf")
     });
+
+    document.getElementById("showPDF-uq").addEventListener("click", function() {
+        showPDF("https://arxiv.org/pdf/1808.07965.pdf")
+    });
 });
 
 // Add arrayBuffer if necessary i.e. Safari
 (function() {
     if (Blob.arrayBuffer != "function") {
         Blob.prototype.arrayBuffer = myArrayBuffer;
     }
```

### Comparing `restoreio-0.2.2/docs/source/_templates/autosummary/class.rst` & `restoreio-0.3.0/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_templates/layout.html` & `restoreio-0.3.0/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/_templates/version.html` & `restoreio-0.3.0/docs/source/_templates/version.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/cite.rst` & `restoreio-0.3.0/docs/source/cite.rst`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ************
 
 How to Cite
 ===========
 
 If you publish work that uses |project|, please consider citing the following manuscripts.
 
-.. [1] Ameli, S., and Shadden. S. C. (2022). A Transport Method for Restoring Incomplete Ocean Current Measurements. *Journal of Geophysical Research: Oceans*, 124, 227-242 |ameli-jgr| |btn-bib-jgr| |btn-view-pdf-jgr|
+.. [1] Ameli, S., and Shadden. S. C. (2019). A Transport Method for Restoring Incomplete Ocean Current Measurements. *Journal of Geophysical Research: Oceans*, 124, 227-242 |ameli-jgr| |btn-bib-jgr| |btn-view-pdf-jgr|
 
    .. raw:: html
 
         <div class="highlight-BibTeX notranslate collapse" id="collapse-bib-jgr">
         <div class="highlight">
         <pre class="language-bib">
         <code class="language-bib">@article{https://doi.org/10.1029/2018JC014254,
@@ -24,15 +24,35 @@
             pages   = {227-242},
             doi     = {https://doi.org/10.1029/2018JC014254},
             year    = {2019}
         }</code></pre>
         </div>
         </div>
 
-.. [2] Ameli, S. (2022). *RestoreIO, a Python Package to Restore Incomplete Oceanographic Dataset*. |restoreio-zenodo| |btn-bib-restoreio|
+.. [2] Ameli, S., and Shadden. S. C. (2023). tochastic Modeling of HF Radar Data for Uncertainty Quantification and Gap Filling. |ameli-uq| |btn-bib-uq| |btn-view-pdf-uq|
+
+   .. raw:: html
+
+        <div class="highlight-BibTeX notranslate collapse" id="collapse-bib-uq">
+        <div class="highlight">
+        <pre class="language-bib">
+        <code class="language-bib">@article{https://doi.org/10.1029/2018JC014254,
+            author  = {Ameli, Siavash and Shadden, Shawn C.},
+            title   = {A Transport Method for Restoring Incomplete Ocean Current Measurements},
+            journal = {Journal of Geophysical Research: Oceans},
+            volume  = {124},
+            number  = {1},
+            pages   = {227-242},
+            doi     = {https://doi.org/10.1029/2018JC014254},
+            year    = {2019}
+        }</code></pre>
+        </div>
+        </div>
+
+.. [3] Ameli, S. (2022). *RestoreIO, a Python Package to Restore Incomplete Oceanographic Dataset*. |restoreio-zenodo| |btn-bib-restoreio|
 
    .. raw:: html
 
         <div class="highlight-BibTeX notranslate collapse" id="collapse-bib-restore">
         <div class="highlight">
         <pre class="language-bib">
         <code class="language-bib">@misc{zenodo.373664668,
@@ -54,26 +74,42 @@
 
 .. |btn-bib-jgr| raw:: html
 
     <button class="btn btn-outline-info btn-sm btn-extra-sm" type="button" data-toggle="collapse" data-target="#collapse-bib-jgr">
         BibTeX
     </button>
 
+.. |btn-bib-uq| raw:: html
+
+    <button class="btn btn-outline-info btn-sm btn-extra-sm" type="button" data-toggle="collapse" data-target="#collapse-bib-uq">
+        BibTeX
+    </button>
+
 .. |btn-bib-restoreio| raw:: html
 
     <button class="btn btn-outline-info btn-sm btn-extra-sm" type="button" data-toggle="collapse" data-target="#collapse-bib-restoreio">
         BibTeX
     </button>
 
 .. |btn-view-pdf-jgr| raw:: html
 
     <button class="btn btn-outline-info btn-sm btn-extra-sm" type="button" id="showPDF-jgr">
         PDF
     </button>
 
+.. |btn-view-pdf-uq| raw:: html
+
+    <button class="btn btn-outline-info btn-sm btn-extra-sm" type="button" id="showPDF-uq">
+        PDF
+    </button>
+
 .. |ameli-jgr| image:: https://img.shields.io/badge/arXiv-1808.07965-b31b1b.svg
    :target: https://doi.org/10.48550/arXiv.1808.07965
    :alt: arXiv 2206.09976
 
+.. |ameli-uq| image:: https://img.shields.io/badge/arXiv-1808.07965-b31b1b.svg
+   :target: https://doi.org/10.48550/arXiv.1808.07965
+   :alt: arXiv 2206.09976
+
 .. |restoreio-zenodo| image:: https://zenodo.org/badge/373664668.svg
    :target: https://zenodo.org/badge/latestdoi/373664668
    :alt: doi: 105281/zenodo.373664668
```

### Comparing `restoreio-0.2.2/docs/source/conf.py` & `restoreio-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/custom_domain.py` & `restoreio-0.3.0/docs/source/custom_domain.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/index.rst` & `restoreio-0.3.0/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -256,16 +256,14 @@
    :target: https://anaconda.org/s-ameli/traceinv
 .. |binder| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/ameli/restoreio/HEAD?filepath=notebooks%2Fquick_start.ipynb
 .. |conda-downloads| image:: https://img.shields.io/conda/dn/s-ameli/restoreio
    :target: https://anaconda.org/s-ameli/restoreio
 .. |tokei| image:: https://tokei.rs/b1/github/ameli/restoreio?category=lines
    :target: https://github.com/ameli/restoreio
-.. .. |tokei-2| image:: https://img.shields.io/badge/code%20lines-31.9k-blue
-..    :target: https://github.com/ameli/restoreio
 .. |languages| image:: https://img.shields.io/github/languages/count/ameli/restoreio
    :target: https://github.com/ameli/restoreio
 .. .. |imate-light| image:: _static/images/icons/logo-imate-light.svg
 ..    :height: 23
 ..    :class: only-light
 .. .. |imate-dark| image:: _static/images/icons/logo-imate-dark.svg
 ..    :height: 23
```

### Comparing `restoreio-0.2.2/docs/source/install.rst` & `restoreio-0.3.0/docs/source/install.rst`

 * *Files 3% similar despite different names*

```diff
@@ -248,29 +248,37 @@
 
 or the following error:
 
 .. prompt::
 
     FileNotFoundError: [Errno 2] No such file or directory: '/opt/miniconda3/lib/python3.10/site-packages/basemap_data_hires-1.3.2-py3.10.egg/mpl_toolkits/basemap_data/epsg'
 
-To solve these issues as follows. First, install ``libgeos`` library by
+To solve these issues, first, install ``libgeos`` library by
 
 .. prompt::
 
     sudo apt install libgeos3.10.2 libgeos-dev -y
 
 
 Next, install ``basemap`` package directly thought its `GitHub repository <https://github.com/matplotlib/basemap>`__ as follows. 
 
 .. prompt::
 
     python -m pip install git+https://github.com/matplotlib/basemap#subdirectory=packages/basemap
     python -m pip install git+https://github.com/matplotlib/basemap#subdirectory=packages/basemap_data
     python -m pip install git+https://github.com/matplotlib/basemap#subdirectory=packages/basemap_data_hires
 
+If the issue is not yet resolved with the above solutions, try reinstalling all prerequisite packages using ``conda`` instead of ``pip`` as follows:
+
+.. prompt::
+
+    conda install -c conda-forge --file conda-recipe/requirements_conda.txt
+
+In the above command, the file ``requirements_conda.txt`` is located in the `source code <https://github.com/ameli/restoreio>`__ under ``/conda-receipe`` directory.
+
 Issue with ``geos``
 -------------------
 
 When building the sphinx documentation, you may get this error:
 
 .. prompt::
```

### Comparing `restoreio-0.2.2/docs/source/notebooks/quick_start.ipynb` & `restoreio-0.3.0/docs/source/notebooks/quick_start.ipynb`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/docs/source/recursive_glob.py` & `restoreio-0.3.0/docs/source/recursive_glob.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/examples/main_VaryingNumModes.py` & `restoreio-0.3.0/examples/restore/main_VaryingNumModes.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/examples/plot_coverage.py` & `restoreio-0.3.0/examples/restore/plot_coverage.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/examples/plot_fixed_size_artificial_mask.py` & `restoreio-0.3.0/examples/restore/plot_fixed_size_artificial_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/examples/plot_variable_d_artificial_masks.py` & `restoreio-0.3.0/examples/restore/plot_variable_d_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/examples/plot_variable_size_artificial_masks.py` & `restoreio-0.3.0/examples/restore/plot_variable_size_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_file_utilities/__init__.py` & `restoreio-0.3.0/restoreio/_file_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_file_utilities/file_utilities.py` & `restoreio-0.3.0/restoreio/_file_utilities/file_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_geography/__init__.py` & `restoreio-0.3.0/restoreio/_geography/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_geography/_find_alpha_shapes.py` & `restoreio-0.3.0/restoreio/_geography/_find_alpha_shapes.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_geography/create_mask_info.py` & `restoreio-0.3.0/restoreio/_geography/create_mask_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_geography/detect_land_ocean.py` & `restoreio-0.3.0/restoreio/_geography/detect_land_ocean.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,19 @@
     elif method == 3:
         # Currently not working, do not use (land are not detected)
         land_indices, ocean_indices = detect_land_ocean_3(
                 lon, lat, verbose=verbose)
     else:
         raise RuntimeError("ExcludeLandFromOcean option is invalid.")
 
+    # If no land is detected, set land indices to nan, which signals other
+    # functions to not consider land.
+    if len(land_indices) == 0:
+        land_indices = numpy.nan
+
     return land_indices, ocean_indices
 
 
 # ========================
 # Do not Detect Land Ocean
 # ========================
 
@@ -71,15 +76,15 @@
     This function is as oppose to "detect_land_ocean_1,2,3". If user chooses
     to not to detect any land, we treat the entire domain as it is in ocean. So
     in this function we return a land_indices as nan, and Ocean Indices as all
     available indices in the grid.
     """
 
     # Do not detect any land.
-    land_indices = numpy.nan
+    land_indices = []
 
     # We treat all the domain as it is the ocean
     ocean_indices_list = []
 
     for lat_index in range(lat.size):
         for lon_index in range(lon.size):
             tuple = (lat_index, lon_index)
```

### Comparing `restoreio-0.2.2/restoreio/_geography/locate_missing_data.py` & `restoreio-0.3.0/restoreio/_geography/locate_missing_data.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_inpaint/_cast_types.py` & `restoreio-0.3.0/restoreio/_inpaint/_cast_types.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_inpaint/_image.py` & `restoreio-0.3.0/restoreio/_inpaint/_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_inpaint/_plot_image.py` & `restoreio-0.3.0/restoreio/_inpaint/_plot_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_inpaint/inpaint.py` & `restoreio-0.3.0/restoreio/_inpaint/inpaint.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_input_output/__init__.py` & `restoreio-0.3.0/restoreio/_input_output/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,12 +3,14 @@
 # SPDX-FileType: SOURCE
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the license found in the LICENSE.txt file in the root directory
 # of this source tree.
 
 
-from .load_dataset import load_dataset                               # noqa F401
-from .load_variables import load_variables                           # noqa F401
-from .writer import write_output_file                                # noqa F401
+from .load_dataset import load_dataset                              # noqa F401
+from .load_variables import load_variables                          # noqa F401
+from .get_datetime_info import get_datetime_info                    # noqa F401
+from .writer import write_output_file                               # noqa F401
 
-__all__ = ['load_dataset', 'load_variables', 'write_output_file']
+__all__ = ['load_dataset', 'load_variables', 'get_datetime_info',
+           'write_output_file']
```

### Comparing `restoreio-0.2.2/restoreio/_input_output/load_dataset.py` & `restoreio-0.3.0/restoreio/_input_output/load_dataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     if verbose:
         print("Message: Loading data ... ")
     sys.stdout.flush()
 
     # Check file extension
     file_extension = os.path.splitext(filename)[1]
-    if file_extension == '.ncml':
+    if file_extension in ['.ncml', '.ncml.gz']:
 
         # Change directory
         data_dir = os.path.dirname(filename)
         current_dir = os.getcwd()
         os.chdir(data_dir)
 
         # NCML
@@ -64,42 +64,73 @@
 
         except BaseException as error:
             print('ERROR: Can not read local ncml file: ' + filename)
             raise error
 
         return agg
 
-    elif file_extension == '.nc':
+    elif file_extension in ['.nc', '.ncd', '.nc.gz']:
 
         try:
             nc = netCDF4.Dataset(filename)
         except BaseException as error:
             print('ERROR: Can not read local netcdf file: ' + filename)
             raise error
 
         return nc
 
     else:
-        raise ValueError("File should be either *.ncml or *.nc.")
+        raise ValueError("File format %s is not recognized." % file_extension)
 
 
 # ===================
 # Load Remote Dataset
 # ===================
 
 def load_remote_dataset(url):
     """
     url can be point to a *.nc or *.ncml file.
     """
 
+    # Check URL is opendap
+    if (url.startswith('http://') is False) and \
+       (url.startswith('https://') is False):
+        raise ValueError('Input data URL does not seem to be a URL. ' +
+                         'A URL should start with "http://" or "https://".')
+
+    elif ("/thredds/dodsC/" not in url) and ("opendap" not in url):
+        raise ValueError('Input data URL is not an OpenDap URL or is not ' +
+                         'hosted on a THREDDs server. Check if your data ' +
+                         'URL contains "/thredds/dodsC/" or "/opendap/".')
+
+    # Check file extension
+    file_extension = os.path.splitext(url)[1]
+
+    # Case of zipped files (get the correct file extension before the '.gz')
+    if file_extension == ".gz":
+        file_extension = os.path.splitext(url[:-3])[1]
+
+    # Note that some opendap urls do not even have a file extension
+    if file_extension != "":
+
+        # If a file extension exists, check if it is a standard netcdf file
+        if file_extension not in \
+                ['.nc', '.ncd', '.nc.gz', '.ncml', '.ncml.gz']:
+            raise ValueError(
+                'The input data URL is not an netcdf file. The URL should ' +
+                'end with ".nc", ".ncd", ".nc.gz", ".ncml", ".ncml.gz", or ' +
+                'without file extension.')
+
     try:
+
+        # nc = open_url(url)
         nc = netCDF4.Dataset(url)
-    except BaseException as error:
-        print('ERROR: Can not read remote file: ' + url)
-        raise error
+
+    except OSError:
+        raise RuntimeError('Unable to read %s.' % url)
 
     return nc
 
 
 # ============
 # Load Dataset
 # ============
@@ -109,14 +140,18 @@
     Dispatches the execution to either of the following two functions:
 
     1. load_local_dataset: For files where the input_filename is a path on the
        local machine.
     2. load_remote_dataset: For files remotely where input_filename is a url.
     """
 
+    if input_filename == '':
+        raise ValueError('Input data is empty. You should provide a local' +
+                         'filename or an OpenDap URL or remote data.')
+
     # Check if the input_filename has a "host" name
     if bool(urlparse(input_filename).netloc):
         # input_filename is a url
         return load_remote_dataset(input_filename)
     else:
         # input_filename is a path
         return load_local_dataset(input_filename, verbose=verbose)
```

### Comparing `restoreio-0.2.2/restoreio/_input_output/load_variables.py` & `restoreio-0.3.0/restoreio/_input_output/load_variables.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_parser/examples.py` & `restoreio-0.3.0/restoreio/_parser/examples.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_parser/formatter.py` & `restoreio-0.3.0/restoreio/_parser/formatter.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots/_display_utilities.py` & `restoreio-0.3.0/examples/uncertainty_quant/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots/_draw_map.py` & `restoreio-0.3.0/examples/uncertainty_quant/_draw_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # =======
 # Imports
 # =======
 
 import numpy
 from mpl_toolkits.basemap import Basemap
-from ._plot_utilities import Polygon
+from _plot_utilities import Polygon
 
 __all__ = ['draw_map', 'draw_axis']
 
 
 # ========
 # Draw map
 # ========
@@ -192,15 +192,15 @@
         # map.drawcounties()
 
         # Set background color
         # map.drawlsmask(land_color='Linen', ocean_color=ocean_color,
         #                lakes=True, zorder=-2)
 
         # map.fillcontinents(color='red', lake_color='white', zorder=0)
-        map.fillcontinents(color=land_color, zorder=1)
+        map.fillcontinents(color=land_color, zorder=2)
 
         # map.bluemarble()
         # map.shadedrelief()
         # map.etopo()
 
     # Map features
     if draw_features:
@@ -222,12 +222,12 @@
         min_parallels, max_parallels = numpy.sort([*parallels])
         parallels[min_parallels][1][0].set_va('bottom')
         parallels[max_parallels][1][0].set_va('top')
 
         # Draw Mapscale
         distance = 0.1 * diff_lon_on_map / 1000.0  # in Km
         distance = 5 * int(distance / 5.0 + 0.5)
-        shift_lon = +0.75 * (max_lon - mid_lon)
-        shift_lat = -0.80 * (max_lat - mid_lat)
+        shift_lon = 0.75 * (max_lon - mid_lon)
+        shift_lat = 0.80 * (max_lat - mid_lat)
         map.drawmapscale(mid_lon+shift_lon, mid_lat+shift_lat, mid_lon,
                          mid_lat, distance, barstyle='simple', units='km',
                          labelstyle='simple', fontsize='7', zorder=100)
```

### Comparing `restoreio-0.2.2/restoreio/_plots/_plot_grid.py` & `restoreio-0.3.0/restoreio/_plots/_plot_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots/_plot_quiver.py` & `restoreio-0.3.0/restoreio/_plots/_plot_quiver.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots/_plot_streamlines.py` & `restoreio-0.3.0/restoreio/_plots/_plot_streamlines.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots/_plot_utilities.py` & `restoreio-0.3.0/restoreio/_plots/_plot_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots/_plot_velocities.py` & `restoreio-0.3.0/restoreio/_plots/_plot_velocities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots/plot_results.py` & `restoreio-0.3.0/restoreio/_plots/plot_results.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots_uq/__init__.py` & `restoreio-0.3.0/restoreio/_plots_uq/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots_uq/_refine_mask.py` & `restoreio-0.3.0/restoreio/_plots_uq/_refine_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots_uq/_shifted_colormap.py` & `restoreio-0.3.0/restoreio/_plots_uq/_shifted_colormap.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots_uq/plot_auto_correlation.py` & `restoreio-0.3.0/restoreio/_plots_uq/plot_auto_correlation.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots_uq/plot_convergence.py` & `restoreio-0.3.0/restoreio/_plots_uq/plot_convergence.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots_uq/plot_cor_cov.py` & `restoreio-0.3.0/restoreio/_plots_uq/plot_cor_cov.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots_uq/plot_ensembles_stat.py` & `restoreio-0.3.0/restoreio/_plots_uq/plot_ensembles_stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,16 @@
         lats_grid_on_map,
         scalar_field,
         title,
         colormap,
         clabel='',
         refined_mask_data={},
         log_norm=False,
-        shift_colormap=False):
+        shift_colormap=False,
+        vmin=None):
     """
     This plots in each of left or right axes.
     """
 
     # Config
     title_fontsize = 12
     label_fontsize = 10
@@ -71,15 +72,15 @@
         # draw = map.contourf(
         #         lons_grid_on_map, lats_grid_on_map, scalar_field,
         #         200, cmap=colormap, corner_mask=False,
         #         rasterized=True, zorder=-1)
     else:
         # Do not plot in log scale
         draw = map.pcolormesh(lons_grid_on_map, lats_grid_on_map,
-                              scalar_field, cmap=colormap,
+                              scalar_field, cmap=colormap, vmin=vmin,
                               rasterized=True, zorder=-1)
 
     # Draw edges lines around mask pixels
     if refined_mask_data is not {}:
 
         # Convert lon and lat degrees to length coordinates on map in meters
         refined_lons_grid_on_map, refined_lats_grid_on_map = map(
@@ -125,14 +126,15 @@
         colormap,
         title,
         title_prefix=('a', 'b'),
         vertical_axes=False,
         refined_mask_data={},
         shift_colormap=False,
         log_norm=False,
+        vmin=None,
         save=True,
         filename='scalar_field',
         clabel='',
         verbose=True):
     """
     This creates a figure with two axes.
 
@@ -167,23 +169,23 @@
 
     # Left axis
     map.ax = ax[0]
     draw_axis(ax[0], lon, lat, map, draw_coastlines=True, draw_features=True)
     title_1 = '(' + title_prefix[0] + ') ' + title + ' (Eastward Component)'
     _plot_on_each_axis(ax[0], map, lons_grid_on_map, lats_grid_on_map,
                        scalar_field_1, title_1, colormap, clabel,
-                       refined_mask_data, log_norm, shift_colormap)
+                       refined_mask_data, log_norm, shift_colormap, vmin=vmin)
 
     # Right axis
     map.ax = ax[1]
     draw_axis(ax[1], lon, lat, map, draw_coastlines=True, draw_features=True)
     title_2 = '(' + title_prefix[1] + ') ' + title + ' (Northward Component)'
     _plot_on_each_axis(ax[1], map, lons_grid_on_map, lats_grid_on_map,
                        scalar_field_2, title_2, colormap, clabel,
-                       refined_mask_data, log_norm, shift_colormap)
+                       refined_mask_data, log_norm, shift_colormap, vmin=vmin)
 
     fig.set_tight_layout(True)
     fig.patch.set_alpha(0)
 
     # Save plot
     if save:
         save_plot(filename, transparent_background=False, pdf=True,
@@ -569,19 +571,19 @@
     # cut = 0.001
     # relative_entropy_east_vel[
     #         numpy.ma.where(relative_entropy_east_vel < cut)] = 0.0
     # relative_entropy_north_vel[
     #         numpy.ma.where(relative_entropy_north_vel < cut)] = 0.0
     _plot_scalar_fields(lon, lat, map, lons_grid_on_map, lats_grid_on_map,
                         js_distance_east_vel, js_distance_north_vel,
-                        cm.Reds, 'JS Distance', title_prefix=('a', 'b'),
+                        cm.YlOrRd, 'JS Distance', title_prefix=('a', 'b'),
                         vertical_axes=False,
                         refined_mask_data=refined_mask_data,
-                        shift_colormap=False, log_norm=False, save=save,
-                        filename="js_distance", clabel='',
+                        shift_colormap=False, log_norm=False, vmin=0.0,
+                        save=save, filename="ensembles_js_distance", clabel='',
                         verbose=verbose)
 
     # Plotting additional entropies between two distributions
     # filename_1 = 'output_full_kl_expansion.nc'
     # filename_2 = 'output_truncated_kl_expansion_m100.nc'
     # import os
     # if os.path.isfile(filename_1) and os.path.isfile(filename_2):
```

### Comparing `restoreio-0.2.2/restoreio/_plots_uq/plot_kl_transform.py` & `restoreio-0.3.0/restoreio/_plots_uq/plot_kl_transform.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_plots_uq/plot_rbf_kernel.py` & `restoreio-0.3.0/restoreio/_plots_uq/plot_rbf_kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,17 @@
                      cmap=plt.cm.Reds, vmin=0.0, vmax=1.0, zorder=-1)
     # Create axes for colorbar that is the same size as the plot axes
     divider = make_axes_locatable(ax1)
     cax = divider.append_axes("right", size="5%", pad=0.09)
 
     fig1.colorbar(p, cax=cax, ticks=[0, 0.5, 1])
     p.set_clim(0, 1)
-    ax1.set_xticks([-window_lon, 0, window_lon], fontsize=13)
-    ax1.set_yticks([-window_lat, 0, window_lat], fontsize=13)
+    ax1.set_xticks([-window_lon, 0, window_lon])
+    ax1.set_yticks([-window_lat, 0, window_lat])
+    ax1.tick_params(labelsize=13)
     ax1.axis('equal')
 
     ax1.set_xlabel(r'$\Delta x_1$', fontsize=14)
     ax1.set_ylabel(r'$\Delta x_2$', fontsize=14)
 
     title = '%s Velocity Data' % vel_component.capitalize()
     if vel_component == 'east':
```

### Comparing `restoreio-0.2.2/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py` & `restoreio-0.3.0/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_restore/__init__.py` & `restoreio-0.3.0/restoreio/_restore/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_restore/_make_array_masked.py` & `restoreio-0.3.0/restoreio/_restore/_make_array_masked.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_restore/refine_grid.py` & `restoreio-0.3.0/restoreio/_restore/refine_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_restore/restore_generated_ensembles.py` & `restoreio-0.3.0/restoreio/_restore/restore_generated_ensembles.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,30 +83,28 @@
 # ===========================
 # Restore Generated Ensembles
 # ===========================
 
 def restore_generated_ensembles(
         diffusivity,
         sweep,
-        timeframe,
         fill_coast,
         alpha,
         convex_hull,
         num_ensembles,
         ratio_num_modes,
         kernel_width,
         scale_error,
-        datetime,
         lon,
         lat,
         land_indices,
         U_all_times,
         V_all_times,
-        east_vel_error_obj,
-        north_vel_error_obj,
+        U_error_all_times,
+        V_error_all_times,
         fill_value,
         plot,
         save=True,
         verbose=False):
     """
     Restore all generated ensembles, and take their mean and std.
 
@@ -124,54 +122,49 @@
           slows down the parallelization. By setting the chunk_size=100, each
           process is assigned 100 iteration, with only 1 function call. So if
           we have 4 processors, each one perform 100 tasks. After each process
           is done with a 100 task, it loads another 100 task from the pool of
           tasks in an unordered manner. The "map" in imap_unordered ensures
           that all processes are assigned a task without having an idle
           process.
-    """
 
-    # Time frame
-    if timeframe is None:
-        # Use the last time frame
-        timeframe = U_all_times.shape[0] - 1
-    else:
-        timeframe = timeframe
+    Note: despite in the notations in this function U_all_times and V_all_times
+    is used, these velocities and their error arrays indeed have only one time
+    since in uncertainty quantification we limited the time index to only one.
+    """
 
-        if timeframe >= U_all_times.shape[0]:
-            raise ValueError('Time frame is out of bound.')
+    # In UQ method, we only process one time index.
+    time_index = 0
 
     # Get one time frame of velocities
-    U_one_time = make_array_masked(U_all_times[timeframe, :, :])
-    V_one_time = make_array_masked(V_all_times[timeframe, :, :])
+    U_one_time = make_array_masked(U_all_times[time_index, :, :])
+    V_one_time = make_array_masked(V_all_times[time_index, :, :])
 
     # Check if data has errors of velocities variable
-    if (east_vel_error_obj is None):
+    if (U_error_all_times is None):
         raise ValueError('Input netCDF data does not have East ' +
                          'Velocity error, which is needed for ' +
                          'uncertainty quantification.')
-    if (north_vel_error_obj is None):
+    if (V_error_all_times is None):
         raise ValueError('Input netCDF data does not have North ' +
                          'Velocity error, which is needed for ' +
                          'uncertainty quantification.')
 
     # Make sure arrays are masked arrays
-    error_U_one_time = make_array_masked(
-            east_vel_error_obj[timeframe, :, :])
-    error_V_one_time = make_array_masked(
-            north_vel_error_obj[timeframe, :, :])
+    U_error_one_time = make_array_masked(U_error_all_times[time_index, :, :])
+    V_error_one_time = make_array_masked(V_error_all_times[time_index, :, :])
 
     # scale Errors
     scale = scale_error  # in m/s unit
-    error_U_one_time *= scale
-    error_V_one_time *= scale
+    U_error_one_time *= scale
+    V_error_one_time *= scale
 
     # Errors are usually squared. Take square root
-    # error_U_one_time = numpy.ma.sqrt(error_U_one_time)
-    # error_V_one_time = numpy.ma.sqrt(error_V_one_time)
+    # U_error_one_time = numpy.ma.sqrt(U_error_one_time)
+    # V_error_one_time = numpy.ma.sqrt(V_error_one_time)
 
     # Find indices of valid points, missing points inside and outside
     # the domain. Note: In the following line, all indices outputs are
     # Nx2, where the first column are latitude indices (not longitude)
     # and the second column indices are longitude indices (not
     # latitude)
     all_missing_indices_in_ocean, \
@@ -195,20 +188,20 @@
             missing_indices_in_ocean_inside_hull,
             missing_indices_in_ocean_outside_hull,
             valid_indices)
 
     # Generate Ensembles (lon and lat are not needed, but only used for
     # plots if uncommented)
     U_all_ensembles = generate_image_ensembles(
-            lon, lat, U_one_time, error_U_one_time, valid_indices,
+            lon, lat, U_one_time, U_error_one_time, valid_indices,
             missing_indices_in_ocean_inside_hull, num_ensembles,
             ratio_num_modes, kernel_width, 'east', plot=plot, save=save,
             verbose=verbose)
     V_all_ensembles = generate_image_ensembles(
-            lon, lat, V_one_time, error_V_one_time, valid_indices,
+            lon, lat, V_one_time, V_error_one_time, valid_indices,
             missing_indices_in_ocean_inside_hull, num_ensembles,
             ratio_num_modes, kernel_width, 'north', plot=plot, save=save,
             verbose=verbose)
 
     # Create a partial function in order to pass a function with only
     # one argument to the multiprocessor
     restore_ensemble_per_process_partial_func = partial(
@@ -270,26 +263,26 @@
     # Get statistics of U inpainted ensembles
     U_all_ensembles_inpainted_stats = get_ensembles_stat(
             land_indices,
             valid_indices,
             missing_indices_in_ocean_inside_hull,
             missing_indices_in_ocean_outside_hull,
             U_one_time,
-            error_U_one_time,
+            U_error_one_time,
             U_all_ensembles_inpainted,
             fill_value)
 
     # Get statistics of V inpainted ensembles
     V_all_ensembles_inpainted_stats = get_ensembles_stat(
             land_indices,
             valid_indices,
             missing_indices_in_ocean_inside_hull,
             missing_indices_in_ocean_outside_hull,
             V_one_time,
-            error_V_one_time,
+            V_error_one_time,
             V_all_ensembles_inpainted,
             fill_value)
 
     # Add empty dimension to the beginning of arrays dimensions for
     # taking into account of time axis.
     U_all_ensembles_inpainted_stats['CentralEnsemble'] = \
         numpy.ma.expand_dims(
@@ -371,16 +364,16 @@
         plot_ensembles_stat(
                 lon,
                 lat,
                 valid_indices,
                 missing_indices_in_ocean_inside_hull,
                 U_one_time,
                 V_one_time,
-                error_U_one_time,
-                error_V_one_time,
+                U_error_one_time,
+                V_error_one_time,
                 U_all_ensembles_inpainted,
                 V_all_ensembles_inpainted,
                 U_all_ensembles_inpainted_stats,
                 V_all_ensembles_inpainted_stats,
                 verbose=verbose)
 
     U_all_ensembles_inpainted_mean = U_all_ensembles_inpainted_stats['Mean']
@@ -391,10 +384,10 @@
     if plot is True:
         plot_convergence(
                 missing_indices_in_ocean_inside_hull,
                 U_all_ensembles_inpainted, V_all_ensembles_inpainted,
                 U_all_ensembles_inpainted_stats,
                 V_all_ensembles_inpainted_stats, save=save, verbose=verbose)
 
-    return timeframe, U_all_ensembles_inpainted_mean, \
+    return U_all_ensembles_inpainted_mean, \
         V_all_ensembles_inpainted_mean, U_all_ensembles_inpainted_std, \
         V_all_ensembles_inpainted_std, mask_info
```

### Comparing `restoreio-0.2.2/restoreio/_restore/restore_main_ensemble.py` & `restoreio-0.3.0/restoreio/_restore/restore_main_ensemble.py`

 * *Files 7% similar despite different names*

```diff
@@ -129,26 +129,25 @@
 # =====================
 # Restore Main Ensemble
 # =====================
 
 def restore_main_ensemble(
         diffusivity,
         sweep,
-        timeframe,
         fill_coast,
         alpha,
         convex_hull,
-        datetime,
         lon,
         lat,
         land_indices,
         U_all_times,
         V_all_times,
         fill_value,
         plot,
+        save=True,
         verbose=False):
     """
     Restore the given data (central ensemble).
 
     Notes on parallelization:
         - We have used multiprocessing.Pool.imap_unordered. Other options are
           apply, apply_async, map, imap, etc.
@@ -172,38 +171,33 @@
     # Create a partial function in order to pass a function with only
     # one argument to the multiprocessor
     restore_timeframe_per_process_partial_func = partial(
             _restore_timeframe_per_process, lon, lat, land_indices,
             U_all_times, V_all_times, diffusivity, sweep, fill_coast,
             convex_hull, alpha, plot, verbose)
 
-    # Restore one or all time frames
-    if timeframe is not None:
-        # Restore only one time frame
-        time_indices = [timeframe]
-    else:
-        # Inpaint all time frames
-        time_indices = range(len(datetime))
-
     # Initialize Inpainted arrays
-    array_shape = (len(time_indices), ) + U_all_times.shape[1:]
+    array_shape = U_all_times.shape
     U_all_times_inpainted = numpy.ma.empty(array_shape,
                                            dtype=float,
                                            fill_value=fill_value)
     V_all_times_inpainted = numpy.ma.empty(array_shape,
                                            dtype=float,
                                            fill_value=fill_value)
     mask_info_all_times = numpy.ma.empty(array_shape,
                                          dtype=float,
                                          fill_value=fill_value)
 
     # Multiprocessing
     num_processors = multiprocessing.cpu_count()
     pool = multiprocessing.Pool(processes=num_processors)
 
+    # Time indices to parallelize over them
+    time_indices = range(array_shape[0])
+
     # Determine chunk size
     chunk_size = int(len(time_indices) / num_processors)
     ratio = 40.0
     chunk_size = int(chunk_size / ratio)
     if chunk_size > 50:
         chunk_size = 50
     elif chunk_size < 5:
@@ -213,41 +207,32 @@
     _plot_data = {}
     progress = 0
     if verbose:
         print("Message: Restoring time frames ...")
         sys.stdout.flush()
 
     if plot is True:
-        if timeframe is not None:
-            plot_time_index = timeframe
-        else:
-            # If no timeframe is specified, use the last time for plot
-            plot_time_index = time_indices[-1]
+        # Use the last time for plot
+        plot_time_index = time_indices[-1]
 
     # Parallel section
     for time_index, U_inpainted, V_inpainted, \
             mask_info, plot_data in pool.imap_unordered(
                     restore_timeframe_per_process_partial_func,
                     time_indices, chunksize=chunk_size):
 
-        # Set index to zero when restoring a single time frame
-        if timeframe is not None:
-            array_time_index = 0
-        else:
-            array_time_index = time_index
-
         # Store plot_data for one time frame to be plotted later.
         if plot is True:
             if time_index == plot_time_index:
                 _plot_data = plot_data
 
         # Set inpainted arrays
-        U_all_times_inpainted[array_time_index, :] = U_inpainted
-        V_all_times_inpainted[array_time_index, :] = V_inpainted
-        mask_info_all_times[array_time_index, :] = mask_info
+        U_all_times_inpainted[time_index, :] = U_inpainted
+        V_all_times_inpainted[time_index, :] = V_inpainted
+        mask_info_all_times[time_index, :] = mask_info
 
         progress += 1
         if verbose:
             print("Progress: %d/%d" % (progress, len(time_indices)))
             sys.stdout.flush()
 
     pool.terminate()
@@ -267,17 +252,17 @@
                 _plot_data['missing_indices_in_ocean_outside_hull'],
                 _plot_data['valid_indices'],
                 _plot_data['hull_points_coord_list'],
                 _plot_data['U_original'],
                 _plot_data['V_original'],
                 _plot_data['U_inpainted'],
                 _plot_data['V_inpainted'],
-                save=True,
+                save=save,
                 verbose=verbose)
 
     # None arrays
     U_all_times_inpainted_error = None
     V_all_times_inpainted_error = None
 
-    return time_indices, U_all_times_inpainted, V_all_times_inpainted, \
+    return U_all_times_inpainted, V_all_times_inpainted, \
         U_all_times_inpainted_error, V_all_times_inpainted_error, \
         mask_info_all_times
```

### Comparing `restoreio-0.2.2/restoreio/_uncertainty_quant/_compute_correlation_matrix.py` & `restoreio-0.3.0/restoreio/_uncertainty_quant/_compute_correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py` & `restoreio-0.3.0/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_uncertainty_quant/_image_utils.py` & `restoreio-0.3.0/restoreio/_uncertainty_quant/_image_utils.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_uncertainty_quant/_statistical_distances.py` & `restoreio-0.3.0/restoreio/_uncertainty_quant/_statistical_distances.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_uncertainty_quant/generate_image_ensembles.py` & `restoreio-0.3.0/restoreio/_uncertainty_quant/generate_image_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.2.2/restoreio/_uncertainty_quant/get_ensembles_stat.py` & `restoreio-0.3.0/restoreio/_uncertainty_quant/get_ensembles_stat.py`

 * *Files 4% similar despite different names*

```diff
@@ -217,25 +217,26 @@
         mean_q = central_data
         std_p = numpy.std(data_ensembles)
         std_q = std_p  # not true in missing domain (here only for simplicity)
         vel_one_time_inpainted_stats['JSdistance'][i, j] = \
             js_distance(mean_p, mean_q, std_p, std_q)
 
         # mask zeros
-        if numpy.fabs(vel_one_time_inpainted_stats['RMSD'][i, j]) < 1e-8:
+        tol = 1e-7
+        if numpy.fabs(vel_one_time_inpainted_stats['RMSD'][i, j]) < tol:
             vel_one_time_inpainted_stats['RMSD'][i, j] = numpy.ma.masked
-        if numpy.fabs(vel_one_time_inpainted_stats['NRMSD'][i, j]) < 1e-8:
+        if numpy.fabs(vel_one_time_inpainted_stats['NRMSD'][i, j]) < tol:
             vel_one_time_inpainted_stats['NRMSD'][i, j] = numpy.ma.masked
-        if numpy.fabs(vel_one_time_inpainted_stats['ExNMSD'][i, j]) < 1e-8:
+        if numpy.fabs(vel_one_time_inpainted_stats['ExNMSD'][i, j]) < tol:
             vel_one_time_inpainted_stats['ExNMSD'][i, j] = numpy.ma.masked
-        if numpy.fabs(vel_one_time_inpainted_stats['Skewness'][i, j]) < 1e-8:
+        if numpy.fabs(vel_one_time_inpainted_stats['Skewness'][i, j]) < tol:
             vel_one_time_inpainted_stats['Skewness'][i, j] = numpy.ma.masked
         if numpy.fabs(
-                vel_one_time_inpainted_stats['RelativeEntropy'][i, j]) < 1e-8:
+                vel_one_time_inpainted_stats['RelativeEntropy'][i, j]) < tol:
             vel_one_time_inpainted_stats['RelativeEntropy'][i, j] = \
                     numpy.ma.masked
         if numpy.fabs(
-                vel_one_time_inpainted_stats['JSdistance'][i, j]) < 1e-8:
+                vel_one_time_inpainted_stats['JSdistance'][i, j]) < tol:
             vel_one_time_inpainted_stats['JSdistance'][i, j] = \
                     numpy.ma.masked
 
     return vel_one_time_inpainted_stats
```

### Comparing `restoreio-0.2.2/restoreio/scripts/scan_netcdf.py` & `restoreio-0.3.0/restoreio/_scripts/scan_netcdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,39 +61,39 @@
 # ===============
 
 def _parse_arguments(argv):
     """
     Parses the argument of the executable and obtains the filename.
 
     Input file is netcdf nc file or ncml file.
-    Output is a strigified Json.
+    Output is a stratified Json.
     """
 
     # -------------
     # Print Version
     # -------------
 
     def _print_version():
 
         version_string = \
-                """
+            """
 Version 0.0.1
 Siavash Ameli
 University of California, Berkeley
-                """
+            """
 
         print(version_string)
 
     # -----------
     # Print Usage
     # -----------
 
     def _print_usage(exec_name):
         usage_string = "Usage: " + exec_name + \
-                " -i <input_filename.{nc, ncml}>"
+            " -i <input_filename.{nc, ncml}>"
         options_string = \
             """
 Required arguments:
 
     -i --input          Input filename. This should be full path. Input file
                         extension can be *.nc or *.ncml.
 
@@ -152,15 +152,15 @@
     if len(argv) < 2:
         _print_usage(argv[0])
         sys.exit(0)
 
     # Check input_filename
     if (input_filename == ''):
         _print_usage(argv[0])
-        raise RuntimeError("input_filename is empty.")
+        _terminate_with_error("Input filename or url is empty.")
 
     return input_filename, scan_velocity_status
 
 
 # ==================
 # Load Local Dataset
 # ==================
@@ -168,15 +168,15 @@
 def _load_local_dataset(filename):
     """
     Opens either ncml or nc file and returns the aggregation file object.
     """
 
     # Check file extension
     file_extension = os.path.splitext(filename)[1]
-    if file_extension == '.ncml':
+    if file_extension in ['.ncml', '.ncml.gz']:
 
         # Change directory
         data_directory = os.path.dirname(filename)
         current_directory = os.getcwd()
         os.chdir(data_directory)
 
         # NCML
@@ -189,22 +189,22 @@
         files_list = [f.path for f in nc.members]
         os.chdir(current_directory)
 
         # Aggregate
         agg = netCDF4.MFDataset(files_list, aggdim='t')
         return agg
 
-    elif file_extension == '.nc':
+    elif file_extension in ['.nc', '.ncd', '.nc.gz']:
 
         nc = netCDF4.Dataset(filename)
         return nc
 
     else:
-        raise RuntimeError("File should be either ncml or nc. filename: " +
-                           filename)
+        _terminate_with_error(
+            "File format %s is not recognized." % file_extension)
 
 
 # ===================
 # Load Remote Dataset
 # ===================
 
 def _load_remote_dataset(url):
@@ -220,41 +220,40 @@
                               'or <code>https://</code>.')
     elif ("/thredds/dodsC/" not in url) and ("opendap" not in url):
         _terminate_with_error('Input data URL is not an <b>OpenDap</b> URL ' +
                               'or is not hosted on a THREDDs server. Check ' +
                               'if your data URL contains ' +
                               '<code>/thredds/dodsC/</code> or ' +
                               '<code>/opendap/</code>.')
-    elif url.endswith(('.nc', '.nc.gz', '.ncd', '.ncml', '.ncml.gz')) is False:
-        _terminate_with_error('The input data URL is not a <i>netcdf</i> ' +
-                              'file. The URL should end with ' +
-                              '<code>.nc</code>, <code>.nc.gz</code>, ' +
-                              '<code>.ncml</code> or <code>.ncml.gz</code>.')
 
     # Check file extension
     file_extension = os.path.splitext(url)[1]
 
     # Case of zipped files (get the correct file extension before the '.gz')
     if file_extension == ".gz":
         file_extension = os.path.splitext(url[:-3])[1]
 
-    if file_extension == '.ncml':
-
-        # nc = open_url(url)
-        nc = netCDF4.Dataset(url)
+    # Note that some opendap urls do not even have a file extension
+    if file_extension != "":
 
-    elif (file_extension == '.nc') or (file_extension == '.ncd'):
+        # If a file extension exists, check if it is a standard netcdf file
+        if file_extension not in \
+                ['.nc', '.ncd', '.nc.gz', '.ncml', '.ncml.gz']:
+            _terminate_with_error(
+                'The input data URL is not an <i>netcdf</i> file. The URL ' +
+                'should end with <code>.nc</code>, <code>.ncd</code>, ' +
+                '<code>.nc.gz</code>, <code>.ncml</code>, ' +
+                '<code>.ncml.gz</code>, or without file extension.')
 
+    try:
+        # nc = open_url(url)
         nc = netCDF4.Dataset(url)
 
-    else:
-        _terminate_with_error('File extension in the data URL should be ' +
-                              'either <code>.nc</code>, ' +
-                              '<code>.nc.gz</code>, <code>.ncml</code> or ' +
-                              '<code>.ncml.gz</code>.')
+    except OSError:
+        _terminate_with_error('Unable to read %s.' % url)
 
     return nc
 
 
 # ============
 # Load Dataset
 # ============
@@ -346,15 +345,15 @@
     - Latitude
     """
 
     # Time
     time_names_list = ['time', 'datetime', 't']
     time_standard_names_list = ['time']
     datetime_obj, datetime_name, datetime_standard_name = _search_variable(
-            agg, time_names_list, time_standard_names_list)
+        agg, time_names_list, time_standard_names_list)
 
     # Check time variable
     if datetime_obj is None:
         _terminate_with_error('Can not find the <i>time</i> variable in ' +
                               'the netcdf file.')
     elif hasattr(datetime_obj, 'units') is False:
         _terminate_with_error('The <t>time</i> variable does not have ' +
@@ -366,15 +365,15 @@
         _terminate_with_error('The <i>time</i> variable size should be at ' +
                               'least <tt>2</tt>.')
 
     # Longitude
     longitude_names_list = ['longitude', 'lon', 'long']
     longitude_standard_names_list = ['longitude']
     longitude_obj, longitude_name, longitude_standard_name = _search_variable(
-            agg, longitude_names_list, longitude_standard_names_list)
+        agg, longitude_names_list, longitude_standard_names_list)
 
     # Check longitude variable
     if longitude_obj is None:
         _terminate_with_error('Can not find the <i>longitude</i> variable ' +
                               'in the netcdf file.')
     elif len(longitude_obj.shape) != 1:
         _terminate_with_error('The <t>longitude</i> variable dimension ' +
@@ -383,15 +382,15 @@
         _terminate_with_error('The <i>longitude</i> variable size should ' +
                               'be at least <tt>2</tt>.')
 
     # Latitude
     latitude_names_list = ['latitude', 'lat']
     latitude_standard_names_list = ['latitude']
     latitude_obj, latitude_name, latitude_standard_name = _search_variable(
-            agg, latitude_names_list, latitude_standard_names_list)
+        agg, latitude_names_list, latitude_standard_names_list)
 
     # Check latitude variable
     if latitude_obj is None:
         _terminate_with_error('Can not find the <i>latitude</i> variable in ' +
                               'the netcdf file.')
     elif len(latitude_obj.shape) != 1:
         _terminate_with_error('The <t>latitude</i> variable dimension ' +
@@ -423,16 +422,16 @@
         _search_variable(agg, east_velocity_names_list,
                          east_velocity_standard_names_list)
 
     # North Velocity
     north_velocity_names_list = ['north_vel', 'northward_vel', 'v',
                                  'north_velocity', 'northward_velocity']
     north_velocity_standard_names_list = [
-            'surface_northward_sea_water_velocity',
-            'northward_sea_water_velocity']
+        'surface_northward_sea_water_velocity',
+        'northward_sea_water_velocity']
     north_velocity_obj, north_velocity_name, north_velocity_standard_name = \
         _search_variable(agg, north_velocity_names_list,
                          north_velocity_standard_names_list)
 
     return east_velocity_obj, north_velocity_obj, east_velocity_name, \
         north_velocity_name, east_velocity_standard_name, \
         north_velocity_standard_name
@@ -495,15 +494,15 @@
             days_list.append(datetime.datetime(
                 year, month, day, hour, minute, second))
 
         # Convert dates to numbers
         datetimes = netCDF4.date2num(days_list, units=datetimes_unit,
                                      calendar=datetimes_calendar)
     else:
-        raise RuntimeError("Datetime ndim is more than 2.")
+        _terminate_with_error("Datetime ndim is more than 2.")
 
     return datetimes, datetimes_unit, datetimes_calendar
 
 
 # =============
 # Get Time Info
 # =============
@@ -515,30 +514,30 @@
 
     datetimes, datetimes_unit, datetimes_calendar = \
         _prepare_datetimes(datetime_obj)
 
     # Initial time
     initial_time = datetimes[0]
     initial_datetime_obj = netCDF4.num2date(
-            initial_time, units=datetimes_unit, calendar=datetimes_calendar)
+        initial_time, units=datetimes_unit, calendar=datetimes_calendar)
 
     initial_time_dict = {
         "Year": str(initial_datetime_obj.year).zfill(4),
         "Month": str(initial_datetime_obj.month).zfill(2),
         "Day": str(initial_datetime_obj.day).zfill(2),
         "Hour": str(initial_datetime_obj.hour).zfill(2),
         "Minute": str(initial_datetime_obj.minute).zfill(2),
         "Second": str(initial_datetime_obj.second).zfill(2),
         "Microsecond": str(initial_datetime_obj.microsecond).zfill(6)
     }
 
     # Round off with microsecond
     if int(initial_time_dict['Microsecond']) > 500000:
         initial_time_dict['Microsecond'] = '000000'
-        initial_time_dict['Second'] = str(int(initial_time_dict['Second'])+1)
+        initial_time_dict['Second'] = str(int(initial_time_dict['Second']) + 1)
 
     # Round off with second
     if int(initial_time_dict['Second']) >= 60:
         excess_second = int(initial_time_dict['Second']) - 60
         initial_time_dict['Second'] = '00'
         initial_time_dict['Minute'] = \
             str(int(initial_time_dict['Minute']) + excess_second + 1)
@@ -556,15 +555,15 @@
         initial_time_dict['Hour'] = '00'
         initial_time_dict['Day'] = \
             str(int(initial_time_dict['Day']) + excess_hour + 1)
 
     # Final time
     final_time = datetimes[-1]
     final_datetime_obj = netCDF4.num2date(
-            final_time, units=datetimes_unit, calendar=datetimes_calendar)
+        final_time, units=datetimes_unit, calendar=datetimes_calendar)
 
     final_time_dict = {
         "Year": str(final_datetime_obj.year).zfill(4),
         "Month": str(final_datetime_obj.month).zfill(2),
         "Day": str(final_datetime_obj.day).zfill(2),
         "Hour": str(final_datetime_obj.hour).zfill(2),
         "Minute": str(final_datetime_obj.minute).zfill(2),
@@ -623,16 +622,16 @@
 
     # Round off with microsecond
     # time_duration = numpy.floor(time_duration + 0.5)
     time_duration = numpy.floor(time_duration)
 
     # Day
     residue = 0.0
-    time_duration_day = int(numpy.floor(time_duration/(24.0*3600.0)))
-    residue = time_duration - float(time_duration_day) * (24.0*3600.0)
+    time_duration_day = int(numpy.floor(time_duration / (24.0 * 3600.0)))
+    residue = time_duration - float(time_duration_day) * (24.0 * 3600.0)
 
     # Hour
     time_duration_hour = int(numpy.floor(residue / 3600.0))
     residue -= float(time_duration_hour) * 3600.0
 
     # Minute
     time_duration_minute = int(numpy.floor(residue / 60.0))
@@ -702,38 +701,38 @@
     view_scale = 1.4
     view_range = numpy.clip(longitude_range * view_scale, 0.0,
                             2.0 * earth_radius * view_scale)
 
     # Pitch Angle, measured from horizon downward. 45 degrees for small ranges,
     # approaches 90 degrees for large ranges.
     pitch_angle = 45.0 + 45.0 * numpy.max(
-            [numpy.fabs(max_longitude-min_longitude)/360.0,
-             numpy.fabs(max_latitude-min_latitude)/180.0])
+        [numpy.fabs(max_longitude - min_longitude) / 360.0,
+         numpy.fabs(max_latitude - min_latitude) / 180.0])
 
     # Bounds for Camera
     latitude_ratio = 0.2
     latitude_span = max_latitude - min_latitude
 
     # On very large latitude spans, the latitude_ratio becomes ineffective.
     camera_min_latitude = numpy.clip(
-            min_latitude - latitude_ratio * latitude_span *
-            (1.0 - latitude_span/180.0), -90.0, 90.0)
+        min_latitude - latitude_ratio * latitude_span *
+        (1.0 - latitude_span / 180.0), -90.0, 90.0)
     camera_max_latitude = numpy.clip(
-            max_latitude + latitude_ratio * latitude_span *
-            (1.0 - latitude_span/180.0), -90.0, 90.0)
+        max_latitude + latitude_ratio * latitude_span *
+        (1.0 - latitude_span / 180.0), -90.0, 90.0)
 
     longitude_ratio = 0.2
     longitude_span = max_longitude - min_longitude
 
     # On very large longitude spans, the longitude_ratio becomes ineffective.
     camera_min_longitude = mid_longitude - numpy.clip(
-        longitude_span/2.0 + longitude_ratio * longitude_span *
+        longitude_span / 2.0 + longitude_ratio * longitude_span *
         (1.0 - longitude_span / 360.0), 0.0, 90.0)
     camera_max_longitude = mid_longitude + numpy.clip(
-        longitude_span/2.0 + longitude_ratio * longitude_span *
+        longitude_span / 2.0 + longitude_ratio * longitude_span *
         (1.0 - longitude_span / 360.0), 0.0, 90.0)
 
     data_bounds_dict = {
         "MinLatitude": str(min_latitude),
         "MidLatitude": str(mid_latitude),
         "MaxLatitude": str(max_latitude),
         "MinLongitude": str(min_longitude),
@@ -803,14 +802,46 @@
         velocity_name = '_'.join(str(s) for s in velocity_name_list)
     else:
         velocity_name = ''
 
     return velocity_name
 
 
+# =====================
+# Get Array Memory Size
+# =====================
+
+def _get_array_memory_size(array):
+    """
+    If array ndim is three, such as (time, lat, lon), this function returns
+    the size of array(0, :, :).
+
+    If array ndim is four, such as (time, depth, lat, lon), this function
+    returns the size of array(0, 0, :, :).
+    """
+
+    # Depending on ndim, exclude time and depth dimensions as they wont be read
+    if array.ndim == 3:
+        shape = array.shape[1:]
+        itemsize = array[0, 0, :0].itemsize
+    elif array.ndim == 4:
+        shape = array.shape[2:]
+        itemsize = array[0, 0, 0, :0].itemsize
+    else:
+        _terminate_with_error('Array ndim should be three or four.')
+
+    # Size of array (excluding time and depth dimensions)
+    size = numpy.prod(shape)
+
+    # Size of array in bytes
+    num_bytes = size * itemsize
+
+    return num_bytes
+
+
 # =================
 # Get Velocity Info
 # =================
 
 def _get_velocity_info(
         east_velocity_obj,
         north_velocity_obj,
@@ -820,42 +851,77 @@
         north_velocity_standard_name):
     """
     Get dictionary of velocities.
     """
 
     # Get the number of indices to be selected for finding min and max.
     num_times = east_velocity_obj.shape[0]
-    num_time_indices = 10  # Selecting 10 samples
+
+    # Get the size of one of the velocity arrays
+    num_bytes = _get_array_memory_size(east_velocity_obj)
+    num_Mbytes = num_bytes / (1024**2)
+
+    # Number of time instances to sample from velocity data
+    if num_Mbytes >= 10.0:
+        # If the array is larger than 10 MB, sample only one time of array
+        num_time_indices = 1
+    elif num_Mbytes >= 1.0:
+        num_time_indices = 2
+    else:
+        num_time_indices = 5
+
+    # Cap the number of time samples by the number of times
     if num_time_indices > num_times:
         num_time_indices = num_times
 
     # The selection of random time indices to be used for finding min and max
     numpy.random.seed(0)
-    times_indices = numpy.random.randint(0, num_times-1, num_time_indices)
+    times_indices = numpy.random.randint(0, num_times - 1, num_time_indices)
 
     # Min/Max velocities for each time frame
     east_velocities_mean = numpy.zeros(len(times_indices), dtype=float)
     east_velocities_std = numpy.zeros(len(times_indices), dtype=float)
     north_velocities_mean = numpy.zeros(len(times_indices), dtype=float)
     north_velocities_std = numpy.zeros(len(times_indices), dtype=float)
 
     # Find Min and Max of each time frame
     for k in range(len(times_indices)):
 
         time_index = times_indices[k]
 
         with numpy.errstate(invalid='ignore'):
-            east_velocities_mean[k] = \
-                numpy.nanmean(east_velocity_obj[time_index, :, :])
-            east_velocities_std[k] = \
-                numpy.nanstd(east_velocity_obj[time_index, :, :])
-            north_velocities_mean[k] = \
-                numpy.nanmean(north_velocity_obj[time_index, :, :])
-            north_velocities_std[k] = \
-                numpy.nanstd(north_velocity_obj[time_index, :, :])
+
+            # Find vel dimension is (time, lat, lon) or (time, depth, lat, lon)
+            if east_velocity_obj.ndim == 3:
+
+                # Velocity dimension is (time, lat, lon)
+                east_velocities_mean[k] = \
+                    numpy.nanmean(east_velocity_obj[time_index, :, :])
+                east_velocities_std[k] = \
+                    numpy.nanstd(east_velocity_obj[time_index, :, :])
+                north_velocities_mean[k] = \
+                    numpy.nanmean(north_velocity_obj[time_index, :, :])
+                north_velocities_std[k] = \
+                    numpy.nanstd(north_velocity_obj[time_index, :, :])
+
+            elif east_velocity_obj.ndim == 4:
+
+                # Velocity dimension is (time, depth, lat, lon)
+                depth_index = 0
+                east_velocities_mean[k] = numpy.nanmean(
+                    east_velocity_obj[time_index, depth_index, :, :])
+                east_velocities_std[k] = numpy.nanstd(
+                    east_velocity_obj[time_index, depth_index, :, :])
+                north_velocities_mean[k] = numpy.nanmean(
+                    north_velocity_obj[time_index, depth_index, :, :])
+                north_velocities_std[k] = numpy.nanstd(
+                    north_velocity_obj[time_index, depth_index, :, :])
+
+            else:
+                _terminate_with_error('Velocity ndim should be three or four.')
 
     # Mean and STD of Velocities among all time frames
     east_velocity_mean = numpy.nanmean(east_velocities_mean)
     east_velocity_std = numpy.nanmean(east_velocities_std)
     north_velocity_mean = numpy.nanmean(north_velocities_mean)
     north_velocity_std = numpy.nanmean(north_velocities_std)
 
@@ -872,15 +938,15 @@
                                north_velocity_mean**2 + north_velocity_std**2)
     typical_velocity_speed = 4.0 * velocity_mean
 
     # Get the velocity name from east and north names
     if (east_velocity_standard_name != '') and \
             (north_velocity_standard_name != ''):
         velocity_standard_name = _get_velocity_name(
-                east_velocity_standard_name, north_velocity_standard_name)
+            east_velocity_standard_name, north_velocity_standard_name)
     else:
         velocity_standard_name = ''
 
     # Create a Velocity Info Dict
     velocity_info_dict = {
         "EastVelocityName": east_velocity_name,
         "NorthVelocityName": north_velocity_name,
@@ -944,20 +1010,24 @@
     dataset_info_dict['SpaceInfo'] = space_info_dict
 
     # Velocities
     if scan_velocity_status is True:
 
         # Get velocity objects
         east_velocity_obj, north_velocity_obj, east_velocity_name, \
-                north_velocity_name, east_velocity_standard_name, \
-                north_velocity_standard_name = _load_velocity_variables(agg)
+            north_velocity_name, east_velocity_standard_name, \
+            north_velocity_standard_name = _load_velocity_variables(agg)
+
+        # Read velocity data and find info
         velocity_info_dict = _get_velocity_info(
-                east_velocity_obj, north_velocity_obj, east_velocity_name,
-                north_velocity_name, east_velocity_standard_name,
-                north_velocity_standard_name)
+            east_velocity_obj, north_velocity_obj, east_velocity_name,
+            north_velocity_name, east_velocity_standard_name,
+            north_velocity_standard_name)
+
+        # Store in dictionary
         dataset_info_dict['VelocityInfo'] = velocity_info_dict
 
     agg.close()
 
     dataset_info_json = json.dumps(dataset_info_dict, indent=4)
     print(dataset_info_json)
     sys.stdout.flush()
```

### Comparing `restoreio-0.2.2/restoreio.egg-info/PKG-INFO` & `restoreio-0.3.0/restoreio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.2.2
+Version: 0.3.0
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
```

### Comparing `restoreio-0.2.2/restoreio.egg-info/SOURCES.txt` & `restoreio-0.3.0/restoreio.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -37,30 +37,45 @@
 docs/source/_static/images/icons/logo-pypi.ico
 docs/source/_static/images/icons/logo-pypi.png
 docs/source/_static/images/icons/logo-pypi.svg
 docs/source/_static/images/icons/logo-restoreio-dark.png
 docs/source/_static/images/icons/logo-restoreio-dark.svg
 docs/source/_static/images/icons/logo-restoreio-light.png
 docs/source/_static/images/icons/logo-restoreio-light.svg
+docs/source/_static/images/plots/cor_cov.png
+docs/source/_static/images/plots/deviation.png
+docs/source/_static/images/plots/ensembles.png
+docs/source/_static/images/plots/ensembles_js_distance.png
+docs/source/_static/images/plots/gdop_coverage.png
+docs/source/_static/images/plots/js_distance.png
+docs/source/_static/images/plots/kl_eigenvalues.png
+docs/source/_static/images/plots/kl_eigenvectors.png
+docs/source/_static/images/plots/orig_vel_and_error.png
+docs/source/_static/images/plots/rbf_kernel_2d.png
 docs/source/_static/js/custom-pydata.js
 docs/source/_templates/layout.html
 docs/source/_templates/sidebar-nav-bs.html
 docs/source/_templates/version.html
 docs/source/_templates/autosummary/attribute.rst
 docs/source/_templates/autosummary/class.rst
 docs/source/_templates/autosummary/method.rst
 docs/source/_templates/autosummary/ndarray_subclass.rst
 docs/source/_templates/autosummary/property.rst
 docs/source/generated/restoreio.restore.rst
 docs/source/notebooks/quick_start.ipynb
-examples/main_VaryingNumModes.py
-examples/plot_coverage.py
-examples/plot_fixed_size_artificial_mask.py
-examples/plot_variable_d_artificial_masks.py
-examples/plot_variable_size_artificial_masks.py
+examples/restore/main_VaryingNumModes.py
+examples/restore/plot_coverage.py
+examples/restore/plot_fixed_size_artificial_mask.py
+examples/restore/plot_variable_d_artificial_masks.py
+examples/restore/plot_variable_size_artificial_masks.py
+examples/uncertainty_quant/_display_utilities.py
+examples/uncertainty_quant/_draw_map.py
+examples/uncertainty_quant/_plot_utilities.py
+examples/uncertainty_quant/plot_gdop_coverage.py
+examples/uncertainty_quant/plot_js_divergence.py
 restoreio/__init__.py
 restoreio/__main__.py
 restoreio/__version__.py
 restoreio.egg-info/PKG-INFO
 restoreio.egg-info/SOURCES.txt
 restoreio.egg-info/dependency_links.txt
 restoreio.egg-info/entry_points.txt
@@ -76,21 +91,22 @@
 restoreio/_geography/locate_missing_data.py
 restoreio/_inpaint/__init__.py
 restoreio/_inpaint/_cast_types.py
 restoreio/_inpaint/_image.py
 restoreio/_inpaint/_plot_image.py
 restoreio/_inpaint/inpaint.py
 restoreio/_input_output/__init__.py
+restoreio/_input_output/get_datetime_info.py
 restoreio/_input_output/load_dataset.py
 restoreio/_input_output/load_variables.py
 restoreio/_input_output/writer.py
 restoreio/_parser/__init__.py
 restoreio/_parser/examples.py
 restoreio/_parser/formatter.py
-restoreio/_parser/parser.py
+restoreio/_parser/parse_arguments.py
 restoreio/_plots/__init__.py
 restoreio/_plots/_display_utilities.py
 restoreio/_plots/_draw_map.py
 restoreio/_plots/_plot_grid.py
 restoreio/_plots/_plot_quiver.py
 restoreio/_plots/_plot_streamlines.py
 restoreio/_plots/_plot_utilities.py
@@ -107,17 +123,22 @@
 restoreio/_plots_uq/plot_rbf_kernel.py
 restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
 restoreio/_restore/__init__.py
 restoreio/_restore/_make_array_masked.py
 restoreio/_restore/refine_grid.py
 restoreio/_restore/restore_generated_ensembles.py
 restoreio/_restore/restore_main_ensemble.py
+restoreio/_scripts/__init__.py
+restoreio/_scripts/scan_netcdf.py
+restoreio/_subset/__init__.py
+restoreio/_subset/_array_utilities.py
+restoreio/_subset/subset_datetime.py
+restoreio/_subset/subset_domain.py
 restoreio/_uncertainty_quant/__init__.py
 restoreio/_uncertainty_quant/_compute_correlation_matrix.py
 restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
 restoreio/_uncertainty_quant/_image_utils.py
 restoreio/_uncertainty_quant/_statistical_distances.py
 restoreio/_uncertainty_quant/generate_image_ensembles.py
 restoreio/_uncertainty_quant/get_ensembles_stat.py
-restoreio/scripts/__init__.py
-restoreio/scripts/scan_netcdf.py
-tests/test_restore.py
+tests/test_restore_local_data.py
+tests/test_restore_remote_data.py
```

### Comparing `restoreio-0.2.2/setup.py` & `restoreio-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         extras_require={
             'test': test_requirements,
             'docs': docs_requirements,
         },
         entry_points={
             "console_scripts": [
                 "restore = restoreio.__main__:main",
-                "scan = restoreio.scripts.scan_netcdf:main"
+                "scan = restoreio._scripts.scan_netcdf:main"
             ]
         },
         classifiers=[
             'Programming Language :: Python',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
```

### Comparing `restoreio-0.2.2/tests/test_restore.py` & `restoreio-0.3.0/tests/test_restore_local_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,39 +44,46 @@
 # ============
 
 def test_restore():
     """
     Test for `restore` function.
     """
 
+    # Data
     input = 'Monterey_Small_2km_Hourly_2017_01.nc'
-    output = 'output.nc'
-    timeframe = 117
+    output = 'output_local_data.nc'
+    min_lon = None
+    max_lon = None
+    min_lat = None
+    max_lat = None
+    time = '2017-01-25T03:00:00'
 
     # Absolute path
     dir = os.path.dirname(os.path.realpath(__file__))
     input = os.path.join(dir, input)
     output = os.path.join(dir, output)
 
     # Check input exists
     if not os.path.exists(input):
         raise RuntimeError('File: %s does not exists.' % input)
 
     # Restore main file
     restore(input, min_file_index='', max_file_index='', output=output,
-            sweep=False, detect_land=True, fill_coast=False, convex_hull=False,
-            alpha=20, refine_grid=1, timeframe=timeframe,
+            min_lon=min_lon, max_lon=max_lon, min_lat=min_lat, max_lat=max_lat,
+            time=time, sweep=False, detect_land=True, fill_coast=False,
+            convex_hull=False, alpha=20, refine_grid=1,
             uncertainty_quant=False, plot=True, verbose=True)
 
     # Uncertainty quantification
     restore(input, min_file_index='', max_file_index='', output=output,
-            sweep=False, detect_land=True, fill_coast=False, convex_hull=False,
-            alpha=20, refine_grid=1, timeframe=timeframe,
-            uncertainty_quant=True, num_ensembles=200, ratio_num_modes=1,
-            kernel_width=5, scale_error=0.08, plot=True, verbose=True)
+            min_lon=min_lon, max_lon=max_lon, min_lat=min_lat, max_lat=max_lat,
+            time=time, sweep=False, detect_land=True, fill_coast=False,
+            convex_hull=False, alpha=20, refine_grid=1, uncertainty_quant=True,
+            num_ensembles=200, ratio_num_modes=1, kernel_width=5,
+            scale_error=0.08, plot=True, verbose=True)
 
     # Remove outputs
     remove_file('*.svg')
     remove_file('*.pdf')
     remove_file(output)
```

### Comparing `restoreio-0.2.2/tox.ini` & `restoreio-0.3.0/tox.ini`

 * *Files identical despite different names*

