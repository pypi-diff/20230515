# Comparing `tmp/transphone-1.4.0.tar.gz` & `tmp/transphone-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transphone-1.4.0.tar", last modified: Mon May  8 16:32:49 2023, max compression
+gzip compressed data, was "dist/transphone-1.4.1.tar", last modified: Mon May 15 07:50:20 2023, max compression
```

## Comparing `transphone-1.4.0.tar` & `transphone-1.4.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1072 2022-10-27 20:49:08.000000 transphone-1.4.0/LICENSE
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-08 16:32:49.000000 transphone-1.4.0/PKG-INFO
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7611 2023-05-08 16:31:27.000000 transphone-1.4.0/README.md
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       38 2023-05-08 16:32:49.000000 transphone-1.4.0/setup.cfg
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      387 2023-05-08 16:31:27.000000 transphone-1.4.0/setup.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/test/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2730 2023-05-08 16:31:27.000000 transphone-1.4.0/test/test_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       47 2022-11-23 17:53:06.000000 transphone-1.4.0/transphone/__init__.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/bin/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:22.000000 transphone-1.4.0/transphone/bin/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1545 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/download_model.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3451 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/eval_epitran.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3551 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/eval_g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3634 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/eval_zsl_g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2844 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2679 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/tokenize.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3816 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/train_g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1618 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/update_model.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      325 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/config.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/data/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:30.000000 transphone-1.4.0/transphone/data/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9103 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/g2p.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/lang/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.0/transphone/lang/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1359 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/lang/base_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/lang/cmn/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.0/transphone/lang/cmn/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    55821 2022-11-24 02:03:19.000000 transphone-1.4.0/transphone/lang/cmn/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1605 2023-01-10 23:31:10.000000 transphone-1.4.0/transphone/lang/cmn/tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/lang/eng/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.0/transphone/lang/eng/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3341 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/lang/eng/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2099 2023-01-10 23:31:10.000000 transphone-1.4.0/transphone/lang/eng/tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6499 2023-01-27 23:36:45.000000 transphone-1.4.0/transphone/lang/epitran_tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1645 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/lang/g2p_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/lang/jpn/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.0/transphone/lang/jpn/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9740 2022-11-25 20:08:08.000000 transphone-1.4.0/transphone/lang/jpn/conv_table.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    15327 2022-11-25 20:04:35.000000 transphone-1.4.0/transphone/lang/jpn/jaconv.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9520 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/lang/jpn/kana2phoneme.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5192 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/lang/jpn/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2637 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/lang/jpn/tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/model/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:35.000000 transphone-1.4.0/transphone/model/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    13693 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/checkpoint_utils.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6628 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/dataset.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5388 2022-03-13 19:18:49.000000 transphone-1.4.0/transphone/model/ensemble.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1782 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/grapheme.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      409 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/loader.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8331 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/lstm.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7420 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/transformer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1722 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/utils.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1046 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/vocab.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/pretrained/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 18:28:14.000000 transphone-1.4.0/transphone/pretrained/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2536 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/run.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3764 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      491 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/utils.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone.egg-info/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone.egg-info/PKG-INFO
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1478 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone.egg-info/SOURCES.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        1 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone.egg-info/dependency_links.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      111 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone.egg-info/requires.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       11 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone.egg-info/top_level.txt
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 07:50:20.000000 transphone-1.4.1/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1072 2022-10-27 20:49:08.000000 transphone-1.4.1/LICENSE
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-15 07:50:20.000000 transphone-1.4.1/PKG-INFO
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8168 2023-05-15 07:50:03.000000 transphone-1.4.1/README.md
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       38 2023-05-15 07:50:20.000000 transphone-1.4.1/setup.cfg
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      387 2023-05-15 07:50:03.000000 transphone-1.4.1/setup.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 07:50:20.000000 transphone-1.4.1/test/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2730 2023-05-08 16:31:27.000000 transphone-1.4.1/test/test_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       47 2022-11-23 17:53:06.000000 transphone-1.4.1/transphone/__init__.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone/bin/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:22.000000 transphone-1.4.1/transphone/bin/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1545 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/bin/download_model.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3451 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/bin/eval_epitran.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3551 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/bin/eval_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3634 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/bin/eval_zsl_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2844 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/bin/g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2679 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/bin/tokenize.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3816 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/bin/train_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1618 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/bin/update_model.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      325 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/config.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone/data/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:30.000000 transphone-1.4.1/transphone/data/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9356 2023-05-15 07:50:03.000000 transphone-1.4.1/transphone/g2p.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone/lang/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.1/transphone/lang/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1359 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/lang/base_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone/lang/cmn/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.1/transphone/lang/cmn/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    55821 2022-11-24 02:03:19.000000 transphone-1.4.1/transphone/lang/cmn/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1750 2023-05-15 07:50:03.000000 transphone-1.4.1/transphone/lang/cmn/tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone/lang/eng/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.1/transphone/lang/eng/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3341 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/lang/eng/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2243 2023-05-15 07:50:03.000000 transphone-1.4.1/transphone/lang/eng/tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9381 2023-05-15 07:50:03.000000 transphone-1.4.1/transphone/lang/epitran_tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1822 2023-05-15 07:50:03.000000 transphone-1.4.1/transphone/lang/g2p_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone/lang/jpn/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.1/transphone/lang/jpn/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9740 2022-11-25 20:08:08.000000 transphone-1.4.1/transphone/lang/jpn/conv_table.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    15327 2022-11-25 20:04:35.000000 transphone-1.4.1/transphone/lang/jpn/jaconv.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9520 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/lang/jpn/kana2phoneme.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5192 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/lang/jpn/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2775 2023-05-15 07:50:03.000000 transphone-1.4.1/transphone/lang/jpn/tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone/model/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:35.000000 transphone-1.4.1/transphone/model/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    13693 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/model/checkpoint_utils.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6628 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/model/dataset.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5388 2022-03-13 19:18:49.000000 transphone-1.4.1/transphone/model/ensemble.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1782 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/model/grapheme.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      409 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/model/loader.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8331 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/model/lstm.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7420 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/model/transformer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1722 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/model/utils.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1046 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/model/vocab.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone/pretrained/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 18:28:14.000000 transphone-1.4.1/transphone/pretrained/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2536 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/run.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1350 2023-05-15 07:50:03.000000 transphone-1.4.1/transphone/tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      491 2023-05-08 16:31:27.000000 transphone-1.4.1/transphone/utils.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone.egg-info/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone.egg-info/PKG-INFO
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1478 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone.egg-info/SOURCES.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        1 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone.egg-info/dependency_links.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      111 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone.egg-info/requires.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       11 2023-05-15 07:50:20.000000 transphone-1.4.1/transphone.egg-info/top_level.txt
```

### Comparing `transphone-1.4.0/LICENSE` & `transphone-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/README.md` & `transphone-1.4.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 # transphone
 
 ![CI Test](https://github.com/xinjli/transphone/actions/workflows/python.yml/badge.svg)
 
-`transphone` is a grapheme-to-phoneme conversion toolkit. It provides phoneme tokenizers as well as approximation G2P model for 8000 languages.
-
-This repo contains our code and pretrained models roughly following our paper accepted at `Findings of ACL 2022`
-
-`Zero-shot Learning for Grapheme to Phoneme Conversion with Language Ensemble`
-
-It is a multilingual G2P (grapheme-to-phoneme) model that can be applied to all 8k languages registered in the [Glottolog database](https://glottolog.org/glottolog/language). You can read our papers at [Open Review](https://openreview.net/pdf?id=dKTTArRu8G2)
-
-Our approach:
-- We first trained our supervised multilingual model with ~900 languages using lexicons from [Wikitionary](https://en.wiktionary.org/wiki/Wiktionary:Main_Page)
-- if the target language (any language from the 8k languages) does not have any training set, we approximate its g2p model by using similar lanuguages from the supervised language sets and ensemble their inference results to obtain the target g2p.
+`transphone` is a multilingual grapheme-to-phoneme conversion toolkit derived from our paper: [Zero-shot Learning for Grapheme to Phoneme Conversion with Language Ensemble](https://aclanthology.org/2022.findings-acl.166/).
 
+It provides approximiated phoneme tokenizers and G2P model for 7546 languages registered in the [Glottolog database](https://glottolog.org/glottolog/language).  You can see the full list of supported languages in [the language doc](./doc/language.md) 
 
 ## Install
 
 transphone is available from pip
 
 ```bash
 pip install transphone
@@ -25,33 +16,33 @@
 
 You can clone this repository and install
 
 ```bash
 python setup.py install
 ```
 
-## Usage
-
-### Tokenizer interface
+## Tokenizer Usage
 
-The tokenizer converts a string into each languages' phonemes
+The tokenizer converts a string into each languages' phonemes. By default, it combines a few approach to decide the pronunciation of a word for the target language:
 
-It will use the following strategy to decide pronunciation
+- **lexicon-based**: it will first lookup lexicon dictionary for pronunciation (from Wikitionary, cmudict, and other sources), currently around 1k languages have at least some entries.
+- **transducer-based**: it will use rule-based transducer from [epitran](https://github.com/dmort27/epitran) for several languages considering accuracy and speed. 
+- **g2p-based**: use the G2P model as described in the next section.
 
-- it will first lookup lexicon dictionary for pronunciation (from Wikitionary, cmudict, and other sources)
-- try identifying rule-based transducer from [Epitran](https://github.com/dmort27/epitran) if supported.
-- fall back to the G2P engine if both previous options are not available.  
+### python interface
 
-Currently, more than 200 languages have lexicon available inside, about 100 languages have epitran supported. Other languages will use G2P instead.
+You can use it from python as follows:
 
 ```python
 In [1]: from transphone import read_tokenizer                                                                                                  
 
+# use 2-char or 3-char ISO id to specify your target language 
 In [2]: eng = read_tokenizer('eng')                                                                                                            
 
+# tokenize a string of text into a list of phonemes
 In [3]: lst = eng.tokenize('hello world')                                                                                                      
 
 In [4]: lst                                                                                                                                    
 Out[4]: ['h', 'ʌ', 'l', 'o', 'w', 'w', 'ɹ̩', 'l', 'd']
 
 In [5]: ids = eng.convert_tokens_to_ids(lst)                                                                                                   
 
@@ -74,17 +65,17 @@
 In [12]: deu = read_tokenizer('deu')                                    
 
 In [13]: deu.tokenize('Hallo Welt')                                     
 Out[13]: ['h', 'a', 'l', 'o', 'v', 'e', 'l', 't']
 
 ```
 
-### G2P Command line
+### command line interface
 
-A command line tool is available
+A command line tool is also available
 
 ```bash
 # compute pronunciation for every word in input file
 $ python -m transphone.run --lang eng --input sample.txt 
 h ɛ l o ʊ
 w ə l d
 t ɹ æ n s f ə ʊ n
@@ -92,15 +83,19 @@
 # by specifying combine flag, you can get word + pronunciation per line
 $ python -m transphone.run --lang eng --input sample.txt --combine=True
 hello h ɛ l o ʊ
 world w ə l d
 transphone t ɹ æ n s f ə ʊ n
 ```
 
-### python G2P interface
+## G2P Backend Usage
+
+The tokenizer in the previous section uses the G2P as one of the backend option. You can also use the G2P model directly.
+
+### python interface
 
 A simple python usage is as follows:
 
 ```python
 In [1]: from transphone.g2p import read_g2p                                                                                                     
 
 # read a pretrained model. It will download the pretrained model automatically into repo_root/data/model
@@ -128,21 +123,40 @@
 gwe   ['t', 'l', 'a', 'n', 's', 'f', 'o', 'n', 'e']
 ibo   ['t', 'l', 'a', 'n', 's', 'p', 'o', 'n', 'e']
 kam   ['t', 'l', 'a', 'n', 's', 'f', 'o', 'n', 'e']
 kik   ['t', 'l', 'a', 'n', 's', 'f', 'ɔ', 'n', 'ɛ']
 Out[5]: ['t', 'l', 'a', 'n', 's', 'f', 'o', 'n', 'e']
 ```
 
-## G2P Models
+### Pretrained Models
+
+This pretrained models roughly following our paper accepted at `Findings of ACL 2022`: [Zero-shot Learning for Grapheme to Phoneme Conversion with Language Ensemble](https://aclanthology.org/2022.findings-acl.166/). 
 
 You can see the G2P evaluation over 1k languages on the [performance doc](./doc/performance/README.md)
 
 Note this is the pure G2P evaluation on unseen words. The tokenizer combines other existing resources (i.e. lexicon) as well, so the tokenizer's performance is expected to be much better than this. 
 
 |        model         | # supported languages | supervised language PER | zero-shot language PER |       description        |
 |:--------------------:|:---------------------:|:-----------------------:|:----------------------:|:------------------------:|
 | 042801_base (latest) |          ~8k          |           13%           |          31%           | based on our work at [1] |
 
+### Training
+
+We also provide the training code for G2P. You can reproduce the pretrained model using `transphone.bin.train_g2p` 
+
+## Epitran backend
+
+This repo also provides a wrapper of a customized version of [epitran](https://github.com/dmort27/epitran). For a few languages, it will use epitran as the backend considering accuracy and speed.
+
+You can also use epitran directly as follows:
+
+```python
+In [1]: tokenizer = read_epitran_tokenizer('spa', use_lexicon=False)
+
+In [2]: tokenizer.tokenize('hola')
+Out[2]: ['o', 'l', 'a']
+```
+
 ## Reference
 
 - [1] Li, Xinjian, et al. "Zero-shot Learning for Grapheme to Phoneme Conversion with Language Ensemble." Findings of the Association for Computational Linguistics: ACL 2022. 2022.
 - [2] Li, Xinjian, et al. "Phone Inventories and Recognition for Every Language" LREC 2022. 2022
```

### Comparing `transphone-1.4.0/test/test_tokenizer.py` & `transphone-1.4.1/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/bin/download_model.py` & `transphone-1.4.1/transphone/bin/download_model.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/bin/eval_epitran.py` & `transphone-1.4.1/transphone/bin/eval_epitran.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/bin/eval_g2p.py` & `transphone-1.4.1/transphone/bin/eval_g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/bin/eval_zsl_g2p.py` & `transphone-1.4.1/transphone/bin/eval_zsl_g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/bin/g2p.py` & `transphone-1.4.1/transphone/bin/g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/bin/tokenize.py` & `transphone-1.4.1/transphone/bin/tokenize.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/bin/train_g2p.py` & `transphone-1.4.1/transphone/bin/train_g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/bin/update_model.py` & `transphone-1.4.1/transphone/bin/update_model.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/g2p.py` & `transphone-1.4.1/transphone/g2p.py`

 * *Files 5% similar despite different names*

```diff
@@ -188,33 +188,41 @@
 
         for target_lang_id in target_langs:
             lang_tag = '<' + target_lang_id + '>'
 
             graphemes = [lang_tag]+[w.lower() for w in list(word)]
 
             grapheme_ids = []
+            normalized_graphemes = []
+
             for grapheme in graphemes:
                 if grapheme not in self.grapheme_vocab:
 
                     # romanize chars not available in training languages
                     romans = list(unidecode.unidecode(grapheme))
 
                     if verbose:
                         print("WARNING: not found grapheme ", grapheme, " in vocab. use ", romans, " instead")
 
                     for roman in romans:
 
                         # discard special chars such as $
                         if roman in self.grapheme_vocab:
                             grapheme_ids.append(self.grapheme_vocab.atoi(roman))
+                            normalized_graphemes.append(roman)
                     continue
+
+                normalized_graphemes.append(grapheme)
                 grapheme_ids.append(self.grapheme_vocab.atoi(grapheme))
 
             grapheme_input.append(grapheme_ids)
 
+            if verbose:
+                print(f"normalized: {word} -> {normalized_graphemes}")
+
         x = torch.LongTensor(grapheme_input).to(TransphoneConfig.device)
 
         phone_output = self.model.inference_batch(x)
 
         for target_lang_id, phone_ids in zip(target_langs, phone_output):
             phones = [self.phoneme_vocab.itoa(phone) for phone in phone_ids]
```

### Comparing `transphone-1.4.0/transphone/lang/base_tokenizer.py` & `transphone-1.4.1/transphone/lang/base_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/lang/cmn/normalizer.py` & `transphone-1.4.1/transphone/lang/cmn/normalizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/lang/cmn/tokenizer.py` & `transphone-1.4.1/transphone/lang/cmn/tokenizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from transphone.utils import import_with_auto_install
 from transphone.lang.base_tokenizer import BaseTokenizer
 from phonepiece.pinyin import PinyinConverter
 from transphone.lang.cmn.normalizer import CMNNormalizer
 
+
+def read_cmn_tokenizer(lang_id='cmn', g2p_model='latest', device=None, use_lexicon=True):
+    return CMNTokenizer(lang_id, g2p_model, device)
+
+
 class CMNTokenizer(BaseTokenizer):
 
     def __init__(self, lang_id='cmn', g2p_model='latest', device=None):
 
         super().__init__(lang_id, g2p_model, device)
 
         # import jieba and pypinyin for segmentation
```

### Comparing `transphone-1.4.0/transphone/lang/eng/normalizer.py` & `transphone-1.4.1/transphone/lang/eng/normalizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/lang/eng/tokenizer.py` & `transphone-1.4.1/transphone/lang/eng/tokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from transphone.utils import import_with_auto_install
 from transphone.lang.base_tokenizer import BaseTokenizer
 from phonepiece.arpa import ArpaConverter
 from transphone.lang.eng.normalizer import ENGNormalizer
 
+def read_eng_tokenizer(lang_id='eng', g2p_model='latest', device=None, use_lexicon=True):
+    return ENGTokenizer(lang_id, g2p_model, device)
+
+
 class ENGTokenizer(BaseTokenizer):
 
     def __init__(self, lang_id='eng', g2p_model='latest', device=None):
 
         super().__init__(lang_id, g2p_model, device)
 
         # import jieba and pypinyin for segmentation
```

### Comparing `transphone-1.4.0/transphone/lang/g2p_tokenizer.py` & `transphone-1.4.1/transphone/lang/g2p_tokenizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from phonepiece.lang import normalize_lang_id
 from phonepiece.lexicon import read_lexicon
 from transphone.lang.base_tokenizer import BaseTokenizer
 
 
+def read_g2p_tokenizer(lang_id, g2p_model='latest', device=None):
+    lang_id = normalize_lang_id(lang_id)
+    return G2PTokenizer(lang_id, g2p_model, device)
+
 class G2PTokenizer(BaseTokenizer):
 
     def __init__(self, lang_id, g2p_model='latest', device=None):
         super().__init__(lang_id, g2p_model, device)
 
         self.lexicon = read_lexicon(lang_id)
 
@@ -32,15 +36,15 @@
                 result.extend(phonemes)
                 self.cache[word] = phonemes
                 log = f"lexicon {word} -> {phonemes}"
                 self.logger.info(log)
                 if verbose:
                     print(log)
             else:
-                phonemes = self.g2p.inference_batch(word, self.lang_id)
+                phonemes = self.g2p.inference_batch(word, self.lang_id, verbose=verbose)
                 remapped_phonemes = self.inventory.remap(phonemes)
 
                 log = f"g2p batch mode: {word} ->  {remapped_phonemes}"
                 self.logger.info(log)
                 if verbose:
                     print(log)
                 self.cache[word] = remapped_phonemes
```

### Comparing `transphone-1.4.0/transphone/lang/jpn/conv_table.py` & `transphone-1.4.1/transphone/lang/jpn/conv_table.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/lang/jpn/jaconv.py` & `transphone-1.4.1/transphone/lang/jpn/jaconv.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/lang/jpn/kana2phoneme.py` & `transphone-1.4.1/transphone/lang/jpn/kana2phoneme.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/lang/jpn/normalizer.py` & `transphone-1.4.1/transphone/lang/jpn/normalizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/lang/jpn/tokenizer.py` & `transphone-1.4.1/transphone/lang/jpn/tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 from transphone.lang.jpn.kana2phoneme import Kana2Phoneme
 from transphone.g2p import read_g2p
 from phonepiece.inventory import read_inventory
 from transphone.lang.jpn import jaconv
 from transphone.lang.base_tokenizer import BaseTokenizer
 from transphone.lang.jpn.normalizer import normalize_neologd, parse_jpn_number, parse_jpn_alphabet
 
+
+def read_jpn_tokenizer(lang_id, g2p_model='latest', device=None, use_lexicon=True):
+    return JPNTokenizer(lang_id, g2p_model, device)
+
 class JPNTokenizer(BaseTokenizer):
 
     def __init__(self, lang_id, g2p_model='latest', device=None):
 
         super().__init__(lang_id, g2p_model, device)
 
         # import mecab and its dict
```

### Comparing `transphone-1.4.0/transphone/model/checkpoint_utils.py` & `transphone-1.4.1/transphone/model/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/model/dataset.py` & `transphone-1.4.1/transphone/model/dataset.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/model/ensemble.py` & `transphone-1.4.1/transphone/model/ensemble.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/model/grapheme.py` & `transphone-1.4.1/transphone/model/grapheme.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/model/lstm.py` & `transphone-1.4.1/transphone/model/lstm.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/model/transformer.py` & `transphone-1.4.1/transphone/model/transformer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/model/utils.py` & `transphone-1.4.1/transphone/model/utils.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/model/vocab.py` & `transphone-1.4.1/transphone/model/vocab.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone/run.py` & `transphone-1.4.1/transphone/run.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.0/transphone.egg-info/SOURCES.txt` & `transphone-1.4.1/transphone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

