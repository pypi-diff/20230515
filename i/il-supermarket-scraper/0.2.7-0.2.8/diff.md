# Comparing `tmp/il-supermarket-scraper-0.2.7.tar.gz` & `tmp/il-supermarket-scraper-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "il-supermarket-scraper-0.2.7.tar", last modified: Tue Jan 31 15:41:14 2023, max compression
+gzip compressed data, was "il-supermarket-scraper-0.2.8.tar", last modified: Sun Feb 12 18:07:12 2023, max compression
```

## Comparing `il-supermarket-scraper-0.2.7.tar` & `il-supermarket-scraper-0.2.8.tar`

### file list

```diff
@@ -1,68 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 15:41:14.634515 il-supermarket-scraper-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-01-31 15:41:14.634515 il-supermarket-scraper-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 15:41:14.626515 il-supermarket-scraper-0.2.7/il_supermarket_scarper/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 15:41:14.630515 il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/apsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/bina.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/cerberus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/multipage_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/publishprice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrapper_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 15:41:14.634515 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/bareket.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/bitan.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/cofix.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/doralon.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/good_pharm.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/hazihinam.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/keshet.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/king_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/maayan2000.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/machsani_ashuk.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/mega.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/mega_market.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/nativ_hashed.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/osherad.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/polizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/ramilevy.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/salachdabach.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/shefa_barcart_ashem.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/shufersal.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/shuk_ahir.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/stop_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/super_pharm.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/super_yuda.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/superdosh.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/tivtaam.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/victory.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/yellow.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/yohananof.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/zolvebegadol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 15:41:14.634515 il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/file_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/gzip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/retrey.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 15:41:14.634515 il-supermarket-scraper-0.2.7/il_supermarket_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-01-31 15:41:14.000000 il-supermarket-scraper-0.2.7/il_supermarket_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-01-31 15:41:14.000000 il-supermarket-scraper-0.2.7/il_supermarket_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 15:41:14.000000 il-supermarket-scraper-0.2.7/il_supermarket_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-31 15:41:14.000000 il-supermarket-scraper-0.2.7/il_supermarket_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-31 15:41:14.000000 il-supermarket-scraper-0.2.7/il_supermarket_scraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-31 15:41:14.634515 il-supermarket-scraper-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-01-31 15:41:03.000000 il-supermarket-scraper-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 18:07:12.290393 il-supermarket-scraper-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-02-12 18:07:12.290393 il-supermarket-scraper-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 18:07:12.278392 il-supermarket-scraper-0.2.8/il_supermarket_scarper/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 18:07:12.278392 il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/apsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/bina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/cerberus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/multipage_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/publishprice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrapper_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 18:07:12.286393 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/bareket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/bitan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/cofix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/doralon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/good_pharm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/hazihinam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/keshet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/king_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/maayan2000.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/machsani_ashuk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/mega.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/mega_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/nativ_hashed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/osherad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/polizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/ramilevy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/salachdabach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/shefa_barcart_ashem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/shufersal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/shuk_ahir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/stop_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/super_pharm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/super_yuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/superdosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/tivtaam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/victory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/yellow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/yohananof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/zolvebegadol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 18:07:12.286393 il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/gzip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/retrey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 18:07:12.290393 il-supermarket-scraper-0.2.8/il_supermarket_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-02-12 18:07:12.000000 il-supermarket-scraper-0.2.8/il_supermarket_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-02-12 18:07:12.000000 il-supermarket-scraper-0.2.8/il_supermarket_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 18:07:12.000000 il-supermarket-scraper-0.2.8/il_supermarket_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-12 18:07:12.000000 il-supermarket-scraper-0.2.8/il_supermarket_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-12 18:07:12.000000 il-supermarket-scraper-0.2.8/il_supermarket_scraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-12 18:07:12.290393 il-supermarket-scraper-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 18:07:12.290393 il-supermarket-scraper-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-02-12 18:06:53.000000 il-supermarket-scraper-0.2.8/tests/test_main.py
```

### Comparing `il-supermarket-scraper-0.2.7/LICENSE.txt` & `il-supermarket-scraper-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/PKG-INFO` & `il-supermarket-scraper-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: il-supermarket-scraper
-Version: 0.2.7
+Version: 0.2.8
 Summary: python package that implement a scraping for israeli supermarket data
 Home-page: https://github.com/jladan/package_demo
 Author: Sefi Erlich
 Author-email: erlichsefi@gmail.com
 License: MIT
 Keywords: israel,israeli,scraper,supermarket
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `il-supermarket-scraper-0.2.7/README.md` & `il-supermarket-scraper-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/apsx.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/apsx.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/bina.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/bina.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/cerberus.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/cerberus.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/engine.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,31 +33,57 @@
             self.storage_path = get_output_folder(self.chain)
         Logger.info(f"Storage path: {self.storage_path}")
 
     def get_storage_path(self):
         """the the storage page of the files downloaded"""
         return self.storage_path
 
-    def is_validate_scraper_found_no_files(self, limit=None, files_types=None):
+    def _is_validate_scraper_found_no_files(
+        self, limit=None, files_types=None, store_id=None, only_latest=False
+    ):
+        Logger.info(
+            f"check if fail is allowd with, limit={limit},"
+            f"files_types={files_types},store_id={store_id},only_latest={only_latest}"
+        )
+        return False
+
+    def is_validate_scraper_found_no_files(
+        self, limit=None, files_types=None, store_id=None, only_latest=False
+    ):
         """return true if its ok the scarper reuturn no enrty"""
 
         # if all the files requested are the update files, is ok the scaraper failed.
         request_only_update_file = False
         if files_types:
             request_only_update_file = True
             for file_type in files_types:
                 if file_type in FileTypesFilters.all_full_files():
                     request_only_update_file = False
-
-        return limit == 0 or files_types == [] or request_only_update_file
+        Logger.info(f"the value of {only_latest} should not affect.")
+        return (
+            limit == 0
+            or files_types == []
+            or request_only_update_file
+            or (store_id and store_id < 0)
+            or self._is_validate_scraper_found_no_files(
+                limit=limit,
+                files_types=files_types,
+                store_id=store_id,
+                only_latest=only_latest,
+            )
+        )
 
     def is_valid_file_empty(self, file_name):
         """it is valid the file is empty"""
         return file_name is None
 
+    def get_store_name_format(self, store_id):
+        """get the expected format of the store in the file name"""
+        return f"-{store_id:03d}-"
+
     def apply_limit(
         self,
         intreable,
         limit=None,
         files_types=None,
         by_function=lambda x: x,
         store_id=None,
@@ -78,21 +104,24 @@
 
         # filter unique links
         intreable_ = self.unique(intreable_, by_function=by_function)
 
         # filter by store id
         if store_id:
             intreable_ = list(
-                filter(lambda x: f"{store_id:03d}-" in by_function(x), intreable_)
+                filter(
+                    lambda x: self.get_store_name_format(store_id) in by_function(x),
+                    intreable_,
+                )
             )
 
         # filter by file type
         if files_types:
             intreable_ = self.filter_file_types(
-                intreable, limit, files_types, by_function
+                intreable_, limit, files_types, by_function
             )
         if only_latest:
             intreable_ = self.get_only_latest(by_function, intreable_)
 
         # filter by limit if the 'files_types' filter is not on.
         if limit and files_types is None:
             assert limit > 0, "Limit must be greater than 0"
@@ -101,18 +130,24 @@
         Logger.info(f"Result length {len(list(intreable_))}")
 
         # raise error if there was nothing to download.
         if len(list(intreable_)) == 0:
             if not (
                 files_was_filtered_since_already_download
                 or self.is_validate_scraper_found_no_files(
-                    limit=limit, files_types=files_types
+                    limit=limit,
+                    files_types=files_types,
+                    store_id=store_id,
+                    only_latest=only_latest,
                 )
             ):
-                raise ValueError(f"No files to download for file {files_types}")
+                raise ValueError(
+                    f"No files to download for file files_types={files_types},"
+                    f"limit={limit},store_id={store_id},only_latest={only_latest}"
+                )
         return intreable_
 
     def filter_file_types(self, intreable, limit, files_types, by_function):
         """filter the file types requested"""
         intreable_ = []
         for type_ in files_types:
             type_files = FileTypesFilters.filter(
```

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/matrix.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/matrix.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/multipage_web.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/multipage_web.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/publishprice.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/publishprice.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,7 +40,10 @@
         )
 
         download_urls: list = list(
             map(lambda x: self.url + self.folder + x.a.attrs["href"], all_trs)
         )
         file_names: list = list(map(lambda x: x.a.attrs["href"].split(".")[0], all_trs))
         return download_urls, file_names
+
+    def get_store_name_format(self, store_id):
+        return f"-{store_id:04d}-"
```

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/engines/web.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/engines/web.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/main.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/main.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrapper_runner.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrapper_runner.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/__init__.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/cofix.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/cofix.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/nativ_hashed.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/nativ_hashed.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,13 +9,12 @@
         super().__init__(
             "Netiv Hasef",
             chain_id="7290058160839",
             url="http://141.226.222.202/",
             folder_name=folder_name,
         )
 
-    def is_validate_scraper_found_no_files(self, limit=None, files_types=None):
+    def _is_validate_scraper_found_no_files(
+        self, limit=None, files_types=None, store_id=None, only_latest=False
+    ):
         # no data on shabat
-        result = super().is_validate_scraper_found_no_files(
-            limit=limit, files_types=files_types
-        )
-        return result or _is_saturday_in_israel() or _is_holiday_in_israel()
+        return _is_saturday_in_israel() or _is_holiday_in_israel()
```

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/polizer.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/polizer.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,18 +9,16 @@
         super().__init__(
             "Polizer",
             chain_id="7291059100008",
             folder_name=folder_name,
             ftp_username="politzer",
         )
 
-    def is_validate_scraper_found_no_files(self, limit=None, files_types=None):
+    def _is_validate_scraper_found_no_files(
+        self, limit=None, files_types=None, store_id=None, only_latest=False
+    ):
         # no data on shabat
-        result = super().is_validate_scraper_found_no_files(
-            limit=limit, files_types=files_types
-        )
-
-        return result or (
+        return (
             files_types is not None
             and len(files_types) == 1
             and files_types[0] == FileTypesFilters.STORE_FILE.name
         )
```

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers/super_pharm.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers/super_pharm.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/scrappers_factory.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/scrappers_factory.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/__init__.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/connection.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,17 @@
 def url_retrieve(url, filename, timeout=30):
     # from urllib.request import urlretrieve
     # urlretrieve(url, filename)
     # >>> add here timeout if needed
     """alternative to urllib.request.urlretrieve"""
     # https://gist.github.com/xflr6/f29ed682f23fd27b6a0b1241f244e6c9
     with contextlib.closing(
-        requests.get(url, stream=True, timeout=timeout)
+        requests.get(
+            url, stream=True, timeout=timeout, headers={"Accept-Encoding": None}
+        )
     ) as _request:
         _request.raise_for_status()
         size = int(_request.headers.get("Content-Length", "-1"))
         read = 0
         with open(filename, "wb") as file:
             for chunk in _request.iter_content(chunk_size=None):
                 time.sleep(0.5)
```

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/file_types.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/file_types.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/gzip_utils.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/gzip_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 def extract_xml_file_from_gz_file(file_save_path):
     """extract xml from gz"""
     try:
         with gzip.open(file_save_path, "rb") as infile:
             with open(os.path.splitext(file_save_path)[0] + ".xml", "wb") as outfile:
                 shutil.copyfileobj(infile, outfile)
     except gzip.BadGzipFile:
-
         try:
             with open(file_save_path, "rb") as response_content:
                 with zipfile.ZipFile(io.BytesIO(response_content.read())) as the_zip:
                     zip_info = the_zip.infolist()[0]
                     with the_zip.open(zip_info) as the_file:
                         with open(
                             os.path.splitext(file_save_path)[0] + ".xml", "wb"
```

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/logger.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/loop.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/loop.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/mongo.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/mongo.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/retrey.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/retrey.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scarper/utils/status.py` & `il-supermarket-scraper-0.2.8/il_supermarket_scarper/utils/status.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 import datetime
 import re
 import os
 import enum
-import requests
 import holidays
 import pytz
 import lxml.html as lh
 from bs4 import BeautifulSoup
 
 from .logger import Logger
+from .connection import session_with_cookies
 
 
-def get_status():
-    """get the number of scarper listed on the gov.il site"""
+def get_statue_page():
+    """fetch the gov.il site"""
     url = "https://www.gov.il/he/departments/legalInfo/cpfta_prices_regulations"
     # Create a handle, page, to handle the contents of the website
-    page = requests.get(url, timeout=10)
+    return session_with_cookies(url, chain_cookie_name="gov_il")
+
+
+def get_status():
+    """get the number of scarper listed on the gov.il site"""
+    page = get_statue_page()
     # Store the contents of the website under doc
     doc = BeautifulSoup(page.content, features="lxml")
     # Parse data that are stored between <tr>..</tr> of HTML
     count = 0
     for element in doc.find_all("strong"):
         if "לצפייה במחירים" in str(element):
             count += 1
 
     return count
 
 
 def get_status_date():
     """get the date change listed on the gov.il site"""
-    url = "https://www.gov.il/he/departments/legalInfo/cpfta_prices_regulations"
-    # Create a handle, page, to handle the contents of the website\
-    page = requests.get(url, timeout=10)
+    page = get_statue_page()
 
     if page.status_code != 200:
         Logger.error(f"request as failed, page body is {page}.")
-        raise ValueError(f"Failed reading site {url}.")
+        raise ValueError("Failed reading the gov.il site.")
     line_with_date = (
         lh.fromstring(page.content)
         .xpath(
             r"""/html/body/section/div/
                                                         div[3]/div/span"""
         )[0]
         .text
```

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scraper.egg-info/PKG-INFO` & `il-supermarket-scraper-0.2.8/il_supermarket_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: il-supermarket-scraper
-Version: 0.2.7
+Version: 0.2.8
 Summary: python package that implement a scraping for israeli supermarket data
 Home-page: https://github.com/jladan/package_demo
 Author: Sefi Erlich
 Author-email: erlichsefi@gmail.com
 License: MIT
 Keywords: israel,israeli,scraper,supermarket
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `il-supermarket-scraper-0.2.7/il_supermarket_scraper.egg-info/SOURCES.txt` & `il-supermarket-scraper-0.2.8/il_supermarket_scraper.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -54,8 +54,10 @@
 il_supermarket_scarper/utils/mongo.py
 il_supermarket_scarper/utils/retrey.py
 il_supermarket_scarper/utils/status.py
 il_supermarket_scraper.egg-info/PKG-INFO
 il_supermarket_scraper.egg-info/SOURCES.txt
 il_supermarket_scraper.egg-info/dependency_links.txt
 il_supermarket_scraper.egg-info/requires.txt
-il_supermarket_scraper.egg-info/top_level.txt
+il_supermarket_scraper.egg-info/top_level.txt
+tests/test_integration.py
+tests/test_main.py
```

### Comparing `il-supermarket-scraper-0.2.7/setup.py` & `il-supermarket-scraper-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         "pytz==2022.4",
         "holidays==0.16",
         "cachetools==5.2.0",
     ],
     tests_require=["pytest==7.1"],
     extras_require={"test": ["pytest"]},
     # *strongly* suggested for sharing
-    version="0.2.7",
+    version="0.2.8",
     # The license can be anything you like
     license="MIT",
     description="python package that implement a scraping for israeli supermarket data",
     # We will also need a readme eventually (there will be a warning)
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["israel", "israeli", "scraper", "supermarket"],
```

