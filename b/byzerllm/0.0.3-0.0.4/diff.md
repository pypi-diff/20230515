# Comparing `tmp/byzerllm-0.0.3.tar.gz` & `tmp/byzerllm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byzerllm-0.0.3.tar", last modified: Wed Apr 26 03:16:20 2023, max compression
+gzip compressed data, was "dist/byzerllm-0.0.4.tar", last modified: Mon May 15 02:54:46 2023, max compression
```

## Comparing `byzerllm-0.0.3.tar` & `byzerllm-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,214 @@
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.102621 byzerllm-0.0.3/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      314 2023-04-26 03:16:20.102350 byzerllm-0.0.3/PKG-INFO
--rw-r--r--   0 allwefantasy   (501) staff       (20)       38 2023-04-26 03:16:20.102692 byzerllm-0.0.3/setup.cfg
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1205 2023-04-24 12:09:56.000000 byzerllm-0.0.3/setup.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.091097 byzerllm-0.0.3/src/
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.092495 byzerllm-0.0.3/src/byzerllm/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-04 03:26:20.000000 byzerllm-0.0.3/src/byzerllm/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.096000 byzerllm-0.0.3/src/byzerllm/chatglm6b/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-04 03:28:57.000000 byzerllm-0.0.3/src/byzerllm/chatglm6b/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     8182 2023-04-04 03:41:37.000000 byzerllm-0.0.3/src/byzerllm/chatglm6b/arguments.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21286 2023-04-20 03:53:12.000000 byzerllm-0.0.3/src/byzerllm/chatglm6b/finetune.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    11575 2023-04-04 03:39:19.000000 byzerllm-0.0.3/src/byzerllm/chatglm6b/trainer_seq2seq.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.097880 byzerllm-0.0.3/src/byzerllm/dolly/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:05.000000 byzerllm-0.0.3/src/byzerllm/dolly/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2029 2023-04-26 03:16:05.000000 byzerllm-0.0.3/src/byzerllm/dolly/consts.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1112 2023-04-26 03:16:05.000000 byzerllm-0.0.3/src/byzerllm/dolly/dolly_inference.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    10065 2023-04-26 03:16:05.000000 byzerllm-0.0.3/src/byzerllm/dolly/generate.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    12156 2023-04-26 03:16:05.000000 byzerllm-0.0.3/src/byzerllm/dolly/trainer.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.098892 byzerllm-0.0.3/src/byzerllm/moss/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    12657 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/finetune_moss.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.101769 byzerllm-0.0.3/src/byzerllm/moss/models/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/models/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5097 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/models/configuration_moss.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6735 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/models/custom_autotune.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31351 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/models/modeling_moss.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    18866 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/models/quantization.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    15952 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/models/tokenization_moss.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    17212 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/moss_inference.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)       22 2023-04-26 03:16:05.000000 byzerllm-0.0.3/src/byzerllm/version.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.093831 byzerllm-0.0.3/src/byzerllm.egg-info/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      314 2023-04-26 03:16:20.000000 byzerllm-0.0.3/src/byzerllm.egg-info/PKG-INFO
--rw-r--r--   0 allwefantasy   (501) staff       (20)      866 2023-04-26 03:16:20.000000 byzerllm-0.0.3/src/byzerllm.egg-info/SOURCES.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-04-26 03:16:20.000000 byzerllm-0.0.3/src/byzerllm.egg-info/dependency_links.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        9 2023-04-26 03:16:20.000000 byzerllm-0.0.3/src/byzerllm.egg-info/top_level.txt
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      411 2023-05-15 02:54:46.000000 byzerllm-0.0.4/PKG-INFO
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/test/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4822 2023-05-12 13:13:03.000000 byzerllm-0.0.4/test/test4.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1769 2023-05-12 13:13:03.000000 byzerllm-0.0.4/test/test5.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      161 2023-05-12 13:13:03.000000 byzerllm-0.0.4/test/test.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      788 2023-05-12 13:13:03.000000 byzerllm-0.0.4/test/test2.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2462 2023-05-12 13:14:31.000000 byzerllm-0.0.4/test/test6.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      541 2023-05-12 13:14:31.000000 byzerllm-0.0.4/test/test7.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      212 2023-05-12 13:13:03.000000 byzerllm-0.0.4/test/test3.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1254 2023-05-12 13:13:03.000000 byzerllm-0.0.4/setup.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       38 2023-05-15 02:54:46.000000 byzerllm-0.0.4/setup.cfg
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm/
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm/bark/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33373 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/generation.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     9139 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/model.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4243 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/api.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30020 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34444 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22660 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18660 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    49004 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21380 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    56628 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22180 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25116 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34020 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33004 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19620 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19676 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23036 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35300 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32580 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    54548 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22556 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26820 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32420 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    50548 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    58492 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29540 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28684 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    37380 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    43564 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21220 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    15516 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    53908 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    45324 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42548 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    44044 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35084 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    13436 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    36364 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34020 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26500 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29964 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42924 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30604 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33860 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    38124 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29324 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    38500 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35940 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39780 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    43084 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21916 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35724 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31460 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22396 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    51084 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42284 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    41268 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29004 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1943 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/readme.md
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16100 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25380 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    45748 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29220 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23356 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34180 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22396 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30500 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21276 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27940 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23356 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22180 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42764 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33380 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    56628 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24260 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31244 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33060 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    57852 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20100 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    36364 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    46604 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    45268 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24156 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24156 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    51668 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18980 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35940 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/en_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29164 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26020 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26396 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    52684 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/it_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16794 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/announcer.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    37964 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29060 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27620 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25436 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22716 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21380 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33380 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26500 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27620 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24580 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19620 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19676 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24956 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    44148 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35084 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34820 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20316 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24796 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30180 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    54548 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22556 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    58652 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25220 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31724 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24420 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/es_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    59348 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/de_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30284 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/assets/prompts/speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5955 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/model_fine.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4110 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/bark/bark_voice.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/moss/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    12657 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/finetune_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/moss/models/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5097 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/models/configuration_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18866 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/models/quantization.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6735 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/models/custom_autotune.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/models/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31351 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/models/modeling_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    15952 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/models/tokenization_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    17212 2023-04-24 12:08:52.000000 byzerllm-0.0.4/src/byzerllm/moss/moss_inference.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       22 2023-05-12 13:29:36.000000 byzerllm-0.0.4/src/byzerllm/version.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      699 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/utils/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2435 2023-05-12 13:14:31.000000 byzerllm-0.0.4/src/byzerllm/utils/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1065 2023-05-12 13:14:31.000000 byzerllm-0.0.4/src/byzerllm/utils/text_generator.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      689 2023-05-12 13:14:31.000000 byzerllm-0.0.4/src/byzerllm/utils/emb.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm/apps/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-05-12 13:14:31.000000 byzerllm-0.0.4/src/byzerllm/apps/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6201 2023-05-15 02:54:13.000000 byzerllm-0.0.4/src/byzerllm/apps/qa.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7620 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/config.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      277 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6263 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/other.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16907 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/common.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11082 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1404 2023-05-12 13:14:31.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/infer.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3000 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/tunning/finetune.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11575 2023-04-04 03:39:19.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/trainer_seq2seq.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8182 2023-04-04 03:41:37.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/arguments.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-04 03:28:57.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21286 2023-04-20 03:53:12.000000 byzerllm-0.0.4/src/byzerllm/chatglm6b/finetune.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/dolly/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10065 2023-04-26 03:16:05.000000 byzerllm-0.0.4/src/byzerllm/dolly/generate.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:05.000000 byzerllm-0.0.4/src/byzerllm/dolly/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2029 2023-04-26 03:16:05.000000 byzerllm-0.0.4/src/byzerllm/dolly/consts.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1112 2023-04-26 03:16:05.000000 byzerllm-0.0.4/src/byzerllm/dolly/dolly_inference.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    12156 2023-04-26 03:16:05.000000 byzerllm-0.0.4/src/byzerllm/dolly/trainer.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:46.000000 byzerllm-0.0.4/src/byzerllm/whisper/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1254 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/whisper/whisper_inference.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-05-12 13:13:03.000000 byzerllm-0.0.4/src/byzerllm/whisper/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm.egg-info/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      411 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm.egg-info/PKG-INFO
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8787 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm.egg-info/SOURCES.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        9 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm.egg-info/top_level.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-05-15 02:54:45.000000 byzerllm-0.0.4/src/byzerllm.egg-info/dependency_links.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `byzerllm-0.0.3/setup.py` & `byzerllm-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,16 +25,18 @@
     name="byzerllm",
     version=__version__,
     description="ByzerLLM: Byzer LLM",
     author="allwefantasy",
     long_description=readme_contents,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
-    packages=find_packages("src"),
-    package_data={},
+    packages=find_packages("src"),    
+    package_data={
+        "byzerllm":['bark/assets/**/*']
+    },
     install_requires=install_requires,
     classifiers=[        
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     requires_python=">=3.9",
```

### Comparing `byzerllm-0.0.3/src/byzerllm/chatglm6b/arguments.py` & `byzerllm-0.0.4/src/byzerllm/chatglm6b/arguments.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.3/src/byzerllm/chatglm6b/finetune.py` & `byzerllm-0.0.4/src/byzerllm/chatglm6b/finetune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.3/src/byzerllm/chatglm6b/trainer_seq2seq.py` & `byzerllm-0.0.4/src/byzerllm/chatglm6b/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.3/src/byzerllm/dolly/consts.py` & `byzerllm-0.0.4/src/byzerllm/dolly/consts.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.3/src/byzerllm/dolly/dolly_inference.py` & `byzerllm-0.0.4/src/byzerllm/dolly/dolly_inference.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.3/src/byzerllm/dolly/generate.py` & `byzerllm-0.0.4/src/byzerllm/dolly/generate.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.3/src/byzerllm/dolly/trainer.py` & `byzerllm-0.0.4/src/byzerllm/dolly/trainer.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.3/src/byzerllm/moss/finetune_moss.py` & `byzerllm-0.0.4/src/byzerllm/moss/finetune_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.3/src/byzerllm/moss/models/configuration_moss.py` & `byzerllm-0.0.4/src/byzerllm/moss/models/configuration_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.3/src/byzerllm/moss/models/custom_autotune.py` & `byzerllm-0.0.4/src/byzerllm/moss/models/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.3/src/byzerllm/moss/models/modeling_moss.py` & `byzerllm-0.0.4/src/byzerllm/moss/models/modeling_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.3/src/byzerllm/moss/models/quantization.py` & `byzerllm-0.0.4/src/byzerllm/moss/models/quantization.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.3/src/byzerllm/moss/models/tokenization_moss.py` & `byzerllm-0.0.4/src/byzerllm/moss/models/tokenization_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.3/src/byzerllm/moss/moss_inference.py` & `byzerllm-0.0.4/src/byzerllm/moss/moss_inference.py`

 * *Files identical despite different names*

