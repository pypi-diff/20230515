# Comparing `tmp/pyrsm-0.7.9.2.tar.gz` & `tmp/pyrsm-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsm-0.7.9.2.tar", last modified: Tue May  2 07:26:11 2023, max compression
+gzip compressed data, was "pyrsm-0.8.0.tar", last modified: Mon May 15 08:52:06 2023, max compression
```

## Comparing `pyrsm-0.7.9.2.tar` & `pyrsm-0.8.0.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.588299 pyrsm-0.7.9.2/
--rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.7.9.2/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      215 2023-03-25 21:03:06.000000 pyrsm-0.7.9.2/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      594 2023-05-02 07:26:11.588385 pyrsm-0.7.9.2/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2625 2023-03-25 21:31:10.000000 pyrsm-0.7.9.2/README.md
--rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.7.9.2/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.581397 pyrsm-0.7.9.2/pyrsm/
--rw-r--r--   0 root         (0) staff       (20)      273 2023-05-01 23:50:01.000000 pyrsm-0.7.9.2/pyrsm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    54297 2023-05-02 07:18:43.000000 pyrsm-0.7.9.2/pyrsm/basics.py
--rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.7.9.2/pyrsm/bins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.582197 pyrsm-0.7.9.2/pyrsm/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.582853 pyrsm-0.7.9.2/pyrsm/data/basics/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/basics/consider.pkl
--rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/basics/demand_uk.pkl
--rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/basics/newspaper.pkl
--rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/basics/salary.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.584075 pyrsm-0.7.9.2/pyrsm/data/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/data/avengers.pkl
--rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/data/diamonds.pkl
--rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/data/publishers.pkl
--rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/data/superheroes.pkl
--rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/data/titanic.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.584353 pyrsm-0.7.9.2/pyrsm/data/design/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/design/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/design/rndnames.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.586045 pyrsm-0.7.9.2/pyrsm/data/model/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/catalog.pkl
--rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/direct_marketing.pkl
--rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/dvd.pkl
--rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/houseprices.pkl
--rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/ideal.pkl
--rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/ketchup.pkl
--rw-r--r--   0 root         (0) staff       (20)      315 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/movie_contract.pkl
--rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/ratings.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.587357 pyrsm-0.7.9.2/pyrsm/data/multivariate/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/carpet.pkl
--rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/city.pkl
--rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/city2.pkl
--rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/computer.pkl
--rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/movie.pkl
--rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/mp3.pkl
--rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/retailers.pkl
--rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/shopping.pkl
--rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/toothpaste.pkl
--rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/tpbrands.pkl
--rw-r--r--   0 root         (0) staff       (20)     1966 2023-01-26 08:23:23.000000 pyrsm-0.7.9.2/pyrsm/example_data.py
--rw-r--r--   0 root         (0) staff       (20)    16298 2023-05-02 07:18:17.000000 pyrsm-0.7.9.2/pyrsm/logit.py
--rw-r--r--   0 root         (0) staff       (20)     2214 2023-02-28 23:28:31.000000 pyrsm-0.7.9.2/pyrsm/notebook.py
--rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.7.9.2/pyrsm/perf.py
--rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/props.py
--rw-r--r--   0 root         (0) staff       (20)    15639 2023-05-02 07:18:33.000000 pyrsm-0.7.9.2/pyrsm/regression.py
--rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.7.9.2/pyrsm/stats.py
--rw-r--r--   0 root         (0) staff       (20)    11145 2023-05-02 07:11:09.000000 pyrsm-0.7.9.2/pyrsm/utils.py
--rw-r--r--   0 root         (0) staff       (20)    23286 2023-04-30 01:31:14.000000 pyrsm-0.7.9.2/pyrsm/visualize.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.582065 pyrsm-0.7.9.2/pyrsm.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      594 2023-05-02 07:26:11.000000 pyrsm-0.7.9.2/pyrsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1632 2023-05-02 07:26:11.000000 pyrsm-0.7.9.2/pyrsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-02 07:26:11.000000 pyrsm-0.7.9.2/pyrsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      130 2023-05-02 07:26:11.000000 pyrsm-0.7.9.2/pyrsm.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-05-02 07:26:11.000000 pyrsm-0.7.9.2/pyrsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)      936 2023-05-02 07:26:11.588694 pyrsm-0.7.9.2/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.588188 pyrsm-0.7.9.2/tests/
--rw-r--r--   0 root         (0) staff       (20)      722 2022-03-07 07:21:43.000000 pyrsm-0.7.9.2/tests/test_basics.py
--rw-r--r--   0 root         (0) staff       (20)     1072 2023-03-05 06:28:28.000000 pyrsm-0.7.9.2/tests/test_bins.py
--rw-r--r--   0 root         (0) staff       (20)      794 2023-01-31 08:59:01.000000 pyrsm-0.7.9.2/tests/test_example_data.py
--rw-r--r--   0 root         (0) staff       (20)     2756 2023-01-21 01:15:24.000000 pyrsm-0.7.9.2/tests/test_perf.py
--rw-r--r--   0 root         (0) staff       (20)      663 2023-01-15 08:28:47.000000 pyrsm-0.7.9.2/tests/test_regression.py
--rw-r--r--   0 root         (0) staff       (20)     2036 2023-03-05 06:38:03.000000 pyrsm-0.7.9.2/tests/test_stats.py
--rw-r--r--   0 root         (0) staff       (20)     1979 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/tests/test_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.661436 pyrsm-0.8.0/
+-rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.0/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      215 2023-03-25 21:03:06.000000 pyrsm-0.8.0/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-05-15 08:52:06.661496 pyrsm-0.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2625 2023-03-25 21:31:10.000000 pyrsm-0.8.0/README.md
+-rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.0/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.652379 pyrsm-0.8.0/pyrsm/
+-rw-r--r--   0 root         (0) staff       (20)      289 2023-05-15 08:50:47.000000 pyrsm-0.8.0/pyrsm/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    54279 2023-05-15 06:31:28.000000 pyrsm-0.8.0/pyrsm/basics.py
+-rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.0/pyrsm/bins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.653735 pyrsm-0.8.0/pyrsm/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.654812 pyrsm-0.8.0/pyrsm/data/basics/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/basics/consider.pkl
+-rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/basics/demand_uk.pkl
+-rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/basics/newspaper.pkl
+-rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/basics/salary.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.655953 pyrsm-0.8.0/pyrsm/data/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/data/avengers.pkl
+-rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/data/diamonds.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/data/publishers.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/data/superheroes.pkl
+-rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/data/titanic.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.656338 pyrsm-0.8.0/pyrsm/data/design/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/design/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/design/rndnames.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.658713 pyrsm-0.8.0/pyrsm/data/model/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/catalog.pkl
+-rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/direct_marketing.pkl
+-rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/dvd.pkl
+-rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/houseprices.pkl
+-rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/ideal.pkl
+-rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/ketchup.pkl
+-rw-r--r--   0 root         (0) staff       (20)      315 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/movie_contract.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/ratings.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.660472 pyrsm-0.8.0/pyrsm/data/multivariate/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/carpet.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/city.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/city2.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/computer.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/movie.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/mp3.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/retailers.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/shopping.pkl
+-rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/toothpaste.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/tpbrands.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1966 2023-01-26 08:23:23.000000 pyrsm-0.8.0/pyrsm/example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     5271 2023-05-07 05:21:24.000000 pyrsm-0.8.0/pyrsm/logit.py
+-rw-r--r--   0 root         (0) staff       (20)    25101 2023-05-15 06:38:12.000000 pyrsm-0.8.0/pyrsm/model.py
+-rw-r--r--   0 root         (0) staff       (20)     2214 2023-02-28 23:28:31.000000 pyrsm-0.8.0/pyrsm/notebook.py
+-rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.0/pyrsm/perf.py
+-rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/props.py
+-rw-r--r--   0 root         (0) staff       (20)     7406 2023-05-15 08:45:10.000000 pyrsm-0.8.0/pyrsm/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.0/pyrsm/stats.py
+-rw-r--r--   0 root         (0) staff       (20)    10313 2023-05-14 21:06:56.000000 pyrsm-0.8.0/pyrsm/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    22540 2023-05-15 06:30:36.000000 pyrsm-0.8.0/pyrsm/visualize.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.653575 pyrsm-0.8.0/pyrsm.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-05-15 08:52:06.000000 pyrsm-0.8.0/pyrsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1644 2023-05-15 08:52:06.000000 pyrsm-0.8.0/pyrsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-15 08:52:06.000000 pyrsm-0.8.0/pyrsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      143 2023-05-15 08:52:06.000000 pyrsm-0.8.0/pyrsm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-05-15 08:52:06.000000 pyrsm-0.8.0/pyrsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)      950 2023-05-15 08:52:06.661779 pyrsm-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.661325 pyrsm-0.8.0/tests/
+-rw-r--r--   0 root         (0) staff       (20)      722 2022-03-07 07:21:43.000000 pyrsm-0.8.0/tests/test_basics.py
+-rw-r--r--   0 root         (0) staff       (20)     1072 2023-03-05 06:28:28.000000 pyrsm-0.8.0/tests/test_bins.py
+-rw-r--r--   0 root         (0) staff       (20)      794 2023-01-31 08:59:01.000000 pyrsm-0.8.0/tests/test_example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     2756 2023-01-21 01:15:24.000000 pyrsm-0.8.0/tests/test_perf.py
+-rw-r--r--   0 root         (0) staff       (20)      657 2023-05-07 05:28:57.000000 pyrsm-0.8.0/tests/test_regression.py
+-rw-r--r--   0 root         (0) staff       (20)     2036 2023-03-05 06:38:03.000000 pyrsm-0.8.0/tests/test_stats.py
+-rw-r--r--   0 root         (0) staff       (20)     1979 2022-02-13 01:24:09.000000 pyrsm-0.8.0/tests/test_utils.py
```

### Comparing `pyrsm-0.7.9.2/LICENSE` & `pyrsm-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/PKG-INFO` & `pyrsm-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.7.9.2
+Version: 0.8.0
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.7.9.2/README.md` & `pyrsm-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/basics.py` & `pyrsm-0.8.0/pyrsm/basics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from cmath import sqrt
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from scipy import stats
 import seaborn as sns
-from .logit import sig_stars
+from .model import sig_stars
 from .utils import ifelse
 from typing import Any, Optional
 from scipy.stats import chisquare
 
 
 class cross_tabs:
     def __init__(self, df: pd.DataFrame, var1: str, var2: str) -> None:
@@ -457,15 +457,15 @@
                         cor_label(cn[i], longest, axes[i, j])
                     elif i > j:
                         cor_plot(df[cn[i]], df[cn[j]], axes[i, j], s_size)
                     else:
                         cor_text(cmat[j, i], pmat[j, i], axes[i, j], dec=2)
 
             plt.subplots_adjust(wspace=0.04, hspace=0.04)
-            plt.show()
+            # plt.show()
 
         cor_mat(self.df, self.cr, self.cp, dec=dec, nobs=nobs, figsize=figsize)
 
 
 class prob_calc:
     # Probability calculator
     def __init__(self, distribution: str, params: dict) -> None:
@@ -473,45 +473,44 @@
         self.__dict__.update(params)
         print("Probability calculator")
 
     def summary(self):
         print(f"Distribution: {self.distribution}")
 
         def calc_f_dist(
-            dfn: int, dfd: int, lb: float = 0, ub: float = 0.95, decimals: int = 3
+            df1: int, df2: int, lb: float = 0, ub: float = 0.95, decimals: int = 3
         ) -> tuple[float, float]:
-            print(f"Df 1:\t{dfn}")
-            print(f"Df 2:\t{dfd}")
-
-            print(f"Mean:\t{round(stats.f.mean(dfn, dfd, loc=lb), decimals)}")
-            print(f"Variance:\t{round(stats.f.var(dfn, dfd, loc=lb), decimals)}")
-            print(f"Lower bound:\t{lb}")
-            print(f"Upper bound:\t{ub}\n")
+            print(f"Df 1        : {df1}")
+            print(f"Df 2        : {df2}")
+            print(f"Mean        : {round(stats.f.mean(df1, df2, loc=lb), decimals)}")
+            print(f"Variance    : {round(stats.f.var(df1, df2, loc=lb), decimals)}")
+            print(f"Lower bound : {lb}")
+            print(f"Upper bound : {ub}\n")
 
             if lb == 0:
-                critical_f = round(stats.f.ppf(q=ub, dfn=dfn, dfd=dfd), decimals)
+                critical_f = round(stats.f.ppf(q=ub, dfn=df1, dfd=df2), decimals)
 
                 _num_decimal_places_in_ub = len(str(ub).split(".")[-1])
 
                 print(f"P(X < {critical_f}) = {ub}")
                 print(
                     f"P(X > {critical_f}) = {round(1 - ub, _num_decimal_places_in_ub)}"
                 )
                 return (0, critical_f)
 
-            critical_f_lower = round(stats.f.ppf(q=lb, dfn=dfn, dfd=dfd), decimals)
+            critical_f_lower = round(stats.f.ppf(q=lb, dfn=df1, dfd=df2), decimals)
 
             _num_decimal_places_in_lb = len(str(lb).split(".")[-1])
 
             print(f"P(X < {critical_f_lower}) = {lb}")
             print(
                 f"P(X > {critical_f_lower}) = {round(1 - lb, _num_decimal_places_in_lb)}"
             )
             ########################################################################################
-            critical_f_upper = round(stats.f.ppf(q=ub, dfn=dfn, dfd=dfd), decimals)
+            critical_f_upper = round(stats.f.ppf(q=ub, dfn=df1, dfd=df2), decimals)
 
             _num_decimal_places_in_ub = len(str(ub).split(".")[-1])
 
             print(f"P(X < {critical_f_upper}) = {ub}")
             print(
                 f"P(X > {critical_f_upper}) = {round(1 - ub, _num_decimal_places_in_ub)}"
             )
@@ -528,20 +527,19 @@
             )
 
             return (critical_f_lower, critical_f_upper)
 
         def calc_t_dist(
             df: int, lb: float = 0, ub: float = 0.95, decimals: int = 3
         ) -> tuple[float, float]:
-            print(f"Df:\t{df}")
-            print(f"Mean:\t{round(stats.t.mean(df), decimals)}")
-            print(f"St. dev:\t{round(stats.t.std(df), decimals)}")
-            print(f"Lower bound:\t{lb}")
-            print(f"Upper bound:\t{ub}")
-            print()
+            print(f"Df          : {df}")
+            print(f"Mean        : {round(stats.t.mean(df), decimals)}")
+            print(f"St. dev     : {round(stats.t.std(df), decimals)}")
+            print(f"Lower bound : {lb}")
+            print(f"Upper bound : {ub}\n")
 
             if lb == 0:
                 critical_t = round(stats.t.ppf(q=ub, df=df), decimals)
 
                 _num_decimal_places_in_ub = len(str(ub).split(".")[-1])
 
                 print(f"P(X < {critical_t}) = {ub}")
@@ -572,52 +570,49 @@
                 len(str(ub).split(".")[-1]), len(str(lb).split(".")[-1])
             )
 
             print(
                 f"P({critical_t_lower} < X < {critical_t_upper}) = {round((ub - lb), _num_decimal_places)}"
             )
             print(
-                f"1 - P({critical_t_lower} < X < {critical_t_upper} = {round(1 - (ub - lb), _num_decimal_places)}"
+                f"1 - P({critical_t_lower} < X < {critical_t_upper}) = {round(1 - (ub - lb), _num_decimal_places)}"
             )
 
             return (critical_t_lower, critical_t_upper)
 
         if self.distribution == "F":
             lb = self.lb if "lb" in self.__dict__ else 0
             ub = self.ub if "ub" in self.__dict__ else 0.95
-            dfn = self.dfn
-            dfd = self.dfd
+            df1 = self.df1
+            df2 = self.df2
             decimals = self.decimals if "decimals" in self.__dict__ else 3
-            calc_f_dist(dfn, dfd, lb, ub, decimals)
+            calc_f_dist(df1, df2, lb, ub, decimals)
 
         elif self.distribution == "t":
             lb = self.lb if "lb" in self.__dict__ else 0
             ub = self.ub if "ub" in self.__dict__ else 0.95
             df = self.df
             decimals = self.decimals if "decimals" in self.__dict__ else 3
             calc_t_dist(df, lb, ub, decimals)
 
     def plot(self):
         def plot_f_dist(
-            dfn: int, dfd: int, lb: float = 0, ub: float = 0.95, decimals: int = 3
+            df1: int, df2: int, lb: float = 0, ub: float = 0.95, decimals: int = 3
         ):
-            x = np.linspace(stats.f.ppf(0, dfn, dfd), stats.f.ppf(0.99, dfn, dfd), 200)
-
-            plt.grid()
-            pdf = stats.f.pdf(x, dfn, dfd)
-
+            x = np.linspace(stats.f.ppf(0, df1, df2), stats.f.ppf(0.99, df1, df2), 200)
+            pdf = stats.f.pdf(x, df1, df2)
             plt.plot(x, pdf, "black", lw=1, alpha=0.6, label="f pdf")
 
             if lb == 0:
-                critical_f = round(stats.f.ppf(q=ub, dfn=dfn, dfd=dfd), decimals)
+                critical_f = round(stats.f.ppf(q=ub, dfn=df1, dfd=df2), decimals)
                 plt.fill_between(x, pdf, where=(x < critical_f), color="slateblue")
                 plt.fill_between(x, pdf, where=(x > critical_f), color="salmon")
             else:
-                critical_f_lower = round(stats.f.ppf(q=lb, dfn=dfn, dfd=dfd), decimals)
-                critical_f_upper = round(stats.f.ppf(q=ub, dfn=dfn, dfd=dfd), decimals)
+                critical_f_lower = round(stats.f.ppf(q=lb, dfn=df1, dfd=df2), decimals)
+                critical_f_upper = round(stats.f.ppf(q=ub, dfn=df1, dfd=df2), decimals)
 
                 plt.fill_between(
                     x,
                     pdf,
                     where=((x > critical_f_upper) | (x < critical_f_lower)),
                     color="slateblue",
                 )
@@ -628,18 +623,15 @@
                     color="salmon",
                 )
 
         def plot_t_dist(
             df: int, lb: float = 0.025, ub: float = 0.975, decimals: int = 3
         ):
             x = np.linspace(stats.t.ppf(0.01, df), stats.t.ppf(0.99, df), 200)
-
-            plt.grid()
             pdf = stats.t.pdf(x, df)
-
             plt.plot(x, pdf, "black", lw=1, alpha=0.6, label="t pdf")
 
             if lb == 0:
                 critical_t = round(stats.t.ppf(q=ub, df=df), decimals)
                 plt.fill_between(x, pdf, where=(x < critical_t), color="slateblue")
                 plt.fill_between(x, pdf, where=(x > critical_t), color="salmon")
             else:
@@ -658,18 +650,18 @@
                     where=((x > critical_t_upper) | (x < critical_t_lower)),
                     color="salmon",
                 )
 
         if self.distribution == "F":
             lb = self.lb if "lb" in self.__dict__ else 0
             ub = self.ub if "ub" in self.__dict__ else 0.95
-            dfn = self.dfn
-            dfd = self.dfd
+            df1 = self.df1
+            df2 = self.df2
             decimals = self.decimals if "decimals" in self.__dict__ else 3
-            plot_f_dist(dfn, dfd, lb, ub, decimals)
+            plot_f_dist(df1, df2, lb, ub, decimals)
 
         elif self.distribution == "t":
             lb = self.lb if "lb" in self.__dict__ else 0
             ub = self.ub if "ub" in self.__dict__ else 0.95
             df = self.df
             decimals = self.decimals if "decimals" in self.__dict__ else 3
             plot_t_dist(df, lb, ub, decimals)
@@ -1278,15 +1270,15 @@
 
         plt.axes(axes[1][1])
         axes[1][1].set_ylabel("y")
         self._plot_distribution(
             x=sample_means, x_label="Density of sample means", density_plot=True
         ).plot()
 
-        plt.show()
+        # plt.show()
 
     def _plot_distribution(
         self, x: list[np.ndarray], x_label: str, density_plot: bool = False
     ) -> matplotlib.axes.Axes:
         stat = "count"
         data = {x_label: x}
 
@@ -1561,8 +1553,8 @@
             )
 
             barplot.axhline(y=z_90, color="k", linestyle="dashed", linewidth=1)
             barplot.axhline(y=z_neg_90, color="k", linestyle="dashed", linewidth=1)
 
             barplot.plot()
 
-        plt.show()
+        # plt.show()
```

### Comparing `pyrsm-0.7.9.2/pyrsm/bins.py` & `pyrsm-0.8.0/pyrsm/bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/basics/consider.pkl` & `pyrsm-0.8.0/pyrsm/data/basics/consider.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/basics/demand_uk.pkl` & `pyrsm-0.8.0/pyrsm/data/basics/demand_uk.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/basics/newspaper.pkl` & `pyrsm-0.8.0/pyrsm/data/basics/newspaper.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/basics/salary.pkl` & `pyrsm-0.8.0/pyrsm/data/basics/salary.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/data/avengers.pkl` & `pyrsm-0.8.0/pyrsm/data/data/avengers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/data/diamonds.pkl` & `pyrsm-0.8.0/pyrsm/data/data/diamonds.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/data/publishers.pkl` & `pyrsm-0.8.0/pyrsm/data/data/publishers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/data/superheroes.pkl` & `pyrsm-0.8.0/pyrsm/data/data/superheroes.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/data/titanic.pkl` & `pyrsm-0.8.0/pyrsm/data/data/titanic.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/design/rndnames.pkl` & `pyrsm-0.8.0/pyrsm/data/design/rndnames.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/model/catalog.pkl` & `pyrsm-0.8.0/pyrsm/data/model/catalog.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/model/direct_marketing.pkl` & `pyrsm-0.8.0/pyrsm/data/model/direct_marketing.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/model/dvd.pkl` & `pyrsm-0.8.0/pyrsm/data/model/dvd.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/model/houseprices.pkl` & `pyrsm-0.8.0/pyrsm/data/model/houseprices.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/model/ideal.pkl` & `pyrsm-0.8.0/pyrsm/data/model/ideal.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/model/ketchup.pkl` & `pyrsm-0.8.0/pyrsm/data/model/ketchup.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/model/ratings.pkl` & `pyrsm-0.8.0/pyrsm/data/model/ratings.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/multivariate/carpet.pkl` & `pyrsm-0.8.0/pyrsm/data/multivariate/carpet.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/multivariate/city.pkl` & `pyrsm-0.8.0/pyrsm/data/multivariate/city.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/multivariate/city2.pkl` & `pyrsm-0.8.0/pyrsm/data/multivariate/city2.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/multivariate/computer.pkl` & `pyrsm-0.8.0/pyrsm/data/multivariate/computer.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/multivariate/movie.pkl` & `pyrsm-0.8.0/pyrsm/data/multivariate/movie.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/multivariate/mp3.pkl` & `pyrsm-0.8.0/pyrsm/data/multivariate/mp3.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/multivariate/retailers.pkl` & `pyrsm-0.8.0/pyrsm/data/multivariate/retailers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/multivariate/shopping.pkl` & `pyrsm-0.8.0/pyrsm/data/multivariate/shopping.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/multivariate/toothpaste.pkl` & `pyrsm-0.8.0/pyrsm/data/multivariate/toothpaste.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/data/multivariate/tpbrands.pkl` & `pyrsm-0.8.0/pyrsm/data/multivariate/tpbrands.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/example_data.py` & `pyrsm-0.8.0/pyrsm/example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/logit.py` & `pyrsm-0.8.0/pyrsm/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,64 @@
 from typing import Union, Optional
+import re
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
+import seaborn as sns
 import statsmodels as sm
-from statsmodels.genmod.families import Binomial
-from statsmodels.genmod.families.links import logit
+import statsmodels.api as sma
 import statsmodels.formula.api as smf
 from statsmodels.stats.outliers_influence import variance_inflation_factor
+from math import ceil
 from scipy import stats
+from sklearn import metrics
 from scipy.special import expit
-from .utils import ifelse
+from .utils import ifelse, expand_grid
 from .stats import weighted_mean, weighted_sd
 from .perf import auc
-from .regression import sig_stars
 
 # from statsmodels.regression.linear_model import RegressionResults as rrs
-from .visualize import pred_plot_sm, vimp_plot_sm, extract_evars, extract_rvar
+# from .visualize import pred_plot_sm, vimp_plot_sm, extract_evars, extract_rvar
+
+
+def extract_evars(model, cn):
+    """
+    Extract a list of the names of the explanatory variables in a statsmodels model
+    """
+    pattern = r"\b\w+\b"
+    evars = re.findall(pattern, model.formula)[1:]
+    evars = [v for v in evars if v in cn]
+    return [v for i, v in enumerate(evars) if v not in evars[:i]]
+
+
+def extract_rvar(model, cn):
+    """
+    Extract name of the response variable in a statsmodels model
+    """
+    pattern = r"\b\w+\b"
+    return re.findall(pattern, model.formula)[0]
+
+
+def sig_stars(pval):
+    pval = np.nan_to_num(pval, nan=1.0)
+    cutpoints = np.array([0.001, 0.01, 0.05, 0.1, np.Inf])
+    symbols = np.array(["***", "**", "*", ".", " "])
+    return [symbols[p < cutpoints][0] for p in pval]
 
 
 def get_mfit(fitted) -> tuple[Optional[dict], Optional[str]]:
+    """
+    Get model fit statistics
+
+    Parameters
+    ----------
+    fitted : A fitted linear or logistic 4egression model
+    """
+
     mfit_dct = None
     model_type = None
     if isinstance(fitted, sm.genmod.generalized_linear_model.GLMResultsWrapper):
         fw = None
         if fitted.model._has_freq_weights:
             fw = fitted.model.freq_weights
 
@@ -206,21 +241,48 @@
 
     if hasattr(fitted, "model"):
         model = fitted.model
     else:
         # legacy for when only an un-fitted model was accepted
         model = fitted
 
-    vif = [variance_inflation_factor(model.exog, i) for i in range(model.exog.shape[1])]
-    df = pd.DataFrame(model.exog_names, columns=["variable"])
+    is_categorical = {
+        item.split("[T.")[0]: ("[T." in item) for item in model.exog_names
+    }
+    if sum(is_categorical.values()) > 0:
+        evar = list(is_categorical.keys())[1:]
+        exog = model.exog[:, 1:]
+        Xcorr = np.linalg.det(np.corrcoef(exog, rowvar=False))
+        df = pd.DataFrame(exog, columns=model.exog_names[1:])
+        vif = []
+        for col, cat in is_categorical.items():
+            if col == "Intercept":
+                continue
+            elif cat:
+                select = [f"{col}[T." in c for c in df.columns]
+                Vcorr = np.linalg.det(df.loc[:, select].corr().values)
+                drop = [lcl == False for lcl in select]
+                Ocorr = np.linalg.det(df.loc[:, drop].corr().values)
+            else:
+                Vcorr = 1
+                Ocorr = np.linalg.det(df.drop(col, axis=1).corr().values)
+
+            vif.append(Vcorr * Ocorr / Xcorr)
+        df = pd.DataFrame(evar, columns=[" "])
+    else:
+        vif = [
+            variance_inflation_factor(model.exog, i) for i in range(model.exog.shape[1])
+        ]
+        df = pd.DataFrame(model.exog_names, columns=[" "])
+
     df["vif"] = vif
     df["Rsq"] = 1 - 1 / df["vif"]
 
     if "Intercept" in model.exog_names:
-        df = df[df["variable"] != "Intercept"]
+        df = df[df[" "] != "Intercept"]
 
     df = df.sort_values("vif", ascending=False).reset_index(drop=True)
 
     if dec is not None:
         df = df.round(dec)
 
     return df
@@ -281,21 +343,26 @@
     exog = smf.logit(formula=form, data=df).exog
 
     low, high = [alpha / 2, 1 - (alpha / 2)]
     Xb = np.dot(exog, fitted.params)
     se = np.sqrt((exog.dot(fitted.cov_params()) * exog).sum(-1))
     me = stats.norm.ppf(high) * se
 
-    return pd.DataFrame(
-        {
-            "prediction": prediction,
-            f"{low*100}%": expit(Xb - me),
-            f"{high*100}%": expit(Xb + me),
-        }
-    )
+    if isinstance(fitted, sm.genmod.generalized_linear_model.GLMResultsWrapper):
+        return pd.DataFrame(
+            {
+                "prediction": prediction,
+                f"{low*100}%": expit(Xb - me),
+                f"{high*100}%": expit(Xb + me),
+            }
+        )
+    elif isinstance(fitted, sm.regression.linear_model.RegressionResultsWrapper):
+        return pd.DataFrame(
+            {"prediction": prediction, f"{low*100}%": Xb - me, f"{high*100}%": Xb + me}
+        )
 
 
 def model_fit(fitted, dec: int = 3, prn: bool = True) -> Union[str, pd.DataFrame]:
     """
     Compute various model fit statistics for a fitted linear or logistic regression model
 
     Parameters
@@ -337,134 +404,370 @@
 F-statistic: {mfit.fvalue[0].round(dec)} df({mfit.ftest_df_model.values[0]:.0f}, {mfit.ftest_df_resid.values[0]:.0f}), p.value {np.where(mfit.ftest_pval.values[0] < .001, "< 0.001", mfit.ftest_pval.values[0].round(dec))}
 Nr obs: {mfit.nobs.values[0]:,.0f}"""
         return output
     else:
         return mfit
 
 
-class logistic:
-    def __init__(
-        self,
-        dataset: pd.DataFrame,
-        rvar: Optional[str] = None,
-        lev: Optional[str] = None,
-        evar: Optional[list[str]] = None,
-        form: Optional[str] = None,
-    ) -> None:
-        """
-        Initialize logistic regression model
-
-        Parameters
-        ----------
-        dataset: pandas DataFrame; dataset
-        evar: List of strings; contains the names of the columns of data to be used as explanatory variables
-        rvar: String; name of the column to be used as the response variable
-        lev: String; name of the level in the response variable
-        ssq: Boolean; whether sum of squared errors need to be reported
-        form: String; formula for the regression equation to use if evar and rvar are not provided
-        """
-        self.dataset = dataset
-        self.rvar = rvar
-        self.lev = lev
-        self.evar = evar
-        self.form = form
-
-        if self.form:
-            self.fitted = smf.glm(
-                formula=self.form, data=self.dataset, family=Binomial(link=logit())
-            ).fit()
-            self.evar = extract_evars(self.fitted.model, self.dataset.columns)
-            self.rvar = extract_rvar(self.fitted.model, self.dataset.columns)
-            self.lev = self.dataset.at[0, self.rvar]
-        else:
-            self.form = f"{self.rvar} ~ {' + '.join(self.evar)}"
-            self.fitted = smf.glm(
-                formula=self.form, data=self.dataset, family=Binomial(link=logit())
-            ).fit()
-
-        df = pd.DataFrame(np.exp(self.fitted.params), columns=["OR"]).dropna()
-        df["OR%"] = 100 * ifelse(df["OR"] < 1, -(1 - df["OR"]), df["OR"] - 1)
-        df["coefficient"] = self.fitted.params
-        df["std.error"] = self.fitted.params / self.fitted.tvalues
-        # wierd but this is what statsmodels uses in summary
-        df["z.value"] = self.fitted.tvalues
-        df["p.value"] = self.fitted.pvalues
-        df["  "] = sig_stars(self.fitted.pvalues)
-        self.coef = df.reset_index()
-
-    def summary(self, dec=3) -> None:
-        """
-        Summarize output from a logistic regression model
-        """
+def coef_plot(
+    fitted,
+    alpha: float = 0.05,
+    intercept: bool = False,
+    incl: str = None,
+    excl: list = [],
+    figsize: tuple = None,
+):
+    """
+    Coefficient plot
 
-        if hasattr(self.dataset, "description"):
-            data_name = self.dataset.description.split("\n")[0].split()[1].lower()
-        else:
-            data_name = "Not available"
+    Parameters
+    ----------
+    fitted : A fitted linear regression model
+    alpha : float
+        Significance level
+    intercept : bool
+        Include intercept in coefficient plot (True or False)
+    incl : str or list of strings
+        Variables to include in the coefficient plot. All will be included by default
+    excl : str or list of strings
+        Variables to exclude from the coefficient plot. None are excluded by default
+
+    Returns
+    -------
+    Matplotlib object
+        Plot of Odds ratios
+    """
+    df = fitted.conf_int(alpha=alpha).reset_index().iloc[::-1]
+    df["coefficient"] = fitted.params[df["index"]].dropna().values
+
+    if not intercept:
+        df = df.query('index != "Intercept"')
+
+    if incl is not None:
+        incl = ifelse(isinstance(incl, str), [incl], incl)
+        rx = "(" + "|".join([f"^\b{v}|^{v}\\[" for v in incl]) + ")"
+        incl = df["index"].str.match(rf"{rx}")
+        if intercept:
+            incl[0] = True
+        df = df[incl]
+
+    if len(excl) > 0 and excl is not None:
+        excl = ifelse(isinstance(excl, str), [excl], excl)
+        rx = "(" + "|".join([f"^\b{v}|^{v}\\[" for v in excl]) + ")"
+        excl = df["index"].str.match(rf"{rx}")
+        if intercept:
+            excl[0] = False
+        df = df[~excl]
+
+    low, high = [100 * alpha / 2, 100 * (1 - (alpha / 2))]
+    df.columns = ["index", f"{low}%", f"{high}%", "coefficient"]
+    err = [df["coefficient"] - df[f"{low}%"], df[f"{high}%"] - df["coefficient"]]
+
+    fig = plt.figure(figsize=figsize)
+    ax = fig.add_subplot()
+    ax.axvline(0, ls="dashdot")
+    ax.errorbar(x="coefficient", y="index", data=df, xerr=err, fmt="none")
+    ax.scatter(x="coefficient", y="index", data=df)
+    ax.set(xlabel="Coefficient")
+    return ax
+
+
+def coef_ci(fitted, alpha: float = 0.05, intercept: bool = True, dec: int = 3):
+    """
+    Confidence interval for coefficient from linear regression
+
+    Parameters
+    ----------
+    fitted : A fitted linear regression model
+    alpha : float
+        Significance level
+    intercept : bool
+        Include intercept in the output (True or False)
+    dec : int
+        Number of decimal places to use in rounding
+
+    Returns
+    -------
+    Pandas dataframe with regression coefficients and confidence intervals
+    """
+
+    df = pd.DataFrame({"coefficient": fitted.params})
 
-        print("Logistic regression (GLM)")
-        print(f"Data                 : {data_name}")
-        print(f"Response variable    : {self.rvar}")
-        print(f"Level                : {self.lev}")
-        print(f"Explanatory variables: {', '.join(self.evar)}")
-        print(f"Null hyp.: there is no effect x on {self.rvar}")
-        print(f"Alt. hyp.: there is an effect of x on {self.rvar}")
-
-        self.coef["OR"] = self.coef["OR"].round(dec)
-        self.coef["coefficient"] = self.coef["coefficient"].round(2)
-        self.coef["std.error"] = self.coef["std.error"].round(dec)
-        self.coef["z.value"] = self.coef["z.value"].round(dec)
-        self.coef["p.value"] = ifelse(
-            self.coef["p.value"] < 0.001, "< .001", self.coef["p.value"].round(dec)
+    low, high = [100 * alpha / 2, 100 * (1 - (alpha / 2))]
+    df[[f"{low}%", f"{high}%"]] = fitted.conf_int(alpha=alpha)
+
+    if dec is None:
+        df["p.values"] = ifelse(fitted.pvalues < 0.001, "< .001", fitted.pvalues)
+    else:
+        df = df.round(dec)
+        df["p.values"] = ifelse(
+            fitted.pvalues < 0.001, "< .001", fitted.pvalues.round(dec)
         )
-        self.coef["OR%"] = [f"{round(o, max(dec-2, 0))}%" for o in self.coef["OR%"]]
-        print(f"\n{self.coef.to_string(index=False)}")
-        print("\nSignif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1")
-        print(f"\n{model_fit(self.fitted)}")
-
-    def ci(self, alpha=0.05, intercept=False, dec=3) -> None:
-        """
-        Confidence intervals for Odds Ratios
-        """
-        print(
-            f"\n{or_ci(self.fitted, alpha=alpha, intercept=intercept).to_string(index=False)}"
+
+    df["  "] = sig_stars(fitted.pvalues)
+    df = df.reset_index()
+
+    if intercept is False:
+        df = df.loc[df["index"] != "Intercept"]
+
+    return df
+
+
+def evalreg(df, rvar: str, pred: str, dec: int = 3):
+    """
+    Evaluate regression models. Calculates R-squared, MSE, and MAE
+
+    Parameters
+    ----------
+    df : Pandas DataFrame or a dictionary of DataFrames with keys to show results for
+        multiple model predictions and datasets (training and test)
+    rvar : str
+        Name of the response variable column in df
+    pred : str
+        Name of the column, of list of column names, in df with model predictions
+    dec : int
+        Number of decimal places to use in rounding
+
+    Examples
+    --------
+    """
+
+    dct = ifelse(isinstance(df, dict), df, {"All": df})
+    pred = ifelse(isinstance(pred, str), [pred], pred)
+
+    def calculate_metrics(key, dfm, pm):
+        return pd.DataFrame().assign(
+            Type=[key],
+            predictor=[pm],
+            n=[dfm.shape[0]],
+            r2=[metrics.r2_score(dfm[rvar], dfm[pm])],
+            mse=[metrics.mean_squared_error(dfm[rvar], dfm[pm])],
+            mae=[metrics.mean_absolute_error(dfm[rvar], dfm[pm])],
         )
 
-    def plot(
-        self,
-        plots="or",
-        alpha=0.05,
-        intercept=False,
-        incl=None,
-        excl=None,
-        incl_int=[],
-        fix=True,
-        hline=False,
-        figsize=None,
-    ) -> None:
-        """
-        Plots for a logistic regression model
-        """
-        if "or" in plots:
-            or_plot(
-                self.fitted,
-                alpha=alpha,
-                intercept=intercept,
-                incl=incl,
-                excl=excl,
-                figsize=figsize,
+    result = pd.concat(
+        [calculate_metrics(key, val, p) for key, val in dct.items() for p in pred],
+        axis=0,
+    )
+    result.index = range(result.shape[0])
+    return result.round(dec)
+
+
+def reg_dashboard(fitted, nobs: int = 1000):
+    """
+    Plot regression residual dashboard
+
+    Parameters
+    ----------
+    fitted : Object with fitted values and residuals
+    nobs: int
+        Number of observations to use for plots.
+        Set to None or -1 to plot all values.
+        The Residuals vs Order plot will only be valid
+        if all observations are plotted
+    """
+    fig, axes = plt.subplots(3, 2, figsize=(10, 10))
+    plt.subplots_adjust(wspace=0.25, hspace=0.4)
+
+    data = pd.DataFrame().assign(
+        fitted=fitted.fittedvalues,
+        actual=fitted.model.endog,
+        resid=fitted.resid,
+        std_resid=fitted.resid / np.std(fitted.resid),
+        order=np.arange(fitted.model.endog.shape[0]),
+    )
+
+    if (nobs != -1 and nobs is not None) and (nobs < data.shape[0]):
+        data = data.sample(nobs)
+
+    sns.regplot(x="fitted", y="actual", data=data, ax=axes[0, 0]).set(
+        title="Actual vs Fitted values", xlabel="Fitted values", ylabel="Actual values"
+    )
+    sns.regplot(x="fitted", y="resid", data=data, ax=axes[0, 1]).set(
+        title="Residuals vs Fitted values", xlabel="Fitted values", ylabel="Residuals"
+    )
+    sns.lineplot(x="order", y="resid", data=data, ax=axes[1, 0]).set(
+        title="Residuals vs Row order", ylabel="Residuals", xlabel=None
+    )
+    sma.qqplot(data.resid, line="s", ax=axes[1, 1])
+    axes[1, 1].title.set_text("Normal Q-Q plot")
+    pdp = data.resid.plot.hist(
+        ax=axes[2, 0],
+        title="Histogram of residuals",
+        xlabel="Residuals",
+        rot=0,
+        color="slateblue",
+    )
+    pdp.set_xlabel("Residuals")
+    sns.kdeplot(
+        data.std_resid, color="green", fill=True, ax=axes[2, 1], common_norm=True
+    )
+
+    # from https://stackoverflow.com/a/52925509/1974918
+    norm_x = np.arange(-3, +3, 0.01)
+    norm_y = stats.norm.pdf(norm_x)
+    sns.lineplot(x=norm_x, y=norm_y, lw=1, ax=axes[2, 1]).set(
+        title="Residuals vs Normal density", xlabel="Residuals"
+    )
+
+
+def sim_prediction(
+    df: pd.DataFrame,
+    vary: list = [],
+    nnv: int = 5,
+    minq: float = 0,
+    maxq: float = 1,
+) -> pd.DataFrame:
+    """
+    Simulate data for prediction
+
+    Parameters
+    ----------
+    df : Pandas DataFrame
+    vary : List of column names or Dictionary with keys and values to use
+    nnv : int
+        Number of values to use to simulate the effect of a numeric variable
+    minq : float
+        Quantile to use for the minimum value of numeric variables
+    maxq : float
+        Quantile to use for the maximum value of numeric variables
+
+    Returns:
+    ----------
+    Pandas DataFrame with values to use for estimation
+    """
+
+    def fix_value(s):
+        if pd.api.types.is_numeric_dtype(s.dtype):
+            return s.mean()
+        else:
+            return s.value_counts().idxmax()
+
+    dct = {c: [fix_value(df[c])] for c in df.columns}
+    dt = df.dtypes
+    if isinstance(vary, dict):
+        # user provided values and ranges
+        for key, val in vary.items():
+            dct[key] = val
+    else:
+        # auto derived values and ranges
+        vary = ifelse(isinstance(vary, str), [vary], vary)
+        for v in vary:
+            if pd.api.types.is_numeric_dtype(df[v].dtype):
+                nu = df[v].nunique()
+                if nu > 2:
+                    dct[v] = np.linspace(
+                        np.quantile(df[v], minq),
+                        np.quantile(df[v], maxq),
+                        min([nu, nnv]),
+                    )
+                else:
+                    dct[v] = [df[v].min(), df[v].max()]
+            else:
+                dct[v] = df[v].unique()
+
+    return expand_grid(dct, dt)
+
+
+def scatter_plot(
+    fitted, df, nobs: int = 1000, figsize: tuple = None, resid=False
+) -> None:
+    """
+    Scatter plot of explanatory and response variables from a fitted regression
+
+    Parameters
+    ----------
+    fitted : A fitted linear regression model
+    df : Pandas DataFrame
+        Data frame with explanatory and response variables
+    nobs : int
+        Number of observations to use for the scatter plots. The default
+        value is 1,000. To use all observations in the plots, use nobs=-1
+    figsize : tuple
+        A tuple that determines the figure size. If None, size is
+        determined based on the number of variables in the model
+    resid : bool
+        If True, use residuals as the response variable
+    """
+
+    exog_names = extract_evars(fitted.model, df.columns)
+
+    if resid:
+        endog = fitted.resid
+        endog_name = "residuals"
+        if df.shape[0] != endog.shape[0]:
+            raise ValueError(
+                "The number of observations in the fitted model and the data frame must be the same"
             )
-        if "pred" in plots:
-            pred_plot_sm(
-                self.fitted,
-                self.dataset,
-                incl=incl,
-                excl=[],
-                incl_int=incl_int,
-                fix=fix,
-                hline=hline,
-                nnv=20,
-                minq=0.025,
-                maxq=0.975,
+        else:
+            df = pd.concat(
+                [
+                    pd.DataFrame({endog_name: endog}),
+                    df[exog_names].copy().reset_index(drop=True),
+                ],
+                axis=1,
             )
-        if "vimp" in plots:
-            vimp_plot_sm(self.fitted, self.dataset, rep=10, ax=None, ret=False)
+    else:
+        endog_name = extract_rvar(fitted.model, df.columns)
+        df = df[[endog_name] + exog_names].copy()
+
+    nr_plots = len(exog_names)
+    if figsize is None:
+        figsize = (10, 2 * max(nr_plots, 4))
+
+    fig, ax = plt.subplots(max(ceil(nr_plots / 2), 2), 2, figsize=figsize)
+    plt.subplots_adjust(wspace=0.25, hspace=0.25)
+
+    idx = 0
+
+    if nobs < df.shape[0] and nobs != np.Inf and nobs != -1:
+        df = df.copy().sample(nobs)
+
+    while idx < nr_plots:
+        row = idx // 2
+        col = idx % 2
+        exog_name = exog_names[idx]
+        if pd.api.types.is_numeric_dtype(df[exog_name].dtype):
+            fig = sns.scatterplot(x=exog_name, y=endog_name, data=df, ax=ax[row, col])
+        else:
+            fig = sns.stripplot(x=exog_name, y=endog_name, data=df, ax=ax[row, col])
+            means = df.groupby(exog_name)[endog_name].mean()
+            levels = list(means.index)
+            # Loop over categories
+            for pos, cat in enumerate(levels):
+                # Add a line for the mean
+                ax[row, col].plot(
+                    [pos - 0.5, pos + 0.5], [means[pos], means[pos]], color="blue"
+                )
+
+        idx += 1
+
+    if nr_plots < 3:
+        ax[-1, -1].remove()
+        ax[-1, 0].remove()
+        if nr_plots == 1:
+            ax[0, -1].remove()
+    elif nr_plots % 2 == 1:
+        ax[-1, -1].remove()
+
+
+def residual_plot(
+    fitted,
+    df,
+    nobs: int = 1000,
+    figsize: tuple = None,
+) -> None:
+    """
+    Plot of variables vs residuals
+
+    Parameters
+    ----------
+    fitted : A fitted linear regression model
+    nobs : int
+        Number of observations to use for the scatter plots. The default
+        value is 1,000. To use all observations in the plots, use nobs=-1
+    figsize : tuple
+        A tuple that determines the figure size. If None, size is
+        determined based on the number of variables in the model
+    """
+
+    scatter_plot(fitted, df, nobs=nobs, figsize=figsize, resid=True)
```

### Comparing `pyrsm-0.7.9.2/pyrsm/notebook.py` & `pyrsm-0.8.0/pyrsm/notebook.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/perf.py` & `pyrsm-0.8.0/pyrsm/perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/props.py` & `pyrsm-0.8.0/pyrsm/props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/stats.py` & `pyrsm-0.8.0/pyrsm/stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/pyrsm/utils.py` & `pyrsm-0.8.0/pyrsm/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -416,32 +416,7 @@
         if private or not i[0].startswith("_"):
             if ins.ismethod(i[1]) or ins.isbuiltin(i[1]):
                 mth.append(i[0])
             else:
                 attr.append(i[0])
 
     return {"methods": mth, "attributes": attr}
-
-
-def group_categorical(
-    df: pd.DataFrame, prefix_sep: str = "["
-) -> tuple[pd.DataFrame, bool]:
-    columns_to_group = {
-        item.split(prefix_sep)[0]: (prefix_sep in item) for item in df.columns
-    }
-    if not any(columns_to_group.values()):
-        return df, False
-
-    series_list = []
-    for col, needs_to_collapse in columns_to_group.items():
-        if needs_to_collapse:
-            categorical_grouped = (
-                df.filter(like=col)
-                .idxmax(axis=1)
-                .apply(lambda x: x.split(prefix_sep, maxsplit=1)[1].split(".")[1][:-1])
-                .rename(col)
-            )
-            series_list.append(categorical_grouped)
-        else:
-            series_list.append(df[col])
-    categorical_grouped_df = pd.concat(series_list, axis=1)
-    return categorical_grouped_df, True
```

### Comparing `pyrsm-0.7.9.2/pyrsm/visualize.py` & `pyrsm-0.8.0/pyrsm/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import math
-import re
 import matplotlib.pyplot as plt
 import pandas as pd
 import numpy as np
 import seaborn as sns
 import statsmodels as sm
 from sklearn.inspection import permutation_importance
 from .utils import ifelse, intersect, setdiff
-from .regression import sim_prediction
+from .model import sim_prediction, extract_evars, extract_rvar
 from .perf import auc
 
 
 def distr_plot(df: pd.DataFrame, cols: list = None, nint: int = 25, **kwargs):
     """
     Plot histograms for numeric variables and frequency plots for categorical.
     variables. Columns of type integer with less than 25 unique values will be
@@ -73,47 +72,15 @@
         axes[-1, -1].remove()
         axes[-1, 0].remove()
         if df.shape[1] == 1:
             axes[0, -1].remove()
     elif df.shape[1] % 2 == 1:
         axes[-1, -1].remove()
 
-    plt.show()
-
-
-def scatter(
-    df: pd.DataFrame,
-    col1: str,
-    col2: str,
-    figsize: tuple[int, int] = (10, 10),
-) -> None:
-    _, ax = plt.subplots(figsize=figsize)
-    ax.set_xlabel(col1)
-    ax.set_ylabel(col2)
-    ax.scatter(df[col1], df[col2])
-
-    plt.show()
-
-
-def extract_evars(model, cn):
-    """
-    Extract a list of the names of the explanatory variables in a statsmodels model
-    """
-    pattern = r"\b\w+\b"
-    evars = re.findall(pattern, model.formula)[1:]
-    evars = [v for v in evars if v in cn]
-    return [v for i, v in enumerate(evars) if v not in evars[:i]]
-
-
-def extract_rvar(model, cn):
-    """
-    Extract name of the response variable in a statsmodels model
-    """
-    pattern = r"\b\w+\b"
-    return re.findall(pattern, model.formula)[0]
+    # plt.show()
 
 
 def pred_plot_sm(
     fitted,
     df,
     incl=None,
     excl=[],
```

### Comparing `pyrsm-0.7.9.2/pyrsm.egg-info/PKG-INFO` & `pyrsm-0.8.0/pyrsm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.7.9.2
+Version: 0.8.0
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.7.9.2/pyrsm.egg-info/SOURCES.txt` & `pyrsm-0.8.0/pyrsm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 pyproject.toml
 setup.cfg
 pyrsm/__init__.py
 pyrsm/basics.py
 pyrsm/bins.py
 pyrsm/example_data.py
 pyrsm/logit.py
+pyrsm/model.py
 pyrsm/notebook.py
 pyrsm/perf.py
 pyrsm/props.py
-pyrsm/regression.py
+pyrsm/regress.py
 pyrsm/stats.py
 pyrsm/utils.py
 pyrsm/visualize.py
 pyrsm.egg-info/PKG-INFO
 pyrsm.egg-info/SOURCES.txt
 pyrsm.egg-info/dependency_links.txt
 pyrsm.egg-info/requires.txt
```

### Comparing `pyrsm-0.7.9.2/setup.cfg` & `pyrsm-0.8.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 	pandas>=0.25.2
 	seaborn>=0.9.0
 	matplotlib>=3.1.1
 	statsmodels>=0.10.1
 	scipy>=1.4.1
 	scikit-learn>=1.0.2
 	IPython>=8.0.1
+	shiny>=0.3.3
 
 [options.packages.find]
 exclude = 
 	*.tests
 	*.tests.*
 	tests.*
 	tests
```

### Comparing `pyrsm-0.7.9.2/tests/test_basics.py` & `pyrsm-0.8.0/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/tests/test_bins.py` & `pyrsm-0.8.0/tests/test_bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/tests/test_example_data.py` & `pyrsm-0.8.0/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/tests/test_perf.py` & `pyrsm-0.8.0/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/tests/test_regression.py` & `pyrsm-0.8.0/tests/test_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import numpy as np
-from pyrsm.regression import sim_prediction
-from pyrsm.regression import reg_dashboard
+from pyrsm.regress import sim_prediction
+from pyrsm.regress import reg_dashboard
 
 np.random.seed(1234)
 nr = 100
 df = pd.DataFrame()
 df["x1"] = np.random.uniform(0, 1, nr)
 df["x2"] = 1 - df["x1"]
 df["x3"] = np.random.choice(["a", "b", "c"], nr)
```

### Comparing `pyrsm-0.7.9.2/tests/test_stats.py` & `pyrsm-0.8.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.2/tests/test_utils.py` & `pyrsm-0.8.0/tests/test_utils.py`

 * *Files identical despite different names*

