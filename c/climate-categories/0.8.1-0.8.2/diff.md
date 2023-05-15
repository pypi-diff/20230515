# Comparing `tmp/climate_categories-0.8.1.tar.gz` & `tmp/climate_categories-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climate_categories-0.8.1.tar", last modified: Wed Apr 26 14:03:08 2023, max compression
+gzip compressed data, was "climate_categories-0.8.2.tar", last modified: Mon May 15 16:33:58 2023, max compression
```

## Comparing `climate_categories-0.8.1.tar` & `climate_categories-0.8.2.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.315656 climate_categories-0.8.1/
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.307656 climate_categories-0.8.1/.github/
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.307656 climate_categories-0.8.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      671 2023-04-26 09:04:13.000000 climate_categories-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      548 2023-04-26 09:04:13.000000 climate_categories-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      571 2023-04-26 09:04:13.000000 climate_categories-0.8.1/.github/ISSUE_TEMPLATE/new_categorization.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      369 2023-04-26 13:19:45.000000 climate_categories-0.8.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.307656 climate_categories-0.8.1/.github/workflows/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      963 2023-04-26 11:23:54.000000 climate_categories-0.8.1/.github/workflows/ci.yml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1331 2023-04-26 11:23:54.000000 climate_categories-0.8.1/.gitignore
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1253 2023-04-26 12:34:31.000000 climate_categories-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      297 2023-04-26 13:26:25.000000 climate_categories-0.8.1/.readthedocs.yml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       38 2023-04-26 09:04:13.000000 climate_categories-0.8.1/.sourcery.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      210 2023-04-26 09:04:13.000000 climate_categories-0.8.1/AUTHORS.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4575 2023-04-26 14:01:13.000000 climate_categories-0.8.1/CHANGELOG.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5446 2023-04-26 11:23:54.000000 climate_categories-0.8.1/CONTRIBUTING.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      651 2023-04-26 09:04:13.000000 climate_categories-0.8.1/LICENSE
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3235 2023-04-26 12:32:41.000000 climate_categories-0.8.1/Makefile
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8931 2023-04-26 14:03:08.315656 climate_categories-0.8.1/PKG-INFO
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3344 2023-04-26 14:02:09.000000 climate_categories-0.8.1/README.rst
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.307656 climate_categories-0.8.1/climate_categories/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1943 2023-04-26 14:01:00.000000 climate_categories-0.8.1/climate_categories/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    41200 2023-04-26 12:37:35.000000 climate_categories-0.8.1/climate_categories/_categories.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    47235 2023-04-26 12:57:44.000000 climate_categories-0.8.1/climate_categories/_conversions.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.311656 climate_categories-0.8.1/climate_categories/data/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    48820 2023-04-26 13:51:54.000000 climate_categories-0.8.1/climate_categories/data/BURDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    39603 2023-04-26 13:51:50.000000 climate_categories-0.8.1/climate_categories/data/BURDI.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    91320 2023-04-26 13:52:03.000000 climate_categories-0.8.1/climate_categories/data/BURDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    64321 2023-04-26 13:51:56.000000 climate_categories-0.8.1/climate_categories/data/BURDI_class.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    84030 2023-04-26 13:49:12.000000 climate_categories-0.8.1/climate_categories/data/CRF1999.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    69834 2023-04-26 13:49:07.000000 climate_categories-0.8.1/climate_categories/data/CRF1999.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172563 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   136709 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   213803 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013_2021.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165299 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013_2021.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   214940 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013_2022.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165976 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013_2022.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   215236 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013_2023.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   166217 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013_2023.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    85443 2023-04-26 13:51:04.000000 climate_categories-0.8.1/climate_categories/data/CRFDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    68686 2023-04-26 13:50:55.000000 climate_categories-0.8.1/climate_categories/data/CRFDI.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   252079 2023-04-26 13:51:45.000000 climate_categories-0.8.1/climate_categories/data/CRFDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172924 2023-04-26 13:51:08.000000 climate_categories-0.8.1/climate_categories/data/CRFDI_class.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2039 2023-04-26 13:48:45.000000 climate_categories-0.8.1/climate_categories/data/GCB.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1795 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/data/GCB.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    60150 2023-04-26 13:49:07.000000 climate_categories-0.8.1/climate_categories/data/IPCC1996.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    51928 2023-04-26 13:49:05.000000 climate_categories-0.8.1/climate_categories/data/IPCC1996.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   146256 2023-04-26 13:48:54.000000 climate_categories-0.8.1/climate_categories/data/IPCC2006.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   126862 2023-04-26 13:48:48.000000 climate_categories-0.8.1/climate_categories/data/IPCC2006.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   149225 2023-04-26 13:49:01.000000 climate_categories-0.8.1/climate_categories/data/IPCC2006_PRIMAP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   128959 2023-04-26 13:48:55.000000 climate_categories-0.8.1/climate_categories/data/IPCC2006_PRIMAP.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    24803 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/RCMIP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18549 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/RCMIP.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/data/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3761 2023-04-26 09:06:11.000000 climate_categories-0.8.1/climate_categories/data/conversion.IPCC1996.IPCC2006.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32498 2023-04-26 13:50:50.000000 climate_categories-0.8.1/climate_categories/data/gas.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    23635 2023-04-26 13:50:49.000000 climate_categories-0.8.1/climate_categories/data/gas.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      304 2023-04-26 11:23:54.000000 climate_categories-0.8.1/climate_categories/search.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.311656 climate_categories-0.8.1/climate_categories/tests/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       48 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3795 2023-04-26 11:23:55.000000 climate_categories-0.8.1/climate_categories/tests/conftest.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.311656 climate_categories-0.8.1/climate_categories/tests/data/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 10:17:34.000000 climate_categories-0.8.1/climate_categories/tests/data/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.8.1/climate_categories/tests/data/broken_conversion_not_allowed.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.8.1/climate_categories/tests/data/broken_conversion_not_existing.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/broken_hierarchical_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      705 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/broken_simple_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.8.1/climate_categories/tests/data/good_conversion.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      650 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/good_conversion_A.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      341 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/good_conversion_B.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      372 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/good_conversion_aux1.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      349 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/good_conversion_aux2.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.8.1/climate_categories/tests/data/good_conversion_reversed.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/hierarchical_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      702 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/simple_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1665 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/examples.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21242 2023-04-26 12:40:48.000000 climate_categories-0.8.1/climate_categories/tests/test_climate_categories.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14271 2023-04-26 11:23:55.000000 climate_categories-0.8.1/climate_categories/tests/test_conversions.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1205 2023-04-26 11:23:54.000000 climate_categories-0.8.1/climate_categories/tests/test_crf.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      769 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/test_di.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      508 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/test_gas.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1296 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/test_ipcc.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     7703 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/test_overcounting.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      596 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/test_primap.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      305 2023-04-26 09:06:11.000000 climate_categories-0.8.1/climate_categories/tests/test_rcmip.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      649 2023-04-26 11:23:54.000000 climate_categories-0.8.1/climate_categories/tests/test_search.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.307656 climate_categories-0.8.1/climate_categories.egg-info/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8931 2023-04-26 14:03:08.000000 climate_categories-0.8.1/climate_categories.egg-info/PKG-INFO
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4001 2023-04-26 14:03:08.000000 climate_categories-0.8.1/climate_categories.egg-info/SOURCES.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-04-26 14:03:08.000000 climate_categories-0.8.1/climate_categories.egg-info/dependency_links.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      326 2023-04-26 14:03:08.000000 climate_categories-0.8.1/climate_categories.egg-info/requires.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       19 2023-04-26 14:03:08.000000 climate_categories-0.8.1/climate_categories.egg-info/top_level.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      130 2023-04-26 09:04:13.000000 climate_categories-0.8.1/codecov.yml
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.315656 climate_categories-0.8.1/data_generation/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       62 2023-04-26 09:06:11.000000 climate_categories-0.8.1/data_generation/.gitignore
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5819 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/BURDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3177 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/BURDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    17598 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/CRF1999.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    65761 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/CRF2013.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    30906 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/CRF2013_2021.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    31721 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/CRF2013_2022.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32225 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/CRF2013_2023.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5318 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/CRFDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/CRFDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11562 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/IPCC1996.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8947 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/IPCC2006.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4254 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/IPCC2006_PRIMAP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8134 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/RCMIP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      272 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/convert_yaml_to_python.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3318 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/gas.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1082 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/utils.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.315656 climate_categories-0.8.1/docs/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      631 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/Makefile
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      241 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/api.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/changelog.rst
--rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5230 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/conf.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       33 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/contributing.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      337 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/credits.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8178 2023-04-26 09:06:11.000000 climate_categories-0.8.1/docs/data.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      325 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/index.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1209 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/installation.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      780 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/make.bat
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/readme.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       40 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/requirements.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18334 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/usage.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      328 2023-04-26 12:59:50.000000 climate_categories-0.8.1/pyproject.toml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-04-26 09:04:13.000000 climate_categories-0.8.1/requirements.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-04-26 09:04:13.000000 climate_categories-0.8.1/requirements_dev.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1662 2023-04-26 14:03:08.315656 climate_categories-0.8.1/setup.cfg
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-04-26 09:08:24.000000 climate_categories-0.8.1/setup.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1381 2023-04-26 14:01:00.000000 climate_categories-0.8.1/tbump.toml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      379 2023-04-26 11:23:54.000000 climate_categories-0.8.1/tox.ini
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      773 2023-04-26 09:04:13.000000 climate_categories-0.8.1/update_changelog.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1181 2023-04-26 11:23:54.000000 climate_categories-0.8.1/update_citation_info.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-15 16:33:58.713663 climate_categories-0.8.2/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-15 16:33:58.709663 climate_categories-0.8.2/.github/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-15 16:33:58.709663 climate_categories-0.8.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      671 2023-04-26 09:04:13.000000 climate_categories-0.8.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      548 2023-04-26 09:04:13.000000 climate_categories-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      571 2023-04-26 09:04:13.000000 climate_categories-0.8.2/.github/ISSUE_TEMPLATE/new_categorization.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      369 2023-04-26 13:19:45.000000 climate_categories-0.8.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-15 16:33:58.709663 climate_categories-0.8.2/.github/workflows/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      963 2023-04-26 11:23:54.000000 climate_categories-0.8.2/.github/workflows/ci.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1331 2023-04-26 11:23:54.000000 climate_categories-0.8.2/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1253 2023-05-10 10:03:13.000000 climate_categories-0.8.2/.pre-commit-config.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      297 2023-04-26 13:26:25.000000 climate_categories-0.8.2/.readthedocs.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       38 2023-04-26 09:04:13.000000 climate_categories-0.8.2/.sourcery.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      216 2023-04-26 14:19:11.000000 climate_categories-0.8.2/AUTHORS.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4792 2023-05-15 16:29:54.000000 climate_categories-0.8.2/CHANGELOG.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5446 2023-04-26 11:23:54.000000 climate_categories-0.8.2/CONTRIBUTING.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      696 2023-04-26 14:19:11.000000 climate_categories-0.8.2/LICENSE
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3267 2023-05-15 16:33:50.000000 climate_categories-0.8.2/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9195 2023-05-15 16:33:58.717663 climate_categories-0.8.2/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3386 2023-05-15 16:32:42.000000 climate_categories-0.8.2/README.rst
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-15 16:33:58.709663 climate_categories-0.8.2/climate_categories/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1949 2023-05-15 16:29:43.000000 climate_categories-0.8.2/climate_categories/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    43152 2023-05-15 16:28:37.000000 climate_categories-0.8.2/climate_categories/_categories.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    47235 2023-04-26 12:57:44.000000 climate_categories-0.8.2/climate_categories/_conversions.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-15 16:33:58.713663 climate_categories-0.8.2/climate_categories/data/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    48820 2023-04-26 13:51:54.000000 climate_categories-0.8.2/climate_categories/data/BURDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    39603 2023-04-26 13:51:50.000000 climate_categories-0.8.2/climate_categories/data/BURDI.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    91320 2023-04-26 13:52:03.000000 climate_categories-0.8.2/climate_categories/data/BURDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    64321 2023-04-26 13:51:56.000000 climate_categories-0.8.2/climate_categories/data/BURDI_class.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    84030 2023-04-26 13:49:12.000000 climate_categories-0.8.2/climate_categories/data/CRF1999.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    69834 2023-04-26 13:49:07.000000 climate_categories-0.8.2/climate_categories/data/CRF1999.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172563 2023-04-26 13:59:42.000000 climate_categories-0.8.2/climate_categories/data/CRF2013.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   136709 2023-04-26 13:59:42.000000 climate_categories-0.8.2/climate_categories/data/CRF2013.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   213803 2023-04-26 13:59:42.000000 climate_categories-0.8.2/climate_categories/data/CRF2013_2021.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165299 2023-04-26 13:59:42.000000 climate_categories-0.8.2/climate_categories/data/CRF2013_2021.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   214940 2023-04-26 13:59:42.000000 climate_categories-0.8.2/climate_categories/data/CRF2013_2022.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165976 2023-04-26 13:59:42.000000 climate_categories-0.8.2/climate_categories/data/CRF2013_2022.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   215236 2023-04-26 13:59:42.000000 climate_categories-0.8.2/climate_categories/data/CRF2013_2023.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   166217 2023-04-26 13:59:42.000000 climate_categories-0.8.2/climate_categories/data/CRF2013_2023.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    85443 2023-04-26 13:51:04.000000 climate_categories-0.8.2/climate_categories/data/CRFDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    68686 2023-04-26 13:50:55.000000 climate_categories-0.8.2/climate_categories/data/CRFDI.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   252079 2023-04-26 13:51:45.000000 climate_categories-0.8.2/climate_categories/data/CRFDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172924 2023-04-26 13:51:08.000000 climate_categories-0.8.2/climate_categories/data/CRFDI_class.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2039 2023-04-26 13:48:45.000000 climate_categories-0.8.2/climate_categories/data/GCB.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1795 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/data/GCB.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    60150 2023-04-26 13:49:07.000000 climate_categories-0.8.2/climate_categories/data/IPCC1996.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    51928 2023-04-26 13:49:05.000000 climate_categories-0.8.2/climate_categories/data/IPCC1996.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   146256 2023-04-26 13:48:54.000000 climate_categories-0.8.2/climate_categories/data/IPCC2006.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   126862 2023-04-26 13:48:48.000000 climate_categories-0.8.2/climate_categories/data/IPCC2006.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   149225 2023-04-26 13:49:01.000000 climate_categories-0.8.2/climate_categories/data/IPCC2006_PRIMAP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   128959 2023-04-26 13:48:55.000000 climate_categories-0.8.2/climate_categories/data/IPCC2006_PRIMAP.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    24803 2023-04-26 13:59:42.000000 climate_categories-0.8.2/climate_categories/data/RCMIP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18549 2023-04-26 13:59:42.000000 climate_categories-0.8.2/climate_categories/data/RCMIP.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/data/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3761 2023-04-26 09:06:11.000000 climate_categories-0.8.2/climate_categories/data/conversion.IPCC1996.IPCC2006.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32498 2023-04-26 13:50:50.000000 climate_categories-0.8.2/climate_categories/data/gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    23635 2023-04-26 13:50:49.000000 climate_categories-0.8.2/climate_categories/data/gas.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      304 2023-04-26 11:23:54.000000 climate_categories-0.8.2/climate_categories/search.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-15 16:33:58.713663 climate_categories-0.8.2/climate_categories/tests/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       48 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3795 2023-04-26 11:23:55.000000 climate_categories-0.8.2/climate_categories/tests/conftest.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-15 16:33:58.713663 climate_categories-0.8.2/climate_categories/tests/data/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 10:17:34.000000 climate_categories-0.8.2/climate_categories/tests/data/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.8.2/climate_categories/tests/data/broken_conversion_not_allowed.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.8.2/climate_categories/tests/data/broken_conversion_not_existing.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/data/broken_hierarchical_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      705 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/data/broken_simple_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.8.2/climate_categories/tests/data/good_conversion.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      650 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/data/good_conversion_A.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      341 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/data/good_conversion_B.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      372 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/data/good_conversion_aux1.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      349 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/data/good_conversion_aux2.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.8.2/climate_categories/tests/data/good_conversion_reversed.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/data/hierarchical_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      702 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/data/simple_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1665 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/examples.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21970 2023-05-15 16:28:37.000000 climate_categories-0.8.2/climate_categories/tests/test_climate_categories.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14271 2023-04-26 11:23:55.000000 climate_categories-0.8.2/climate_categories/tests/test_conversions.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1205 2023-04-26 11:23:54.000000 climate_categories-0.8.2/climate_categories/tests/test_crf.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      769 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/test_di.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      508 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/test_gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1296 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/test_ipcc.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     7703 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/test_overcounting.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      596 2023-04-26 09:04:13.000000 climate_categories-0.8.2/climate_categories/tests/test_primap.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      305 2023-04-26 09:06:11.000000 climate_categories-0.8.2/climate_categories/tests/test_rcmip.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      649 2023-04-26 11:23:54.000000 climate_categories-0.8.2/climate_categories/tests/test_search.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-15 16:33:58.709663 climate_categories-0.8.2/climate_categories.egg-info/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9195 2023-05-15 16:33:58.000000 climate_categories-0.8.2/climate_categories.egg-info/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4001 2023-05-15 16:33:58.000000 climate_categories-0.8.2/climate_categories.egg-info/SOURCES.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-05-15 16:33:58.000000 climate_categories-0.8.2/climate_categories.egg-info/dependency_links.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      307 2023-05-15 16:33:58.000000 climate_categories-0.8.2/climate_categories.egg-info/requires.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       19 2023-05-15 16:33:58.000000 climate_categories-0.8.2/climate_categories.egg-info/top_level.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      130 2023-04-26 09:04:13.000000 climate_categories-0.8.2/codecov.yml
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-15 16:33:58.713663 climate_categories-0.8.2/data_generation/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       62 2023-04-26 09:06:11.000000 climate_categories-0.8.2/data_generation/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5819 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/BURDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3177 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/BURDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    17598 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/CRF1999.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    65761 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/CRF2013.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    30906 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/CRF2013_2021.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    31721 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/CRF2013_2022.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32225 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/CRF2013_2023.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5318 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/CRFDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/CRFDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11562 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/IPCC1996.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8947 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/IPCC2006.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4254 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/IPCC2006_PRIMAP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8134 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/RCMIP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      272 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/convert_yaml_to_python.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3318 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1082 2023-04-26 13:44:45.000000 climate_categories-0.8.2/data_generation/utils.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-15 16:33:58.713663 climate_categories-0.8.2/docs/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      631 2023-04-26 09:04:13.000000 climate_categories-0.8.2/docs/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      241 2023-04-26 09:04:13.000000 climate_categories-0.8.2/docs/api.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-04-26 09:04:13.000000 climate_categories-0.8.2/docs/changelog.rst
+-rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-05-10 09:47:08.000000 climate_categories-0.8.2/docs/conf.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       33 2023-04-26 09:04:13.000000 climate_categories-0.8.2/docs/contributing.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      337 2023-04-26 09:04:13.000000 climate_categories-0.8.2/docs/credits.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8179 2023-05-10 10:01:49.000000 climate_categories-0.8.2/docs/data.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      325 2023-04-26 09:04:13.000000 climate_categories-0.8.2/docs/index.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1209 2023-04-26 09:04:13.000000 climate_categories-0.8.2/docs/installation.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      780 2023-04-26 09:04:13.000000 climate_categories-0.8.2/docs/make.bat
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-04-26 09:04:13.000000 climate_categories-0.8.2/docs/readme.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       21 2023-05-10 09:48:15.000000 climate_categories-0.8.2/docs/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18889 2023-05-15 16:28:37.000000 climate_categories-0.8.2/docs/usage.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      328 2023-04-26 12:59:50.000000 climate_categories-0.8.2/pyproject.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-04-26 09:04:13.000000 climate_categories-0.8.2/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-04-26 09:04:13.000000 climate_categories-0.8.2/requirements_dev.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1647 2023-05-15 16:33:58.717663 climate_categories-0.8.2/setup.cfg
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-04-26 09:08:24.000000 climate_categories-0.8.2/setup.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1381 2023-05-15 16:29:43.000000 climate_categories-0.8.2/tbump.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      379 2023-04-26 11:23:54.000000 climate_categories-0.8.2/tox.ini
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      773 2023-04-26 09:04:13.000000 climate_categories-0.8.2/update_changelog.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1181 2023-04-26 11:23:54.000000 climate_categories-0.8.2/update_citation_info.py
```

### Comparing `climate_categories-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md` & `climate_categories-0.8.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md` & `climate_categories-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/.github/ISSUE_TEMPLATE/new_categorization.md` & `climate_categories-0.8.2/.github/ISSUE_TEMPLATE/new_categorization.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/.github/workflows/ci.yml` & `climate_categories-0.8.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/.gitignore` & `climate_categories-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/.pre-commit-config.yaml` & `climate_categories-0.8.2/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       - id: check-ast
       - id: fix-byte-order-marker
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: detect-private-key
       - id: mixed-line-ending
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: 'v0.0.263'
+    rev: 'v0.0.265'
     hooks:
       - id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
   - repo: https://github.com/psf/black
     rev: '23.3.0'
     hooks:
       - id: black
```

### Comparing `climate_categories-0.8.1/CHANGELOG.rst` & `climate_categories-0.8.2/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 Changelog
 =========
 
+0.8.2 (2023-05-15)
+------------------
+* Remove pygments-csv-lexer dependency for docs building.
+* Add function to find leaf children of a category, useful for re-calculating top-level
+  categories from constituents.
+
 0.8.1 (2023-04-26)
 ------------------
 * regenerate data included in the package to benefit
   from latest fixes in data generation scripts.
 
 0.8.0 (2023-04-26)
 ------------------
```

### Comparing `climate_categories-0.8.1/CONTRIBUTING.rst` & `climate_categories-0.8.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/LICENSE` & `climate_categories-0.8.2/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Apache Software License 2.0
 
 Copyright (c) 2021 Potsdam-Institut für Klimafolgenforschung e.V.
 Copyright (c) 2021 Robert Gieseke
+Copyright (c) 2023 Climate Resource Pty Ltd.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `climate_categories-0.8.1/Makefile` & `climate_categories-0.8.2/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 	rm -rf build/
 
 update-citation: ## Update the citation information from zenodo
 	venv/bin/python update_citation_info.py
 	git commit -am 'Update citation information from zenodo.'
 
 release: dist ## package and upload a release
-	venv/bin/twine upload dist/*
+	venv/bin/twine upload --repository climate-categories dist/*
 
 dist: clean venv ## builds source and wheel package
 	venv/bin/python -m build
 	ls -l dist
 
 install: clean ## install the package to the active Python's site-packages
 	python setup.py install
```

### Comparing `climate_categories-0.8.1/PKG-INFO` & `climate_categories-0.8.2/climate_categories.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: climate_categories
-Version: 0.8.1
+Name: climate-categories
+Version: 0.8.2
 Summary: Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 Home-page: https://github.com/pik-primap/climate_categories
 Author: Mika Pflüger
-Author-email: mika.pflueger@pik-potsdam.de
+Author-email: mika.pflueger@climate-resource.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://climate-categories.readthedocs.io/
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -79,36 +79,44 @@
 
 License
 -------
 Copyright 2021, Potsdam-Institut für Klimafolgenforschung e.V.
 
 Copyright 2021, Robert Gieseke
 
+Copyright 2023, Climate Resource Pty Ltd
+
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this
 file except in compliance with the License. You may obtain a copy of the License at
 
 https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software distributed under
 the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied. See the License for the specific language governing
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-04-26).
-pik-primap/climate_categories: climate_categories Version 0.8.1.
-Zenodo. https://doi.org/10.5281/zenodo.7867951
+Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-05-15).
+pik-primap/climate_categories: climate_categories Version 0.8.2.
+Zenodo. https://doi.org/10.5281/zenodo.7938167
 
 =========
 Changelog
 =========
 
+0.8.2 (2023-05-15)
+------------------
+* Remove pygments-csv-lexer dependency for docs building.
+* Add function to find leaf children of a category, useful for re-calculating top-level
+  categories from constituents.
+
 0.8.1 (2023-04-26)
 ------------------
 * regenerate data included in the package to benefit
   from latest fixes in data generation scripts.
 
 0.8.0 (2023-04-26)
 ------------------
```

### Comparing `climate_categories-0.8.1/README.rst` & `climate_categories-0.8.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -55,24 +55,26 @@
 
 License
 -------
 Copyright 2021, Potsdam-Institut für Klimafolgenforschung e.V.
 
 Copyright 2021, Robert Gieseke
 
+Copyright 2023, Climate Resource Pty Ltd
+
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this
 file except in compliance with the License. You may obtain a copy of the License at
 
 https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software distributed under
 the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied. See the License for the specific language governing
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-04-26).
-pik-primap/climate_categories: climate_categories Version 0.8.1.
-Zenodo. https://doi.org/10.5281/zenodo.7867951
+Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-05-15).
+pik-primap/climate_categories: climate_categories Version 0.8.2.
+Zenodo. https://doi.org/10.5281/zenodo.7938167
```

### Comparing `climate_categories-0.8.1/climate_categories/__init__.py` & `climate_categories-0.8.2/climate_categories/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Access to all categorizations is provided directly at the module level, using the
 names of categorizations. To access the example categorization `Excat`, simply use
 `climate_categories.Excat` .
 """
 
 __author__ = """Mika Pflüger"""
-__email__ = "mika.pflueger@pik-potsdam.de"
-__version__ = "0.8.1"
+__email__ = "mika.pflueger@climate-resource.com"
+__version__ = "0.8.2"
 
 import importlib
 import importlib.resources
 
 from . import (
     search,
 )
```

### Comparing `climate_categories-0.8.1/climate_categories/_categories.py` & `climate_categories-0.8.2/climate_categories/_categories.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Classes to represent and query categorical systems."""
 
 import datetime
 import functools
 import importlib
 import importlib.resources
+import itertools
 import pathlib
 import pickle
 import typing
 
 import natsort
 import networkx as nx
 import pandas
@@ -176,14 +177,38 @@
     def descendants(self) -> set["HierarchicalCategory"]:
         """The sets of subcategories comprising this category directly or indirectly.
 
         Note that all possible descendants are returned, not only "canonical" ones."""
         return self.categorization.descendants(self)
 
     @property
+    def is_leaf(self) -> bool:
+        """Is this category a leaf category, i.e. without children?"""
+        return not any(self.children)
+
+    @property
+    def leaf_children(self) -> list[set["HierarchicalCategory"]]:
+        """The sets of subcategories which are descendants of this category and do not
+        have children themselves.
+
+        Sets of children are chased separately, so each set of leaf children is
+        self-sufficient to reconstruct this category (if the categorization allows
+        reconstructing categories from their children, i.e. if total_sum is set)."""
+        ret = []
+        for children in self.children:
+            n = []
+            for child in children:
+                if child.is_leaf:
+                    n.append([{child}])
+                else:
+                    n.append(child.leaf_children)
+            ret += [set(itertools.chain(*x)) for x in itertools.product(*n)]
+        return ret
+
+    @property
     def level(self) -> int:
         """The level of the category.
 
         The canonical top-level category has level 1 and its children have level 2 etc.
 
         To calculate the level, only the first ("canonical") set of children is
         considered for intermediate categories.
@@ -1057,22 +1082,45 @@
         for _, child, setno in self._graph.edges(cat, "set"):
             if setno not in children_dict:
                 children_dict[setno] = []
             children_dict[setno].append(child)
 
         return [set(children_dict[x]) for x in sorted(children_dict.keys())]
 
-    def descendants(self, cat: typing.Union[str, HierarchicalCategory]):
+    def descendants(
+        self, cat: typing.Union[str, HierarchicalCategory]
+    ) -> set[HierarchicalCategory]:
         """All descendants of the given category, i.e. the direct children and their
         children, etc."""
         if not isinstance(cat, HierarchicalCategory):
             return self.descendants(self._all_codes_map[cat])
 
         return set(nx.descendants(self._graph, cat))
 
+    def is_leaf(self, cat: typing.Union[str, HierarchicalCategory]) -> bool:
+        """Is the category a leaf category, i.e. without children?"""
+        if not isinstance(cat, HierarchicalCategory):
+            return self.is_leaf(self._all_codes_map[cat])
+
+        return cat.is_leaf
+
+    def leaf_children(
+        self, cat: typing.Union[str, HierarchicalCategory]
+    ) -> list[set[HierarchicalCategory]]:
+        """The sets of subcategories which are descendants of the category and do not
+        have children themselves.
+
+        Sets of children are chased separately, so each set of leaf children is
+        self-sufficient to reconstruct this category (if the categorization allows
+        reconstructing categories from their children, i.e. if total_sum is set)."""
+        if not isinstance(cat, HierarchicalCategory):
+            return self.leaf_children(self._all_codes_map[cat])
+
+        return cat.leaf_children
+
 
 def from_pickle(
     filepath: typing.Union[str, pathlib.Path, typing.IO[bytes]]
 ) -> typing.Union[Categorization, HierarchicalCategorization]:
     """De-serialize Categorization or HierarchicalCategorization from a file written by
     to_pickle.
```

### Comparing `climate_categories-0.8.1/climate_categories/_conversions.py` & `climate_categories-0.8.2/climate_categories/_conversions.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/BURDI.py` & `climate_categories-0.8.2/climate_categories/data/BURDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/BURDI.yaml` & `climate_categories-0.8.2/climate_categories/data/BURDI.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/BURDI_class.py` & `climate_categories-0.8.2/climate_categories/data/BURDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/BURDI_class.yaml` & `climate_categories-0.8.2/climate_categories/data/BURDI_class.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/CRF1999.py` & `climate_categories-0.8.2/climate_categories/data/CRF1999.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/CRF1999.yaml` & `climate_categories-0.8.2/climate_categories/data/CRF1999.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/CRF2013.py` & `climate_categories-0.8.2/climate_categories/data/CRF2013.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/CRF2013.yaml` & `climate_categories-0.8.2/climate_categories/data/CRF2013.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/CRF2013_2021.py` & `climate_categories-0.8.2/climate_categories/data/CRF2013_2021.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/CRF2013_2021.yaml` & `climate_categories-0.8.2/climate_categories/data/CRF2013_2021.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/CRF2013_2022.py` & `climate_categories-0.8.2/climate_categories/data/CRF2013_2022.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/CRF2013_2022.yaml` & `climate_categories-0.8.2/climate_categories/data/CRF2013_2022.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/CRF2013_2023.py` & `climate_categories-0.8.2/climate_categories/data/CRF2013_2023.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/CRF2013_2023.yaml` & `climate_categories-0.8.2/climate_categories/data/CRF2013_2023.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/CRFDI.py` & `climate_categories-0.8.2/climate_categories/data/CRFDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/CRFDI.yaml` & `climate_categories-0.8.2/climate_categories/data/CRFDI.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/CRFDI_class.py` & `climate_categories-0.8.2/climate_categories/data/CRFDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/CRFDI_class.yaml` & `climate_categories-0.8.2/climate_categories/data/CRFDI_class.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/GCB.py` & `climate_categories-0.8.2/climate_categories/data/GCB.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/GCB.yaml` & `climate_categories-0.8.2/climate_categories/data/GCB.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/IPCC1996.py` & `climate_categories-0.8.2/climate_categories/data/IPCC1996.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/IPCC1996.yaml` & `climate_categories-0.8.2/climate_categories/data/IPCC1996.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/IPCC2006.py` & `climate_categories-0.8.2/climate_categories/data/IPCC2006.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/IPCC2006.yaml` & `climate_categories-0.8.2/climate_categories/data/IPCC2006.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/IPCC2006_PRIMAP.py` & `climate_categories-0.8.2/climate_categories/data/IPCC2006_PRIMAP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/IPCC2006_PRIMAP.yaml` & `climate_categories-0.8.2/climate_categories/data/IPCC2006_PRIMAP.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/RCMIP.py` & `climate_categories-0.8.2/climate_categories/data/RCMIP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/RCMIP.yaml` & `climate_categories-0.8.2/climate_categories/data/RCMIP.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/conversion.IPCC1996.IPCC2006.csv` & `climate_categories-0.8.2/climate_categories/data/conversion.IPCC1996.IPCC2006.csv`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/gas.py` & `climate_categories-0.8.2/climate_categories/data/gas.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/data/gas.yaml` & `climate_categories-0.8.2/climate_categories/data/gas.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/tests/conftest.py` & `climate_categories-0.8.2/climate_categories/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/tests/data/broken_hierarchical_categorization.yaml` & `climate_categories-0.8.2/climate_categories/tests/data/broken_hierarchical_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/tests/data/broken_simple_categorization.yaml` & `climate_categories-0.8.2/climate_categories/tests/data/broken_simple_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/tests/data/good_conversion_A.yaml` & `climate_categories-0.8.2/climate_categories/tests/data/good_conversion_A.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/tests/data/hierarchical_categorization.yaml` & `climate_categories-0.8.2/climate_categories/tests/data/hierarchical_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/tests/data/simple_categorization.yaml` & `climate_categories-0.8.2/climate_categories/tests/data/simple_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/tests/examples.py` & `climate_categories-0.8.2/climate_categories/tests/examples.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/tests/test_climate_categories.py` & `climate_categories-0.8.2/climate_categories/tests/test_climate_categories.py`

 * *Files 6% similar despite different names*

```diff
@@ -274,14 +274,28 @@
             HierCat["2"],
             HierCat["1A"],
             HierCat["1B"],
             HierCat["2A"],
             HierCat["2B"],
         }
 
+        assert HierCat["1A"].is_leaf
+        assert not HierCat["1"].is_leaf
+        assert HierCat.is_leaf("3A")
+        assert HierCat.leaf_children("1") == [{HierCat["1A"], HierCat["1B"]}]
+        assert HierCat.leaf_children("0X3") == [
+            {HierCat["1A"], HierCat["1B"], HierCat["2A"], HierCat["2B"]}
+        ]
+        assert HierCat.leaf_children("0") == [
+            {HierCat["1A"], HierCat["1B"], HierCat["2A"], HierCat["2B"], HierCat["3A"]},
+            {HierCat["1A"], HierCat["1B"], HierCat["2A"], HierCat["2B"], HierCat["3A"]},
+            {HierCat["1A"], HierCat["1B"], HierCat["2A"], HierCat["2B"], HierCat["3A"]},
+        ]
+        assert HierCat.leaf_children("OT") == [{HierCat["1B"], HierCat["2B"]}]
+
         with pytest.raises(
             ValueError,
             match="'OT' is not a transitive child of the canonical top level '0'.",
         ):
             HierCat.level("OT")
 
     def test_dict_like(self, HierCat: climate_categories.HierarchicalCategorization):
```

### Comparing `climate_categories-0.8.1/climate_categories/tests/test_conversions.py` & `climate_categories-0.8.2/climate_categories/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/tests/test_crf.py` & `climate_categories-0.8.2/climate_categories/tests/test_crf.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/tests/test_di.py` & `climate_categories-0.8.2/climate_categories/tests/test_di.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/tests/test_ipcc.py` & `climate_categories-0.8.2/climate_categories/tests/test_ipcc.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/tests/test_overcounting.py` & `climate_categories-0.8.2/climate_categories/tests/test_overcounting.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/tests/test_primap.py` & `climate_categories-0.8.2/climate_categories/tests/test_primap.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories/tests/test_search.py` & `climate_categories-0.8.2/climate_categories/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/climate_categories.egg-info/PKG-INFO` & `climate_categories-0.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: climate-categories
-Version: 0.8.1
+Name: climate_categories
+Version: 0.8.2
 Summary: Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 Home-page: https://github.com/pik-primap/climate_categories
 Author: Mika Pflüger
-Author-email: mika.pflueger@pik-potsdam.de
+Author-email: mika.pflueger@climate-resource.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://climate-categories.readthedocs.io/
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -79,36 +79,44 @@
 
 License
 -------
 Copyright 2021, Potsdam-Institut für Klimafolgenforschung e.V.
 
 Copyright 2021, Robert Gieseke
 
+Copyright 2023, Climate Resource Pty Ltd
+
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this
 file except in compliance with the License. You may obtain a copy of the License at
 
 https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software distributed under
 the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied. See the License for the specific language governing
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-04-26).
-pik-primap/climate_categories: climate_categories Version 0.8.1.
-Zenodo. https://doi.org/10.5281/zenodo.7867951
+Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-05-15).
+pik-primap/climate_categories: climate_categories Version 0.8.2.
+Zenodo. https://doi.org/10.5281/zenodo.7938167
 
 =========
 Changelog
 =========
 
+0.8.2 (2023-05-15)
+------------------
+* Remove pygments-csv-lexer dependency for docs building.
+* Add function to find leaf children of a category, useful for re-calculating top-level
+  categories from constituents.
+
 0.8.1 (2023-04-26)
 ------------------
 * regenerate data included in the package to benefit
   from latest fixes in data generation scripts.
 
 0.8.0 (2023-04-26)
 ------------------
```

### Comparing `climate_categories-0.8.1/climate_categories.egg-info/SOURCES.txt` & `climate_categories-0.8.2/climate_categories.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/BURDI.py` & `climate_categories-0.8.2/data_generation/BURDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/BURDI_class.py` & `climate_categories-0.8.2/data_generation/BURDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/CRF1999.py` & `climate_categories-0.8.2/data_generation/CRF1999.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/CRF2013.py` & `climate_categories-0.8.2/data_generation/CRF2013.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/CRF2013_2021.py` & `climate_categories-0.8.2/data_generation/CRF2013_2021.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/CRF2013_2022.py` & `climate_categories-0.8.2/data_generation/CRF2013_2022.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/CRF2013_2023.py` & `climate_categories-0.8.2/data_generation/CRF2013_2023.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/CRFDI.py` & `climate_categories-0.8.2/data_generation/CRFDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/CRFDI_class.py` & `climate_categories-0.8.2/data_generation/CRFDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/IPCC1996.py` & `climate_categories-0.8.2/data_generation/IPCC1996.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/IPCC2006.py` & `climate_categories-0.8.2/data_generation/IPCC2006.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/IPCC2006_PRIMAP.py` & `climate_categories-0.8.2/data_generation/IPCC2006_PRIMAP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/RCMIP.py` & `climate_categories-0.8.2/data_generation/RCMIP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/gas.py` & `climate_categories-0.8.2/data_generation/gas.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/data_generation/utils.py` & `climate_categories-0.8.2/data_generation/utils.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/docs/Makefile` & `climate_categories-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/docs/conf.py` & `climate_categories-0.8.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 release = climate_categories.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -100,15 +100,15 @@
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ["_static"]
+# html_static_path = ["_static"]
 
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "climate_categoriesdoc"
```

### Comparing `climate_categories-0.8.1/docs/data.rst` & `climate_categories-0.8.2/docs/data.rst`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,14 @@
 In formulas and lists, category codes that
 consist of alphanumeric characters and dots can be written directly, and other category
 codes must be enclosed in ``"`` characters.
 
 Example
 -------
 
-.. code-block:: csv
+.. code-block:: yaml
 
     # comment: an example conversion
     # institution: PIK
     IPCC1996,gas,IPCC2006,comment
     4 + 5,,3,Both sectors were combined
     4.D,N2O,3.C.4 + 3.C.5,N2O emissions are separated into own categories
```

### Comparing `climate_categories-0.8.1/docs/installation.rst` & `climate_categories-0.8.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/docs/make.bat` & `climate_categories-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/docs/usage.ipynb` & `climate_categories-0.8.2/docs/usage.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954545454545455%*

 * *Differences: {"'cells'": "{insert: [(25, OrderedDict([('cell_type', 'markdown'), ('source', ['### Finding leaf "*

 * *            "descendants\\n', '\\n', 'For purposes like re-calculating top-level categories from "*

 * *            "simple leaf categories, it\\n', 'is useful to find the descendants of a category "*

 * *            "which have no children. Use the\\n', '`leaf_children` property to do so.']), "*

 * *            "('metadata', OrderedDict([('collapsed', False)]))])), (26, OrderedDict([('cell_type', "*

 * *            "'code'), (' […]*

```diff
@@ -377,14 +377,38 @@
             "source": [
                 "HierAltEx[\"0\"].children"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
+                "collapsed": false
+            },
+            "source": [
+                "### Finding leaf descendants\n",
+                "\n",
+                "For purposes like re-calculating top-level categories from simple leaf categories, it\n",
+                "is useful to find the descendants of a category which have no children. Use the\n",
+                "`leaf_children` property to do so."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "HierEx[\"0\"].leaf_children"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
                 "collapsed": false,
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
                 "### Extending categorizations\n",
```

### Comparing `climate_categories-0.8.1/setup.cfg` & `climate_categories-0.8.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [metadata]
 name = climate_categories
-version = 0.8.1
+version = 0.8.2
 author = Mika Pflüger
-author_email = mika.pflueger@pik-potsdam.de
+author_email = mika.pflueger@climate-resource.com
 description = Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 long_description = file: README.rst, CHANGELOG.rst
 long_description_content_type = text/x-rst
 url = https://github.com/pik-primap/climate_categories
 project_urls = 
 	Documentation = https://climate-categories.readthedocs.io/
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering :: Atmospheric Science
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
@@ -61,15 +61,14 @@
 	ipykernel
 	nbsphinx
 	networkx
 	xdoctest
 	camelot-py[plot] >= 0.11.0
 	tox
 	unfccc_di_api >= 3.0.1
-	pygments-csv-lexer
 	openscm-units
 	black
 
 [options.package_data]
 * = 
 	*.yaml
 	*.csv
```

### Comparing `climate_categories-0.8.1/tbump.toml` & `climate_categories-0.8.2/tbump.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/pik-primap/climate_categories/"
 
 [version]
-current = "0.8.1"
+current = "0.8.2"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `climate_categories-0.8.1/update_changelog.py` & `climate_categories-0.8.2/update_changelog.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.1/update_citation_info.py` & `climate_categories-0.8.2/update_citation_info.py`

 * *Files identical despite different names*

