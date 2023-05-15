# Comparing `tmp/plerr-2.1.0.tar.gz` & `tmp/plerr-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plerr-2.1.0.tar", last modified: Wed Jun 29 08:10:39 2022, max compression
+gzip compressed data, was "plerr-3.0.0.tar", last modified: Wed Jun 29 08:24:37 2022, max compression
```

## Comparing `plerr-2.1.0.tar` & `plerr-3.0.0.tar`

### file list

```diff
@@ -1,333 +1,333 @@
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.503733 plerr-2.1.0/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1075 2022-06-29 07:29:53.000000 plerr-2.1.0/LICENSE
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      130 2022-06-29 07:29:53.000000 plerr-2.1.0/MANIFEST.in
--rw-rw-r--   0 laptop    (1000) laptop    (1000)    37861 2022-06-29 08:10:39.503733 plerr-2.1.0/PKG-INFO
--rw-rw-r--   0 laptop    (1000) laptop    (1000)    36641 2022-06-29 07:29:53.000000 plerr-2.1.0/README.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.483733 plerr-2.1.0/plerr/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)       22 2022-06-29 07:50:42.000000 plerr-2.1.0/plerr/__init__.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)       86 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/__main__.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1176 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/cli.py
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.483733 plerr-2.1.0/plerr/errors/
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.483733 plerr-2.1.0/plerr/errors/async/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      715 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/async/E1700.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1028 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/async/E1701.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.487733 plerr-2.1.0/plerr/errors/basic/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      491 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/C0102.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      486 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/C0103.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      521 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/C0112.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      473 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/C0114.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      443 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/C0115.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      762 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/C0116.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      530 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/C0121.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      628 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/C0122.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      749 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/C0123.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      719 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0100.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      840 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0101.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      535 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0102.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      617 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0103.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      603 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0104.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      577 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0105.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      499 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0106.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      643 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0107.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      515 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0108.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      869 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0110.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      629 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0111.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      601 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0112.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      576 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0113.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      569 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0114.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      751 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0115.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      639 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0116.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      707 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0117.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      746 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0118.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      657 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/E0119.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      619 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/R0123.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      500 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/R0124.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      574 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0101.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      642 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0102.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      490 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0104.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      765 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0105.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      583 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0106.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      518 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0107.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      648 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0108.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      529 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0109.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      389 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0111.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      671 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0120.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      758 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0122.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      674 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0123.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      818 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0124.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      401 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0125.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      477 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0126.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      382 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0127.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      396 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0128.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      593 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0143.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      753 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0150.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      446 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/basic/W0199.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.487733 plerr-2.1.0/plerr/errors/broad-try-clause/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      359 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/broad-try-clause/W0717.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.491733 plerr-2.1.0/plerr/errors/classes/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      691 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/C0202.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      867 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/C0203.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      919 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/C0204.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      660 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/C0205.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      722 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/E0202.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      680 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/E0203.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      476 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/E0211.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      543 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/E0213.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      639 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/E0236.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      698 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/E0237.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      554 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/E0238.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      414 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/E0239.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      494 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/E0240.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      419 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/E0241.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      430 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/E0242.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      851 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/E0301.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      779 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/E0302.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      485 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/E0303.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      464 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/F0202.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      556 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/R0201.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      515 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/R0202.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      498 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/R0203.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      566 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/R0205.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      550 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/R0206.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      541 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/W0201.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      577 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/W0211.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      629 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/W0212.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      728 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/W0221.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      408 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/W0222.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      576 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/W0223.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      661 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/W0231.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      450 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/W0232.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      975 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/W0233.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      717 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/W0235.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      638 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/classes/W0236.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.491733 plerr-2.1.0/plerr/errors/compare-to-empty-string/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      406 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/compare-to-empty-string/C1901.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.491733 plerr-2.1.0/plerr/errors/compare-to-zero/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      388 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/compare-to-zero/C2001.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.491733 plerr-2.1.0/plerr/errors/deprecated-builtins/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      553 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/deprecated-builtins/W0141.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.491733 plerr-2.1.0/plerr/errors/design/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      680 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/design/R0901.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      929 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/design/R0902.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      590 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/design/R0903.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      757 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/design/R0904.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1014 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/design/R0911.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1510 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/design/R0912.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      408 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/design/R0913.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      463 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/design/R0914.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      514 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/design/R0915.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      648 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/design/R0916.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1047 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/design/R1260.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.491733 plerr-2.1.0/plerr/errors/docstyle/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      404 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/docstyle/C0198.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      941 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/docstyle/C0199.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.491733 plerr-2.1.0/plerr/errors/else-if-used/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      564 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/else-if-used/R5501.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.491733 plerr-2.1.0/plerr/errors/exceptions/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      773 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/exceptions/E0701.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      602 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/exceptions/E0702.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      657 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/exceptions/E0703.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      794 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/exceptions/E0704.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      460 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/exceptions/E0710.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      478 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/exceptions/E0711.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      535 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/exceptions/E0712.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      415 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/exceptions/W0702.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      446 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/exceptions/W0703.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      491 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/exceptions/W0705.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      581 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/exceptions/W0706.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      550 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/exceptions/W0711.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      570 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/exceptions/W0715.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      605 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/exceptions/W0716.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.491733 plerr-2.1.0/plerr/errors/format/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      468 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/format/C0301.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      364 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/format/C0302.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      512 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/format/C0303.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      468 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/format/C0304.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      357 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/format/C0305.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      396 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/format/C0321.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      451 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/format/C0325.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      390 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/format/C0326.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      372 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/format/C0327.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      381 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/format/C0328.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      322 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/format/C0330.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      417 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/format/W0301.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      415 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/format/W0311.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      365 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/format/W0312.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.495733 plerr-2.1.0/plerr/errors/imports/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      462 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/C0410.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      630 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/C0411.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      471 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/C0412.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      403 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/C0413.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      496 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/C0414.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      437 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/C0415.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      461 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/E0401.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      516 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/E0402.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      569 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/R0401.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      460 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/W0401.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      353 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/W0402.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      341 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/W0404.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      411 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/W0406.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      301 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/W0407.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      523 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/imports/W0410.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.495733 plerr-2.1.0/plerr/errors/logging/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      411 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/logging/E1200.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      486 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/logging/E1201.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      376 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/logging/E1205.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      373 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/logging/E1206.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      991 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/logging/W1201.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      913 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/logging/W1202.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.495733 plerr-2.1.0/plerr/errors/miscellaneous/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      377 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/miscellaneous/I0023.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      367 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/miscellaneous/W0511.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.495733 plerr-2.1.0/plerr/errors/multiple-types/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      389 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/multiple-types/R0204.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.495733 plerr-2.1.0/plerr/errors/newstyle/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      556 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/newstyle/E1003.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.495733 plerr-2.1.0/plerr/errors/overlap-except/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      365 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/overlap-except/W0714.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.495733 plerr-2.1.0/plerr/errors/parameter-documentation/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      676 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/parameter-documentation/W9005.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      926 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/parameter-documentation/W9006.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      375 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/parameter-documentation/W9008.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      368 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/parameter-documentation/W9010.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      519 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/parameter-documentation/W9011.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      530 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/parameter-documentation/W9012.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      364 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/parameter-documentation/W9013.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      364 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/parameter-documentation/W9014.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      621 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/parameter-documentation/W9015.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      647 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/parameter-documentation/W9016.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      644 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/parameter-documentation/W9017.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      647 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/parameter-documentation/W9018.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.495733 plerr-2.1.0/plerr/errors/refactoring/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      382 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/C0113.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      569 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/C0200.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      595 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/C0201.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      632 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/C1801.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      399 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1701.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      511 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1702.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      510 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1703.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      727 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1704.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      938 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1705.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      377 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1706.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      599 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1707.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      672 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1708.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      387 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1709.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      867 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1710.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      512 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1711.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      531 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1712.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      527 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1713.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      661 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1714.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      490 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1715.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      571 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1716.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      637 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1717.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      535 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1718.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      503 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1719.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      752 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1720.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      587 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1721.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      586 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1722.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      730 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1723.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      748 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/refactoring/R1724.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.495733 plerr-2.1.0/plerr/errors/similarities/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      457 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/similarities/R0801.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.495733 plerr-2.1.0/plerr/errors/spelling/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      375 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/spelling/C0401.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      381 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/spelling/C0402.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      393 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/spelling/C0403.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.499733 plerr-2.1.0/plerr/errors/stdlib/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      468 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/stdlib/E1507.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      651 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/stdlib/W1501.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      559 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/stdlib/W1502.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      839 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/stdlib/W1503.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      449 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/stdlib/W1505.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      747 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/stdlib/W1506.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      532 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/stdlib/W1507.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      566 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/stdlib/W1508.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      970 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/stdlib/W1509.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      702 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/stdlib/W1510.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.499733 plerr-2.1.0/plerr/errors/string/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      424 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/E1300.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      396 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/E1301.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      580 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/E1302.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      423 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/E1303.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      537 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/E1304.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      478 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/E1305.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      433 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/E1306.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      451 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/E1307.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      397 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/E1310.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      435 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/W1300.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      463 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/W1301.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      405 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/W1302.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      496 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/W1303.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      631 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/W1304.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      560 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/W1305.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      493 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/W1306.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      513 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/W1307.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      430 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/W1308.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      396 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/W1401.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      457 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/W1402.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      436 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/string/W1403.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.499733 plerr-2.1.0/plerr/errors/typecheck/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      361 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1101.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      389 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1102.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      525 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1111.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      423 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1120.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      446 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1121.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      556 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1123.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      562 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1124.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      370 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1125.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      595 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1126.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      451 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1127.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      481 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1128.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      596 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1129.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      441 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1130.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      409 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1131.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      367 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1132.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      819 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1133.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      371 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1134.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      739 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1135.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      721 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1136.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      870 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1137.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      717 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1138.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      434 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1139.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      481 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1140.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      568 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/E1141.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      518 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/I1101.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      638 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/W1113.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      446 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/typecheck/W1114.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.503733 plerr-2.1.0/plerr/errors/variables/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      480 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/E0601.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      451 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/E0602.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      644 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/E0603.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      528 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/E0604.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      780 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/E0611.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      675 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/E0633.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      692 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0601.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      599 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0602.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      597 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0603.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      494 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0604.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      601 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0611.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      369 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0612.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      394 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0613.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      458 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0614.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      485 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0621.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      387 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0622.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      383 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0623.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      652 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0631.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      417 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0632.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      699 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0640.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      487 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0641.md
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      385 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/errors/variables/W0642.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.503733 plerr-2.1.0/plerr/tests/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)        0 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/tests/__init__.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1486 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/tests/command_output_fixture.txt
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     2649 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/tests/test_cli_module.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     2385 2022-06-29 07:29:53.000000 plerr-2.1.0/plerr/tests/test_package.py
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:10:39.483733 plerr-2.1.0/plerr.egg-info/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)    37861 2022-06-29 08:10:39.000000 plerr-2.1.0/plerr.egg-info/PKG-INFO
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     9246 2022-06-29 08:10:39.000000 plerr-2.1.0/plerr.egg-info/SOURCES.txt
--rw-rw-r--   0 laptop    (1000) laptop    (1000)        1 2022-06-29 08:10:39.000000 plerr-2.1.0/plerr.egg-info/dependency_links.txt
--rw-rw-r--   0 laptop    (1000) laptop    (1000)       42 2022-06-29 08:10:39.000000 plerr-2.1.0/plerr.egg-info/entry_points.txt
--rw-rw-r--   0 laptop    (1000) laptop    (1000)       17 2022-06-29 08:10:39.000000 plerr-2.1.0/plerr.egg-info/requires.txt
--rw-rw-r--   0 laptop    (1000) laptop    (1000)        6 2022-06-29 08:10:39.000000 plerr-2.1.0/plerr.egg-info/top_level.txt
--rw-rw-r--   0 laptop    (1000) laptop    (1000)       38 2022-06-29 08:10:39.503733 plerr-2.1.0/setup.cfg
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1837 2022-06-29 07:48:33.000000 plerr-2.1.0/setup.py
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.053338 plerr-3.0.0/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)     1075 2022-06-29 07:29:53.000000 plerr-3.0.0/LICENSE
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      130 2022-06-29 07:29:53.000000 plerr-3.0.0/MANIFEST.in
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)    37957 2022-06-29 08:24:37.053338 plerr-3.0.0/PKG-INFO
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)    36787 2022-06-29 08:13:11.000000 plerr-3.0.0/README.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.033337 plerr-3.0.0/plerr/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)       22 2022-06-29 08:17:15.000000 plerr-3.0.0/plerr/__init__.py
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)       86 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/__main__.py
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)     1176 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/cli.py
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.033337 plerr-3.0.0/plerr/errors/
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.033337 plerr-3.0.0/plerr/errors/async/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      715 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/async/E1700.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)     1028 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/async/E1701.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.037338 plerr-3.0.0/plerr/errors/basic/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      491 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/C0102.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      486 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/C0103.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      521 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/C0112.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      473 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/C0114.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      443 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/C0115.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      762 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/C0116.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      530 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/C0121.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      628 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/C0122.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      749 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/C0123.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      719 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0100.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      840 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0101.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      535 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0102.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      617 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0103.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      603 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0104.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      577 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0105.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      499 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0106.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      643 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0107.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      515 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0108.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      869 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0110.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      629 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0111.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      601 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0112.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      576 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0113.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      569 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0114.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      751 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0115.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      639 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0116.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      707 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0117.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      746 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0118.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      657 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/E0119.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      619 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/R0123.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      500 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/R0124.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      574 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0101.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      642 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0102.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      490 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0104.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      765 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0105.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      583 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0106.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      518 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0107.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      648 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0108.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      529 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0109.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      389 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0111.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      671 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0120.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      758 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0122.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      674 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0123.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      818 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0124.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      401 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0125.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      477 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0126.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      382 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0127.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      396 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0128.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      593 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0143.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      753 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0150.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      446 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/basic/W0199.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.037338 plerr-3.0.0/plerr/errors/broad-try-clause/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      359 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/broad-try-clause/W0717.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.041338 plerr-3.0.0/plerr/errors/classes/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      691 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/C0202.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      867 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/C0203.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      919 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/C0204.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      660 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/C0205.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      722 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/E0202.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      680 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/E0203.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      476 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/E0211.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      543 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/E0213.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      639 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/E0236.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      698 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/E0237.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      554 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/E0238.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      414 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/E0239.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      494 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/E0240.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      419 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/E0241.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      430 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/E0242.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      851 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/E0301.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      779 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/E0302.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      485 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/E0303.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      464 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/F0202.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      556 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/R0201.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      515 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/R0202.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      498 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/R0203.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      566 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/R0205.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      550 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/R0206.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      541 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/W0201.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      577 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/W0211.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      629 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/W0212.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      728 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/W0221.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      408 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/W0222.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      576 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/W0223.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      661 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/W0231.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      450 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/W0232.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      975 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/W0233.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      717 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/W0235.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      638 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/classes/W0236.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.041338 plerr-3.0.0/plerr/errors/compare-to-empty-string/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      406 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/compare-to-empty-string/C1901.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.041338 plerr-3.0.0/plerr/errors/compare-to-zero/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      388 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/compare-to-zero/C2001.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.041338 plerr-3.0.0/plerr/errors/deprecated-builtins/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      553 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/deprecated-builtins/W0141.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.041338 plerr-3.0.0/plerr/errors/design/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      680 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/design/R0901.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      929 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/design/R0902.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      590 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/design/R0903.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      757 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/design/R0904.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)     1014 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/design/R0911.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)     1510 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/design/R0912.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      408 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/design/R0913.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      463 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/design/R0914.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      514 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/design/R0915.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      648 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/design/R0916.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)     1047 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/design/R1260.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.041338 plerr-3.0.0/plerr/errors/docstyle/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      404 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/docstyle/C0198.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      941 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/docstyle/C0199.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.041338 plerr-3.0.0/plerr/errors/else-if-used/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      564 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/else-if-used/R5501.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.041338 plerr-3.0.0/plerr/errors/exceptions/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      773 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/exceptions/E0701.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      602 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/exceptions/E0702.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      657 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/exceptions/E0703.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      794 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/exceptions/E0704.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      460 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/exceptions/E0710.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      478 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/exceptions/E0711.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      535 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/exceptions/E0712.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      415 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/exceptions/W0702.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      446 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/exceptions/W0703.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      491 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/exceptions/W0705.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      581 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/exceptions/W0706.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      550 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/exceptions/W0711.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      570 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/exceptions/W0715.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      605 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/exceptions/W0716.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.045338 plerr-3.0.0/plerr/errors/format/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      468 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/format/C0301.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      364 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/format/C0302.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      512 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/format/C0303.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      468 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/format/C0304.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      357 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/format/C0305.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      396 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/format/C0321.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      451 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/format/C0325.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      390 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/format/C0326.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      372 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/format/C0327.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      381 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/format/C0328.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      322 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/format/C0330.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      417 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/format/W0301.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      415 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/format/W0311.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      365 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/format/W0312.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.045338 plerr-3.0.0/plerr/errors/imports/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      462 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/C0410.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      630 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/C0411.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      471 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/C0412.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      403 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/C0413.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      496 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/C0414.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      437 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/C0415.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      461 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/E0401.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      516 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/E0402.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      569 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/R0401.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      460 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/W0401.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      353 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/W0402.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      341 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/W0404.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      411 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/W0406.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      301 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/W0407.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      523 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/imports/W0410.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.045338 plerr-3.0.0/plerr/errors/logging/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      411 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/logging/E1200.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      486 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/logging/E1201.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      376 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/logging/E1205.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      373 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/logging/E1206.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      991 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/logging/W1201.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      913 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/logging/W1202.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.045338 plerr-3.0.0/plerr/errors/miscellaneous/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      377 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/miscellaneous/I0023.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      367 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/miscellaneous/W0511.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.045338 plerr-3.0.0/plerr/errors/multiple-types/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      389 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/multiple-types/R0204.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.045338 plerr-3.0.0/plerr/errors/newstyle/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      556 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/newstyle/E1003.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.045338 plerr-3.0.0/plerr/errors/overlap-except/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      365 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/overlap-except/W0714.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.045338 plerr-3.0.0/plerr/errors/parameter-documentation/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      676 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/parameter-documentation/W9005.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      926 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/parameter-documentation/W9006.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      375 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/parameter-documentation/W9008.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      368 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/parameter-documentation/W9010.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      519 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/parameter-documentation/W9011.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      530 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/parameter-documentation/W9012.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      364 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/parameter-documentation/W9013.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      364 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/parameter-documentation/W9014.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      621 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/parameter-documentation/W9015.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      647 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/parameter-documentation/W9016.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      644 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/parameter-documentation/W9017.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      647 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/parameter-documentation/W9018.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.049337 plerr-3.0.0/plerr/errors/refactoring/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      382 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/C0113.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      569 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/C0200.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      595 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/C0201.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      632 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/C1801.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      399 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1701.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      511 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1702.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      510 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1703.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      727 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1704.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      938 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1705.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      377 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1706.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      599 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1707.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      672 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1708.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      387 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1709.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      867 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1710.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      512 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1711.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      531 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1712.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      527 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1713.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      661 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1714.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      490 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1715.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      571 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1716.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      637 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1717.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      535 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1718.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      503 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1719.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      752 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1720.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      587 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1721.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      586 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1722.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      730 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1723.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      748 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/refactoring/R1724.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.049337 plerr-3.0.0/plerr/errors/similarities/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      457 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/similarities/R0801.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.049337 plerr-3.0.0/plerr/errors/spelling/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      375 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/spelling/C0401.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      381 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/spelling/C0402.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      393 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/spelling/C0403.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.049337 plerr-3.0.0/plerr/errors/stdlib/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      468 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/stdlib/E1507.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      651 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/stdlib/W1501.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      559 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/stdlib/W1502.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      839 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/stdlib/W1503.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      449 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/stdlib/W1505.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      747 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/stdlib/W1506.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      532 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/stdlib/W1507.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      566 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/stdlib/W1508.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      970 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/stdlib/W1509.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      702 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/stdlib/W1510.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.049337 plerr-3.0.0/plerr/errors/string/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      424 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/E1300.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      396 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/E1301.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      580 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/E1302.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      423 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/E1303.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      537 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/E1304.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      478 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/E1305.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      433 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/E1306.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      451 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/E1307.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      397 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/E1310.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      435 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/W1300.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      463 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/W1301.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      405 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/W1302.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      496 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/W1303.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      631 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/W1304.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      560 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/W1305.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      493 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/W1306.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      513 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/W1307.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      430 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/W1308.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      396 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/W1401.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      457 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/W1402.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      436 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/string/W1403.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.053338 plerr-3.0.0/plerr/errors/typecheck/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      361 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1101.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      389 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1102.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      525 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1111.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      423 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1120.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      446 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1121.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      556 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1123.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      562 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1124.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      370 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1125.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      595 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1126.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      451 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1127.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      481 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1128.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      596 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1129.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      441 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1130.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      409 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1131.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      367 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1132.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      819 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1133.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      371 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1134.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      739 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1135.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      721 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1136.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      870 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1137.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      717 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1138.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      434 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1139.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      481 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1140.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      568 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/E1141.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      518 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/I1101.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      638 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/W1113.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      446 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/typecheck/W1114.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.053338 plerr-3.0.0/plerr/errors/variables/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      480 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/E0601.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      451 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/E0602.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      644 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/E0603.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      528 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/E0604.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      780 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/E0611.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      675 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/E0633.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      692 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0601.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      599 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0602.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      597 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0603.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      494 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0604.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      601 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0611.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      369 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0612.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      394 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0613.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      458 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0614.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      485 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0621.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      387 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0622.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      383 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0623.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      652 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0631.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      417 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0632.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      699 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0640.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      487 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0641.md
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)      385 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/errors/variables/W0642.md
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.053338 plerr-3.0.0/plerr/tests/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)        0 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/tests/__init__.py
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)     1486 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/tests/command_output_fixture.txt
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)     2649 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/tests/test_cli_module.py
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)     2385 2022-06-29 07:29:53.000000 plerr-3.0.0/plerr/tests/test_package.py
+drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2022-06-29 08:24:37.033337 plerr-3.0.0/plerr.egg-info/
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)    37957 2022-06-29 08:24:37.000000 plerr-3.0.0/plerr.egg-info/PKG-INFO
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)     9246 2022-06-29 08:24:37.000000 plerr-3.0.0/plerr.egg-info/SOURCES.txt
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)        1 2022-06-29 08:24:37.000000 plerr-3.0.0/plerr.egg-info/dependency_links.txt
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)       42 2022-06-29 08:24:37.000000 plerr-3.0.0/plerr.egg-info/entry_points.txt
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)       17 2022-06-29 08:24:37.000000 plerr-3.0.0/plerr.egg-info/requires.txt
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)        6 2022-06-29 08:24:37.000000 plerr-3.0.0/plerr.egg-info/top_level.txt
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)       38 2022-06-29 08:24:37.053338 plerr-3.0.0/setup.cfg
+-rw-rw-r--   0 laptop    (1000) laptop    (1000)     1788 2022-06-29 08:16:11.000000 plerr-3.0.0/setup.py
```

### Comparing `plerr-2.1.0/LICENSE` & `plerr-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/PKG-INFO` & `plerr-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: plerr
-Version: 2.1.0
+Version: 3.0.0
 Summary: A list of pylint-errors with reasoning and examples of erroneous and correct code.
 Home-page: https://github.com/vald-phoenix/pylint-errors
 Author: Vladyslav Krylasov
 Author-email: vladyslav.krylasov@gmail.com
 License: UNKNOWN
 Keywords: pylint,errors,documentation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
   <br>
-  <a href="https://github.com/vald-phoenix/pylint-errors"><img src="media/logo.png" width="200px" height="auto" alt="plerr"></a>
+  <a href="https://github.com/vald-phoenix/pylint-errors">
+      <img src="https://raw.githubusercontent.com/vald-phoenix/pylint-errors/master/media/logo.png" width="200px" height="auto" alt="plerr">
+  </a>
   <br>
 </h1>
 
 <h4 align="center">A list of pylint-errors with reasoning and examples of erroneous and correct code.</h4>
 
 <p align="center">
   <a href="https://github.com/vald-phoenix/pylint-error">
@@ -55,15 +56,15 @@
       <img src="https://img.shields.io/pypi/v/plerr">
   </a>
   <a href="https://pypi.org/project/plerr/">
       <img src="https://img.shields.io/pypi/wheel/plerr">
   </a>
 </p>
 
-![Example](media/example.svg)
+![Example](https://raw.githubusercontent.com/vald-phoenix/pylint-errors/master/media/example.svg)
 
 ## Table of contents
 
 - [CLI usage](#cli-usage)
   - [Stable release](#stable-release)
   - [Dev builds](#dev-builds)
 - [List of errors](#list-of-errors)
```

#### html2text {}

```diff
@@ -1,160 +1,160 @@
-Metadata-Version: 2.1 Name: plerr Version: 2.1.0 Summary: A list of pylint-
+Metadata-Version: 2.1 Name: plerr Version: 3.0.0 Summary: A list of pylint-
 errors with reasoning and examples of erroneous and correct code. Home-page:
 https://github.com/vald-phoenix/pylint-errors Author: Vladyslav Krylasov
 Author-email: vladyslav.krylasov@gmail.com License: UNKNOWN Keywords:
 pylint,errors,documentation Platform: UNKNOWN Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Topic :: Software Development
-:: Documentation Classifier: Topic :: Software Development :: Libraries ::
-Python Modules Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE
+Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: Implementation :: CPython Classifier: Topic
+:: Software Development :: Documentation Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Software
+Development :: Quality Assurance Requires-Python: >=3.7 Description-Content-
+Type: text/markdown License-File: LICENSE
                                     ******
                                    [plerr]
                                      ******
    *** A list of pylint-errors with reasoning and examples of erroneous and
                                correct code. ***
  [https://img.shields.io/badge/made_in-ukraine-ffd700.svg?labelColor=0057b7]
 [https://img.shields.io/pypi/l/plerr] [https://github.com/vald-phoenix/pylint-
   errors/workflows/CI/badge.svg] [https://codecov.io/gh/vald-phoenix/pylint-
 errors/branch/master/graph/badge.svg] [https://img.shields.io/pypi/pyversions/
   plerr] [https://img.shields.io/pypi/v/plerr] [https://img.shields.io/pypi/
                                  wheel/plerr]
-![Example](media/example.svg) ## Table of contents - [CLI usage](#cli-usage) -
-[Stable release](#stable-release) - [Dev builds](#dev-builds) - [List of
-errors](#list-of-errors) ## CLI usage It's not required to install CLI util as
-long as you can navigate list of errors [here](#list-of-errors) or on this
-[web-site](https://vald-phoenix.github.io/pylint-errors/) but you may want to
-do so. ### Stable release You can install a stable release simply by such
-commands: ```console $ python3 -m pip install plerr $ plerr r1710 ``` For
-[pipx](https://github.com/pipxproject/pipx): ```console $ python3 -m pip
-install pipx # if not yet installed pipx $ python3 -m pipx ensurepath # ensure
-directory where pipx stores apps is on PATH $ pipx install plerr $ plerr r1710
-``` ### Dev builds In order to use development `plerr` builds you need to
-invoke the following commands: ```console $ git clone https://github.com/vald-
-phoenix/pylint-errors.git $ sudo apt update && sudo apt install -y python3-pip
-# if not yet installed $ cd pylint-errors $ python3 setup.py test $ python3
-setup.py install --user $ python3 -m plerr r1710 ``` [pipx](https://github.com/
-pipxproject/pipx) users may install the library by such commands: ```console $
-git clone https://github.com/vald-phoenix/pylint-errors.git $ sudo apt install
--y make python3-pip python3-venv # if not yet installed $ cd pylint-errors $
-python3 -m pip install pipx wheel # install a package to build a wheel and pipx
-$ python3 -m pipx ensurepath # ensure directory where pipx stores apps is on
-PATH $ python3 setup.py test # run tests $ make clean $ python3 setup.py
-bdist_wheel # build a binary wheel $ pipx install dist/* # install a binary
-wheel by pipx $ plerr r1710 ``` In order to get the latest updates just `git
-pull origin master` and invoke a command in the root of the project (`sudo apt
-install make` if not yet installed) `make rai` to install to Python 3 user
-space site packages or `make raip` for pipx. ## List of errors Error codes with
-**[+]** mean they've got examples of bad and good code. Rationalisation
-provided for all entries. ### Async Checker Messages - [E1700 (yield-inside-
-async-function)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
-async/E1700) **[+]** - [E1701 (not-async-context-manager)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/async/E1701) **[+]** ### Basic
-Checker Messages - [C0102 (blacklisted-name)](https://vald-phoenix.github.io/
-pylint-errors/plerr/errors/basic/C0102) **[+]** - [C0103 (invalid-name)](https:
-//vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0103) **[+]** -
-[C0112 (empty-docstring)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/C0112) **[+]** - [C0114 (missing-module-docstring)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/C0114) **[+]** - [C0115
-(missing-class-docstring)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/C0115) **[+]** - [C0116 (missing-function-docstring)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0116) **[+]** - [C0121
-(singleton-comparison)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/C0121) **[+]** - [C0122 (misplaced-comparison-constant)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0122) **[+]** - [C0123
-(unidiomatic-typecheck)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/C0123) **[+]** - [E0100 (init-is-generator)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0100) **[+]** - [E0101
-(return-in-init)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
-basic/E0101) **[+]** - [E0102 (function-redefined)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0102) **[+]** - [E0103
-(not-in-loop)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
-E0103) **[+]** - [E0104 (return-outside-function)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0104) **[+]** - [E0105
-(yield-outside-function)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/E0105) **[+]** - [E0106 (return-arg-in-generator)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0106) - [E0107
-(nonexistent-operator)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/E0107) **[+]** - [E0108 (duplicate-argument-name)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0108) **[+]** - [E0110
-(abstract-class-instantiated)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/E0110) **[+]** - [E0111 (bad-reversed-sequence)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0111) **[+]** - [E0112
-(too-many-star-expressions)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/E0112) **[+]** - [E0113 (invalid-star-assignment-target)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0113) **[+]**
-- [E0114 (star-needs-assignment-target)](https://vald-phoenix.github.io/pylint-
-errors/plerr/errors/basic/E0114) **[+]** - [E0115 (nonlocal-and-global)](https:
-//vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0115) **[+]** -
-[E0116 (continue-in-finally)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/E0116) **[+]** - [E0117 (nonlocal-without-binding)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0117) **[+]** - [E0118
-(used-prior-global-declaration)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/E0118) **[+]** - [E0119 (misplaced-format-function)](https:/
-/vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0119) **[+]** -
-[R0123 (literal-comparison)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/R0123) **[+]** - [R0124 (comparison-with-itself)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/R0124) **[+]** - [W0101
-(unreachable)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
-W0101) **[+]** - [W0102 (dangerous-default-value)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0102) **[+]** - [W0104
-(pointless-statement)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0104) **[+]** - [W0105 (pointless-string-statement)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0105) **[+]** - [W0106
-(expression-not-assigned)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0106) **[+]** - [W0107 (unnecessary-pass)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0107) **[+]** - [W0108
-(unnecessary-lambda)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0108) **[+]** - [W0109 (duplicate-key)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0109) **[+]** - [W0111
-(assign-to-new-keyword)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0111) **[+]** - [W0120 (useless-else-on-loop)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0120) **[+]** - [W0122
-(exec-used)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
-W0122) **[+]** - [W0123 (eval-used)](https://vald-phoenix.github.io/pylint-
-errors/plerr/errors/basic/W0123) **[+]** - [W0124 (confusing-with-statement)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0124) **[+]**
-- [W0125 (using-constant-test)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/W0125) - [W0126 (missing-parentheses-for-call-in-test)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0126) -
-[W0127 (self-assigning-variable)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/W0127) **[+]** - [W0128 (redeclared-assigned-name)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0128) - [W0143
-(comparison-with-callable)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0143) **[+]** - [W0150 (lost-exception)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0150) **[+]** - [W0199
-(assert-on-tuple)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
-basic/W0199) **[+]** ### Broad Try Clause Checker Messages - [W0717 (too-many-
-try-statements)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
-broad-try-clause/W0717) ### Classes Checker Messages - [C0202 (bad-classmethod-
-argument)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/
-C0202) **[+]** - [C0203 (bad-mcs-method-argument)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/classes/C0203) **[+]** - [C0204
-(bad-mcs-classmethod-argument)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/classes/C0204) **[+]** - [C0205 (single-string-used-for-slots)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/C0205) **
-[+]** - [E0202 (method-hidden)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/classes/E0202) **[+]** - [E0203 (access-member-before-definition)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0203) **
-[+]** - [E0211 (no-method-argument)](https://vald-phoenix.github.io/pylint-
-errors/plerr/errors/classes/E0211) **[+]** - [E0213 (no-self-argument)](https:/
-/vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0213) **[+]** -
-[E0236 (invalid-slots-object)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/classes/E0236) **[+]** - [E0237 (assigning-non-slot)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0237) **[+]** -
-[E0238 (invalid-slots)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/classes/E0238) **[+]** - [E0239 (inherit-non-class)](https://vald-
+![Example](https://raw.githubusercontent.com/vald-phoenix/pylint-errors/master/
+media/example.svg) ## Table of contents - [CLI usage](#cli-usage) - [Stable
+release](#stable-release) - [Dev builds](#dev-builds) - [List of errors](#list-
+of-errors) ## CLI usage It's not required to install CLI util as long as you
+can navigate list of errors [here](#list-of-errors) or on this [web-site]
+(https://vald-phoenix.github.io/pylint-errors/) but you may want to do so. ###
+Stable release You can install a stable release simply by such commands:
+```console $ python3 -m pip install plerr $ plerr r1710 ``` For [pipx](https://
+github.com/pipxproject/pipx): ```console $ python3 -m pip install pipx # if not
+yet installed pipx $ python3 -m pipx ensurepath # ensure directory where pipx
+stores apps is on PATH $ pipx install plerr $ plerr r1710 ``` ### Dev builds In
+order to use development `plerr` builds you need to invoke the following
+commands: ```console $ git clone https://github.com/vald-phoenix/pylint-
+errors.git $ sudo apt update && sudo apt install -y python3-pip # if not yet
+installed $ cd pylint-errors $ python3 setup.py test $ python3 setup.py install
+--user $ python3 -m plerr r1710 ``` [pipx](https://github.com/pipxproject/pipx)
+users may install the library by such commands: ```console $ git clone https://
+github.com/vald-phoenix/pylint-errors.git $ sudo apt install -y make python3-
+pip python3-venv # if not yet installed $ cd pylint-errors $ python3 -m pip
+install pipx wheel # install a package to build a wheel and pipx $ python3 -
+m pipx ensurepath # ensure directory where pipx stores apps is on PATH $
+python3 setup.py test # run tests $ make clean $ python3 setup.py bdist_wheel #
+build a binary wheel $ pipx install dist/* # install a binary wheel by pipx $
+plerr r1710 ``` In order to get the latest updates just `git pull origin
+master` and invoke a command in the root of the project (`sudo apt install
+make` if not yet installed) `make rai` to install to Python 3 user space site
+packages or `make raip` for pipx. ## List of errors Error codes with **[+]**
+mean they've got examples of bad and good code. Rationalisation provided for
+all entries. ### Async Checker Messages - [E1700 (yield-inside-async-function)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/async/E1700) **[+]**
+- [E1701 (not-async-context-manager)](https://vald-phoenix.github.io/pylint-
+errors/plerr/errors/async/E1701) **[+]** ### Basic Checker Messages - [C0102
+(blacklisted-name)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/C0102) **[+]** - [C0103 (invalid-name)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/basic/C0103) **[+]** - [C0112 (empty-docstring)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0112) **[+]**
+- [C0114 (missing-module-docstring)](https://vald-phoenix.github.io/pylint-
+errors/plerr/errors/basic/C0114) **[+]** - [C0115 (missing-class-docstring)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0115) **[+]**
+- [C0116 (missing-function-docstring)](https://vald-phoenix.github.io/pylint-
+errors/plerr/errors/basic/C0116) **[+]** - [C0121 (singleton-comparison)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0121) **[+]**
+- [C0122 (misplaced-comparison-constant)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/basic/C0122) **[+]** - [C0123 (unidiomatic-
+typecheck)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
+C0123) **[+]** - [E0100 (init-is-generator)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/basic/E0100) **[+]** - [E0101 (return-in-init)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0101) **[+]**
+- [E0102 (function-redefined)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/E0102) **[+]** - [E0103 (not-in-loop)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0103) **[+]** - [E0104
+(return-outside-function)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0104) **[+]** - [E0105 (yield-outside-function)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0105) **[+]** - [E0106
+(return-arg-in-generator)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0106) - [E0107 (nonexistent-operator)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0107) **[+]** - [E0108
+(duplicate-argument-name)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0108) **[+]** - [E0110 (abstract-class-instantiated)](https://
+vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0110) **[+]** - [E0111
+(bad-reversed-sequence)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0111) **[+]** - [E0112 (too-many-star-expressions)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0112) **[+]** - [E0113
+(invalid-star-assignment-target)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/E0113) **[+]** - [E0114 (star-needs-assignment-target)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0114) **[+]**
+- [E0115 (nonlocal-and-global)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/E0115) **[+]** - [E0116 (continue-in-finally)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0116) **[+]** - [E0117
+(nonlocal-without-binding)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0117) **[+]** - [E0118 (used-prior-global-declaration)](https://
+vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0118) **[+]** - [E0119
+(misplaced-format-function)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/E0119) **[+]** - [R0123 (literal-comparison)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/R0123) **[+]** - [R0124
+(comparison-with-itself)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/R0124) **[+]** - [W0101 (unreachable)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0101) **[+]** - [W0102
+(dangerous-default-value)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/W0102) **[+]** - [W0104 (pointless-statement)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0104) **[+]** - [W0105
+(pointless-string-statement)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/W0105) **[+]** - [W0106 (expression-not-assigned)](https://
+vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0106) **[+]** - [W0107
+(unnecessary-pass)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/W0107) **[+]** - [W0108 (unnecessary-lambda)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0108) **[+]** - [W0109
+(duplicate-key)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/W0109) **[+]** - [W0111 (assign-to-new-keyword)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0111) **[+]** - [W0120
+(useless-else-on-loop)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/W0120) **[+]** - [W0122 (exec-used)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0122) **[+]** - [W0123
+(eval-used)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
+W0123) **[+]** - [W0124 (confusing-with-statement)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0124) **[+]** - [W0125
+(using-constant-test)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/W0125) - [W0126 (missing-parentheses-for-call-in-test)](https://
+vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0126) - [W0127 (self-
+assigning-variable)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/W0127) **[+]** - [W0128 (redeclared-assigned-name)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0128) - [W0143 (comparison-
+with-callable)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/W0143) **[+]** - [W0150 (lost-exception)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/basic/W0150) **[+]** - [W0199 (assert-on-tuple)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0199) **[+]**
+### Broad Try Clause Checker Messages - [W0717 (too-many-try-statements)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/broad-try-clause/
+W0717) ### Classes Checker Messages - [C0202 (bad-classmethod-argument)](https:
+//vald-phoenix.github.io/pylint-errors/plerr/errors/classes/C0202) **[+]** -
+[C0203 (bad-mcs-method-argument)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/classes/C0203) **[+]** - [C0204 (bad-mcs-classmethod-argument)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/C0204) **
+[+]** - [C0205 (single-string-used-for-slots)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/classes/C0205) **[+]** - [E0202 (method-hidden)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0202) **
+[+]** - [E0203 (access-member-before-definition)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/classes/E0203) **[+]** - [E0211
+(no-method-argument)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/classes/E0211) **[+]** - [E0213 (no-self-argument)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/classes/E0213) **[+]** - [E0236
+(invalid-slots-object)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/classes/E0236) **[+]** - [E0237 (assigning-non-slot)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/classes/E0237) **[+]** - [E0238
+(invalid-slots)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+classes/E0238) **[+]** - [E0239 (inherit-non-class)](https://vald-
 phoenix.github.io/pylint-errors/plerr/errors/classes/E0239) **[+]** - [E0240
 (inconsistent-mro)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
 classes/E0240) **[+]** - [E0241 (duplicate-bases)](https://vald-
 phoenix.github.io/pylint-errors/plerr/errors/classes/E0241) **[+]** - [E0242
 (class-variable-slots-conflict)](https://vald-phoenix.github.io/pylint-errors/
 plerr/errors/classes/E0242) **[+]** - [E0301 (non-iterator-returned)](https://
 vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0301) **[+]** -
```

### Comparing `plerr-2.1.0/README.md` & `plerr-3.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 <h1 align="center">
   <br>
-  <a href="https://github.com/vald-phoenix/pylint-errors"><img src="media/logo.png" width="200px" height="auto" alt="plerr"></a>
+  <a href="https://github.com/vald-phoenix/pylint-errors">
+      <img src="https://raw.githubusercontent.com/vald-phoenix/pylint-errors/master/media/logo.png" width="200px" height="auto" alt="plerr">
+  </a>
   <br>
 </h1>
 
 <h4 align="center">A list of pylint-errors with reasoning and examples of erroneous and correct code.</h4>
 
 <p align="center">
   <a href="https://github.com/vald-phoenix/pylint-error">
@@ -26,15 +28,15 @@
       <img src="https://img.shields.io/pypi/v/plerr">
   </a>
   <a href="https://pypi.org/project/plerr/">
       <img src="https://img.shields.io/pypi/wheel/plerr">
   </a>
 </p>
 
-![Example](media/example.svg)
+![Example](https://raw.githubusercontent.com/vald-phoenix/pylint-errors/master/media/example.svg)
 
 ## Table of contents
 
 - [CLI usage](#cli-usage)
   - [Stable release](#stable-release)
   - [Dev builds](#dev-builds)
 - [List of errors](#list-of-errors)
```

#### html2text {}

```diff
@@ -5,139 +5,140 @@
                                correct code. ***
  [https://img.shields.io/badge/made_in-ukraine-ffd700.svg?labelColor=0057b7]
 [https://img.shields.io/pypi/l/plerr] [https://github.com/vald-phoenix/pylint-
   errors/workflows/CI/badge.svg] [https://codecov.io/gh/vald-phoenix/pylint-
 errors/branch/master/graph/badge.svg] [https://img.shields.io/pypi/pyversions/
   plerr] [https://img.shields.io/pypi/v/plerr] [https://img.shields.io/pypi/
                                  wheel/plerr]
-![Example](media/example.svg) ## Table of contents - [CLI usage](#cli-usage) -
-[Stable release](#stable-release) - [Dev builds](#dev-builds) - [List of
-errors](#list-of-errors) ## CLI usage It's not required to install CLI util as
-long as you can navigate list of errors [here](#list-of-errors) or on this
-[web-site](https://vald-phoenix.github.io/pylint-errors/) but you may want to
-do so. ### Stable release You can install a stable release simply by such
-commands: ```console $ python3 -m pip install plerr $ plerr r1710 ``` For
-[pipx](https://github.com/pipxproject/pipx): ```console $ python3 -m pip
-install pipx # if not yet installed pipx $ python3 -m pipx ensurepath # ensure
-directory where pipx stores apps is on PATH $ pipx install plerr $ plerr r1710
-``` ### Dev builds In order to use development `plerr` builds you need to
-invoke the following commands: ```console $ git clone https://github.com/vald-
-phoenix/pylint-errors.git $ sudo apt update && sudo apt install -y python3-pip
-# if not yet installed $ cd pylint-errors $ python3 setup.py test $ python3
-setup.py install --user $ python3 -m plerr r1710 ``` [pipx](https://github.com/
-pipxproject/pipx) users may install the library by such commands: ```console $
-git clone https://github.com/vald-phoenix/pylint-errors.git $ sudo apt install
--y make python3-pip python3-venv # if not yet installed $ cd pylint-errors $
-python3 -m pip install pipx wheel # install a package to build a wheel and pipx
-$ python3 -m pipx ensurepath # ensure directory where pipx stores apps is on
-PATH $ python3 setup.py test # run tests $ make clean $ python3 setup.py
-bdist_wheel # build a binary wheel $ pipx install dist/* # install a binary
-wheel by pipx $ plerr r1710 ``` In order to get the latest updates just `git
-pull origin master` and invoke a command in the root of the project (`sudo apt
-install make` if not yet installed) `make rai` to install to Python 3 user
-space site packages or `make raip` for pipx. ## List of errors Error codes with
-**[+]** mean they've got examples of bad and good code. Rationalisation
-provided for all entries. ### Async Checker Messages - [E1700 (yield-inside-
-async-function)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
-async/E1700) **[+]** - [E1701 (not-async-context-manager)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/async/E1701) **[+]** ### Basic
-Checker Messages - [C0102 (blacklisted-name)](https://vald-phoenix.github.io/
-pylint-errors/plerr/errors/basic/C0102) **[+]** - [C0103 (invalid-name)](https:
-//vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0103) **[+]** -
-[C0112 (empty-docstring)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/C0112) **[+]** - [C0114 (missing-module-docstring)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/C0114) **[+]** - [C0115
-(missing-class-docstring)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/C0115) **[+]** - [C0116 (missing-function-docstring)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0116) **[+]** - [C0121
-(singleton-comparison)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/C0121) **[+]** - [C0122 (misplaced-comparison-constant)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0122) **[+]** - [C0123
-(unidiomatic-typecheck)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/C0123) **[+]** - [E0100 (init-is-generator)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0100) **[+]** - [E0101
-(return-in-init)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
-basic/E0101) **[+]** - [E0102 (function-redefined)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0102) **[+]** - [E0103
-(not-in-loop)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
-E0103) **[+]** - [E0104 (return-outside-function)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0104) **[+]** - [E0105
-(yield-outside-function)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/E0105) **[+]** - [E0106 (return-arg-in-generator)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0106) - [E0107
-(nonexistent-operator)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/E0107) **[+]** - [E0108 (duplicate-argument-name)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0108) **[+]** - [E0110
-(abstract-class-instantiated)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/E0110) **[+]** - [E0111 (bad-reversed-sequence)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0111) **[+]** - [E0112
-(too-many-star-expressions)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/E0112) **[+]** - [E0113 (invalid-star-assignment-target)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0113) **[+]**
-- [E0114 (star-needs-assignment-target)](https://vald-phoenix.github.io/pylint-
-errors/plerr/errors/basic/E0114) **[+]** - [E0115 (nonlocal-and-global)](https:
-//vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0115) **[+]** -
-[E0116 (continue-in-finally)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/E0116) **[+]** - [E0117 (nonlocal-without-binding)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0117) **[+]** - [E0118
-(used-prior-global-declaration)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/E0118) **[+]** - [E0119 (misplaced-format-function)](https:/
-/vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0119) **[+]** -
-[R0123 (literal-comparison)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/R0123) **[+]** - [R0124 (comparison-with-itself)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/R0124) **[+]** - [W0101
-(unreachable)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
-W0101) **[+]** - [W0102 (dangerous-default-value)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0102) **[+]** - [W0104
-(pointless-statement)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0104) **[+]** - [W0105 (pointless-string-statement)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0105) **[+]** - [W0106
-(expression-not-assigned)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0106) **[+]** - [W0107 (unnecessary-pass)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0107) **[+]** - [W0108
-(unnecessary-lambda)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0108) **[+]** - [W0109 (duplicate-key)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0109) **[+]** - [W0111
-(assign-to-new-keyword)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0111) **[+]** - [W0120 (useless-else-on-loop)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0120) **[+]** - [W0122
-(exec-used)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
-W0122) **[+]** - [W0123 (eval-used)](https://vald-phoenix.github.io/pylint-
-errors/plerr/errors/basic/W0123) **[+]** - [W0124 (confusing-with-statement)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0124) **[+]**
-- [W0125 (using-constant-test)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/W0125) - [W0126 (missing-parentheses-for-call-in-test)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0126) -
-[W0127 (self-assigning-variable)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/W0127) **[+]** - [W0128 (redeclared-assigned-name)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0128) - [W0143
-(comparison-with-callable)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0143) **[+]** - [W0150 (lost-exception)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0150) **[+]** - [W0199
-(assert-on-tuple)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
-basic/W0199) **[+]** ### Broad Try Clause Checker Messages - [W0717 (too-many-
-try-statements)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
-broad-try-clause/W0717) ### Classes Checker Messages - [C0202 (bad-classmethod-
-argument)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/
-C0202) **[+]** - [C0203 (bad-mcs-method-argument)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/classes/C0203) **[+]** - [C0204
-(bad-mcs-classmethod-argument)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/classes/C0204) **[+]** - [C0205 (single-string-used-for-slots)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/C0205) **
-[+]** - [E0202 (method-hidden)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/classes/E0202) **[+]** - [E0203 (access-member-before-definition)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0203) **
-[+]** - [E0211 (no-method-argument)](https://vald-phoenix.github.io/pylint-
-errors/plerr/errors/classes/E0211) **[+]** - [E0213 (no-self-argument)](https:/
-/vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0213) **[+]** -
-[E0236 (invalid-slots-object)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/classes/E0236) **[+]** - [E0237 (assigning-non-slot)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0237) **[+]** -
-[E0238 (invalid-slots)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/classes/E0238) **[+]** - [E0239 (inherit-non-class)](https://vald-
+![Example](https://raw.githubusercontent.com/vald-phoenix/pylint-errors/master/
+media/example.svg) ## Table of contents - [CLI usage](#cli-usage) - [Stable
+release](#stable-release) - [Dev builds](#dev-builds) - [List of errors](#list-
+of-errors) ## CLI usage It's not required to install CLI util as long as you
+can navigate list of errors [here](#list-of-errors) or on this [web-site]
+(https://vald-phoenix.github.io/pylint-errors/) but you may want to do so. ###
+Stable release You can install a stable release simply by such commands:
+```console $ python3 -m pip install plerr $ plerr r1710 ``` For [pipx](https://
+github.com/pipxproject/pipx): ```console $ python3 -m pip install pipx # if not
+yet installed pipx $ python3 -m pipx ensurepath # ensure directory where pipx
+stores apps is on PATH $ pipx install plerr $ plerr r1710 ``` ### Dev builds In
+order to use development `plerr` builds you need to invoke the following
+commands: ```console $ git clone https://github.com/vald-phoenix/pylint-
+errors.git $ sudo apt update && sudo apt install -y python3-pip # if not yet
+installed $ cd pylint-errors $ python3 setup.py test $ python3 setup.py install
+--user $ python3 -m plerr r1710 ``` [pipx](https://github.com/pipxproject/pipx)
+users may install the library by such commands: ```console $ git clone https://
+github.com/vald-phoenix/pylint-errors.git $ sudo apt install -y make python3-
+pip python3-venv # if not yet installed $ cd pylint-errors $ python3 -m pip
+install pipx wheel # install a package to build a wheel and pipx $ python3 -
+m pipx ensurepath # ensure directory where pipx stores apps is on PATH $
+python3 setup.py test # run tests $ make clean $ python3 setup.py bdist_wheel #
+build a binary wheel $ pipx install dist/* # install a binary wheel by pipx $
+plerr r1710 ``` In order to get the latest updates just `git pull origin
+master` and invoke a command in the root of the project (`sudo apt install
+make` if not yet installed) `make rai` to install to Python 3 user space site
+packages or `make raip` for pipx. ## List of errors Error codes with **[+]**
+mean they've got examples of bad and good code. Rationalisation provided for
+all entries. ### Async Checker Messages - [E1700 (yield-inside-async-function)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/async/E1700) **[+]**
+- [E1701 (not-async-context-manager)](https://vald-phoenix.github.io/pylint-
+errors/plerr/errors/async/E1701) **[+]** ### Basic Checker Messages - [C0102
+(blacklisted-name)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/C0102) **[+]** - [C0103 (invalid-name)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/basic/C0103) **[+]** - [C0112 (empty-docstring)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0112) **[+]**
+- [C0114 (missing-module-docstring)](https://vald-phoenix.github.io/pylint-
+errors/plerr/errors/basic/C0114) **[+]** - [C0115 (missing-class-docstring)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0115) **[+]**
+- [C0116 (missing-function-docstring)](https://vald-phoenix.github.io/pylint-
+errors/plerr/errors/basic/C0116) **[+]** - [C0121 (singleton-comparison)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0121) **[+]**
+- [C0122 (misplaced-comparison-constant)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/basic/C0122) **[+]** - [C0123 (unidiomatic-
+typecheck)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
+C0123) **[+]** - [E0100 (init-is-generator)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/basic/E0100) **[+]** - [E0101 (return-in-init)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0101) **[+]**
+- [E0102 (function-redefined)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/E0102) **[+]** - [E0103 (not-in-loop)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0103) **[+]** - [E0104
+(return-outside-function)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0104) **[+]** - [E0105 (yield-outside-function)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0105) **[+]** - [E0106
+(return-arg-in-generator)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0106) - [E0107 (nonexistent-operator)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0107) **[+]** - [E0108
+(duplicate-argument-name)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0108) **[+]** - [E0110 (abstract-class-instantiated)](https://
+vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0110) **[+]** - [E0111
+(bad-reversed-sequence)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0111) **[+]** - [E0112 (too-many-star-expressions)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0112) **[+]** - [E0113
+(invalid-star-assignment-target)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/E0113) **[+]** - [E0114 (star-needs-assignment-target)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0114) **[+]**
+- [E0115 (nonlocal-and-global)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/E0115) **[+]** - [E0116 (continue-in-finally)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0116) **[+]** - [E0117
+(nonlocal-without-binding)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0117) **[+]** - [E0118 (used-prior-global-declaration)](https://
+vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0118) **[+]** - [E0119
+(misplaced-format-function)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/E0119) **[+]** - [R0123 (literal-comparison)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/R0123) **[+]** - [R0124
+(comparison-with-itself)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/R0124) **[+]** - [W0101 (unreachable)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0101) **[+]** - [W0102
+(dangerous-default-value)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/W0102) **[+]** - [W0104 (pointless-statement)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0104) **[+]** - [W0105
+(pointless-string-statement)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/W0105) **[+]** - [W0106 (expression-not-assigned)](https://
+vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0106) **[+]** - [W0107
+(unnecessary-pass)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/W0107) **[+]** - [W0108 (unnecessary-lambda)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0108) **[+]** - [W0109
+(duplicate-key)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/W0109) **[+]** - [W0111 (assign-to-new-keyword)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0111) **[+]** - [W0120
+(useless-else-on-loop)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/W0120) **[+]** - [W0122 (exec-used)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0122) **[+]** - [W0123
+(eval-used)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
+W0123) **[+]** - [W0124 (confusing-with-statement)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0124) **[+]** - [W0125
+(using-constant-test)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/W0125) - [W0126 (missing-parentheses-for-call-in-test)](https://
+vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0126) - [W0127 (self-
+assigning-variable)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/W0127) **[+]** - [W0128 (redeclared-assigned-name)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0128) - [W0143 (comparison-
+with-callable)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/W0143) **[+]** - [W0150 (lost-exception)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/basic/W0150) **[+]** - [W0199 (assert-on-tuple)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0199) **[+]**
+### Broad Try Clause Checker Messages - [W0717 (too-many-try-statements)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/broad-try-clause/
+W0717) ### Classes Checker Messages - [C0202 (bad-classmethod-argument)](https:
+//vald-phoenix.github.io/pylint-errors/plerr/errors/classes/C0202) **[+]** -
+[C0203 (bad-mcs-method-argument)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/classes/C0203) **[+]** - [C0204 (bad-mcs-classmethod-argument)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/C0204) **
+[+]** - [C0205 (single-string-used-for-slots)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/classes/C0205) **[+]** - [E0202 (method-hidden)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0202) **
+[+]** - [E0203 (access-member-before-definition)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/classes/E0203) **[+]** - [E0211
+(no-method-argument)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/classes/E0211) **[+]** - [E0213 (no-self-argument)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/classes/E0213) **[+]** - [E0236
+(invalid-slots-object)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/classes/E0236) **[+]** - [E0237 (assigning-non-slot)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/classes/E0237) **[+]** - [E0238
+(invalid-slots)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+classes/E0238) **[+]** - [E0239 (inherit-non-class)](https://vald-
 phoenix.github.io/pylint-errors/plerr/errors/classes/E0239) **[+]** - [E0240
 (inconsistent-mro)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
 classes/E0240) **[+]** - [E0241 (duplicate-bases)](https://vald-
 phoenix.github.io/pylint-errors/plerr/errors/classes/E0241) **[+]** - [E0242
 (class-variable-slots-conflict)](https://vald-phoenix.github.io/pylint-errors/
 plerr/errors/classes/E0242) **[+]** - [E0301 (non-iterator-returned)](https://
 vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0301) **[+]** -
```

### Comparing `plerr-2.1.0/plerr/cli.py` & `plerr-3.0.0/plerr/cli.py`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/async/E1700.md` & `plerr-3.0.0/plerr/errors/async/E1700.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/async/E1701.md` & `plerr-3.0.0/plerr/errors/async/E1701.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/C0112.md` & `plerr-3.0.0/plerr/errors/basic/C0112.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/C0116.md` & `plerr-3.0.0/plerr/errors/basic/C0116.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/C0121.md` & `plerr-3.0.0/plerr/errors/basic/C0121.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/C0122.md` & `plerr-3.0.0/plerr/errors/basic/C0122.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/C0123.md` & `plerr-3.0.0/plerr/errors/basic/C0123.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0100.md` & `plerr-3.0.0/plerr/errors/basic/E0100.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0101.md` & `plerr-3.0.0/plerr/errors/basic/E0101.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0102.md` & `plerr-3.0.0/plerr/errors/basic/E0102.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0103.md` & `plerr-3.0.0/plerr/errors/basic/E0103.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0104.md` & `plerr-3.0.0/plerr/errors/basic/E0104.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0105.md` & `plerr-3.0.0/plerr/errors/basic/E0105.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0107.md` & `plerr-3.0.0/plerr/errors/basic/E0107.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0108.md` & `plerr-3.0.0/plerr/errors/basic/E0108.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0110.md` & `plerr-3.0.0/plerr/errors/basic/E0110.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0111.md` & `plerr-3.0.0/plerr/errors/basic/E0111.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0112.md` & `plerr-3.0.0/plerr/errors/basic/E0112.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0113.md` & `plerr-3.0.0/plerr/errors/basic/E0113.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0114.md` & `plerr-3.0.0/plerr/errors/basic/E0114.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0115.md` & `plerr-3.0.0/plerr/errors/basic/E0115.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0116.md` & `plerr-3.0.0/plerr/errors/basic/E0116.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0117.md` & `plerr-3.0.0/plerr/errors/basic/E0117.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0118.md` & `plerr-3.0.0/plerr/errors/basic/E0118.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/E0119.md` & `plerr-3.0.0/plerr/errors/basic/E0119.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/R0123.md` & `plerr-3.0.0/plerr/errors/basic/R0123.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/W0101.md` & `plerr-3.0.0/plerr/errors/basic/W0101.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/W0102.md` & `plerr-3.0.0/plerr/errors/basic/W0102.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/W0105.md` & `plerr-3.0.0/plerr/errors/basic/W0105.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/W0106.md` & `plerr-3.0.0/plerr/errors/basic/W0106.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/W0107.md` & `plerr-3.0.0/plerr/errors/basic/W0107.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/W0108.md` & `plerr-3.0.0/plerr/errors/basic/W0108.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/W0109.md` & `plerr-3.0.0/plerr/errors/basic/W0109.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/W0120.md` & `plerr-3.0.0/plerr/errors/basic/W0120.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/W0122.md` & `plerr-3.0.0/plerr/errors/basic/W0122.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/W0123.md` & `plerr-3.0.0/plerr/errors/basic/W0123.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/W0124.md` & `plerr-3.0.0/plerr/errors/basic/W0124.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/W0143.md` & `plerr-3.0.0/plerr/errors/basic/W0143.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/basic/W0150.md` & `plerr-3.0.0/plerr/errors/basic/W0150.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/C0202.md` & `plerr-3.0.0/plerr/errors/classes/C0202.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/C0203.md` & `plerr-3.0.0/plerr/errors/classes/C0203.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/C0204.md` & `plerr-3.0.0/plerr/errors/classes/C0204.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/C0205.md` & `plerr-3.0.0/plerr/errors/classes/C0205.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/E0202.md` & `plerr-3.0.0/plerr/errors/classes/E0202.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/E0203.md` & `plerr-3.0.0/plerr/errors/classes/E0203.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/E0213.md` & `plerr-3.0.0/plerr/errors/classes/E0213.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/E0236.md` & `plerr-3.0.0/plerr/errors/classes/E0236.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/E0237.md` & `plerr-3.0.0/plerr/errors/classes/E0237.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/E0238.md` & `plerr-3.0.0/plerr/errors/classes/E0238.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/E0301.md` & `plerr-3.0.0/plerr/errors/classes/E0301.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/E0302.md` & `plerr-3.0.0/plerr/errors/classes/E0302.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/R0201.md` & `plerr-3.0.0/plerr/errors/classes/R0201.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/R0202.md` & `plerr-3.0.0/plerr/errors/classes/R0202.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/R0205.md` & `plerr-3.0.0/plerr/errors/classes/R0205.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/R0206.md` & `plerr-3.0.0/plerr/errors/classes/R0206.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/W0201.md` & `plerr-3.0.0/plerr/errors/classes/W0201.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/W0211.md` & `plerr-3.0.0/plerr/errors/classes/W0211.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/W0212.md` & `plerr-3.0.0/plerr/errors/classes/W0212.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/W0221.md` & `plerr-3.0.0/plerr/errors/classes/W0221.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/W0223.md` & `plerr-3.0.0/plerr/errors/classes/W0223.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/W0231.md` & `plerr-3.0.0/plerr/errors/classes/W0231.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/W0233.md` & `plerr-3.0.0/plerr/errors/classes/W0233.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/W0235.md` & `plerr-3.0.0/plerr/errors/classes/W0235.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/classes/W0236.md` & `plerr-3.0.0/plerr/errors/classes/W0236.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/deprecated-builtins/W0141.md` & `plerr-3.0.0/plerr/errors/deprecated-builtins/W0141.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/design/R0901.md` & `plerr-3.0.0/plerr/errors/design/R0901.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/design/R0902.md` & `plerr-3.0.0/plerr/errors/design/R0902.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/design/R0903.md` & `plerr-3.0.0/plerr/errors/design/R0903.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/design/R0904.md` & `plerr-3.0.0/plerr/errors/design/R0904.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/design/R0911.md` & `plerr-3.0.0/plerr/errors/design/R0911.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/design/R0912.md` & `plerr-3.0.0/plerr/errors/design/R0912.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/design/R0915.md` & `plerr-3.0.0/plerr/errors/design/R0915.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/design/R0916.md` & `plerr-3.0.0/plerr/errors/design/R0916.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/design/R1260.md` & `plerr-3.0.0/plerr/errors/design/R1260.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/docstyle/C0199.md` & `plerr-3.0.0/plerr/errors/docstyle/C0199.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/else-if-used/R5501.md` & `plerr-3.0.0/plerr/errors/else-if-used/R5501.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/exceptions/E0701.md` & `plerr-3.0.0/plerr/errors/exceptions/E0701.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/exceptions/E0702.md` & `plerr-3.0.0/plerr/errors/exceptions/E0702.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/exceptions/E0703.md` & `plerr-3.0.0/plerr/errors/exceptions/E0703.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/exceptions/E0704.md` & `plerr-3.0.0/plerr/errors/exceptions/E0704.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/exceptions/E0712.md` & `plerr-3.0.0/plerr/errors/exceptions/E0712.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/exceptions/W0706.md` & `plerr-3.0.0/plerr/errors/exceptions/W0706.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/exceptions/W0711.md` & `plerr-3.0.0/plerr/errors/exceptions/W0711.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/exceptions/W0715.md` & `plerr-3.0.0/plerr/errors/exceptions/W0715.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/exceptions/W0716.md` & `plerr-3.0.0/plerr/errors/exceptions/W0716.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/format/C0303.md` & `plerr-3.0.0/plerr/errors/format/C0303.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/imports/C0411.md` & `plerr-3.0.0/plerr/errors/imports/C0411.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/imports/E0402.md` & `plerr-3.0.0/plerr/errors/imports/E0402.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/imports/R0401.md` & `plerr-3.0.0/plerr/errors/imports/R0401.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/imports/W0410.md` & `plerr-3.0.0/plerr/errors/imports/W0410.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/logging/W1201.md` & `plerr-3.0.0/plerr/errors/logging/W1201.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/logging/W1202.md` & `plerr-3.0.0/plerr/errors/logging/W1202.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/newstyle/E1003.md` & `plerr-3.0.0/plerr/errors/newstyle/E1003.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/parameter-documentation/W9005.md` & `plerr-3.0.0/plerr/errors/parameter-documentation/W9005.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/parameter-documentation/W9006.md` & `plerr-3.0.0/plerr/errors/parameter-documentation/W9006.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/parameter-documentation/W9011.md` & `plerr-3.0.0/plerr/errors/parameter-documentation/W9011.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/parameter-documentation/W9012.md` & `plerr-3.0.0/plerr/errors/parameter-documentation/W9012.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/parameter-documentation/W9015.md` & `plerr-3.0.0/plerr/errors/parameter-documentation/W9015.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/parameter-documentation/W9016.md` & `plerr-3.0.0/plerr/errors/parameter-documentation/W9016.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/parameter-documentation/W9017.md` & `plerr-3.0.0/plerr/errors/parameter-documentation/W9017.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/parameter-documentation/W9018.md` & `plerr-3.0.0/plerr/errors/parameter-documentation/W9018.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/C0200.md` & `plerr-3.0.0/plerr/errors/refactoring/C0200.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/C0201.md` & `plerr-3.0.0/plerr/errors/refactoring/C0201.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/C1801.md` & `plerr-3.0.0/plerr/errors/refactoring/C1801.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1704.md` & `plerr-3.0.0/plerr/errors/refactoring/R1704.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1705.md` & `plerr-3.0.0/plerr/errors/refactoring/R1705.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1707.md` & `plerr-3.0.0/plerr/errors/refactoring/R1707.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1708.md` & `plerr-3.0.0/plerr/errors/refactoring/R1708.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1710.md` & `plerr-3.0.0/plerr/errors/refactoring/R1710.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1711.md` & `plerr-3.0.0/plerr/errors/refactoring/R1711.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1712.md` & `plerr-3.0.0/plerr/errors/refactoring/R1712.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1713.md` & `plerr-3.0.0/plerr/errors/refactoring/R1713.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1714.md` & `plerr-3.0.0/plerr/errors/refactoring/R1714.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1716.md` & `plerr-3.0.0/plerr/errors/refactoring/R1716.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1717.md` & `plerr-3.0.0/plerr/errors/refactoring/R1717.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1718.md` & `plerr-3.0.0/plerr/errors/refactoring/R1718.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1720.md` & `plerr-3.0.0/plerr/errors/refactoring/R1720.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1721.md` & `plerr-3.0.0/plerr/errors/refactoring/R1721.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1722.md` & `plerr-3.0.0/plerr/errors/refactoring/R1722.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1723.md` & `plerr-3.0.0/plerr/errors/refactoring/R1723.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/refactoring/R1724.md` & `plerr-3.0.0/plerr/errors/refactoring/R1724.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/stdlib/W1501.md` & `plerr-3.0.0/plerr/errors/stdlib/W1501.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/stdlib/W1502.md` & `plerr-3.0.0/plerr/errors/stdlib/W1502.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/stdlib/W1503.md` & `plerr-3.0.0/plerr/errors/stdlib/W1503.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/stdlib/W1506.md` & `plerr-3.0.0/plerr/errors/stdlib/W1506.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/stdlib/W1507.md` & `plerr-3.0.0/plerr/errors/stdlib/W1507.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/stdlib/W1508.md` & `plerr-3.0.0/plerr/errors/stdlib/W1508.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/stdlib/W1509.md` & `plerr-3.0.0/plerr/errors/stdlib/W1509.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/stdlib/W1510.md` & `plerr-3.0.0/plerr/errors/stdlib/W1510.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/string/E1302.md` & `plerr-3.0.0/plerr/errors/string/E1302.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/string/E1304.md` & `plerr-3.0.0/plerr/errors/string/E1304.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/string/W1304.md` & `plerr-3.0.0/plerr/errors/string/W1304.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/string/W1305.md` & `plerr-3.0.0/plerr/errors/string/W1305.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/string/W1307.md` & `plerr-3.0.0/plerr/errors/string/W1307.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/typecheck/E1111.md` & `plerr-3.0.0/plerr/errors/typecheck/E1111.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/typecheck/E1123.md` & `plerr-3.0.0/plerr/errors/typecheck/E1123.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/typecheck/E1124.md` & `plerr-3.0.0/plerr/errors/typecheck/E1124.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/typecheck/E1126.md` & `plerr-3.0.0/plerr/errors/typecheck/E1126.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/typecheck/E1129.md` & `plerr-3.0.0/plerr/errors/typecheck/E1129.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/typecheck/E1133.md` & `plerr-3.0.0/plerr/errors/typecheck/E1133.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/typecheck/E1135.md` & `plerr-3.0.0/plerr/errors/typecheck/E1135.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/typecheck/E1136.md` & `plerr-3.0.0/plerr/errors/typecheck/E1136.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/typecheck/E1137.md` & `plerr-3.0.0/plerr/errors/typecheck/E1137.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/typecheck/E1138.md` & `plerr-3.0.0/plerr/errors/typecheck/E1138.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/typecheck/E1141.md` & `plerr-3.0.0/plerr/errors/typecheck/E1141.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/typecheck/I1101.md` & `plerr-3.0.0/plerr/errors/typecheck/I1101.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/typecheck/W1113.md` & `plerr-3.0.0/plerr/errors/typecheck/W1113.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/variables/E0603.md` & `plerr-3.0.0/plerr/errors/variables/E0603.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/variables/E0604.md` & `plerr-3.0.0/plerr/errors/variables/E0604.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/variables/E0611.md` & `plerr-3.0.0/plerr/errors/variables/E0611.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/variables/E0633.md` & `plerr-3.0.0/plerr/errors/variables/E0633.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/variables/W0601.md` & `plerr-3.0.0/plerr/errors/variables/W0601.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/variables/W0602.md` & `plerr-3.0.0/plerr/errors/variables/W0602.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/variables/W0603.md` & `plerr-3.0.0/plerr/errors/variables/W0603.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/variables/W0611.md` & `plerr-3.0.0/plerr/errors/variables/W0611.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/variables/W0631.md` & `plerr-3.0.0/plerr/errors/variables/W0631.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/errors/variables/W0640.md` & `plerr-3.0.0/plerr/errors/variables/W0640.md`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/tests/command_output_fixture.txt` & `plerr-3.0.0/plerr/tests/command_output_fixture.txt`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/tests/test_cli_module.py` & `plerr-3.0.0/plerr/tests/test_cli_module.py`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr/tests/test_package.py` & `plerr-3.0.0/plerr/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/plerr.egg-info/PKG-INFO` & `plerr-3.0.0/plerr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: plerr
-Version: 2.1.0
+Version: 3.0.0
 Summary: A list of pylint-errors with reasoning and examples of erroneous and correct code.
 Home-page: https://github.com/vald-phoenix/pylint-errors
 Author: Vladyslav Krylasov
 Author-email: vladyslav.krylasov@gmail.com
 License: UNKNOWN
 Keywords: pylint,errors,documentation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
   <br>
-  <a href="https://github.com/vald-phoenix/pylint-errors"><img src="media/logo.png" width="200px" height="auto" alt="plerr"></a>
+  <a href="https://github.com/vald-phoenix/pylint-errors">
+      <img src="https://raw.githubusercontent.com/vald-phoenix/pylint-errors/master/media/logo.png" width="200px" height="auto" alt="plerr">
+  </a>
   <br>
 </h1>
 
 <h4 align="center">A list of pylint-errors with reasoning and examples of erroneous and correct code.</h4>
 
 <p align="center">
   <a href="https://github.com/vald-phoenix/pylint-error">
@@ -55,15 +56,15 @@
       <img src="https://img.shields.io/pypi/v/plerr">
   </a>
   <a href="https://pypi.org/project/plerr/">
       <img src="https://img.shields.io/pypi/wheel/plerr">
   </a>
 </p>
 
-![Example](media/example.svg)
+![Example](https://raw.githubusercontent.com/vald-phoenix/pylint-errors/master/media/example.svg)
 
 ## Table of contents
 
 - [CLI usage](#cli-usage)
   - [Stable release](#stable-release)
   - [Dev builds](#dev-builds)
 - [List of errors](#list-of-errors)
```

#### html2text {}

```diff
@@ -1,160 +1,160 @@
-Metadata-Version: 2.1 Name: plerr Version: 2.1.0 Summary: A list of pylint-
+Metadata-Version: 2.1 Name: plerr Version: 3.0.0 Summary: A list of pylint-
 errors with reasoning and examples of erroneous and correct code. Home-page:
 https://github.com/vald-phoenix/pylint-errors Author: Vladyslav Krylasov
 Author-email: vladyslav.krylasov@gmail.com License: UNKNOWN Keywords:
 pylint,errors,documentation Platform: UNKNOWN Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Topic :: Software Development
-:: Documentation Classifier: Topic :: Software Development :: Libraries ::
-Python Modules Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE
+Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: Implementation :: CPython Classifier: Topic
+:: Software Development :: Documentation Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Software
+Development :: Quality Assurance Requires-Python: >=3.7 Description-Content-
+Type: text/markdown License-File: LICENSE
                                     ******
                                    [plerr]
                                      ******
    *** A list of pylint-errors with reasoning and examples of erroneous and
                                correct code. ***
  [https://img.shields.io/badge/made_in-ukraine-ffd700.svg?labelColor=0057b7]
 [https://img.shields.io/pypi/l/plerr] [https://github.com/vald-phoenix/pylint-
   errors/workflows/CI/badge.svg] [https://codecov.io/gh/vald-phoenix/pylint-
 errors/branch/master/graph/badge.svg] [https://img.shields.io/pypi/pyversions/
   plerr] [https://img.shields.io/pypi/v/plerr] [https://img.shields.io/pypi/
                                  wheel/plerr]
-![Example](media/example.svg) ## Table of contents - [CLI usage](#cli-usage) -
-[Stable release](#stable-release) - [Dev builds](#dev-builds) - [List of
-errors](#list-of-errors) ## CLI usage It's not required to install CLI util as
-long as you can navigate list of errors [here](#list-of-errors) or on this
-[web-site](https://vald-phoenix.github.io/pylint-errors/) but you may want to
-do so. ### Stable release You can install a stable release simply by such
-commands: ```console $ python3 -m pip install plerr $ plerr r1710 ``` For
-[pipx](https://github.com/pipxproject/pipx): ```console $ python3 -m pip
-install pipx # if not yet installed pipx $ python3 -m pipx ensurepath # ensure
-directory where pipx stores apps is on PATH $ pipx install plerr $ plerr r1710
-``` ### Dev builds In order to use development `plerr` builds you need to
-invoke the following commands: ```console $ git clone https://github.com/vald-
-phoenix/pylint-errors.git $ sudo apt update && sudo apt install -y python3-pip
-# if not yet installed $ cd pylint-errors $ python3 setup.py test $ python3
-setup.py install --user $ python3 -m plerr r1710 ``` [pipx](https://github.com/
-pipxproject/pipx) users may install the library by such commands: ```console $
-git clone https://github.com/vald-phoenix/pylint-errors.git $ sudo apt install
--y make python3-pip python3-venv # if not yet installed $ cd pylint-errors $
-python3 -m pip install pipx wheel # install a package to build a wheel and pipx
-$ python3 -m pipx ensurepath # ensure directory where pipx stores apps is on
-PATH $ python3 setup.py test # run tests $ make clean $ python3 setup.py
-bdist_wheel # build a binary wheel $ pipx install dist/* # install a binary
-wheel by pipx $ plerr r1710 ``` In order to get the latest updates just `git
-pull origin master` and invoke a command in the root of the project (`sudo apt
-install make` if not yet installed) `make rai` to install to Python 3 user
-space site packages or `make raip` for pipx. ## List of errors Error codes with
-**[+]** mean they've got examples of bad and good code. Rationalisation
-provided for all entries. ### Async Checker Messages - [E1700 (yield-inside-
-async-function)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
-async/E1700) **[+]** - [E1701 (not-async-context-manager)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/async/E1701) **[+]** ### Basic
-Checker Messages - [C0102 (blacklisted-name)](https://vald-phoenix.github.io/
-pylint-errors/plerr/errors/basic/C0102) **[+]** - [C0103 (invalid-name)](https:
-//vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0103) **[+]** -
-[C0112 (empty-docstring)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/C0112) **[+]** - [C0114 (missing-module-docstring)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/C0114) **[+]** - [C0115
-(missing-class-docstring)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/C0115) **[+]** - [C0116 (missing-function-docstring)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0116) **[+]** - [C0121
-(singleton-comparison)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/C0121) **[+]** - [C0122 (misplaced-comparison-constant)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0122) **[+]** - [C0123
-(unidiomatic-typecheck)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/C0123) **[+]** - [E0100 (init-is-generator)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0100) **[+]** - [E0101
-(return-in-init)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
-basic/E0101) **[+]** - [E0102 (function-redefined)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0102) **[+]** - [E0103
-(not-in-loop)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
-E0103) **[+]** - [E0104 (return-outside-function)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0104) **[+]** - [E0105
-(yield-outside-function)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/E0105) **[+]** - [E0106 (return-arg-in-generator)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0106) - [E0107
-(nonexistent-operator)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/E0107) **[+]** - [E0108 (duplicate-argument-name)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/E0108) **[+]** - [E0110
-(abstract-class-instantiated)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/E0110) **[+]** - [E0111 (bad-reversed-sequence)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0111) **[+]** - [E0112
-(too-many-star-expressions)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/E0112) **[+]** - [E0113 (invalid-star-assignment-target)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0113) **[+]**
-- [E0114 (star-needs-assignment-target)](https://vald-phoenix.github.io/pylint-
-errors/plerr/errors/basic/E0114) **[+]** - [E0115 (nonlocal-and-global)](https:
-//vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0115) **[+]** -
-[E0116 (continue-in-finally)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/E0116) **[+]** - [E0117 (nonlocal-without-binding)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0117) **[+]** - [E0118
-(used-prior-global-declaration)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/E0118) **[+]** - [E0119 (misplaced-format-function)](https:/
-/vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0119) **[+]** -
-[R0123 (literal-comparison)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/R0123) **[+]** - [R0124 (comparison-with-itself)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/R0124) **[+]** - [W0101
-(unreachable)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
-W0101) **[+]** - [W0102 (dangerous-default-value)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0102) **[+]** - [W0104
-(pointless-statement)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0104) **[+]** - [W0105 (pointless-string-statement)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0105) **[+]** - [W0106
-(expression-not-assigned)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0106) **[+]** - [W0107 (unnecessary-pass)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0107) **[+]** - [W0108
-(unnecessary-lambda)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0108) **[+]** - [W0109 (duplicate-key)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0109) **[+]** - [W0111
-(assign-to-new-keyword)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0111) **[+]** - [W0120 (useless-else-on-loop)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0120) **[+]** - [W0122
-(exec-used)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
-W0122) **[+]** - [W0123 (eval-used)](https://vald-phoenix.github.io/pylint-
-errors/plerr/errors/basic/W0123) **[+]** - [W0124 (confusing-with-statement)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0124) **[+]**
-- [W0125 (using-constant-test)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/W0125) - [W0126 (missing-parentheses-for-call-in-test)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0126) -
-[W0127 (self-assigning-variable)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/basic/W0127) **[+]** - [W0128 (redeclared-assigned-name)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0128) - [W0143
-(comparison-with-callable)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/basic/W0143) **[+]** - [W0150 (lost-exception)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/basic/W0150) **[+]** - [W0199
-(assert-on-tuple)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
-basic/W0199) **[+]** ### Broad Try Clause Checker Messages - [W0717 (too-many-
-try-statements)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
-broad-try-clause/W0717) ### Classes Checker Messages - [C0202 (bad-classmethod-
-argument)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/
-C0202) **[+]** - [C0203 (bad-mcs-method-argument)](https://vald-
-phoenix.github.io/pylint-errors/plerr/errors/classes/C0203) **[+]** - [C0204
-(bad-mcs-classmethod-argument)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/classes/C0204) **[+]** - [C0205 (single-string-used-for-slots)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/C0205) **
-[+]** - [E0202 (method-hidden)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/classes/E0202) **[+]** - [E0203 (access-member-before-definition)]
-(https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0203) **
-[+]** - [E0211 (no-method-argument)](https://vald-phoenix.github.io/pylint-
-errors/plerr/errors/classes/E0211) **[+]** - [E0213 (no-self-argument)](https:/
-/vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0213) **[+]** -
-[E0236 (invalid-slots-object)](https://vald-phoenix.github.io/pylint-errors/
-plerr/errors/classes/E0236) **[+]** - [E0237 (assigning-non-slot)](https://
-vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0237) **[+]** -
-[E0238 (invalid-slots)](https://vald-phoenix.github.io/pylint-errors/plerr/
-errors/classes/E0238) **[+]** - [E0239 (inherit-non-class)](https://vald-
+![Example](https://raw.githubusercontent.com/vald-phoenix/pylint-errors/master/
+media/example.svg) ## Table of contents - [CLI usage](#cli-usage) - [Stable
+release](#stable-release) - [Dev builds](#dev-builds) - [List of errors](#list-
+of-errors) ## CLI usage It's not required to install CLI util as long as you
+can navigate list of errors [here](#list-of-errors) or on this [web-site]
+(https://vald-phoenix.github.io/pylint-errors/) but you may want to do so. ###
+Stable release You can install a stable release simply by such commands:
+```console $ python3 -m pip install plerr $ plerr r1710 ``` For [pipx](https://
+github.com/pipxproject/pipx): ```console $ python3 -m pip install pipx # if not
+yet installed pipx $ python3 -m pipx ensurepath # ensure directory where pipx
+stores apps is on PATH $ pipx install plerr $ plerr r1710 ``` ### Dev builds In
+order to use development `plerr` builds you need to invoke the following
+commands: ```console $ git clone https://github.com/vald-phoenix/pylint-
+errors.git $ sudo apt update && sudo apt install -y python3-pip # if not yet
+installed $ cd pylint-errors $ python3 setup.py test $ python3 setup.py install
+--user $ python3 -m plerr r1710 ``` [pipx](https://github.com/pipxproject/pipx)
+users may install the library by such commands: ```console $ git clone https://
+github.com/vald-phoenix/pylint-errors.git $ sudo apt install -y make python3-
+pip python3-venv # if not yet installed $ cd pylint-errors $ python3 -m pip
+install pipx wheel # install a package to build a wheel and pipx $ python3 -
+m pipx ensurepath # ensure directory where pipx stores apps is on PATH $
+python3 setup.py test # run tests $ make clean $ python3 setup.py bdist_wheel #
+build a binary wheel $ pipx install dist/* # install a binary wheel by pipx $
+plerr r1710 ``` In order to get the latest updates just `git pull origin
+master` and invoke a command in the root of the project (`sudo apt install
+make` if not yet installed) `make rai` to install to Python 3 user space site
+packages or `make raip` for pipx. ## List of errors Error codes with **[+]**
+mean they've got examples of bad and good code. Rationalisation provided for
+all entries. ### Async Checker Messages - [E1700 (yield-inside-async-function)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/async/E1700) **[+]**
+- [E1701 (not-async-context-manager)](https://vald-phoenix.github.io/pylint-
+errors/plerr/errors/async/E1701) **[+]** ### Basic Checker Messages - [C0102
+(blacklisted-name)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/C0102) **[+]** - [C0103 (invalid-name)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/basic/C0103) **[+]** - [C0112 (empty-docstring)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0112) **[+]**
+- [C0114 (missing-module-docstring)](https://vald-phoenix.github.io/pylint-
+errors/plerr/errors/basic/C0114) **[+]** - [C0115 (missing-class-docstring)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0115) **[+]**
+- [C0116 (missing-function-docstring)](https://vald-phoenix.github.io/pylint-
+errors/plerr/errors/basic/C0116) **[+]** - [C0121 (singleton-comparison)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/C0121) **[+]**
+- [C0122 (misplaced-comparison-constant)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/basic/C0122) **[+]** - [C0123 (unidiomatic-
+typecheck)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
+C0123) **[+]** - [E0100 (init-is-generator)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/basic/E0100) **[+]** - [E0101 (return-in-init)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0101) **[+]**
+- [E0102 (function-redefined)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/E0102) **[+]** - [E0103 (not-in-loop)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0103) **[+]** - [E0104
+(return-outside-function)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0104) **[+]** - [E0105 (yield-outside-function)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0105) **[+]** - [E0106
+(return-arg-in-generator)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0106) - [E0107 (nonexistent-operator)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0107) **[+]** - [E0108
+(duplicate-argument-name)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0108) **[+]** - [E0110 (abstract-class-instantiated)](https://
+vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0110) **[+]** - [E0111
+(bad-reversed-sequence)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0111) **[+]** - [E0112 (too-many-star-expressions)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0112) **[+]** - [E0113
+(invalid-star-assignment-target)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/E0113) **[+]** - [E0114 (star-needs-assignment-target)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0114) **[+]**
+- [E0115 (nonlocal-and-global)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/E0115) **[+]** - [E0116 (continue-in-finally)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/E0116) **[+]** - [E0117
+(nonlocal-without-binding)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/E0117) **[+]** - [E0118 (used-prior-global-declaration)](https://
+vald-phoenix.github.io/pylint-errors/plerr/errors/basic/E0118) **[+]** - [E0119
+(misplaced-format-function)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/E0119) **[+]** - [R0123 (literal-comparison)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/R0123) **[+]** - [R0124
+(comparison-with-itself)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/R0124) **[+]** - [W0101 (unreachable)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0101) **[+]** - [W0102
+(dangerous-default-value)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/W0102) **[+]** - [W0104 (pointless-statement)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0104) **[+]** - [W0105
+(pointless-string-statement)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/basic/W0105) **[+]** - [W0106 (expression-not-assigned)](https://
+vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0106) **[+]** - [W0107
+(unnecessary-pass)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/W0107) **[+]** - [W0108 (unnecessary-lambda)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0108) **[+]** - [W0109
+(duplicate-key)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/W0109) **[+]** - [W0111 (assign-to-new-keyword)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0111) **[+]** - [W0120
+(useless-else-on-loop)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/W0120) **[+]** - [W0122 (exec-used)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0122) **[+]** - [W0123
+(eval-used)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/
+W0123) **[+]** - [W0124 (confusing-with-statement)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0124) **[+]** - [W0125
+(using-constant-test)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/basic/W0125) - [W0126 (missing-parentheses-for-call-in-test)](https://
+vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0126) - [W0127 (self-
+assigning-variable)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/W0127) **[+]** - [W0128 (redeclared-assigned-name)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/basic/W0128) - [W0143 (comparison-
+with-callable)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+basic/W0143) **[+]** - [W0150 (lost-exception)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/basic/W0150) **[+]** - [W0199 (assert-on-tuple)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/basic/W0199) **[+]**
+### Broad Try Clause Checker Messages - [W0717 (too-many-try-statements)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/broad-try-clause/
+W0717) ### Classes Checker Messages - [C0202 (bad-classmethod-argument)](https:
+//vald-phoenix.github.io/pylint-errors/plerr/errors/classes/C0202) **[+]** -
+[C0203 (bad-mcs-method-argument)](https://vald-phoenix.github.io/pylint-errors/
+plerr/errors/classes/C0203) **[+]** - [C0204 (bad-mcs-classmethod-argument)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/C0204) **
+[+]** - [C0205 (single-string-used-for-slots)](https://vald-phoenix.github.io/
+pylint-errors/plerr/errors/classes/C0205) **[+]** - [E0202 (method-hidden)]
+(https://vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0202) **
+[+]** - [E0203 (access-member-before-definition)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/classes/E0203) **[+]** - [E0211
+(no-method-argument)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/classes/E0211) **[+]** - [E0213 (no-self-argument)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/classes/E0213) **[+]** - [E0236
+(invalid-slots-object)](https://vald-phoenix.github.io/pylint-errors/plerr/
+errors/classes/E0236) **[+]** - [E0237 (assigning-non-slot)](https://vald-
+phoenix.github.io/pylint-errors/plerr/errors/classes/E0237) **[+]** - [E0238
+(invalid-slots)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
+classes/E0238) **[+]** - [E0239 (inherit-non-class)](https://vald-
 phoenix.github.io/pylint-errors/plerr/errors/classes/E0239) **[+]** - [E0240
 (inconsistent-mro)](https://vald-phoenix.github.io/pylint-errors/plerr/errors/
 classes/E0240) **[+]** - [E0241 (duplicate-bases)](https://vald-
 phoenix.github.io/pylint-errors/plerr/errors/classes/E0241) **[+]** - [E0242
 (class-variable-slots-conflict)](https://vald-phoenix.github.io/pylint-errors/
 plerr/errors/classes/E0242) **[+]** - [E0301 (non-iterator-returned)](https://
 vald-phoenix.github.io/pylint-errors/plerr/errors/classes/E0301) **[+]** -
```

### Comparing `plerr-2.1.0/plerr.egg-info/SOURCES.txt` & `plerr-3.0.0/plerr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plerr-2.1.0/setup.py` & `plerr-3.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,26 +24,25 @@
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/vald-phoenix/pylint-errors',
     packages=setuptools.find_packages(),
     install_requires=['Pygments==2.12.0'],
     test_suite='plerr.tests.test_package',
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     include_package_data=True,
     keywords=['pylint', 'errors', 'documentation'],
     entry_points={'console_scripts': ['plerr=plerr.cli:main']},
     classifiers=[
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Software Development :: Documentation',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

