# Comparing `tmp/phonepiece-1.4.0.tar.gz` & `tmp/phonepiece-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phonepiece-1.4.0.tar", last modified: Mon May  8 07:39:00 2023, max compression
+gzip compressed data, was "dist/phonepiece-1.4.2.tar", last modified: Mon May 15 08:10:13 2023, max compression
```

## Comparing `phonepiece-1.4.0.tar` & `phonepiece-1.4.2.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 07:39:00.000000 phonepiece-1.4.0/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    22240 2022-11-27 22:18:32.000000 phonepiece-1.4.0/LICENSE.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      266 2023-05-08 07:39:00.000000 phonepiece-1.4.0/PKG-INFO
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6709 2023-05-08 07:38:53.000000 phonepiece-1.4.0/README.md
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       47 2022-09-01 15:22:55.000000 phonepiece-1.4.0/phonepiece/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1896 2023-04-26 09:50:41.000000 phonepiece-1.4.0/phonepiece/arpa.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece/bin/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:48:28.000000 phonepiece-1.4.0/phonepiece/bin/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1404 2022-09-08 18:19:22.000000 phonepiece-1.4.0/phonepiece/bin/download_model.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     4402 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/bin/eval_distance.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1479 2023-01-06 00:58:31.000000 phonepiece-1.4.0/phonepiece/bin/update_model.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      248 2022-11-28 19:48:04.000000 phonepiece-1.4.0/phonepiece/config.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece/data/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 18:20:26.000000 phonepiece-1.4.0/phonepiece/data/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      256 2021-06-23 15:57:09.000000 phonepiece-1.4.0/phonepiece/data/arpabet.csv
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     4351 2022-11-28 17:35:17.000000 phonepiece-1.4.0/phonepiece/data/ipa-xsampa.csv
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   363488 2022-11-28 17:35:17.000000 phonepiece-1.4.0/phonepiece/data/ipa_all.csv
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7452 2023-02-14 03:40:22.000000 phonepiece-1.4.0/phonepiece/data/ipa_base.csv
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   232037 2020-03-04 19:47:15.000000 phonepiece-1.4.0/phonepiece/data/language.tsv
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   175859 2020-06-27 15:14:04.000000 phonepiece-1.4.0/phonepiece/data/phoible-segments-features.tsv
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      559 2022-11-23 19:56:36.000000 phonepiece-1.4.0/phonepiece/data/pinyin2ipa.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   575995 2021-07-28 15:08:54.000000 phonepiece-1.4.0/phonepiece/data/tree.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9598 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/distance.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2116 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/epitran.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9245 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/inventory.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7268 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/ipa.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3577 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/lang.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2731 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/lexicon.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     4257 2023-01-23 20:09:34.000000 phonepiece-1.4.0/phonepiece/pinyin.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1398 2023-02-17 19:39:59.000000 phonepiece-1.4.0/phonepiece/timit.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5613 2023-01-29 19:56:05.000000 phonepiece-1.4.0/phonepiece/unit.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1602 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/utils.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece.egg-info/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      266 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece.egg-info/PKG-INFO
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      972 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece.egg-info/SOURCES.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        1 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece.egg-info/dependency_links.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       43 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece.egg-info/requires.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       11 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece.egg-info/top_level.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       38 2023-05-08 07:39:00.000000 phonepiece-1.4.0/setup.cfg
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      491 2023-05-08 07:38:53.000000 phonepiece-1.4.0/setup.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 07:39:00.000000 phonepiece-1.4.0/test/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      265 2023-05-08 07:38:53.000000 phonepiece-1.4.0/test/test_distance.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      589 2023-01-20 21:23:48.000000 phonepiece-1.4.0/test/test_epitran.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1048 2023-01-29 19:58:17.000000 phonepiece-1.4.0/test/test_inventory.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1684 2023-02-14 03:40:22.000000 phonepiece-1.4.0/test/test_ipa.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      221 2023-01-06 00:52:08.000000 phonepiece-1.4.0/test/test_lexicon.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 08:10:13.000000 phonepiece-1.4.2/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    22240 2022-11-27 22:18:32.000000 phonepiece-1.4.2/LICENSE.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      266 2023-05-15 08:10:13.000000 phonepiece-1.4.2/PKG-INFO
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6709 2023-05-08 07:38:53.000000 phonepiece-1.4.2/README.md
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 08:10:13.000000 phonepiece-1.4.2/phonepiece/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       47 2022-09-01 15:22:55.000000 phonepiece-1.4.2/phonepiece/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1896 2023-04-26 09:50:41.000000 phonepiece-1.4.2/phonepiece/arpa.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 08:10:13.000000 phonepiece-1.4.2/phonepiece/bin/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:48:28.000000 phonepiece-1.4.2/phonepiece/bin/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1404 2022-09-08 18:19:22.000000 phonepiece-1.4.2/phonepiece/bin/download_model.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     4898 2023-05-15 08:04:55.000000 phonepiece-1.4.2/phonepiece/bin/eval_distance.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1018 2023-05-15 08:04:55.000000 phonepiece-1.4.2/phonepiece/bin/info.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      497 2023-05-15 08:04:55.000000 phonepiece-1.4.2/phonepiece/bin/list_lang.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1479 2023-01-06 00:58:31.000000 phonepiece-1.4.2/phonepiece/bin/update_model.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      248 2022-11-28 19:48:04.000000 phonepiece-1.4.2/phonepiece/config.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 08:10:13.000000 phonepiece-1.4.2/phonepiece/data/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 18:20:26.000000 phonepiece-1.4.2/phonepiece/data/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      256 2021-06-23 15:57:09.000000 phonepiece-1.4.2/phonepiece/data/arpabet.csv
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     4351 2022-11-28 17:35:17.000000 phonepiece-1.4.2/phonepiece/data/ipa-xsampa.csv
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   363488 2022-11-28 17:35:17.000000 phonepiece-1.4.2/phonepiece/data/ipa_all.csv
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7452 2023-02-14 03:40:22.000000 phonepiece-1.4.2/phonepiece/data/ipa_base.csv
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   232037 2020-03-04 19:47:15.000000 phonepiece-1.4.2/phonepiece/data/language.tsv
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   175859 2020-06-27 15:14:04.000000 phonepiece-1.4.2/phonepiece/data/phoible-segments-features.tsv
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      559 2022-11-23 19:56:36.000000 phonepiece-1.4.2/phonepiece/data/pinyin2ipa.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   575995 2021-07-28 15:08:54.000000 phonepiece-1.4.2/phonepiece/data/tree.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9598 2023-05-08 07:38:53.000000 phonepiece-1.4.2/phonepiece/distance.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2116 2023-05-08 07:38:53.000000 phonepiece-1.4.2/phonepiece/epitran.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    10983 2023-05-15 08:04:55.000000 phonepiece-1.4.2/phonepiece/inventory.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7286 2023-05-15 08:04:55.000000 phonepiece-1.4.2/phonepiece/ipa.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3718 2023-05-15 08:04:55.000000 phonepiece-1.4.2/phonepiece/lang.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2731 2023-05-08 07:38:53.000000 phonepiece-1.4.2/phonepiece/lexicon.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     4257 2023-01-23 20:09:34.000000 phonepiece-1.4.2/phonepiece/pinyin.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1398 2023-02-17 19:39:59.000000 phonepiece-1.4.2/phonepiece/timit.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5737 2023-05-15 08:04:55.000000 phonepiece-1.4.2/phonepiece/unit.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1602 2023-05-08 07:38:53.000000 phonepiece-1.4.2/phonepiece/utils.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 08:10:13.000000 phonepiece-1.4.2/phonepiece.egg-info/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      266 2023-05-15 08:10:13.000000 phonepiece-1.4.2/phonepiece.egg-info/PKG-INFO
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1023 2023-05-15 08:10:13.000000 phonepiece-1.4.2/phonepiece.egg-info/SOURCES.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        1 2023-05-15 08:10:13.000000 phonepiece-1.4.2/phonepiece.egg-info/dependency_links.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       43 2023-05-15 08:10:13.000000 phonepiece-1.4.2/phonepiece.egg-info/requires.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       11 2023-05-15 08:10:13.000000 phonepiece-1.4.2/phonepiece.egg-info/top_level.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       38 2023-05-15 08:10:13.000000 phonepiece-1.4.2/setup.cfg
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      491 2023-05-15 08:04:55.000000 phonepiece-1.4.2/setup.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 08:10:13.000000 phonepiece-1.4.2/test/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      323 2023-05-15 08:04:55.000000 phonepiece-1.4.2/test/test_distance.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      589 2023-01-20 21:23:48.000000 phonepiece-1.4.2/test/test_epitran.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1048 2023-01-29 19:58:17.000000 phonepiece-1.4.2/test/test_inventory.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1684 2023-02-14 03:40:22.000000 phonepiece-1.4.2/test/test_ipa.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      221 2023-01-06 00:52:08.000000 phonepiece-1.4.2/test/test_lexicon.py
```

### Comparing `phonepiece-1.4.0/LICENSE.txt` & `phonepiece-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/README.md` & `phonepiece-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/arpa.py` & `phonepiece-1.4.2/phonepiece/arpa.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/bin/download_model.py` & `phonepiece-1.4.2/phonepiece/bin/download_model.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/bin/eval_distance.py` & `phonepiece-1.4.2/phonepiece/bin/eval_distance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,16 @@
 import sys
 from pathlib import Path
 from phonepiece.distance import phonological_distance, fast_edit_distance, edit_distance
 import argparse
 from tqdm import tqdm
 from collections import Counter
 
-if __name__ == '__main__':
-
-    parser = argparse.ArgumentParser(description='Read the contents of two files.')
-    parser.add_argument( '--hyp', help='the path to the hypothesis file')
-    parser.add_argument('--ref', help='the path to the reference file')
-    parser.add_argument('-f', '--format', default='kaldi', help='kaldi or text')
-    parser.add_argument('-o', '--output', help='the path to the reference file')
-    parser.add_argument('-v', '--verbose', type=bool ,default=False)
-
-    args = parser.parse_args()
-    output = args.output
-    ref = args.ref
-    hyp = args.hyp
-    verbose = args.verbose
-    file_format = args.format
 
-    assert file_format in ['kaldi', 'text']
+def eval_distance(hyp, ref, output=None, file_format='kaldi', verbose=True, return_counter=False):
 
     w = None
     if output is not None:
         Path(output).parent.mkdir(exist_ok=True, parents=True)
         w = open(output, "w")
 
     expect_label = {}
@@ -47,15 +32,15 @@
     tot_sub_cnt = 0
     tot_del_cnt = 0
 
     add_counter = Counter()
     del_counter = Counter()
     sub_counter = Counter()
 
-    for i, line in tqdm(enumerate(open(hyp, 'r').readlines())):
+    for i, line in enumerate(tqdm(open(hyp, 'r').readlines())):
         fields = line.strip().split()
 
         if file_format == 'kaldi':
             utt_id = fields[0]
             hyp = fields[1:]
         else:
             utt_id = f"{i:05d}"
@@ -82,17 +67,17 @@
             err_cnt = fast_edit_distance(ref, hyp)
 
         tot_err_cnt += err_cnt
         tot_dst_cnt += dst_cnt
         tot_len_cnt += all_cnt
 
     print(f"------------------------------------")
-    print(f"TOTAL ERR: {tot_err_cnt}\n")
-    print(f"TOTAL DST: {tot_dst_cnt}\n")
-    print(f"TOTAL LEN: {tot_len_cnt}\n")
+    print(f"TOTAL ERR: {tot_err_cnt}")
+    print(f"TOTAL DST: {tot_dst_cnt:.3f}")
+    print(f"TOTAL LEN: {tot_len_cnt}")
 
     if verbose:
         print(f"TOTAL ADD {tot_add_cnt:.3f}: {add_counter.most_common(10)}")
         print(f"TOTAL DEL {tot_del_cnt:.3f}: {del_counter.most_common(10)}")
         print(f"TOTAL SUB {tot_sub_cnt:.3f}: {sub_counter.most_common(10)}")
 
     if tot_len_cnt != 0:
@@ -123,8 +108,43 @@
                 w.write(f"TOTAL ADD RATE: {tot_add_cnt / tot_len_cnt:.3f}\n")
                 w.write(f"TOTAL DEL RATE: {tot_del_cnt / tot_len_cnt:.3f}\n")
                 w.write(f"TOTAL SUB RATE: {tot_sub_cnt / tot_len_cnt:.3f}\n")
 
             w.write(f"TOTAL DST RATE: {tot_dst_cnt/tot_len_cnt:.3f}\n")
 
         w.write(f"------------------------------------\n")
-        w.close()
+        w.close()
+
+    err_rate = 0
+    if tot_len_cnt != 0:
+        err_rate = tot_err_cnt/tot_len_cnt
+
+    dst_rate = 0
+    if tot_len_cnt != 0:
+        dst_rate = tot_dst_cnt/tot_len_cnt
+
+    if return_counter:
+        return (err_rate, dst_rate, add_counter, del_counter, sub_counter)
+    else:
+        return (err_rate, dst_rate)
+
+
+
+if __name__ == '__main__':
+
+    parser = argparse.ArgumentParser(description='Read the contents of two files.')
+    parser.add_argument( '--hyp', help='the path to the hypothesis file')
+    parser.add_argument('--ref', help='the path to the reference file')
+    parser.add_argument('-f', '--format', default='kaldi', help='kaldi or text')
+    parser.add_argument('-o', '--output', help='the path to the reference file')
+    parser.add_argument('-v', '--verbose', type=bool ,default=True)
+
+    args = parser.parse_args()
+    output = args.output
+    ref = args.ref
+    hyp = args.hyp
+    verbose = args.verbose
+    file_format = args.format
+
+    assert file_format in ['kaldi', 'text']
+
+    eval_distance(hyp, ref, output, file_format=file_format, verbose=verbose)
```

### Comparing `phonepiece-1.4.0/phonepiece/bin/update_model.py` & `phonepiece-1.4.2/phonepiece/bin/update_model.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/data/ipa-xsampa.csv` & `phonepiece-1.4.2/phonepiece/data/ipa-xsampa.csv`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/data/ipa_all.csv` & `phonepiece-1.4.2/phonepiece/data/ipa_all.csv`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/data/ipa_base.csv` & `phonepiece-1.4.2/phonepiece/data/ipa_base.csv`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/data/language.tsv` & `phonepiece-1.4.2/phonepiece/data/language.tsv`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/data/phoible-segments-features.tsv` & `phonepiece-1.4.2/phonepiece/data/phoible-segments-features.tsv`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/data/pinyin2ipa.txt` & `phonepiece-1.4.2/phonepiece/data/pinyin2ipa.txt`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/data/tree.txt` & `phonepiece-1.4.2/phonepiece/data/tree.txt`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/distance.py` & `phonepiece-1.4.2/phonepiece/distance.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/epitran.py` & `phonepiece-1.4.2/phonepiece/epitran.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/inventory.py` & `phonepiece-1.4.2/phonepiece/inventory.py`

 * *Files 23% similar despite different names*

```diff
@@ -121,51 +121,102 @@
 
     for phoneme in inv.phoneme.elems[1:-1]:
         w.write(phoneme+' '+' '.join(allophone[phoneme])+'\n')
 
     w.close()
 
 
-def create_inventory(lang_id, phoneme_lst):
+def create_inventory(lang_id, phoneme_lst_or_phoneme2phone):
     """
     a simple interfact to create an customized inventory from a phoneme set.
     Assume each phoneme is realized by the same phone
 
     :param lang_id:
     :type lang_id: str
     :param phoneme_lst:
     :type phoneme_lst:
     :return:
     :rtype:
     """
 
-    phoneme_lst = sorted(list(phoneme_lst))
-    phoneme_unit = create_unit(phoneme_lst)
-    phone_unit = create_unit(phoneme_lst)
+    if isinstance(phoneme_lst_or_phoneme2phone, list):
+
+        phoneme_lst = phoneme_lst_or_phoneme2phone
+
+        phoneme_lst = sorted(list(phoneme_lst))
+        phoneme_unit = create_unit(phoneme_lst)
+        phone_unit = create_unit(phoneme_lst)
+
+        phone2phoneme = defaultdict(list)
+        phoneme2phone = defaultdict(list)
+
+        for phoneme in phoneme_lst:
+            phone2phoneme[phoneme] = [phoneme]
+            phoneme2phone[phoneme] = [phoneme]
+
+        # blk and eos would be considered as phone/phonemes as well
+        phone2phoneme['<blk>'] = ['<blk>']
+        phone2phoneme['<eos>'] = ['<eos>']
+        phoneme2phone['<blk>'] = ['<blk>']
+        phoneme2phone['<eos>'] = ['<eos>']
+
+        model_name = 'customized'
+
+        return Inventory(lang_id, model_name, phoneme_unit, phone_unit, phone2phoneme, phoneme2phone)
+
+    else:
+        assert isinstance(phoneme_lst_or_phoneme2phone, dict)
+
+        phoneme2phone = phoneme_lst_or_phoneme2phone
+        phoneme_lst = sorted(list(phoneme2phone.keys()))
+        phoneme_unit = create_unit(phoneme_lst)
+
+        phone2phoneme = defaultdict(list)
+
+        for phoneme, phone_lst in phoneme2phone.items():
+            for phone in phone_lst:
+                phone2phoneme[phone].append(phoneme)
+
+        phone_lst = sorted(list(phone2phoneme.keys()))
+        phone_unit = create_unit(phone_lst)
+
+        model_name = 'customized'
+
+        phone2phoneme['<blk>'] = ['<blk>']
+        phone2phoneme['<eos>'] = ['<eos>']
+        phoneme2phone['<blk>'] = ['<blk>']
+        phoneme2phone['<eos>'] = ['<eos>']
+
+        return Inventory(lang_id, model_name, phoneme_unit, phone_unit, phone2phoneme, phoneme2phone)
+
+
+def create_inventory_from_phone2phoneme(lang_id, phone2phoneme):
+
+    phone_lst = sorted(list(phone2phoneme.keys()))
+    phone_unit = create_unit(phone_lst)
 
-    phone2phoneme = defaultdict(list)
     phoneme2phone = defaultdict(list)
 
-    for phoneme in phoneme_lst:
-        phone2phoneme[phoneme] = [phoneme]
-        phoneme2phone[phoneme] = [phoneme]
+    for phone, phoneme_lst in phone2phoneme.items():
+        for phoneme in phoneme_lst:
+            phoneme2phone[phoneme].append(phone)
 
+    phoneme_lst = sorted(list(phoneme2phone.keys()))
+    phoneme_unit = create_unit(phoneme_lst)
+
+    model_name = 'customized'
 
-    # blk and eos would be considered as phone/phonemes as well
     phone2phoneme['<blk>'] = ['<blk>']
     phone2phoneme['<eos>'] = ['<eos>']
     phoneme2phone['<blk>'] = ['<blk>']
     phoneme2phone['<eos>'] = ['<eos>']
 
-    model_name = 'customized'
-
     return Inventory(lang_id, model_name, phoneme_unit, phone_unit, phone2phoneme, phoneme2phone)
 
 
-
 def is_inventory_available(lang_id, model_name='latest'):
 
     # check whether a customized path is used or not
     if (Path(model_name) / lang_id).exists():
         return True
     else:
         lang_dir = PhonePieceConfig.data_path / 'model' / model_name / lang_id
```

### Comparing `phonepiece-1.4.0/phonepiece/ipa.py` & `phonepiece-1.4.2/phonepiece/ipa.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 from phonepiece.config import PhonePieceConfig
 import csv
 import unicodedata
 from collections import defaultdict
 
 _norm_rules = [
     (':', 'ː'),
+    ('g', 'ɡ'),
     ("ɡ̥", "k"),
     ('g', 'q̠'),
     ('d̥', "t"),
     ("b̥", "b"),
     ("'", "ʼ"),
     ("I", "ɪ"),
     ('O', 'o'),
     ('Y', 'ʏ'),
     ('ɚ', 'ə˞'),
     ('ɝ', 'ɜ˞'),
     ('ә', 'ə'),
     ('ˈ', ''),
     ('tʃ', 't͡ʃ'),
     ('dʒ','d͡ʒ'),
-    ('N', 'n'), # special handling for JPN N
+    ('N', 'ɴ'), # special handling for JPN N
     # tones: ˩˨˧˦˥
     ('˩', ''),
     ('˨', ''),
     ('˧', ''),
     ('˦', ''),
     ('˥', ''),
 ]
```

### Comparing `phonepiece-1.4.0/phonepiece/lang.py` & `phonepiece-1.4.2/phonepiece/lang.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,20 @@
 
     language = languages.get(part1=lang_id)
     iso3 = language.part3
     if iso3 in _macro_to_individual:
         return _macro_to_individual[iso3]
     return iso3
 
+def read_lang_name(lang_id):
+    lang_id = normalize_lang_id(lang_id)
+    language = languages.get(part3=lang_id)
+    return language.name
+
+
 def read_all_langs():
 
     tree = read_tree()
     iso_lst = list(tree.iso2path.keys())
     return iso_lst
```

### Comparing `phonepiece-1.4.0/phonepiece/lexicon.py` & `phonepiece-1.4.2/phonepiece/lexicon.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/pinyin.py` & `phonepiece-1.4.2/phonepiece/pinyin.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/timit.py` & `phonepiece-1.4.2/phonepiece/timit.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece/unit.py` & `phonepiece-1.4.2/phonepiece/unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,20 @@
         w.write(u+'\n')
 
     w.close()
 
 
 def create_unit(unit_lst):
 
+    if '<blk>' in unit_lst:
+        unit_lst.remove('<blk>')
+
+    if '<eos>' in unit_lst:
+        unit_lst.remove('<eos>')
+
     unit_to_id = dict()
 
     unit_to_id['<blk>'] = 0
 
     idx = 0
 
     for i, unit in enumerate(sorted(unit_lst)):
```

### Comparing `phonepiece-1.4.0/phonepiece/utils.py` & `phonepiece-1.4.2/phonepiece/utils.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/phonepiece.egg-info/SOURCES.txt` & `phonepiece-1.4.2/phonepiece.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 phonepiece.egg-info/SOURCES.txt
 phonepiece.egg-info/dependency_links.txt
 phonepiece.egg-info/requires.txt
 phonepiece.egg-info/top_level.txt
 phonepiece/bin/__init__.py
 phonepiece/bin/download_model.py
 phonepiece/bin/eval_distance.py
+phonepiece/bin/info.py
+phonepiece/bin/list_lang.py
 phonepiece/bin/update_model.py
 phonepiece/data/__init__.py
 phonepiece/data/arpabet.csv
 phonepiece/data/ipa-xsampa.csv
 phonepiece/data/ipa_all.csv
 phonepiece/data/ipa_base.csv
 phonepiece/data/language.tsv
```

### Comparing `phonepiece-1.4.0/test/test_epitran.py` & `phonepiece-1.4.2/test/test_epitran.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/test/test_inventory.py` & `phonepiece-1.4.2/test/test_inventory.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.4.0/test/test_ipa.py` & `phonepiece-1.4.2/test/test_ipa.py`

 * *Files identical despite different names*

