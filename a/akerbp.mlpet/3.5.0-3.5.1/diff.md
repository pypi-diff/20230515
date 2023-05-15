# Comparing `tmp/akerbp.mlpet-3.5.0.tar.gz` & `tmp/akerbp.mlpet-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akerbp.mlpet-3.5.0.tar", max compression
+gzip compressed data, was "akerbp.mlpet-3.5.1.tar", last modified: Mon May 15 12:49:52 2023, max compression
```

## Comparing `akerbp.mlpet-3.5.0.tar` & `akerbp.mlpet-3.5.1.tar`

### file list

```diff
@@ -1,35 +1,137 @@
--rw-r--r--   0        0        0    11320 2023-03-24 07:41:07.459159 akerbp.mlpet-3.5.0/LICENSE
--rw-r--r--   0        0        0     5504 2023-03-24 07:41:07.459159 akerbp.mlpet-3.5.0/README.md
--rw-r--r--   0        0        0     1774 2023-03-24 07:41:07.483159 akerbp.mlpet-3.5.0/pyproject.toml
--rw-r--r--   0        0        0      499 2023-03-24 07:41:07.483159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 07:41:07.483159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/data/__init__.py
--rw-r--r--   0        0        0     8846 2023-03-24 07:41:07.483159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/data/mappings.py
--rw-r--r--   0        0        0    10241 2023-03-24 07:41:07.483159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/data/npd_fm_gp_sy_key_dic.pcl
--rw-r--r--   0        0        0     4995 2023-03-24 07:41:07.483159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/dataloader.py
--rw-r--r--   0        0        0    38280 2023-03-24 07:41:07.483159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/dataset.py
--rw-r--r--   0        0        0    29096 2023-03-24 07:41:07.483159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/feature_engineering.py
--rw-r--r--   0        0        0    16008 2023-03-24 07:41:07.487159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/imputers.py
--rw-r--r--   0        0        0    14307 2023-03-24 07:41:07.487159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/petrophysical_features.py
--rw-r--r--   0        0        0    18016 2023-03-24 07:41:07.487159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/plotting.py
--rw-r--r--   0        0        0    51691 2023-03-24 07:41:07.487159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/plotting_helpers.py
--rw-r--r--   0        0        0     3981 2023-03-24 07:41:07.487159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/plotting_variables.py
--rw-r--r--   0        0        0    37276 2023-03-24 07:41:07.487159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/preprocessors.py
--rw-r--r--   0        0        0      172 2023-03-24 07:41:07.487159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/client.py
--rw-r--r--   0        0        0  5616970 2023-03-24 07:41:07.515159 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/data/15_9-23.las
--rw-r--r--   0        0        0  7480569 2023-03-24 07:41:07.551160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/data/25_2-7.las
--rw-r--r--   0        0        0  4598499 2023-03-24 07:41:07.575160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/data/35_12-1.las
--rw-r--r--   0        0        0    29332 2023-03-24 07:41:07.575160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/data/data.py
--rw-r--r--   0        0        0     4140 2023-03-24 07:41:07.575160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/data/test_mappings.yaml
--rw-r--r--   0        0        0      695 2023-03-24 07:41:07.575160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/data/test_settings.yaml
--rw-r--r--   0        0        0      608 2023-03-24 07:41:07.575160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_dataloader.py
--rw-r--r--   0        0        0     5361 2023-03-24 07:41:07.575160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_dataset.py
--rw-r--r--   0        0        0     6156 2023-03-24 07:41:07.575160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_feature_engineering.py
--rw-r--r--   0        0        0     1023 2023-03-24 07:41:07.575160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_imputers.py
--rw-r--r--   0        0        0     1857 2023-03-24 07:41:07.575160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_petrophysical_features.py
--rw-r--r--   0        0        0     1179 2023-03-24 07:41:07.575160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_preprocessors.py
--rw-r--r--   0        0        0     1579 2023-03-24 07:41:07.575160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_transformer.py
--rw-r--r--   0        0        0     4768 2023-03-24 07:41:07.575160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_utilities.py
--rw-r--r--   0        0        0     4160 2023-03-24 07:41:07.575160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/transformer.py
--rw-r--r--   0        0        0    60903 2023-03-24 07:41:07.575160 akerbp.mlpet-3.5.0/src/akerbp/mlpet/utilities.py
--rw-r--r--   0        0        0     6897 2023-03-24 07:41:26.505885 akerbp.mlpet-3.5.0/setup.py
--rw-r--r--   0        0        0     6930 2023-03-24 07:41:26.506574 akerbp.mlpet-3.5.0/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.591736 akerbp.mlpet-3.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    19183 2023-05-15 12:49:52.591736 akerbp.mlpet-3.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5504 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2813 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.551735 akerbp.mlpet-3.5.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/Makefile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.547735 akerbp.mlpet-3.5.1/docs/build/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.555735 akerbp.mlpet-3.5.1/docs/build/doctrees/
+-rw-rw-rw-   0 root         (0) root         (0)    45723 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.dataloader.doctree
+-rw-rw-rw-   0 root         (0) root         (0)    75232 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.dataset.doctree
+-rw-rw-rw-   0 root         (0) root         (0)   102852 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.doctree
+-rw-rw-rw-   0 root         (0) root         (0)   206422 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.feature_engineering.doctree
+-rw-rw-rw-   0 root         (0) root         (0)    91063 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.imputers.doctree
+-rw-rw-rw-   0 root         (0) root         (0)   180488 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.preprocessors.doctree
+-rw-rw-rw-   0 root         (0) root         (0)   260035 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.utilities.doctree
+-rw-rw-rw-   0 root         (0) root         (0)   231460 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/environment.pickle
+-rw-rw-rw-   0 root         (0) root         (0)    20072 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/index.doctree
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.555735 akerbp.mlpet-3.5.1/docs/build/html/
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/.buildinfo
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.555735 akerbp.mlpet-3.5.1/docs/build/html/_modules/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.547735 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.559735 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/
+-rw-rw-rw-   0 root         (0) root         (0)    25163 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/dataloader.html
+-rw-rw-rw-   0 root         (0) root         (0)   104462 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/dataset.html
+-rw-rw-rw-   0 root         (0) root         (0)   179606 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/feature_engineering.html
+-rw-rw-rw-   0 root         (0) root         (0)    63553 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/imputers.html
+-rw-rw-rw-   0 root         (0) root         (0)   114510 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/preprocessors.html
+-rw-rw-rw-   0 root         (0) root         (0)    25544 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/transformer.html
+-rw-rw-rw-   0 root         (0) root         (0)   158706 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/utilities.html
+-rw-rw-rw-   0 root         (0) root         (0)    10828 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/index.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.559735 akerbp.mlpet-3.5.1/docs/build/html/_sources/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.dataloader.rst.txt
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.dataset.rst.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.feature_engineering.rst.txt
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.imputers.rst.txt
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.preprocessors.rst.txt
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.rst.txt
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.utilities.rst.txt
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/index.rst.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.563736 akerbp.mlpet-3.5.1/docs/build/html/_static/
+-rw-rw-rw-   0 root         (0) root         (0)    14692 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/basic.css
+-rw-rw-rw-   0 root         (0) root         (0)     9758 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/doctools.js
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/documentation_options.js
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/file.png
+-rw-rw-rw-   0 root         (0) root         (0)   287630 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/jquery-3.5.1.js
+-rw-rw-rw-   0 root         (0) root         (0)    89476 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    10854 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/language_data.js
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/minus.png
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/plus.png
+-rw-rw-rw-   0 root         (0) root         (0)    20800 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/pygments.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.563736 akerbp.mlpet-3.5.1/docs/build/html/_static/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/scripts/furo-extensions.js
+-rw-rw-rw-   0 root         (0) root         (0)     4861 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/scripts/furo.js
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/scripts/furo.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    27037 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/scripts/furo.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    16793 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/searchtools.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.563736 akerbp.mlpet-3.5.1/docs/build/html/_static/styles/
+-rw-rw-rw-   0 root         (0) root         (0)     5286 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/styles/furo-extensions.css
+-rw-rw-rw-   0 root         (0) root         (0)     7166 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/styles/furo-extensions.css.map
+-rw-rw-rw-   0 root         (0) root         (0)    46533 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/styles/furo.css
+-rw-rw-rw-   0 root         (0) root         (0)    68704 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/styles/furo.css.map
+-rw-rw-rw-   0 root         (0) root         (0)    68420 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/underscore-1.13.1.js
+-rw-rw-rw-   0 root         (0) root         (0)    19530 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/underscore.js
+-rw-rw-rw-   0 root         (0) root         (0)    23735 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.dataloader.html
+-rw-rw-rw-   0 root         (0) root         (0)    31194 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.dataset.html
+-rw-rw-rw-   0 root         (0) root         (0)    80364 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.feature_engineering.html
+-rw-rw-rw-   0 root         (0) root         (0)    40397 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.html
+-rw-rw-rw-   0 root         (0) root         (0)    34042 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.imputers.html
+-rw-rw-rw-   0 root         (0) root         (0)    56620 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.preprocessors.html
+-rw-rw-rw-   0 root         (0) root         (0)    80790 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.utilities.html
+-rw-rw-rw-   0 root         (0) root         (0)    33642 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/genindex.html
+-rw-rw-rw-   0 root         (0) root         (0)    18106 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/objects.inv
+-rw-rw-rw-   0 root         (0) root         (0)    12305 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/py-modindex.html
+-rw-rw-rw-   0 root         (0) root         (0)    10462 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/search.html
+-rw-rw-rw-   0 root         (0) root         (0)    17979 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/searchindex.js
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/make.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.563736 akerbp.mlpet-3.5.1/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.dataloader.rst
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.dataset.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.feature_engineering.rst
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.imputers.rst
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.preprocessors.rst
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.rst
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.utilities.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2199 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1950 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-15 12:49:52.591736 akerbp.mlpet-3.5.1/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.547735 akerbp.mlpet-3.5.1/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.547735 akerbp.mlpet-3.5.1/src/akerbp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.567736 akerbp.mlpet-3.5.1/src/akerbp/mlpet/
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.567736 akerbp.mlpet-3.5.1/src/akerbp/mlpet/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8846 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/data/mappings.py
+-rw-rw-rw-   0 root         (0) root         (0)    10241 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/data/npd_fm_gp_sy_key_dic.pcl
+-rw-rw-rw-   0 root         (0) root         (0)     4995 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/dataloader.py
+-rw-rw-rw-   0 root         (0) root         (0)    38374 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    29870 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/feature_engineering.py
+-rw-rw-rw-   0 root         (0) root         (0)    16008 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/imputers.py
+-rw-rw-rw-   0 root         (0) root         (0)    14307 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/petrophysical_features.py
+-rw-rw-rw-   0 root         (0) root         (0)    18016 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)    51691 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/plotting_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3981 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/plotting_variables.py
+-rw-rw-rw-   0 root         (0) root         (0)    37276 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/preprocessors.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.571735 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.591736 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)  5616970 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/15_9-23.las
+-rw-rw-rw-   0 root         (0) root         (0)  7480569 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/25_2-7.las
+-rw-rw-rw-   0 root         (0) root         (0)  4598499 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/35_12-1.las
+-rw-rw-rw-   0 root         (0) root         (0)    28130 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4140 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/test_mappings.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/test_settings.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_dataloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     5361 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     4239 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_feature_engineering.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_imputers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_petrophysical_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_preprocessors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1579 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4548 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     4160 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)    63414 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/utilities.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.567736 akerbp.mlpet-3.5.1/src/akerbp.mlpet.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    19183 2023-05-15 12:49:52.000000 akerbp.mlpet-3.5.1/src/akerbp.mlpet.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4486 2023-05-15 12:49:52.000000 akerbp.mlpet-3.5.1/src/akerbp.mlpet.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-15 12:49:52.000000 akerbp.mlpet-3.5.1/src/akerbp.mlpet.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-05-15 12:49:52.000000 akerbp.mlpet-3.5.1/src/akerbp.mlpet.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-15 12:49:52.000000 akerbp.mlpet-3.5.1/src/akerbp.mlpet.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/version.py
```

### Comparing `akerbp.mlpet-3.5.0/LICENSE` & `akerbp.mlpet-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/README.md` & `akerbp.mlpet-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/data/mappings.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/data/mappings.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/data/npd_fm_gp_sy_key_dic.pcl` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/data/npd_fm_gp_sy_key_dic.pcl`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/dataloader.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/dataloader.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/dataset.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import warnings
 from collections.abc import Iterable
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Set, Union
 
+import numpy as np
 import pandas as pd
 import yaml
 from pandas.core.frame import DataFrame
 from tqdm.auto import tqdm
 
 import akerbp.mlpet.data.mappings as default_mappings
 import akerbp.mlpet.dataloader as dl
@@ -78,14 +79,16 @@
 
     def __set_defaults(self) -> None:
         """
         Set necessary defaults for proper class use
         """
         if not hasattr(self, "num_filler"):
             self.num_filler = 0
+        elif self.num_filler is None:
+            self.num_filler = np.nan
 
         if not hasattr(self, "cat_filler"):
             self.cat_filler = "MISSING"
 
         if not hasattr(self, "keep_columns"):
             self.keep_columns = []
```

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/feature_engineering.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/feature_engineering.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 
     Args:
         df (pd.DataFrame): dataframe with columns to calculate log10 from
 
     Keyword Args:
         log_features (list, optional): list of column names for the columns that should be
             loggified. Defaults to None
-        num_filler (float, optional): value that represents a missing value in the
-            log_features. Defaults to None.
+        num_filler (float, optional): value to fill NaNs with. Defaults to None
 
     Returns:
         pd.DataFrame: New dataframe with calculated log columns
     """
     log_features: List[str] = kwargs.get("log_features", None)
     num_filler: float = kwargs.get("num_filler", None)
     if log_features is not None:
@@ -454,42 +453,58 @@
                 mappings["group_levels"],
             )
             formation_labels, formation_levels = (
                 mappings["formation_labels"],
                 mappings["formation_levels"],
             )
 
-            if (len(group_levels) != len(group_labels) + 1) or (
-                len(formation_levels) != len(formation_labels) + 1
-            ):
-                warnings.warn(
-                    f"The formation top information for {well} is invalid! "
-                    "Please refer to the docstring of this method to understand "
-                    "the format in which formation top mappings should be provided."
-                )
-                continue
+            # Handle groups
+            if group_labels and group_levels:
+                if len(group_levels) != len(group_labels) + 1:
+                    warnings.warn(
+                        f"The group tops information for {well} is invalid! "
+                        "Please refer to the docstring of this method to understand "
+                        "the format in which formation top mappings should be provided."
+                    )
+                    continue
+
+                well_df = df_[df_[id_column] == well]
+                df_.loc[well_df.index, "GROUP"] = pd.cut(
+                    well_df[depth_column],
+                    bins=group_levels,
+                    labels=group_labels,
+                    include_lowest=True,
+                    right=False,
+                    ordered=False,
+                ).astype("object")
+            else:
+                warnings.warn(f"No GROUP information found for {well}.")
+
+            # Handle formations
+            if formation_labels and formation_levels:
+                if len(formation_levels) != len(formation_labels) + 1:
+                    warnings.warn(
+                        f"The formation tops information for {well} is invalid! "
+                        "Please refer to the docstring of this method to understand "
+                        "the format in which formation top mappings should be provided."
+                    )
+                    continue
+
+                well_df = df_[df_[id_column] == well]
+                df_.loc[well_df.index, "FORMATION"] = pd.cut(
+                    well_df[depth_column],
+                    bins=formation_levels,
+                    labels=formation_labels,
+                    include_lowest=True,
+                    right=False,
+                    ordered=False,
+                ).astype("object")
+            else:
+                warnings.warn(f"No FORMATION information found for {well}.")
 
-            well_df = df_[df_[id_column] == well]
-            df_.loc[well_df.index, "GROUP"] = pd.cut(
-                well_df[depth_column],
-                bins=group_levels,
-                labels=group_labels,
-                include_lowest=True,
-                right=False,
-                ordered=False,
-            ).astype("object")
-
-            df_.loc[well_df.index, "FORMATION"] = pd.cut(
-                well_df[depth_column],
-                bins=formation_levels,
-                labels=formation_labels,
-                include_lowest=True,
-                right=False,
-                ordered=False,
-            ).astype("object")
         df_ = utilities.normalize_group_formation_system(df_, add_systems)
 
     else:
         raise ValueError(
             "A formation tops label could not be added to the provided dataframe"
             " because some keyword arguments were missing!"
         )
```

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/imputers.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/imputers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/petrophysical_features.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/petrophysical_features.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/plotting.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/plotting.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/plotting_helpers.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/plotting_helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/plotting_variables.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/plotting_variables.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/preprocessors.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/preprocessors.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/data/15_9-23.las` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/15_9-23.las`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/data/25_2-7.las` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/25_2-7.las`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/data/35_12-1.las` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/35_12-1.las`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/data/data.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1095,55 +1095,7 @@
             1142978: "25/10-10",
             1142979: "25/10-10",
             1142980: "25/10-10",
             1142981: "25/10-10",
         },
     }
 )
-
-DEPTH_TREND_X = pd.DataFrame(
-    {
-        "TVDBML": {
-            0: 1900.7523452000005,
-            1: 1900.90531154,
-            2: 1901.0572781,
-            3: 1901.20924466,
-            4: 1901.362211,
-        },
-        "GROUP": {
-            0: "SHETLAND",
-            1: "SHETLAND",
-            2: "SHETLAND",
-            3: "SHETLAND",
-            4: "SHETLAND",
-        },
-        "FORMATION": {
-            0: "SPRINGAR FM",
-            1: "BRYGGE",
-            2: "SPRINGAR FM",
-            3: "SPRINGAR FM",
-            4: "SPRINGAR FM",
-        },
-        "well": {
-            0: "6201_11-3_R",
-            1: "6201_11-3_R",
-            2: "6201_11-3_R",
-            3: "6201_11-3_R",
-            4: "6201_11-3_R",
-        },
-    }
-)
-
-DEPTH_TREND_Y = pd.DataFrame(
-    {
-        "DEN_trend": {0: 2.263, 1: 2.024, 2: 2.263, 3: 2.263, 4: 2.263},
-        "DEN_trend_P10": {0: 2.111, 1: 1.861, 2: 2.111, 3: 2.111, 4: 2.111},
-        "DEN_trend_P90": {0: 2.415, 1: 2.187, 2: 2.415, 3: 2.415, 4: 2.415},
-        "well": {
-            0: "6201_11-3_R",
-            1: "6201_11-3_R",
-            2: "6201_11-3_R",
-            3: "6201_11-3_R",
-            4: "6201_11-3_R",
-        },
-    }
-)
```

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/data/test_mappings.yaml` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/test_mappings.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/data/test_settings.yaml` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/test_settings.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_dataloader.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_dataloader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from akerbp.mlpet.dataloader import DataLoader
-from akerbp.mlpet.tests.client import CLIENT
+from akerbp.mlpet.tests.client import CLIENT_READ
 
 
 def test_load_from_cdf():
     dl = DataLoader()
     df = dl.load_from_cdf(
-        client=CLIENT, metadata={"wellbore_name": "25/2-7", "subtype": "BEST"}
+        client=CLIENT_READ, metadata={"wellbore_name": "25/2-7", "subtype": "BEST"}
     )
     assert df.shape[0] > 0
 
 
 def test_load_from_las():
     dl = DataLoader()
```

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_dataset.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_feature_engineering.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_feature_engineering.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pytest
 from pandas.testing import assert_frame_equal
 
 from akerbp.mlpet import feature_engineering
-from akerbp.mlpet.tests.client import CLIENT, CLIENT_FUNCTIONS
-from akerbp.mlpet.tests.data.data import DEPTH_TREND_X, DEPTH_TREND_Y
+from akerbp.mlpet.tests.client import CLIENT_READ, CLIENT_WRITE
 from akerbp.mlpet.tests.data.data import FORMATION_DF as FORMATION_DF_WITH_SYSTEMS
 from akerbp.mlpet.tests.data.data import (
     FORMATION_TOPS_MAPPER,
     TEST_DF,
     VERTICAL_DEPTHS_MAPPER,
     VERTICAL_DF,
 )
@@ -33,159 +32,100 @@
     assert_frame_equal(df_with_tops.sort_index(axis=1), FORMATION_DF.sort_index(axis=1))
 
 
 def test_add_formations_and_groups_using_client():
     df_with_tops = feature_engineering.add_formations_and_groups(
         FORMATION_DF[[DEPTH_COL, ID_COLUMN]],
         id_column=ID_COLUMN,
-        client=CLIENT,
+        client=CLIENT_READ,
     )
     assert_frame_equal(df_with_tops.sort_index(axis=1), FORMATION_DF.sort_index(axis=1))
 
 
 def test_add_formations_and_groups_using_client_with_systems():
     df_with_tops = feature_engineering.add_formations_and_groups(
         FORMATION_DF[[DEPTH_COL, ID_COLUMN]],
         id_column=ID_COLUMN,
-        client=CLIENT,
+        client=CLIENT_READ,
         add_systems=True,
     )
     assert_frame_equal(
         df_with_tops.sort_index(axis=1), FORMATION_DF_WITH_SYSTEMS.sort_index(axis=1)
     )
 
 
-def test_add_formations_and_groups_when_no_client_nor_mapping_is_provided():
-    _ = feature_engineering.add_formations_and_groups(
-        FORMATION_DF[[DEPTH_COL, ID_COLUMN]],
-        id_column=ID_COLUMN,
-    )
-
-
 def test_add_vertical_depths_using_mapper():
     df_with_vertical_depths = feature_engineering.add_vertical_depths(
         VERTICAL_DF[[DEPTH_COL, ID_COLUMN]],
-        vertical_depths_mapper=VERTICAL_DEPTHS_MAPPER,
+        trajectory_mapping=VERTICAL_DEPTHS_MAPPER,
         id_column=ID_COLUMN,
         md_column=DEPTH_COL,
     )
 
     assert_frame_equal(
         df_with_vertical_depths.sort_index(axis=1), VERTICAL_DF.sort_index(axis=1)
     )
 
 
 def test_add_vertical_depths_using_client():
     df_with_vertical_depths = feature_engineering.add_vertical_depths(
         VERTICAL_DF[[DEPTH_COL, ID_COLUMN]],
         id_column=ID_COLUMN,
         md_column=DEPTH_COL,
-        client=CLIENT,
-    )
-
-    assert_frame_equal(
-        df_with_vertical_depths.sort_index(axis=1),
-        VERTICAL_DF.sort_index(axis=1),
-    )
-
-
-def test_add_vertical_depths_when_no_client_nor_mapping_is_provided():
-    df_with_vertical_depths = feature_engineering.add_vertical_depths(
-        VERTICAL_DF[[DEPTH_COL, ID_COLUMN]],
-        id_column=ID_COLUMN,
-        md_column=DEPTH_COL,
+        client=CLIENT_READ,
     )
 
     assert_frame_equal(
         df_with_vertical_depths.sort_index(axis=1),
         VERTICAL_DF.sort_index(axis=1),
     )
 
 
-def test_add_wellbore_coordinates_no_client_nor_mapping_is_provided():
-    df_with_wellbore_coordinates = feature_engineering.add_wellbore_coordinates(
-        VERTICAL_DF[[DEPTH_COL, ID_COLUMN]],
-        id_column=ID_COLUMN,
-        md_column=DEPTH_COL,
-    )
-    coordinate_columns = ["X", "Y"]
-    assertions = [
-        col in df_with_wellbore_coordinates.columns for col in coordinate_columns
-    ]
-    assert len(assertions) == sum(assertions)
-
-
 def test_add_wellbore_coordinates_wrong_trajectory_type_override_with_default():
     df_with_wellbore_coordinates = feature_engineering.add_wellbore_coordinates(
         VERTICAL_DF[[DEPTH_COL, ID_COLUMN]],
         id_column=ID_COLUMN,
         md_column=DEPTH_COL,
         trajectory_type="wrong_trajectory_type",
+        client=CLIENT_READ,
     )
     coordinate_columns = ["X", "Y"]
     assertions = [
         col in df_with_wellbore_coordinates.columns for col in coordinate_columns
     ]
     assert len(assertions) == sum(assertions)
 
 
-def test_add_trajectory_data_no_client_nor_mapping_is_provided():
-    df_with_trajectory_data = feature_engineering.add_trajectory_data(
-        VERTICAL_DF[[DEPTH_COL, ID_COLUMN]],
-        id_column=ID_COLUMN,
-        md_column=DEPTH_COL,
-    )
-    trajectory_columns = ["X", "Y", "TVDBML", "TVDSS", "TVDKB"]
-    assertions = [col in df_with_trajectory_data.columns for col in trajectory_columns]
-    assert len(assertions) == sum(assertions)
-
-
 def test_add_trajectory_data_wrong_trajectory_type_raise_error():
     with pytest.raises(ValueError, match="Invalid trajectory_type provided!"):
         _ = feature_engineering.add_trajectory_data(
             VERTICAL_DF[[DEPTH_COL, ID_COLUMN]],
             id_column=ID_COLUMN,
             md_column=DEPTH_COL,
             trajectory_type="wrong_trajectory_type",
+            client=CLIENT_READ,
         )
 
 
 def test_add_well_metadata():
     metadata = {"30/11-6 S": {"FOO": 0}, "25/7-4 S": {"FOO": 1}}
     df = feature_engineering.add_well_metadata(
         TEST_DF,
         metadata_dict=metadata,
         metadata_columns=["FOO"],
         id_column=ID_COLUMN,
     )
     assert "FOO" in df.columns.tolist()
 
 
-def test_add_depth_trend():
-    result = feature_engineering.add_depth_trend(
-        DEPTH_TREND_X,
-        id_column="well",
-        env="prod",
-        return_file=False,
-        return_CI=True,
-        client=CLIENT_FUNCTIONS,
-        keyword_arguments=dict(
-            nan_numerical_value=-9999,
-            nan_textual_value="MISSING",
-        ),
-    )
-
-    assert DEPTH_TREND_Y.equals(result[DEPTH_TREND_Y.columns])
-
-
 def test_add_petrophysical_features_add_VSH_call_CDF_model_return_only_vsh_aut():
     df = TEST_DF.rename(columns={"DENC": "DEN"})
     petrophysical_features = ["VSH"]
     result = feature_engineering.add_petrophysical_features(
         df=df,
         id_column=ID_COLUMN,
         petrophysical_features=petrophysical_features,
         keyword_arguments=VSH_KWARGS,
-        client=CLIENT_FUNCTIONS,
+        client=CLIENT_WRITE,
     )
     output_curves = result.columns
     assert "VSH" in output_curves, "'VSH' not added to dataframe"
```

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_imputers.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_imputers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_petrophysical_features.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_petrophysical_features.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import pandas as pd
 
 from akerbp.mlpet import feature_engineering, petrophysical_features
 from akerbp.mlpet.dataloader import DataLoader
-from akerbp.mlpet.tests.client import CLIENT, CLIENT_FUNCTIONS
+from akerbp.mlpet.tests.client import CLIENT_READ, CLIENT_WRITE
 
 WELL = "15/3-5"
 ID_COLUMN = "well_name"
 VSH_KWARGS = {
     "nan_numerical_value": -9999,
     "nan_textual_value": "MISSING",
     "VSH_curves": ["GR"],
@@ -25,33 +25,33 @@
     df = petrophysical_features.calculate_CALI_BS(input)
     assert "CALI-BS" in df.columns.tolist()
 
 
 def test_calculate_VSH():
     dl = DataLoader()
     df = dl.load_from_cdf(
-        client=CLIENT, metadata={"wellbore_name": WELL, "subtype": "BEST"}
+        client=CLIENT_READ, metadata={"wellbore_name": WELL, "subtype": "BEST"}
     )
     df[ID_COLUMN] = WELL
     df = petrophysical_features.calculate_LFI(df)
     # BS is required but missing in this sequence to init to all nans
     df["BS"] = np.nan
     df = feature_engineering.add_formations_and_groups(
-        df, id_column=ID_COLUMN, depth_column="DEPTH"
+        df, id_column=ID_COLUMN, depth_column="DEPTH", client=CLIENT_READ
     )
     df = feature_engineering.add_vertical_depths(
-        df, id_column=ID_COLUMN, md_column="DEPTH"
+        df, id_column=ID_COLUMN, md_column="DEPTH", client=CLIENT_READ
     )
 
     df_out = petrophysical_features.calculate_VSH(
         df,
         id_column=ID_COLUMN,
         env="prod",
         return_CI=True,
-        client=CLIENT_FUNCTIONS,
+        client=CLIENT_WRITE,
         keyword_arguments=dict(
             calculate_denneu=True,
             VSH_curves=["GR", "LFI"],
             groups_column_name="GROUP",
             formations_column_name="FORMATION",
             return_only_vsh_aut=False,
             nan_numerical_value=-9999,
```

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_preprocessors.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_preprocessors.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_transformer.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/tests/test_utilities.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_utilities.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,79 +2,78 @@
 
 import pandas as pd
 import pytest
 import yaml
 from cognite.client.exceptions import CogniteAuthError
 
 from akerbp.mlpet import utilities as utils
+from akerbp.mlpet.tests.client import CLIENT_WRITE as CLIENT_READ
 from akerbp.mlpet.tests.data.data import (
     FORMATION_TOPS_MAPPER,
     TEST_DF,
     VERTICAL_DEPTHS_MAPPER,
 )
-from akerbp.mlpet.utilities import get_cognite_client
 
 ID_COLUMNS = "well_name"
 VSH_KWARGS = {
     "nan_numerical_value": -9999,
     "nan_textual_value": "MISSING",
     "VSH_curves": ["GR"],
 }
 
 
-CLIENT = get_cognite_client(permission_scope="read")
 WELL_NAMES = ["25/10-10"]
 
 
 def test_get_formation_tops():
-    formation_tops_mapper = utils.get_formation_tops(WELL_NAMES, CLIENT)
+    formation_tops_mapper = utils.get_formation_tops(WELL_NAMES, CLIENT_READ)
     assert formation_tops_mapper == FORMATION_TOPS_MAPPER
 
 
 def test_get_vertical_depths():
-    retrieved_vertical_depths = utils.get_vertical_depths(WELL_NAMES, CLIENT)
+    retrieved_vertical_depths = utils.get_vertical_depths(WELL_NAMES, CLIENT_READ)
     # empty_queries should be an empty list for the provided WELL_NAMES
     assert retrieved_vertical_depths == VERTICAL_DEPTHS_MAPPER
 
 
 def test_get_trajectory_mapper_from_cdf_returns_all_fields():
     fields = ["MD", "TVDBML", "TVDSS", "TVDKB", "X", "Y"]
-    trajectory_mapper = utils.get_trajectory_mapper_from_cdf(WELL_NAMES, CLIENT)
+    trajectory_mapper = utils.get_trajectory_mapper_from_cdf(WELL_NAMES, CLIENT_READ)
     fields_in_mapper = trajectory_mapper[WELL_NAMES[0]].keys()
     assertions = [field in fields_in_mapper for field in fields]
     assertions_ = [field in fields for field in fields_in_mapper]
     assert sum(assertions) == len(assertions) and sum(assertions_) == len(assertions_)
 
 
 def test_get_vertical_depths_returns_no_coordinates():
-    vertical_depths_mapper = utils.get_vertical_depths(WELL_NAMES, CLIENT)
+    vertical_depths_mapper = utils.get_vertical_depths(WELL_NAMES, CLIENT_READ)
     fields = vertical_depths_mapper[WELL_NAMES[0]].keys()
     coordinate_fields = ["X", "Y"]
     assertions = [coordinate not in fields for coordinate in coordinate_fields]
     assert sum(assertions) == len(assertions)
 
 
 def test_get_vertical_depths_returns_vertical_depths():
-    vertical_depths_mapper = utils.get_vertical_depths(WELL_NAMES, CLIENT)
+    vertical_depths_mapper = utils.get_vertical_depths(WELL_NAMES, CLIENT_READ)
     fields = vertical_depths_mapper[WELL_NAMES[0]].keys()
     depth_fields = ["TVDBML", "TVDSS", "TVDKB"]
     assertions = [depth in fields for depth in depth_fields]
     assert sum(assertions) == len(assertions)
 
 
 def test_get_wellbore_coordinates_returns_coordinates():
-    coordinates_mapper = utils.get_wellbore_coordinates(WELL_NAMES, CLIENT)
+    coordinates_mapper = utils.get_wellbore_coordinates(WELL_NAMES, CLIENT_READ)
     fields = coordinates_mapper[WELL_NAMES[0]].keys()
     coordinate_fields = ["X", "Y"]
     assertions = [coordinate in fields for coordinate in coordinate_fields]
     assert sum(assertions) == len(assertions)
 
 
 def test_get_wellbore_coordinates_returns_no_vertical_depths():
-    coordinates_mapper = utils.get_wellbore_coordinates(WELL_NAMES, CLIENT)
+    coordinates_mapper = utils.get_wellbore_coordinates(WELL_NAMES, CLIENT_READ)
     fields = coordinates_mapper[WELL_NAMES[0]].keys()
     vertical_depths = ["TVDBML", "TVDSS", "TVDKB"]
     assertions = [depth not in fields for depth in vertical_depths]
     assert sum(assertions) == len(assertions)
 
 
 def test_remove_wo_label():
@@ -101,34 +100,27 @@
         ("UNKNOWN FM", -9999, "UNKNOWN FM", -9999),
         ("UNKNOWN GP", -9999, "UNKNOWN GP", "HEGRE GP"),
         (-9999, -9999, -9999, "TRIASSIC SY"),
     )
 
 
 def test_get_well_metadata():
-    metadata = utils.get_well_metadata(client=CLIENT, well_names=WELL_NAMES)
+    metadata = utils.get_well_metadata(client=CLIENT_READ, well_names=WELL_NAMES)
     assert metadata[WELL_NAMES[0]]["CDF_wellName"] == WELL_NAMES[0]
 
 
-def test_get_cognite_client_no_args_returns_logged_in_client():
-    client = utils.get_cognite_client()
-    logged_in = client.login.status().logged_in
-    assert logged_in
-
-
-def test_get_cognite_client_pass_api_key_returns_logged_in_client():
+def test_get_cognite_client_is_logged_in():
     client_id = os.environ["COGNITE_CLIENT_ID_READ"]
     client_secret = os.environ["COGNITE_CLIENT_SECRET_READ"]
 
     client = utils.get_cognite_client(
         client_id=client_id,
         client_secret=client_secret,
     )
-    logged_in = client.login.status().logged_in
-    assert logged_in
+    assert client.iam.token.inspect() is not None
 
 
 def test_get_cognite_client_wrong_credentials_raise_exception():
     wrong_id = "wrong_id_go_home"
     wrong_secret = "wrong_secret_go_home"
     client = utils.get_cognite_client(client_id=wrong_id, client_secret=wrong_secret)
     with pytest.raises(CogniteAuthError):
```

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/transformer.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/transformer.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.0/src/akerbp/mlpet/utilities.py` & `akerbp.mlpet-3.5.1/src/akerbp/mlpet/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+import base64
 import importlib.resources
 import json
 import os
 import re
 import warnings
 from functools import lru_cache
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 from cognite.client import ClientConfig, CogniteClient
 from cognite.client.credentials import OAuthClientCredentials
 from cognite.client.data_classes import Asset, AssetList
+from cryptography.hazmat.primitives import hashes, padding, serialization
+from cryptography.hazmat.primitives.asymmetric import padding as asym_padding
+from cryptography.hazmat.primitives.asymmetric import rsa
+from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from numpy import float64
 from scipy.interpolate import interp1d
 
 import akerbp.mlpet.data
 import akerbp.mlpet.preprocessors as preprocessors
 
 
@@ -453,15 +458,14 @@
     y = df[target_column]
     return X, y
 
 
 def normalize(
     col: pd.Series, ref_min: float64, ref_max: float64, col_min: float, col_max: float
 ) -> pd.Series:
-
     """
     Helper function that applies min-max normalization on a pandas series and
     rescales it according to a reference range according to the following formula:
 
         ref_low + ((col - col_min) * (ref_max - ref_min) / (col_max - col_min))
 
     Args:
@@ -589,33 +593,39 @@
         "DATUM_ELEVATION_UNIT": [
             "DATUM_ELEVATION_DSDS_UNIT",
             "datum-unit",
         ],
         "LATITUDE": [
             "Latitude",
             "SURFACE_NODE_LATITUDE",
-            "y",
         ],
         "LONGITUDE": [
             "Longitude",
             "SURFACE_NODE_LONGITUDE",
-            "x",
         ],
     }
 
     # Helper function to find best match from fuzzy search results
-    def _find_best_match(assetlist: AssetList, wellName: str) -> str:
+    def _find_best_match(
+        assetlist: AssetList, wellName: str
+    ) -> Tuple[str, Optional[Asset]]:
         # Compares only the alphanumerics of the wellName (ie. punctuation removed)
         # If no match is found it returns an empty string
-        pat = re.compile(r"[^a-zA-Z0-9\-]+")
+        pat = re.compile(r"[^a-zA-Z0-9]+")
+
+        def _stripper(s: str, split: str) -> str:
+            return pat.sub("", s).rsplit(split)[0].strip()
+
         for asset in assetlist:
             name: str = asset.name
-            if pat.sub("", name) == pat.sub("", wellName):
-                return name
-        return ""
+            if _stripper(name, "T") == _stripper(wellName, "T"):
+                return name, asset
+            elif _stripper(name, "R") == _stripper(wellName, "R"):
+                return name, asset
+        return "", None
 
     # Helper function to retrieve asset with most relevant metadata in the case
     # of multiple matches
     def _merge_assets(assetlist: List[Asset]) -> pd.Series:
         metadata = {}
         for asset in assetlist:
             metadata.update(asset.to_pandas().squeeze().to_dict())
@@ -624,32 +634,47 @@
         return merged
 
     # First retrieve metadata from the Cognite asset API
     meta = []
     for well in well_names:
         try:
             # First try list search
-            assets: Union[AssetList, List[Asset]] = client.assets.list(name=well)
+            assets: Union[AssetList, List[Asset]] = client.assets.list(
+                name=well,
+                metadata={"type": "Wellbore"},
+            )
             if len(assets) == 0:
-                # If first attempt failed use fuzzy search to retrieve proper
-                # well name. Find best match based on alphanumeric equality
-                wellName = _find_best_match(
-                    client.assets.search(name=well, limit=10), well
+                # If first attempt failed try a list search again but assuming
+                # the well name was specified in techlog form
+                tl_well_name = well.replace("_", "/", 1).replace("_", " ")
+                assets = client.assets.list(
+                    name=tl_well_name,
+                    metadata={"type": "Wellbore"},
                 )
-                if not wellName:
-                    raise IndexError
+                if len(assets) == 0:
+                    # If second attempt fails use fuzzy search to retrieve proper
+                    # well name. Find best match based on alphanumeric equality
+                    wellName, asset = _find_best_match(
+                        client.assets.search(
+                            name=well,
+                            filter={"metadata": {"type": "Wellbore"}},
+                            limit=10,
+                        ),
+                        well,
+                    )
+                    if not wellName:
+                        raise IndexError
+                    assets = [asset]
+                else:
+                    wellName = tl_well_name
                 warnings.warn(
                     f"Could not find a direct match for '{well}' in the CDF Assets"
                     f" database. Closest match found is '{wellName}'. Using the "
                     "metadata from that asset!"
                 )
-                # Then retrieve asset using list API
-                assets = client.assets.list(
-                    name=wellName, metadata={"type": "Wellbore"}
-                )
             if len(assets) > 1:
                 # Sort by time with first element being most recent
                 assets = sorted(assets, key=lambda x: x.last_updated_time)
                 # Some wells are stored several times as assets??
                 # In this case merge them all together to retrieve as much
                 # metadata as possible.
                 series_meta = _merge_assets(assets)
@@ -1427,15 +1452,15 @@
     Helper function to create a CogniteClient instance.
 
     Args:
         client_id (str): Client id to authenticate the client with
         client_secret (str): Client secret to authenticate the client with
         cognite_project_id (str): The project ID to use for the CogniteClient, Defaults to akbp-subsurface
         cognite_client_id (str): The client ID to use for the CogniteClient
-        persmission_scope (str): The permission scope to use for the CogniteClient, either "read" or "write", deafult to "read"
+        persmission_scope (str): The permission scope to use for the CogniteClient, either "read" or "write", default to "read" (only relevant if using akerbp.mlops)
 
         Returns:
             CogniteClient: The created CogniteClient instance
     """
     permission = permission_scope.lower()
     if permission not in ["read", "write"]:
         raise ValueError(
@@ -1461,15 +1486,15 @@
         if client_id is None or client_secret is None:
             from akerbp.mlops.core.config import client_secrets as secrets
 
             client_id = secrets[f"id-{permission}"]
             client_secret = secrets[f"secret-{permission}"]
         else:
             pass
-    except KeyError as e:
+    except ModuleNotFoundError as e:
         raise Exception(
             f"Need to set client id and secret for permission scope {permission_scope} as environment variables to initialize a client"
         ) from e
 
     credentials = OAuthClientCredentials(
         token_url=f"https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token",
         client_id=client_id,
@@ -1573,23 +1598,52 @@
         client = get_cognite_client(permission_scope="write")
     function = client.functions.retrieve(external_id=cdf_external_id)
     if function is None:
         raise ValueError(
             f"No function with external ID {cdf_external_id} found in Cognite!"
         )
     in_data["return_file"] = return_file
+    # Create an RSA key pair to encrypt the results in the function
+    private_key = rsa.generate_private_key(
+        public_exponent=65537,
+        key_size=2048,
+    )
+    public_key = private_key.public_key()
+    pem = public_key.public_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PublicFormat.SubjectPublicKeyInfo,
+    )
+    in_data["public_key"] = pem.decode()
 
     results = function.call(in_data).get_response()
     if results["status"] == "error":
         keys = [k for k in list(results) if "message" in k.lower()]
         if keys:
             raise ValueError(f"Function returned an error: {results[keys[0]]}")
         else:
             raise ValueError(f"Function returned an error: {results}")
     if return_file:
-        predictions = json.loads(
-            client.files.download_bytes(external_id=results["prediction_file"])
-        )
+        ciphertext = client.files.download_bytes(external_id=results["prediction_file"])
+        encrypted = results.get("data_encrypted", False)
+        if encrypted:
+            print("Decrypting predictions received from Cognite!")
+            encrypted_key = base64.b64decode(results["encrypted_key"].encode())
+            key = private_key.decrypt(
+                encrypted_key,
+                asym_padding.OAEP(
+                    mgf=asym_padding.MGF1(algorithm=hashes.SHA256()),
+                    algorithm=hashes.SHA256(),
+                    label=None,
+                ),
+            )
+            algo = algorithms.AES(key)
+            decryptor = Cipher(algo, modes.CBC(b"1234567890123456")).decryptor()
+            padded_data = decryptor.update(ciphertext) + decryptor.finalize()
+            unpadder = padding.PKCS7(algo.block_size).unpadder()
+            content = unpadder.update(padded_data) + unpadder.finalize()
+        else:
+            content = ciphertext
+        predictions = json.loads(content)
     else:
         predictions = results["prediction"]
 
     return predictions
```

