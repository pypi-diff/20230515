# Comparing `tmp/cikuu-2022.8.2.tar.gz` & `tmp/cikuu-2022.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cikuu-2022.8.2.tar", last modified: Sat May  6 09:49:02 2023, max compression
+gzip compressed data, was "cikuu-2022.8.3.tar", last modified: Mon May 15 02:22:55 2023, max compression
```

## Comparing `cikuu-2022.8.2.tar` & `cikuu-2022.8.3.tar`

### file list

```diff
@@ -1,373 +1,380 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:02.152003 cikuu-2022.8.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-03-04 12:51:34.000000 cikuu-2022.8.2/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-05-06 09:49:02.152003 cikuu-2022.8.2/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:48:59.431992 cikuu-2022.8.2/api/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-03-04 12:49:43.000000 cikuu-2022.8.2/api/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2086 2023-03-04 12:49:43.000000 cikuu-2022.8.2/api/c4.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1236 2023-03-04 12:49:46.000000 cikuu-2022.8.2/api/chunk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1399 2023-03-04 12:49:49.000000 cikuu-2022.8.2/api/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1069 2023-03-04 12:49:43.000000 cikuu-2022.8.2/api/dm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21647 2023-03-04 12:49:44.000000 cikuu-2022.8.2/api/es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4595 2023-03-04 12:49:46.000000 cikuu-2022.8.2/api/feishu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1480 2023-03-04 12:49:49.000000 cikuu-2022.8.2/api/mynac.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2994 2023-03-04 12:49:44.000000 cikuu-2022.8.2/api/sntjson-es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-03-04 12:49:44.000000 cikuu-2022.8.2/api/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1333 2023-03-04 12:49:46.000000 cikuu-2022.8.2/api/wget.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:48:59.431992 cikuu-2022.8.2/app/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:49:46.000000 cikuu-2022.8.2/app/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:48:59.451992 cikuu-2022.8.2/app/dmdsk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2097 2023-03-04 12:49:46.000000 cikuu-2022.8.2/app/dmdsk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2298 2023-03-04 12:49:46.000000 cikuu-2022.8.2/app/dmdsk/app_navbar.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:48:59.487993 cikuu-2022.8.2/app/dmdsk/func/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:49:49.000000 cikuu-2022.8.2/app/dmdsk/func/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      495 2023-03-04 12:49:44.000000 cikuu-2022.8.2/app/dmdsk/func/dim-awl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2023-03-04 12:49:44.000000 cikuu-2022.8.2/app/dmdsk/func/dims.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2023-03-04 12:49:46.000000 cikuu-2022.8.2/app/dmdsk/func/eidv.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-03-04 12:49:49.000000 cikuu-2022.8.2/app/dmdsk/func/feedback.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      364 2023-03-04 12:49:44.000000 cikuu-2022.8.2/app/dmdsk/func/info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-03-04 12:49:44.000000 cikuu-2022.8.2/app/dmdsk/func/lemma.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      208 2023-03-04 12:49:46.000000 cikuu-2022.8.2/app/dmdsk/func/scores.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      490 2023-03-04 12:49:49.000000 cikuu-2022.8.2/app/dmdsk/func/sent.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-03-04 12:49:44.000000 cikuu-2022.8.2/app/dmdsk/func/trp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      708 2023-03-04 12:49:49.000000 cikuu-2022.8.2/app/dmdsk/index.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:48:59.487993 cikuu-2022.8.2/cikuu.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-05-06 09:48:58.000000 cikuu-2022.8.2/cikuu.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6254 2023-05-06 09:48:58.000000 cikuu-2022.8.2/cikuu.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-06 09:48:58.000000 cikuu-2022.8.2/cikuu.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-06 09:48:58.000000 cikuu-2022.8.2/cikuu.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-05-06 09:48:58.000000 cikuu-2022.8.2/cikuu.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:00.999999 cikuu-2022.8.2/dic/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6977 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      272 2023-03-04 12:49:46.000000 cikuu-2022.8.2/dic/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    72703 2023-03-04 12:49:46.000000 cikuu-2022.8.2/dic/adjlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15209 2023-03-04 12:49:48.000000 cikuu-2022.8.2/dic/advlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2036481 2023-05-04 07:44:16.000000 cikuu-2022.8.2/dic/bnc_wordlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   742662 2023-03-04 12:49:49.000000 cikuu-2022.8.2/dic/confu_set.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1423371 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/ecdic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8101 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/errants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   716825 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/essays.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   479692 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/frame.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1966581 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/lemma_lex.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   446749 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/lemma_mf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182701 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/lemma_scale.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1724920 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/lex_lemma.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4088 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/mwe_disconj.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10043 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/mwe_pv.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173703 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/n_is_sb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173515 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/nounlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3696547 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/nyt_wc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      438 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/oneself.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41916 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/orals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/poslist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2786732 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/propbank.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1350 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/stoplist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      686 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/to_redislite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    90499 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/verbform.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9125 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/verblist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   147209 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/verbtag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   357010 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/vocab.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42948 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/word_awl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   825665 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/word_bits.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   518752 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/word_grade.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46473 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/word_gsl1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42152 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/word_gsl2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2765429 2023-03-04 12:51:15.000000 cikuu-2022.8.2/dic/word_idf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2717304 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/word_oov.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3086978 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/word_pos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182843 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/word_scale.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  4370200 2023-03-04 12:51:15.000000 cikuu-2022.8.2/dic/wordattr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   300932 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/wordcnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   353846 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/wordlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   957421 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/wordlist_ed1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   100665 2023-03-04 12:51:15.000000 cikuu-2022.8.2/dic/wordnet_verb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1150605 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/wordpos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    53593 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/words.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.231999 cikuu-2022.8.2/dsk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7973 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4196 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    94356 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5471 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/dm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2874 2023-03-06 07:28:15.000000 cikuu-2022.8.2/dsk/dsk-hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-03-06 07:28:15.000000 cikuu-2022.8.2/dsk/dsk-req.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4928 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/dsk-to-dskmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9144 2023-05-01 01:51:11.000000 cikuu-2022.8.2/dsk/dsk2023.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3970 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/dskapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/dskes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4444 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/dskmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5532 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/dskmkf_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2465 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/dsktrain.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7228 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/essaydm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      899 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/gears-xdsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4284 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/gecv1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7911 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6162 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/innersim.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6946 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/json-to-dskmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9243 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/kvrdsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8998 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/mkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/mqconsume.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    83132 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/pingyu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3416 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/score.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6150 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/sntsdims.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      936 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2220 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/tok-hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3629 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/uvidsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6616 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/wps-gec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13783 2023-04-23 13:45:01.000000 cikuu-2022.8.2/dsk/wps-xgec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11219 2023-04-23 13:45:08.000000 cikuu-2022.8.2/dsk/wps7000.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9689 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/xessay.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10368 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/xgecv1-test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2023-04-23 13:45:57.000000 cikuu-2022.8.2/dsk/xgecv1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4396 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/xmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2902 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/xsnt-gec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2186 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/xsnt-spacy.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.500001 cikuu-2022.8.2/en/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80279 2023-03-20 11:54:15.000000 cikuu-2022.8.2/en/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5503 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6169 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/annotate.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.512001 cikuu-2022.8.2/en/arc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    74716 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/arc/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1257 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/arc/sntjson-innodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15868 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/arc/sntjson-naclite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6901 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/arc/sntjson-naclite0.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23369 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/arc/sntjson-nacp-20230206.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26784 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/arc/sntjson-nacp-20230207.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4-cl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3675 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4-fts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      999 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/c4-gram-upload.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      984 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4-gram.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      875 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4-grams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      768 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4-np.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      482 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/c4-postag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      589 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4-trp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2039 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4cl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      491 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4down.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1884 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/c4gram-mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2812 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4gram-upsert.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1731 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4gram.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5885 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4gramcl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3602 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/c4matcher.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1401 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4np.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3683 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4postag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4skenp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1096 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/c4tree.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4trp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4vp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      811 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/clause.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6120 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/dims.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16963 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/docfts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8115 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/docjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-03-16 03:10:14.000000 cikuu-2022.8.2/en/en-hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8717 2023-03-25 07:35:03.000000 cikuu-2022.8.2/en/es-index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/esbulk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3777 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/esfile.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6311 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3506 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/exchunk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1159 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/exphrase.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1387 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/extrp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4656 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/havc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      181 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18434 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/kpsi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4234 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/lempostag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6454 2023-03-16 12:13:36.000000 cikuu-2022.8.2/en/nacp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/nlp-lit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4581 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/nlp-lmdb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1900 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/postag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/shav.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/silite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1506 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/snt-esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4786 2023-03-16 12:13:36.000000 cikuu-2022.8.2/en/sntjson-fts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2023-03-16 12:13:36.000000 cikuu-2022.8.2/en/sntjson-kpsnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8237 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/sntjson-mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13520 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/sntjson-nacp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      963 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/sntjson-parse-snt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2031 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/sntjson-si.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1613 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/sntjson-spacy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      569 2023-03-18 08:29:48.000000 cikuu-2022.8.2/en/sntjson-topk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-04-30 03:58:22.000000 cikuu-2022.8.2/en/sntjson-tosnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3888 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/sntjson-trpx.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/sntjson-vp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2612 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/spacybs-esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30937 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/spacybs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2733 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/spider-esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6730 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/sqlsi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30005 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/terms.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9544 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/verbnet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1874 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/xsnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1093 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/zset-load.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.532001 cikuu-2022.8.2/gecdsk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9234 2023-05-03 03:14:08.000000 cikuu-2022.8.2/gecdsk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      704 2023-05-03 03:19:37.000000 cikuu-2022.8.2/gecdsk/essays.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.580001 cikuu-2022.8.2/lit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16540 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1467 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/common.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.588001 cikuu-2022.8.2/lit/es/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5386 2023-03-04 12:50:48.000000 cikuu-2022.8.2/lit/es/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:15.000000 cikuu-2022.8.2/lit/es/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:27.000000 cikuu-2022.8.2/lit/essay.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/filling.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1905 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/fillmul.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      778 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/hello-pages.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      587 2023-03-04 12:51:27.000000 cikuu-2022.8.2/lit/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/mock-scoring.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.588001 cikuu-2022.8.2/lit/penly/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/penly/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/penly/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/penly-resend.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1827 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/redis-dump.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-03-04 12:51:27.000000 cikuu-2022.8.2/lit/reorder.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1689 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/restore.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1152 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/scoring.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/single.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2023-03-04 12:51:27.000000 cikuu-2022.8.2/lit/sntspolish.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1091 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/sntupgrade.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1000 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/student-input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1002 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/teacher-admin.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.608001 cikuu-2022.8.2/lit/yulk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      668 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/yulk/YULK.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/yulk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/yulk/common.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.636001 cikuu-2022.8.2/lit/yulk/func/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1063 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/bipos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/cola.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      666 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/corpuslist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      549 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      501 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/eshyb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      581 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/given-expect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/gramx-single.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1256 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/lemma.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1912 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/lemvs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/pos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      793 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/posvs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1925 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/style-in-mul.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      313 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/style.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      353 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/wcloud.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1547 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/wordrank.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-03-04 12:51:27.000000 cikuu-2022.8.2/lit/yulk/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1255 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/yulk/lemma.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.640001 cikuu-2022.8.2/pipe/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4906 2023-03-04 12:51:27.000000 cikuu-2022.8.2/pipe/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2622 2023-03-04 12:51:18.000000 cikuu-2022.8.2/pipe/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4039 2023-03-04 12:51:18.000000 cikuu-2022.8.2/pipe/redisgec8180.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6514 2023-03-04 12:51:27.000000 cikuu-2022.8.2/pipe/xgecv1.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.640001 cikuu-2022.8.2/rabbitmq/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3075 2023-04-30 03:58:22.000000 cikuu-2022.8.2/rabbitmq/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.660001 cikuu-2022.8.2/redisr/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      746 2023-04-30 03:58:22.000000 cikuu-2022.8.2/redisr/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8210 2023-05-04 00:09:32.000000 cikuu-2022.8.2/redisr/glove-get.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4302 2023-05-03 09:15:53.000000 cikuu-2022.8.2/redisr/glove.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8249 2023-05-04 11:54:55.000000 cikuu-2022.8.2/redisr/sntvec-get.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.664001 cikuu-2022.8.2/sbert/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-04 10:29:10.000000 cikuu-2022.8.2/sbert/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1316 2023-03-04 12:51:18.000000 cikuu-2022.8.2/sbert/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-03 08:06:44.000000 cikuu-2022.8.2/sbert/hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      868 2023-05-04 13:39:29.000000 cikuu-2022.8.2/sbert/redis-sntvec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2379 2023-05-05 09:11:12.000000 cikuu-2022.8.2/sbert/sntvec-so.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13086 2023-03-04 12:51:18.000000 cikuu-2022.8.2/sbert/sntvec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-06 09:49:02.152003 cikuu-2022.8.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      799 2023-05-06 09:48:53.000000 cikuu-2022.8.2/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.692001 cikuu-2022.8.2/so/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32697 2023-05-06 03:47:46.000000 cikuu-2022.8.2/so/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2177 2023-05-02 11:43:44.000000 cikuu-2022.8.2/so/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1116 2023-05-06 09:45:29.000000 cikuu-2022.8.2/so/dis-eev.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2040 2023-05-05 09:11:12.000000 cikuu-2022.8.2/so/dis-essays.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-05-05 09:11:12.000000 cikuu-2022.8.2/so/dis-folder.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2493 2023-05-03 03:14:08.000000 cikuu-2022.8.2/so/dsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2088 2023-05-03 03:14:08.000000 cikuu-2022.8.2/so/folder.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1707 2023-05-06 09:45:29.000000 cikuu-2022.8.2/so/index-dis.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1559 2023-03-04 12:51:18.000000 cikuu-2022.8.2/so/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1746 2023-03-04 12:51:18.000000 cikuu-2022.8.2/so/loades.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.716001 cikuu-2022.8.2/sqlite/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6138 2023-05-01 13:24:28.000000 cikuu-2022.8.2/sqlite/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      500 2023-05-01 14:50:34.000000 cikuu-2022.8.2/sqlite/__main__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.888002 cikuu-2022.8.2/util/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5596 2023-05-05 02:24:34.000000 cikuu-2022.8.2/util/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6002 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4407 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/annotate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3455 2023-03-04 12:51:34.000000 cikuu-2022.8.2/util/bcp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2820 2023-03-04 12:51:30.000000 cikuu-2022.8.2/util/c4data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1748 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/client-blpop.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/client-xwps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3219 2023-03-04 12:51:34.000000 cikuu-2022.8.2/util/clientx.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9342 2023-03-04 12:51:30.000000 cikuu-2022.8.2/util/dsk-util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/fire-test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      357 2023-03-04 12:51:34.000000 cikuu-2022.8.2/util/frame.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4097 2023-03-04 12:51:30.000000 cikuu-2022.8.2/util/kvr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1730 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/mq.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      713 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/nldp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      796 2023-03-04 12:51:34.000000 cikuu-2022.8.2/util/pubsub-sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1665 2023-03-04 12:51:30.000000 cikuu-2022.8.2/util/pubsub2api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      505 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/sent-diff.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3123 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/spider.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      430 2023-03-04 12:51:34.000000 cikuu-2022.8.2/util/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      928 2023-03-04 12:51:30.000000 cikuu-2022.8.2/util/sqlitedict-load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4749 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/wps-blpop.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36149 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/wps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-03-04 12:51:34.000000 cikuu-2022.8.2/util/xfile.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      345 2023-03-04 12:51:30.000000 cikuu-2022.8.2/util/xgec-blpop120.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      371 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/xrange.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2034 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/xsnt-spacy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1521 2023-03-04 12:51:34.000000 cikuu-2022.8.2/util/xstream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1323 2023-03-04 12:51:30.000000 cikuu-2022.8.2/util/xtest-params.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1404 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/xtest.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.896002 cikuu-2022.8.2/uviapp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2144 2023-05-01 14:50:34.000000 cikuu-2022.8.2/uviapp/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:02.112003 cikuu-2022.8.2/uvirun/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/Jinja2-test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2151 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3034 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6573 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/c4es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2777 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/c4gramsi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4734 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/cos_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      753 2023-04-30 03:58:22.000000 cikuu-2022.8.2/uvirun/demo_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22269 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/dsk_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5335 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/echart_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4778 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/elastic_fastapi.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:02.128003 cikuu-2022.8.2/uvirun/errant/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      813 2023-03-04 12:51:33.000000 cikuu-2022.8.2/uvirun/errant/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7269 2023-03-04 12:51:33.000000 cikuu-2022.8.2/uvirun/errant/alignment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3788 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/errant/annotator.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:02.144003 cikuu-2022.8.2/uvirun/errant/commands/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.2/uvirun/errant/commands/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16344 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/errant/commands/compare_m2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-03-04 12:51:30.000000 cikuu-2022.8.2/uvirun/errant/commands/m2_to_m2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3801 2023-03-04 12:51:33.000000 cikuu-2022.8.2/uvirun/errant/commands/parallel_to_m2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2352 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/errant/edit.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:02.152003 cikuu-2022.8.2/uvirun/errant/en/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.2/uvirun/errant/en/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16879 2023-03-04 12:51:33.000000 cikuu-2022.8.2/uvirun/errant/en/classifier.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12340 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/errant/en/lancaster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5602 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/errant/en/merger.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10943 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/errant_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14040 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/es1_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25631 2023-03-20 01:06:12.000000 cikuu-2022.8.2/uvirun/es_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4806 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/essay_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18163 2023-04-30 03:58:22.000000 cikuu-2022.8.2/uvirun/exchunk_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18525 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/feishu_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3892 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/flair_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1809 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/ftp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1010 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/fusion_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3717 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/gec_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2850 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/gec_fastapi_33000.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13116 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/gensim_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6638 2023-04-12 02:56:55.000000 cikuu-2022.8.2/uvirun/gramx_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2562 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/hnswlib_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/kenlm_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6264 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/kpsi_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/kvr_dskdm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/kvr_dskdm1230.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19126 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/nldp_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4490 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/nltk_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/nsp_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10222 2023-03-16 03:10:15.000000 cikuu-2022.8.2/uvirun/penlykvr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6558 2023-05-04 10:29:10.000000 cikuu-2022.8.2/uvirun/sbert_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/single_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32687 2023-04-30 03:58:22.000000 cikuu-2022.8.2/uvirun/spacy_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4320 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/textacy_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2089 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/trans_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4113 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/unmasker_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8742 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/util_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45795 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/uviredis.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37415 2023-04-13 09:21:47.000000 cikuu-2022.8.2/uvirun/yulk-nac.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:55.290706 cikuu-2022.8.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-03-04 12:51:34.000000 cikuu-2022.8.3/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-05-15 02:22:55.290706 cikuu-2022.8.3/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:52.474696 cikuu-2022.8.3/api/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-03-04 12:49:43.000000 cikuu-2022.8.3/api/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2086 2023-03-04 12:49:43.000000 cikuu-2022.8.3/api/c4.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1236 2023-03-04 12:49:46.000000 cikuu-2022.8.3/api/chunk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1399 2023-03-04 12:49:49.000000 cikuu-2022.8.3/api/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1069 2023-03-04 12:49:43.000000 cikuu-2022.8.3/api/dm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21647 2023-03-04 12:49:44.000000 cikuu-2022.8.3/api/es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4595 2023-03-04 12:49:46.000000 cikuu-2022.8.3/api/feishu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1480 2023-03-04 12:49:49.000000 cikuu-2022.8.3/api/mynac.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2994 2023-03-04 12:49:44.000000 cikuu-2022.8.3/api/sntjson-es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-03-04 12:49:44.000000 cikuu-2022.8.3/api/sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1333 2023-03-04 12:49:46.000000 cikuu-2022.8.3/api/wget.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:52.474696 cikuu-2022.8.3/app/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:49:46.000000 cikuu-2022.8.3/app/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:52.494696 cikuu-2022.8.3/app/dmdsk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2097 2023-03-04 12:49:46.000000 cikuu-2022.8.3/app/dmdsk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2298 2023-03-04 12:49:46.000000 cikuu-2022.8.3/app/dmdsk/app_navbar.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:52.542696 cikuu-2022.8.3/app/dmdsk/func/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:49:49.000000 cikuu-2022.8.3/app/dmdsk/func/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      495 2023-03-04 12:49:44.000000 cikuu-2022.8.3/app/dmdsk/func/dim-awl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2023-03-04 12:49:44.000000 cikuu-2022.8.3/app/dmdsk/func/dims.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2023-03-04 12:49:46.000000 cikuu-2022.8.3/app/dmdsk/func/eidv.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-03-04 12:49:49.000000 cikuu-2022.8.3/app/dmdsk/func/feedback.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      364 2023-03-04 12:49:44.000000 cikuu-2022.8.3/app/dmdsk/func/info.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-03-04 12:49:44.000000 cikuu-2022.8.3/app/dmdsk/func/lemma.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      208 2023-03-04 12:49:46.000000 cikuu-2022.8.3/app/dmdsk/func/scores.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      490 2023-03-04 12:49:49.000000 cikuu-2022.8.3/app/dmdsk/func/sent.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-03-04 12:49:44.000000 cikuu-2022.8.3/app/dmdsk/func/trp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      708 2023-03-04 12:49:49.000000 cikuu-2022.8.3/app/dmdsk/index.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:52.546696 cikuu-2022.8.3/cikuu.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-05-15 02:22:51.000000 cikuu-2022.8.3/cikuu.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6368 2023-05-15 02:22:51.000000 cikuu-2022.8.3/cikuu.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-15 02:22:51.000000 cikuu-2022.8.3/cikuu.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-15 02:22:51.000000 cikuu-2022.8.3/cikuu.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-05-15 02:22:51.000000 cikuu-2022.8.3/cikuu.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.158702 cikuu-2022.8.3/dic/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6977 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      272 2023-03-04 12:49:46.000000 cikuu-2022.8.3/dic/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    72703 2023-03-04 12:49:46.000000 cikuu-2022.8.3/dic/adjlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15209 2023-03-04 12:49:48.000000 cikuu-2022.8.3/dic/advlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2036481 2023-05-04 07:44:16.000000 cikuu-2022.8.3/dic/bnc_wordlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   742662 2023-03-04 12:49:49.000000 cikuu-2022.8.3/dic/confu_set.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1423371 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/ecdic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8101 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/errants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   716825 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/essays.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   479692 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/frame.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1966581 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/lemma_lex.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   446749 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/lemma_mf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182701 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/lemma_scale.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1724920 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/lex_lemma.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4088 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/mwe_disconj.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10043 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/mwe_pv.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173703 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/n_is_sb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173515 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/nounlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3696547 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dic/nyt_wc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      438 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/oneself.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41916 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/orals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/poslist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2786732 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dic/propbank.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1350 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/stoplist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      686 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/to_redislite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    90499 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/verbform.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9125 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dic/verblist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   147209 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/verbtag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   357010 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/vocab.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43159 2023-05-08 05:59:19.000000 cikuu-2022.8.3/dic/word_awl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   825665 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dic/word_bits.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   518752 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/word_grade.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46473 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/word_gsl1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42152 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/word_gsl2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2765429 2023-03-04 12:51:15.000000 cikuu-2022.8.3/dic/word_idf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2717304 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dic/word_oov.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3086978 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dic/word_pos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182843 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/word_scale.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  4370200 2023-03-04 12:51:15.000000 cikuu-2022.8.3/dic/wordattr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   300932 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dic/wordcnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   353846 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dic/wordlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   957421 2023-03-04 12:50:25.000000 cikuu-2022.8.3/dic/wordlist_ed1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   100665 2023-03-04 12:51:15.000000 cikuu-2022.8.3/dic/wordnet_verb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1150605 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dic/wordpos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    53593 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dic/words.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.414703 cikuu-2022.8.3/dsk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7973 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4196 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    94356 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5471 2023-03-04 12:51:16.000000 cikuu-2022.8.3/dsk/dm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2874 2023-03-06 07:28:15.000000 cikuu-2022.8.3/dsk/dsk-hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-03-06 07:28:15.000000 cikuu-2022.8.3/dsk/dsk-req.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4928 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/dsk-to-dskmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9144 2023-05-01 01:51:11.000000 cikuu-2022.8.3/dsk/dsk2023.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3970 2023-03-04 12:51:16.000000 cikuu-2022.8.3/dsk/dskapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/dskes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4444 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/dskmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5532 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/dskmkf_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2465 2023-03-04 12:51:16.000000 cikuu-2022.8.3/dsk/dsktrain.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7228 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/essaydm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      899 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/gears-xdsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4284 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/gecv1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7911 2023-03-04 12:51:16.000000 cikuu-2022.8.3/dsk/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6162 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/innersim.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6946 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/json-to-dskmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9243 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/kvrdsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-03-04 12:51:16.000000 cikuu-2022.8.3/dsk/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8998 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/mkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/mqconsume.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    83132 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/pingyu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3416 2023-03-04 12:51:16.000000 cikuu-2022.8.3/dsk/score.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6150 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/sntsdims.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      936 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2220 2023-03-04 12:51:16.000000 cikuu-2022.8.3/dsk/tok-hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3629 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/uvidsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6616 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/wps-gec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13783 2023-04-23 13:45:01.000000 cikuu-2022.8.3/dsk/wps-xgec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11422 2023-05-11 14:49:06.000000 cikuu-2022.8.3/dsk/wps7000.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9689 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/xessay.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10368 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/xgecv1-test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2023-04-23 13:45:57.000000 cikuu-2022.8.3/dsk/xgecv1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4396 2023-03-04 12:51:16.000000 cikuu-2022.8.3/dsk/xmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2902 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/xsnt-gec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2186 2023-03-04 12:50:48.000000 cikuu-2022.8.3/dsk/xsnt-spacy.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.614704 cikuu-2022.8.3/en/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80279 2023-03-20 11:54:15.000000 cikuu-2022.8.3/en/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5503 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6169 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/annotate.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.622704 cikuu-2022.8.3/en/arc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    74716 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/arc/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1257 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/arc/sntjson-innodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15868 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/arc/sntjson-naclite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6901 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/arc/sntjson-naclite0.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23369 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/arc/sntjson-nacp-20230206.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26784 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/arc/sntjson-nacp-20230207.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4-cl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3675 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4-fts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      999 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/c4-gram-upload.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      984 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4-gram.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      875 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4-grams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      768 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4-np.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      482 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/c4-postag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      589 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4-trp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2039 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4cl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      491 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4down.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1884 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/c4gram-mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2812 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4gram-upsert.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1731 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4gram.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5885 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4gramcl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3602 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/c4matcher.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1401 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4np.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3683 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4postag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4skenp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1096 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/c4tree.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4trp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/c4vp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      811 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/clause.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6120 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/dims.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16963 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/docfts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8115 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/docjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-03-16 03:10:14.000000 cikuu-2022.8.3/en/en-hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8717 2023-03-25 07:35:03.000000 cikuu-2022.8.3/en/es-index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/esbulk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3777 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/esfile.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6311 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3506 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/exchunk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1159 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/exphrase.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1387 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/extrp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4656 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/havc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      181 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18434 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/kpsi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4234 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/lempostag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6454 2023-03-16 12:13:36.000000 cikuu-2022.8.3/en/nacp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/nlp-lit.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4581 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/nlp-lmdb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1900 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/postag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/shav.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/silite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1506 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/snt-esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4786 2023-03-16 12:13:36.000000 cikuu-2022.8.3/en/sntjson-fts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2023-03-16 12:13:36.000000 cikuu-2022.8.3/en/sntjson-kpsnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8237 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/sntjson-mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13520 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/sntjson-nacp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      963 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/sntjson-parse-snt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2031 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/sntjson-si.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1613 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/sntjson-spacy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      569 2023-03-18 08:29:48.000000 cikuu-2022.8.3/en/sntjson-topk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-04-30 03:58:22.000000 cikuu-2022.8.3/en/sntjson-tosnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3888 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/sntjson-trpx.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/sntjson-vp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2612 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/spacybs-esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30937 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/spacybs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2733 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/spider-esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6730 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/sqlsi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30005 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/terms.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9544 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/verbnet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1874 2023-03-04 12:50:48.000000 cikuu-2022.8.3/en/xsnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1093 2023-03-04 12:51:16.000000 cikuu-2022.8.3/en/zset-load.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.642704 cikuu-2022.8.3/gecdsk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9234 2023-05-03 03:14:08.000000 cikuu-2022.8.3/gecdsk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      704 2023-05-03 03:19:37.000000 cikuu-2022.8.3/gecdsk/essays.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-05-11 08:23:32.000000 cikuu-2022.8.3/gecdsk/hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      943 2023-05-11 09:20:53.000000 cikuu-2022.8.3/gecdsk/paravs.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.694704 cikuu-2022.8.3/lit/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16540 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1467 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/common.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.698704 cikuu-2022.8.3/lit/es/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5386 2023-03-04 12:50:48.000000 cikuu-2022.8.3/lit/es/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:15.000000 cikuu-2022.8.3/lit/es/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:27.000000 cikuu-2022.8.3/lit/essay.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/filling.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1905 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/fillmul.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      778 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/hello-pages.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      587 2023-03-04 12:51:27.000000 cikuu-2022.8.3/lit/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/mock-scoring.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.702704 cikuu-2022.8.3/lit/penly/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/penly/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/penly/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/penly-resend.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1827 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/redis-dump.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-03-04 12:51:27.000000 cikuu-2022.8.3/lit/reorder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1689 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/restore.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1152 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/scoring.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/single.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2023-03-04 12:51:27.000000 cikuu-2022.8.3/lit/sntspolish.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1091 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/sntupgrade.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1000 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/student-input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1002 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/teacher-admin.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.722704 cikuu-2022.8.3/lit/yulk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      668 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/yulk/YULK.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/yulk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/yulk/common.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.746704 cikuu-2022.8.3/lit/yulk/func/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1063 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/bipos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/cola.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      666 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/corpuslist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      549 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      501 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/eshyb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      581 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/given-expect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/gramx-single.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1256 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/lemma.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1912 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/lemvs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/pos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      793 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/posvs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1925 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/style-in-mul.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      313 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/style.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      353 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/wcloud.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1547 2023-03-04 12:51:16.000000 cikuu-2022.8.3/lit/yulk/func/wordrank.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-03-04 12:51:27.000000 cikuu-2022.8.3/lit/yulk/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1255 2023-03-04 12:51:18.000000 cikuu-2022.8.3/lit/yulk/lemma.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.750704 cikuu-2022.8.3/pipe/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4906 2023-03-04 12:51:27.000000 cikuu-2022.8.3/pipe/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2622 2023-03-04 12:51:18.000000 cikuu-2022.8.3/pipe/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4039 2023-03-04 12:51:18.000000 cikuu-2022.8.3/pipe/redisgec8180.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6514 2023-03-04 12:51:27.000000 cikuu-2022.8.3/pipe/xgecv1.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.754704 cikuu-2022.8.3/rabbitmq/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3075 2023-04-30 03:58:22.000000 cikuu-2022.8.3/rabbitmq/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.798704 cikuu-2022.8.3/redisr/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      746 2023-04-30 03:58:22.000000 cikuu-2022.8.3/redisr/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8210 2023-05-04 00:09:32.000000 cikuu-2022.8.3/redisr/glove-get.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4302 2023-05-03 09:15:53.000000 cikuu-2022.8.3/redisr/glove.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8249 2023-05-04 11:54:55.000000 cikuu-2022.8.3/redisr/sntvec-get.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.830705 cikuu-2022.8.3/sbert/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-04 10:29:10.000000 cikuu-2022.8.3/sbert/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1316 2023-03-04 12:51:18.000000 cikuu-2022.8.3/sbert/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-03 08:06:44.000000 cikuu-2022.8.3/sbert/hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      868 2023-05-04 13:39:29.000000 cikuu-2022.8.3/sbert/redis-sntvec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2379 2023-05-05 09:11:12.000000 cikuu-2022.8.3/sbert/sntvec-so.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13086 2023-03-04 12:51:18.000000 cikuu-2022.8.3/sbert/sntvec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-15 02:22:55.290706 cikuu-2022.8.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      791 2023-05-15 02:22:47.000000 cikuu-2022.8.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.902705 cikuu-2022.8.3/so/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32320 2023-05-12 09:57:14.000000 cikuu-2022.8.3/so/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2177 2023-05-02 11:43:44.000000 cikuu-2022.8.3/so/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4719 2023-05-11 09:20:53.000000 cikuu-2022.8.3/so/batch-dis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1660 2023-05-12 09:56:32.000000 cikuu-2022.8.3/so/batch-sntspacy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      907 2023-05-11 14:51:44.000000 cikuu-2022.8.3/so/dis-bnc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1259 2023-05-11 14:51:44.000000 cikuu-2022.8.3/so/dis-eev.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2040 2023-05-05 09:11:12.000000 cikuu-2022.8.3/so/dis-essays.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-05-05 09:11:12.000000 cikuu-2022.8.3/so/dis-folder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-05-09 13:44:41.000000 cikuu-2022.8.3/so/dis-tosnts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2493 2023-05-03 03:14:08.000000 cikuu-2022.8.3/so/dsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1226 2023-05-10 06:45:18.000000 cikuu-2022.8.3/so/dump-pos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2088 2023-05-03 03:14:08.000000 cikuu-2022.8.3/so/folder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1559 2023-03-04 12:51:18.000000 cikuu-2022.8.3/so/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1746 2023-03-04 12:51:18.000000 cikuu-2022.8.3/so/loades.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1222 2023-05-09 12:36:44.000000 cikuu-2022.8.3/so/tok-idf.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:54.926705 cikuu-2022.8.3/sqlite/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6138 2023-05-01 13:24:28.000000 cikuu-2022.8.3/sqlite/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      500 2023-05-01 14:50:34.000000 cikuu-2022.8.3/sqlite/__main__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:55.026705 cikuu-2022.8.3/util/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6259 2023-05-10 06:34:51.000000 cikuu-2022.8.3/util/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6002 2023-03-04 12:51:33.000000 cikuu-2022.8.3/util/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4407 2023-03-04 12:51:33.000000 cikuu-2022.8.3/util/annotate.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3455 2023-03-04 12:51:34.000000 cikuu-2022.8.3/util/bcp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2820 2023-03-04 12:51:30.000000 cikuu-2022.8.3/util/c4data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1748 2023-03-04 12:51:33.000000 cikuu-2022.8.3/util/client-blpop.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2023-03-04 12:51:33.000000 cikuu-2022.8.3/util/client-xwps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3219 2023-03-04 12:51:34.000000 cikuu-2022.8.3/util/clientx.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9342 2023-03-04 12:51:30.000000 cikuu-2022.8.3/util/dsk-util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:33.000000 cikuu-2022.8.3/util/fire-test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      357 2023-03-04 12:51:34.000000 cikuu-2022.8.3/util/frame.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4097 2023-03-04 12:51:30.000000 cikuu-2022.8.3/util/kvr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1730 2023-03-04 12:51:33.000000 cikuu-2022.8.3/util/mq.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      713 2023-03-04 12:51:33.000000 cikuu-2022.8.3/util/nldp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      796 2023-03-04 12:51:34.000000 cikuu-2022.8.3/util/pubsub-sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1665 2023-03-04 12:51:30.000000 cikuu-2022.8.3/util/pubsub2api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      505 2023-03-04 12:51:33.000000 cikuu-2022.8.3/util/sent-diff.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3123 2023-03-04 12:51:33.000000 cikuu-2022.8.3/util/spider.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      430 2023-03-04 12:51:34.000000 cikuu-2022.8.3/util/sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      928 2023-03-04 12:51:30.000000 cikuu-2022.8.3/util/sqlitedict-load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4749 2023-03-04 12:51:33.000000 cikuu-2022.8.3/util/wps-blpop.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36149 2023-03-04 12:51:33.000000 cikuu-2022.8.3/util/wps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-03-04 12:51:34.000000 cikuu-2022.8.3/util/xfile.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      345 2023-03-04 12:51:30.000000 cikuu-2022.8.3/util/xgec-blpop120.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      371 2023-03-04 12:51:33.000000 cikuu-2022.8.3/util/xrange.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2034 2023-03-04 12:51:33.000000 cikuu-2022.8.3/util/xsnt-spacy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1521 2023-03-04 12:51:34.000000 cikuu-2022.8.3/util/xstream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1323 2023-03-04 12:51:30.000000 cikuu-2022.8.3/util/xtest-params.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1404 2023-03-04 12:51:33.000000 cikuu-2022.8.3/util/xtest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:55.030705 cikuu-2022.8.3/uviapp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2144 2023-05-01 14:50:34.000000 cikuu-2022.8.3/uviapp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:55.238706 cikuu-2022.8.3/uvirun/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-03-04 12:51:44.000000 cikuu-2022.8.3/uvirun/Jinja2-test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2151 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3034 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6573 2023-03-04 12:51:41.000000 cikuu-2022.8.3/uvirun/c4es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2777 2023-03-04 12:51:44.000000 cikuu-2022.8.3/uvirun/c4gramsi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4734 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/cos_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      753 2023-04-30 03:58:22.000000 cikuu-2022.8.3/uvirun/demo_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23119 2023-05-11 08:35:49.000000 cikuu-2022.8.3/uvirun/dsk_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5335 2023-03-04 12:51:44.000000 cikuu-2022.8.3/uvirun/echart_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4778 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/elastic_fastapi.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:55.270706 cikuu-2022.8.3/uvirun/errant/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      813 2023-03-04 12:51:33.000000 cikuu-2022.8.3/uvirun/errant/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7269 2023-03-04 12:51:33.000000 cikuu-2022.8.3/uvirun/errant/alignment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3788 2023-03-04 12:51:41.000000 cikuu-2022.8.3/uvirun/errant/annotator.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:55.282706 cikuu-2022.8.3/uvirun/errant/commands/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.3/uvirun/errant/commands/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16344 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/errant/commands/compare_m2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-03-04 12:51:30.000000 cikuu-2022.8.3/uvirun/errant/commands/m2_to_m2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3801 2023-03-04 12:51:33.000000 cikuu-2022.8.3/uvirun/errant/commands/parallel_to_m2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2352 2023-03-04 12:51:41.000000 cikuu-2022.8.3/uvirun/errant/edit.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 02:22:55.286706 cikuu-2022.8.3/uvirun/errant/en/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.3/uvirun/errant/en/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16879 2023-03-04 12:51:33.000000 cikuu-2022.8.3/uvirun/errant/en/classifier.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12340 2023-03-04 12:51:41.000000 cikuu-2022.8.3/uvirun/errant/en/lancaster.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5602 2023-03-04 12:51:41.000000 cikuu-2022.8.3/uvirun/errant/en/merger.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10943 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/errant_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14040 2023-03-04 12:51:41.000000 cikuu-2022.8.3/uvirun/es1_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25631 2023-03-20 01:06:12.000000 cikuu-2022.8.3/uvirun/es_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4806 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/essay_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18163 2023-04-30 03:58:22.000000 cikuu-2022.8.3/uvirun/exchunk_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18525 2023-03-04 12:51:41.000000 cikuu-2022.8.3/uvirun/feishu_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3892 2023-03-04 12:51:44.000000 cikuu-2022.8.3/uvirun/flair_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1809 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/ftp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1010 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/fusion_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3717 2023-03-04 12:51:41.000000 cikuu-2022.8.3/uvirun/gec_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2850 2023-03-04 12:51:44.000000 cikuu-2022.8.3/uvirun/gec_fastapi_33000.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13116 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/gensim_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6638 2023-04-12 02:56:55.000000 cikuu-2022.8.3/uvirun/gramx_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2562 2023-03-04 12:51:41.000000 cikuu-2022.8.3/uvirun/hnswlib_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-03-04 12:51:44.000000 cikuu-2022.8.3/uvirun/kenlm_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6264 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/kpsi_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/kvr_dskdm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:41.000000 cikuu-2022.8.3/uvirun/kvr_dskdm1230.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19126 2023-03-04 12:51:44.000000 cikuu-2022.8.3/uvirun/nldp_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4490 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/nltk_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/nsp_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10222 2023-03-16 03:10:15.000000 cikuu-2022.8.3/uvirun/penlykvr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6558 2023-05-04 10:29:10.000000 cikuu-2022.8.3/uvirun/sbert_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/single_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32688 2023-05-08 12:37:28.000000 cikuu-2022.8.3/uvirun/spacy_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4644 2023-05-10 06:34:51.000000 cikuu-2022.8.3/uvirun/textacy_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2089 2023-03-04 12:51:44.000000 cikuu-2022.8.3/uvirun/trans_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4113 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/unmasker_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8742 2023-03-04 12:51:34.000000 cikuu-2022.8.3/uvirun/util_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45795 2023-03-04 12:51:41.000000 cikuu-2022.8.3/uvirun/uviredis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37415 2023-04-13 09:21:47.000000 cikuu-2022.8.3/uvirun/yulk-nac.py
```

### Comparing `cikuu-2022.8.2/api/c4.py` & `cikuu-2022.8.3/api/c4.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/api/chunk.py` & `cikuu-2022.8.3/api/chunk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/api/common.py` & `cikuu-2022.8.3/api/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/api/dm.py` & `cikuu-2022.8.3/api/dm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/api/es.py` & `cikuu-2022.8.3/api/es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/api/feishu.py` & `cikuu-2022.8.3/api/feishu.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/api/mynac.py` & `cikuu-2022.8.3/api/mynac.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/api/sntjson-es.py` & `cikuu-2022.8.3/api/sntjson-es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/api/wget.py` & `cikuu-2022.8.3/api/wget.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/app/dmdsk/__init__.py` & `cikuu-2022.8.3/app/dmdsk/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/app/dmdsk/app_navbar.py` & `cikuu-2022.8.3/app/dmdsk/app_navbar.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/app/dmdsk/func/lemma.py` & `cikuu-2022.8.3/app/dmdsk/func/lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/app/dmdsk/func/trp.py` & `cikuu-2022.8.3/app/dmdsk/func/trp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/app/dmdsk/index.py` & `cikuu-2022.8.3/app/dmdsk/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/cikuu.egg-info/SOURCES.txt` & `cikuu-2022.8.3/cikuu.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,16 @@
 en/arc/sntjson-innodb.py
 en/arc/sntjson-naclite.py
 en/arc/sntjson-naclite0.py
 en/arc/sntjson-nacp-20230206.py
 en/arc/sntjson-nacp-20230207.py
 gecdsk/__init__.py
 gecdsk/essays.py
+gecdsk/hello.py
+gecdsk/paravs.py
 lit/__init__.py
 lit/common.py
 lit/essay.py
 lit/filling.py
 lit/fillmul.py
 lit/hello-pages.py
 lit/index.py
@@ -244,22 +246,27 @@
 sbert/__main__.py
 sbert/hello.py
 sbert/redis-sntvec.py
 sbert/sntvec-so.py
 sbert/sntvec.py
 so/__init__.py
 so/__main__.py
+so/batch-dis.py
+so/batch-sntspacy.py
+so/dis-bnc.py
 so/dis-eev.py
 so/dis-essays.py
 so/dis-folder.py
+so/dis-tosnts.py
 so/dsk.py
+so/dump-pos.py
 so/folder.py
-so/index-dis.py
 so/load.py
 so/loades.py
+so/tok-idf.py
 sqlite/__init__.py
 sqlite/__main__.py
 util/__init__.py
 util/__main__.py
 util/annotate.py
 util/bcp.py
 util/c4data.py
```

### Comparing `cikuu-2022.8.2/dic/__init__.py` & `cikuu-2022.8.3/dic/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/adjlist.py` & `cikuu-2022.8.3/dic/adjlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/advlist.py` & `cikuu-2022.8.3/dic/advlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/bnc_wordlist.py` & `cikuu-2022.8.3/dic/bnc_wordlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/confu_set.py` & `cikuu-2022.8.3/dic/confu_set.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/ecdic.py` & `cikuu-2022.8.3/dic/ecdic.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/errants.py` & `cikuu-2022.8.3/dic/errants.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/essays.py` & `cikuu-2022.8.3/dic/essays.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/frame.py` & `cikuu-2022.8.3/dic/frame.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/lemma_lex.py` & `cikuu-2022.8.3/dic/lemma_lex.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/lemma_mf.py` & `cikuu-2022.8.3/dic/lemma_mf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/lemma_scale.py` & `cikuu-2022.8.3/dic/lemma_scale.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/lex_lemma.py` & `cikuu-2022.8.3/dic/lex_lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/mwe_disconj.py` & `cikuu-2022.8.3/dic/mwe_disconj.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/mwe_pv.py` & `cikuu-2022.8.3/dic/mwe_pv.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/n_is_sb.py` & `cikuu-2022.8.3/dic/n_is_sb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/nounlist.py` & `cikuu-2022.8.3/dic/nounlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/nyt_wc.py` & `cikuu-2022.8.3/dic/nyt_wc.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/orals.py` & `cikuu-2022.8.3/dic/orals.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/propbank.py` & `cikuu-2022.8.3/dic/propbank.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/stoplist.py` & `cikuu-2022.8.3/dic/stoplist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/to_redislite.py` & `cikuu-2022.8.3/dic/to_redislite.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/verbform.py` & `cikuu-2022.8.3/dic/verbform.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/verblist.py` & `cikuu-2022.8.3/dic/verblist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/verbtag.py` & `cikuu-2022.8.3/dic/verbtag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/vocab.py` & `cikuu-2022.8.3/dic/vocab.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/word_awl.py` & `cikuu-2022.8.3/dic/word_awl.py`

 * *Files 1% similar despite different names*

```diff
@@ -3121,14 +3121,21 @@
 	with open('word_awl.json','w') as fw: 
 		fw.write(json.dumps([ w for w in word_awl]))
 
 def tsv():
 	with open('awl.tsv','w') as fw: 
 		[ fw.write(f"{w}\n") for w in word_awl]
 
+def tolem():
+	from dic import lex_lemma
+	import json
+	lemmas = set([ lex_lemma.lex_lemma.get(w,w) for w in word_awl])
+	with open('awl-lemma.json','w') as fw: 
+		fw.write(json.dumps([w for w in lemmas]) + "\n")
+
 def tomysql(db, host='172.18.0.1', port=3307):
 	''' db: kpsi  '''
 	import pymysql
 	my_conn = pymysql.connect(host=host,port=port,user='root',password='cikuutest!',db=db)
 	with my_conn.cursor() as cursor: 
 		cursor.execute(f"drop TABLE if exists word_awl")
 		cursor.execute(f"CREATE TABLE if not exists word_awl(word varchar(64) COLLATE latin1_bin not null primary key) engine=myisam  DEFAULT CHARSET=latin1 COLLATE=latin1_bin")
```

### Comparing `cikuu-2022.8.2/dic/word_bits.py` & `cikuu-2022.8.3/dic/word_bits.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/word_grade.py` & `cikuu-2022.8.3/dic/word_grade.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/word_gsl1.py` & `cikuu-2022.8.3/dic/word_gsl1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/word_gsl2.py` & `cikuu-2022.8.3/dic/word_gsl2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/word_idf.py` & `cikuu-2022.8.3/dic/word_idf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/word_oov.py` & `cikuu-2022.8.3/dic/word_oov.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/word_pos.py` & `cikuu-2022.8.3/dic/word_pos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/word_scale.py` & `cikuu-2022.8.3/dic/word_scale.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/wordattr.py` & `cikuu-2022.8.3/dic/wordattr.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/wordcnt.py` & `cikuu-2022.8.3/dic/wordcnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/wordlist.py` & `cikuu-2022.8.3/dic/wordlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/wordlist_ed1.py` & `cikuu-2022.8.3/dic/wordlist_ed1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/wordnet_verb.py` & `cikuu-2022.8.3/dic/wordnet_verb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/wordpos.py` & `cikuu-2022.8.3/dic/wordpos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dic/words.py` & `cikuu-2022.8.3/dic/words.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/__init__.py` & `cikuu-2022.8.3/dsk/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/__main__.py` & `cikuu-2022.8.3/dsk/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/common.py` & `cikuu-2022.8.3/dsk/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/dm.py` & `cikuu-2022.8.3/dsk/dm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/dsk-hello.py` & `cikuu-2022.8.3/dsk/dsk-hello.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/dsk-to-dskmkf.py` & `cikuu-2022.8.3/dsk/dsk-to-dskmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/dsk2023.py` & `cikuu-2022.8.3/dsk/dsk2023.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/dskapi.py` & `cikuu-2022.8.3/dsk/dskapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/dskes.py` & `cikuu-2022.8.3/dsk/dskes.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/dskmkf.py` & `cikuu-2022.8.3/dsk/dskmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/dskmkf_fastapi.py` & `cikuu-2022.8.3/dsk/dskmkf_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/dsktrain.py` & `cikuu-2022.8.3/dsk/dsktrain.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/essaydm.py` & `cikuu-2022.8.3/dsk/essaydm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/gears-xdsk.py` & `cikuu-2022.8.3/dsk/gears-xdsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/gecv1.py` & `cikuu-2022.8.3/dsk/gecv1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/index.py` & `cikuu-2022.8.3/dsk/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/innersim.py` & `cikuu-2022.8.3/dsk/innersim.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/json-to-dskmkf.py` & `cikuu-2022.8.3/dsk/json-to-dskmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/kvrdsk.py` & `cikuu-2022.8.3/dsk/kvrdsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/load.py` & `cikuu-2022.8.3/dsk/load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/mkf.py` & `cikuu-2022.8.3/dsk/mkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/mqconsume.py` & `cikuu-2022.8.3/dsk/mqconsume.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/pingyu.py` & `cikuu-2022.8.3/dsk/pingyu.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/score.py` & `cikuu-2022.8.3/dsk/score.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/sntsdims.py` & `cikuu-2022.8.3/dsk/sntsdims.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/test.py` & `cikuu-2022.8.3/dsk/test.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/tok-hello.py` & `cikuu-2022.8.3/dsk/tok-hello.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/uvidsk.py` & `cikuu-2022.8.3/dsk/uvidsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/wps-gec.py` & `cikuu-2022.8.3/dsk/wps-gec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/wps-xgec.py` & `cikuu-2022.8.3/dsk/wps-xgec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/wps7000.py` & `cikuu-2022.8.3/dsk/wps7000.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 
 def _get_docs(snts, ttl:int=37200): # it is better where there is a outside xsnt-spacy consumer, but it is not a must 
 	reslist = redis.r.mget([f"snt:{snt}" for snt in snts])
 	return  [ ( doc:=spacy.nlp(snt), redis.r.setex(f"snt:{snt}", ttl, json.dumps(doc.to_json()) ), doc )[-1] if res is None else  spacy.tokens.Doc(spacy.nlp.vocab).from_json(json.loads(res) ) for snt, res in zip(snts, reslist) ]
 
 from fastapi import FastAPI, File, UploadFile,Form, Body
 from fastapi.responses import HTMLResponse
-app = fastapi.FastAPI() 
+app	= FastAPI(openapi_url="/wps/openapi.json", docs_url="/wps/docs", redoc_url="/wps/redoc") 
 from fastapi.middleware.cors import CORSMiddleware  #https://fastapi.tiangolo.com/zh/tutorial/cors/
 app.add_middleware(CORSMiddleware, allow_origins=['*'], allow_credentials=True, allow_methods=["*"], allow_headers=["*"],)
+
 @app.get('/')
-def home(): return HTMLResponse(content=f"<h2> dsk api for wps, redis6626 is the local cache, spacy 3.4.1 needed</h2><a href='/docs'> docs </a> | <a href='/redoc'> redoc </a><br> 2023.4.23")
+@app.get('/wps')
+def home(): return HTMLResponse(content=f"<h2> dsk api for wps, redis6626 is the local cache, spacy 3.4.1 needed </h2>  hostname: {socket.gethostname()}, <br> IP: {socket.gethostbyname(socket.gethostname())} <br> | <a href='/wps/docs'> docs </a> | <a href='/wps/redoc'> redoc </a>   <br>2023-5-11")
 
 dskhost	=	os.getenv('dskhost', "172.17.0.1:7095") #gpu120.wrask.com:7095
 gechost =	os.getenv('gechost', 'gpu120.wrask.com:7626') # HTTP api, on top of redis6626, xadd-blpop 
 
 @app.post('/wps-gec-dsk')
 def wps_xgec_dsk(arr:dict={"essay":"English is a internationaly language which becomes importantly for modern world. 中文In China, English is took to be a foreigh language which many student choosed to learn. They begin to studying English at a early age. They use at least one hour to learn English knowledges a day. Even kids in kindergarten have begun learning simple words. That's a good phenomenan, for English is essential nowadays. In addition to, some people think English is superior than Chinese. In me opinion, though English is for great significance, but English is after all a foreign language. it is hard for people to see eye to eye. English do help us read English original works, but Chinese helps us learn a true China. Only by characters Chinese literature can send off its brilliance. Learning a country's culture, especial its classic culture, the first thing is learn its language. Because of we are Chinese, why do we give up our mother tongue and learn our owne culture through a foreign language?"}
 		, use_gec:bool=True, topk_gec:int=64, gec_local:bool=False, max_snt_len:int=2048, with_score:bool=True, score_snts:int=32, internal_sim_default:float=0.2, ibeg_byte:bool=True, diffmerge:bool=False,  timeout:int=9, ttl:int=39200):  
@@ -70,15 +72,15 @@
 
 	except Exception as ex:
 		print(">>gecv1_dsk Ex:", ex, "\t|", arr)
 		exc_type, exc_value, exc_traceback_obj = sys.exc_info()
 		traceback.print_tb(exc_traceback_obj)
 
 
-@app.post('/dims-score')
+@app.post('/wps-dims-score')
 def dims_score(doc:dict={"doc_tc": 191.0, "asl": 74.6154, "ttr2": 62.2009, "ttr": 57.0651, "ast": 14.6923, "snt_num": 13.0, "cl_sum": 8.0, "pred_diff_max3": 5.9, "ttr1": 5.5769, "word_diff_avg": 4.7957, "awl": 4.2723, "prmods_tc": 4.2308, "e_snt.fitted": 3.0, "ast_sd": 1.3431, "mwe_pv": 1.0769, "spell_correct_ratio": 1.0, "kp_correct_ratio": 0.8849, "internal_sim": 0.8794574205761223, "mwe_disconj": 0.8462, "simple_sent_ri": 0.7647, "cl_ratio": 0.6162, "snt_correct_ratio": 0.3077, "simple_sent_ratio": 0.3077, "grammar_correct_ri": 0.3077, "prmods_ratio": 0.2763, "word_gt7": 0.2669, "n_ratio": 0.2407, "v_ratio": 0.1884, "jj_ratio": 0.1099, "art_ratio": 0.0523, "comma_ratio": 0.0471, "b3_b1": 0.0411, "rb_ratio": 0.0366, "b3": 0.0262, "cc_ratio": 0.0157, "kp_correct_ri": 0.0},
 			formula:dict={ "ast":[9.9, 11.99, 15.3, 18.51, 25.32,				2,0.0882, 0.3241],
 				"awl":[3.5, 4.1, 4.56, 5.1, 6.0,					3,0.0882, 0.5],
 				"b3":[0, 0.03, 0.08, 0.12, 0.15 ,					1, 0.0956, 0.2096],
 				"cl_sum":[1, 6.68, 12, 16, 26,						2,0.0441, 0.1621],
 				"grammar_correct_ri":[0.6, 0.85, 0.92, 0.97,1.0,	2,0.0368, 0.1352],
 				"internal_sim":[0.0, 0.08, 0.2, 0.3, 0.4,			4, 0.0735, 0.7688],
@@ -93,15 +95,15 @@
 				"ttr1":[3.43, 4.28, 5.2, 6, 6.8,					3, 0.0882, 0.5],
 				"word_diff_avg":[4.47, 4.73, 5.25,5.8, 6.6,			1, 0.0441, 0.0967],
 				"word_gt7":[0.11, 0.19, 0.3, 0.42, 0.49,			1, 0.0588, 0.1289]} , internal_sim_default:float=0.2): 
 	'''  formula is read from mysql config, 2022.11.20 '''
 	if not 'internal_sim' in doc : doc['internal_sim'] = internal_sim_default
 	return score.dims_score(doc, formula)
 
-@app.get("/spacy-sntbr")
+@app.get("/wps-sntbr")
 def sntbr(text:str="The quick fox jumped over the lazy dog. The justice delayed is justice denied.", trim:bool=False, with_pid:bool=False):
 	''' 2022.8.10 '''
 	from spacy.lang import en
 	if not hasattr(sntbr, 'inst'): 
 		sntbr.inst = en.English()
 		sntbr.inst.add_pipe("sentencizer")
 
@@ -111,15 +113,15 @@
 	pid = 0 #spacy.sntpidoff	= lambda essay: (pid:=0, doc:=spacy.sntbr(essay), [ ( pid := pid + 1 if "\n" in snt.text else pid,  (snt.text, pid, doc[snt.start].idx))[-1] for snt in  doc.sents] )[-1]
 	arr = []
 	for snt in  doc.sents:
 		if "\n" in snt.text: pid = pid + 1 
 		arr.append( (snt.text, pid) ) 
 	return arr 
 
-@app.get('/host-info')
+@app.get('/wps-host-info')
 def host_info(): return {"host": platform.node(), "hostname": socket.gethostname(), "ip": socket.gethostbyname(socket.gethostname()) }
 
 if __name__ == '__main__':
 	uvicorn.run(app, host='0.0.0.0', port=7000)
 
 '''
 docker run -d --restart=always -p 7000:8000 --name wps7000 -v /data/cikuu/pypi/dsk:/dsk -e rport=6665 wrask/gecv1 uvicorn wps7000:app --host 0.0.0.0 --app-dir /dsk --reload --workers 2
```

#### html2text {}

```diff
@@ -19,22 +19,25 @@
 from en.dims import docs_to_dims def _get_docs(snts, ttl:int=37200): # it is
 better where there is a outside xsnt-spacy consumer, but it is not a must
 reslist = redis.r.mget([f"snt:{snt}" for snt in snts]) return [ ( doc:
 =spacy.nlp(snt), redis.r.setex(f"snt:{snt}", ttl, json.dumps(doc.to_json()) ),
 doc )[-1] if res is None else spacy.tokens.Doc(spacy.nlp.vocab).from_json
 (json.loads(res) ) for snt, res in zip(snts, reslist) ] from fastapi import
 FastAPI, File, UploadFile,Form, Body from fastapi.responses import HTMLResponse
-app = fastapi.FastAPI() from fastapi.middleware.cors import CORSMiddleware
+app = FastAPI(openapi_url="/wps/openapi.json", docs_url="/wps/docs",
+redoc_url="/wps/redoc") from fastapi.middleware.cors import CORSMiddleware
 #https://fastapi.tiangolo.com/zh/tutorial/cors/ app.add_middleware
 (CORSMiddleware, allow_origins=['*'], allow_credentials=True, allow_methods=
-["*"], allow_headers=["*"],) @app.get('/') def home(): return HTMLResponse
-(content=f"
+["*"], allow_headers=["*"],) @app.get('/') @app.get('/wps') def home(): return
+HTMLResponse(content=f"
 ***** dsk api for wps, redis6626 is the local cache, spacy 3.4.1 needed *****
-docs | redoc
-2023.4.23") dskhost = os.getenv('dskhost', "172.17.0.1:7095")
+hostname: {socket.gethostname()},
+IP: {socket.gethostbyname(socket.gethostname())}
+| docs | redoc
+2023-5-11") dskhost = os.getenv('dskhost', "172.17.0.1:7095")
 #gpu120.wrask.com:7095 gechost = os.getenv('gechost', 'gpu120.wrask.com:7626')
 # HTTP api, on top of redis6626, xadd-blpop @app.post('/wps-gec-dsk') def
 wps_xgec_dsk(arr:dict={"essay":"English is a internationaly language which
 becomes importantly for modern world. ä¸­æIn China, English is took to be a
 foreigh language which many student choosed to learn. They begin to studying
 English at a early age. They use at least one hour to learn English knowledges
 a day. Even kids in kindergarten have begun learning simple words. That's a
@@ -80,17 +83,17 @@
 ['pingyu'] = pingyu.get_pingyu(dims) fds = [ sntmkf.get(snt, {'feedback':{},
 'meta':{'snt':snt}}) for snt in snts ] [ fd['meta'].update({"sid":i}) for i, fd
 in enumerate(fds) ] [ fd['meta'].update({"pid":sntpid[1], "snt_ori": sntpid
 [0]}) for sntpid, fd in zip(sntpids,fds) ] arr["timing"] = time.time() - start
 res = {'snt': fds, "info": arr} if 'dims' in dir() and dims: res.update({'doc':
 dims}) return res except Exception as ex: print(">>gecv1_dsk Ex:", ex, "\t|",
 arr) exc_type, exc_value, exc_traceback_obj = sys.exc_info() traceback.print_tb
-(exc_traceback_obj) @app.post('/dims-score') def dims_score(doc:dict={"doc_tc":
-191.0, "asl": 74.6154, "ttr2": 62.2009, "ttr": 57.0651, "ast": 14.6923,
-"snt_num": 13.0, "cl_sum": 8.0, "pred_diff_max3": 5.9, "ttr1": 5.5769,
+(exc_traceback_obj) @app.post('/wps-dims-score') def dims_score(doc:dict=
+{"doc_tc": 191.0, "asl": 74.6154, "ttr2": 62.2009, "ttr": 57.0651, "ast":
+14.6923, "snt_num": 13.0, "cl_sum": 8.0, "pred_diff_max3": 5.9, "ttr1": 5.5769,
 "word_diff_avg": 4.7957, "awl": 4.2723, "prmods_tc": 4.2308, "e_snt.fitted":
 3.0, "ast_sd": 1.3431, "mwe_pv": 1.0769, "spell_correct_ratio": 1.0,
 "kp_correct_ratio": 0.8849, "internal_sim": 0.8794574205761223, "mwe_disconj":
 0.8462, "simple_sent_ri": 0.7647, "cl_ratio": 0.6162, "snt_correct_ratio":
 0.3077, "simple_sent_ratio": 0.3077, "grammar_correct_ri": 0.3077,
 "prmods_ratio": 0.2763, "word_gt7": 0.2669, "n_ratio": 0.2407, "v_ratio":
 0.1884, "jj_ratio": 0.1099, "art_ratio": 0.0523, "comma_ratio": 0.0471,
@@ -107,25 +110,25 @@
 0.1352], "simple_sent_ri":[0.4, 0.65, 0.9, 0.95, 1, 2, 0.0368, 0.1352],
 "snt_correct_ratio":[0.01, 0.2, 0.45, 0.75, 1, 1, 0.0368, 0.0807],
 "spell_correct_ratio":[0.8, 0.9, 0.97, 0.99, 1, 1, 0.1471, 0.3226], "ttr1":
 [3.43, 4.28, 5.2, 6, 6.8, 3, 0.0882, 0.5], "word_diff_avg":[4.47, 4.73,
 5.25,5.8, 6.6, 1, 0.0441, 0.0967], "word_gt7":[0.11, 0.19, 0.3, 0.42, 0.49, 1,
 0.0588, 0.1289]} , internal_sim_default:float=0.2): ''' formula is read from
 mysql config, 2022.11.20 ''' if not 'internal_sim' in doc : doc['internal_sim']
-= internal_sim_default return score.dims_score(doc, formula) @app.get("/spacy-
+= internal_sim_default return score.dims_score(doc, formula) @app.get("/wps-
 sntbr") def sntbr(text:str="The quick fox jumped over the lazy dog. The justice
 delayed is justice denied.", trim:bool=False, with_pid:bool=False): '''
 2022.8.10 ''' from spacy.lang import en if not hasattr(sntbr, 'inst'):
 sntbr.inst = en.English() sntbr.inst.add_pipe("sentencizer") doc = sntbr.inst
 (text) if not with_pid: return [ snt.text.strip() if trim else snt.text for snt
 in doc.sents] pid = 0 #spacy.sntpidoff = lambda essay: (pid:=0, doc:
 =spacy.sntbr(essay), [ ( pid := pid + 1 if "\n" in snt.text else pid,
 (snt.text, pid, doc[snt.start].idx))[-1] for snt in doc.sents] )[-1] arr = []
 for snt in doc.sents: if "\n" in snt.text: pid = pid + 1 arr.append( (snt.text,
-pid) ) return arr @app.get('/host-info') def host_info(): return {"host":
+pid) ) return arr @app.get('/wps-host-info') def host_info(): return {"host":
 platform.node(), "hostname": socket.gethostname(), "ip": socket.gethostbyname
 (socket.gethostname()) } if __name__ == '__main__': uvicorn.run(app,
 host='0.0.0.0', port=7000) ''' docker run -d --restart=always -p 7000:8000 --
 name wps7000 -v /data/cikuu/pypi/dsk:/dsk -e rport=6665 wrask/gecv1 uvicorn
 wps7000:app --host 0.0.0.0 --app-dir /dsk --reload --workers 2 >>gecv1_dsk Ex:
 cannot switch to a different thread | {'essay': 'The supplier is responsible
 for any changes or unacceptable conditions of the final looking or practicality
```

### Comparing `cikuu-2022.8.2/dsk/xessay.py` & `cikuu-2022.8.3/dsk/xessay.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/xgecv1-test.py` & `cikuu-2022.8.3/dsk/xgecv1-test.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/xgecv1.py` & `cikuu-2022.8.3/dsk/xgecv1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/xmkf.py` & `cikuu-2022.8.3/dsk/xmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/xsnt-gec.py` & `cikuu-2022.8.3/dsk/xsnt-gec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/dsk/xsnt-spacy.py` & `cikuu-2022.8.3/dsk/xsnt-spacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/__init__.py` & `cikuu-2022.8.3/en/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/__main__.py` & `cikuu-2022.8.3/en/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/annotate.py` & `cikuu-2022.8.3/en/annotate.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/arc/__init__.py` & `cikuu-2022.8.3/en/arc/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/arc/sntjson-innodb.py` & `cikuu-2022.8.3/en/arc/sntjson-innodb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/arc/sntjson-naclite.py` & `cikuu-2022.8.3/en/arc/sntjson-naclite.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/arc/sntjson-naclite0.py` & `cikuu-2022.8.3/en/arc/sntjson-naclite0.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/arc/sntjson-nacp-20230206.py` & `cikuu-2022.8.3/en/arc/sntjson-nacp-20230206.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/arc/sntjson-nacp-20230207.py` & `cikuu-2022.8.3/en/arc/sntjson-nacp-20230207.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4-cl.py` & `cikuu-2022.8.3/en/c4-cl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4-fts.py` & `cikuu-2022.8.3/en/c4-fts.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4-gram-upload.py` & `cikuu-2022.8.3/en/c4-gram-upload.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4-gram.py` & `cikuu-2022.8.3/en/c4-gram.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4-grams.py` & `cikuu-2022.8.3/en/c4-grams.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4-np.py` & `cikuu-2022.8.3/en/c4-np.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4-trp.py` & `cikuu-2022.8.3/en/c4-trp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4cl.py` & `cikuu-2022.8.3/en/c4cl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4gram-mysql.py` & `cikuu-2022.8.3/en/c4gram-mysql.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4gram-upsert.py` & `cikuu-2022.8.3/en/c4gram-upsert.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4gram.py` & `cikuu-2022.8.3/en/c4gram.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4gramcl.py` & `cikuu-2022.8.3/en/c4gramcl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4matcher.py` & `cikuu-2022.8.3/en/c4matcher.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4np.py` & `cikuu-2022.8.3/en/c4np.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4postag.py` & `cikuu-2022.8.3/en/c4postag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4skenp.py` & `cikuu-2022.8.3/en/c4skenp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4tree.py` & `cikuu-2022.8.3/en/c4tree.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4trp.py` & `cikuu-2022.8.3/en/c4trp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/c4vp.py` & `cikuu-2022.8.3/en/c4vp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/clause.py` & `cikuu-2022.8.3/en/clause.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/dims.py` & `cikuu-2022.8.3/en/dims.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/docfts.py` & `cikuu-2022.8.3/en/docfts.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/docjson.py` & `cikuu-2022.8.3/en/docjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/es-index.py` & `cikuu-2022.8.3/en/es-index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/esbulk.py` & `cikuu-2022.8.3/en/esbulk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/esfile.py` & `cikuu-2022.8.3/en/esfile.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/esjson.py` & `cikuu-2022.8.3/en/esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/exchunk.py` & `cikuu-2022.8.3/en/exchunk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/exphrase.py` & `cikuu-2022.8.3/en/exphrase.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/extrp.py` & `cikuu-2022.8.3/en/extrp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/havc.py` & `cikuu-2022.8.3/en/havc.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/kpsi.py` & `cikuu-2022.8.3/en/kpsi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/lempostag.py` & `cikuu-2022.8.3/en/lempostag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/nacp.py` & `cikuu-2022.8.3/en/nacp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/nlp-lit.py` & `cikuu-2022.8.3/en/nlp-lit.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/nlp-lmdb.py` & `cikuu-2022.8.3/en/nlp-lmdb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/postag.py` & `cikuu-2022.8.3/en/postag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/shav.py` & `cikuu-2022.8.3/en/shav.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/silite.py` & `cikuu-2022.8.3/en/silite.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/snt-esjson.py` & `cikuu-2022.8.3/en/snt-esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/sntjson-fts.py` & `cikuu-2022.8.3/en/sntjson-fts.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/sntjson-kpsnt.py` & `cikuu-2022.8.3/en/sntjson-kpsnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/sntjson-mysql.py` & `cikuu-2022.8.3/en/sntjson-mysql.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/sntjson-nacp.py` & `cikuu-2022.8.3/en/sntjson-nacp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/sntjson-parse-snt.py` & `cikuu-2022.8.3/en/sntjson-parse-snt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/sntjson-si.py` & `cikuu-2022.8.3/en/sntjson-si.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/sntjson-spacy.py` & `cikuu-2022.8.3/en/sntjson-spacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/sntjson-topk.py` & `cikuu-2022.8.3/en/sntjson-topk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/sntjson-tosnt.py` & `cikuu-2022.8.3/en/sntjson-tosnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/sntjson-trpx.py` & `cikuu-2022.8.3/en/sntjson-trpx.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/sntjson-vp.py` & `cikuu-2022.8.3/en/sntjson-vp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/spacybs-esjson.py` & `cikuu-2022.8.3/en/spacybs-esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/spacybs.py` & `cikuu-2022.8.3/en/spacybs.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/spider-esjson.py` & `cikuu-2022.8.3/en/spider-esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/sqlsi.py` & `cikuu-2022.8.3/en/sqlsi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/terms.py` & `cikuu-2022.8.3/en/terms.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/verbnet.py` & `cikuu-2022.8.3/en/verbnet.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/xsnt.py` & `cikuu-2022.8.3/en/xsnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/en/zset-load.py` & `cikuu-2022.8.3/en/zset-load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/gecdsk/__init__.py` & `cikuu-2022.8.3/gecdsk/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/gecdsk/essays.py` & `cikuu-2022.8.3/gecdsk/essays.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/__init__.py` & `cikuu-2022.8.3/lit/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/common.py` & `cikuu-2022.8.3/lit/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/es/__init__.py` & `cikuu-2022.8.3/lit/es/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/es/index.py` & `cikuu-2022.8.3/lit/es/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/essay.py` & `cikuu-2022.8.3/lit/essay.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/fillmul.py` & `cikuu-2022.8.3/lit/fillmul.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/hello-pages.py` & `cikuu-2022.8.3/lit/hello-pages.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/index.py` & `cikuu-2022.8.3/lit/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/mock-scoring.py` & `cikuu-2022.8.3/lit/mock-scoring.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/penly/index.py` & `cikuu-2022.8.3/lit/penly/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/penly-resend.py` & `cikuu-2022.8.3/lit/penly-resend.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/redis-dump.py` & `cikuu-2022.8.3/lit/redis-dump.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/reorder.py` & `cikuu-2022.8.3/lit/reorder.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/restore.py` & `cikuu-2022.8.3/lit/restore.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/scoring.py` & `cikuu-2022.8.3/lit/scoring.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/single.py` & `cikuu-2022.8.3/lit/single.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/sntspolish.py` & `cikuu-2022.8.3/lit/sntspolish.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/sntupgrade.py` & `cikuu-2022.8.3/lit/sntupgrade.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/student-input.py` & `cikuu-2022.8.3/lit/student-input.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/teacher-admin.py` & `cikuu-2022.8.3/lit/teacher-admin.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/YULK.py` & `cikuu-2022.8.3/lit/yulk/YULK.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/common.py` & `cikuu-2022.8.3/lit/yulk/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/func/bipos.py` & `cikuu-2022.8.3/lit/yulk/func/bipos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/func/cola.py` & `cikuu-2022.8.3/lit/yulk/func/cola.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/func/common.py` & `cikuu-2022.8.3/lit/yulk/func/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/func/corpuslist.py` & `cikuu-2022.8.3/lit/yulk/func/corpuslist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/func/es.py` & `cikuu-2022.8.3/lit/yulk/func/es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/func/given-expect.py` & `cikuu-2022.8.3/lit/yulk/func/given-expect.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/func/gramx-single.py` & `cikuu-2022.8.3/lit/yulk/func/gramx-single.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/func/lemma.py` & `cikuu-2022.8.3/lit/yulk/func/lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/func/lemvs.py` & `cikuu-2022.8.3/lit/yulk/func/lemvs.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/func/pos.py` & `cikuu-2022.8.3/lit/yulk/func/pos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/func/posvs.py` & `cikuu-2022.8.3/lit/yulk/func/posvs.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/func/style-in-mul.py` & `cikuu-2022.8.3/lit/yulk/func/style-in-mul.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/func/wordrank.py` & `cikuu-2022.8.3/lit/yulk/func/wordrank.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/index.py` & `cikuu-2022.8.3/lit/yulk/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/lit/yulk/lemma.py` & `cikuu-2022.8.3/lit/yulk/lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/pipe/__init__.py` & `cikuu-2022.8.3/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/pipe/__main__.py` & `cikuu-2022.8.3/pipe/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/pipe/redisgec8180.py` & `cikuu-2022.8.3/pipe/redisgec8180.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/pipe/xgecv1.py` & `cikuu-2022.8.3/pipe/xgecv1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/rabbitmq/__init__.py` & `cikuu-2022.8.3/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/redisr/__init__.py` & `cikuu-2022.8.3/redisr/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/redisr/glove-get.py` & `cikuu-2022.8.3/redisr/glove-get.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/redisr/glove.py` & `cikuu-2022.8.3/redisr/glove.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/redisr/sntvec-get.py` & `cikuu-2022.8.3/redisr/sntvec-get.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/sbert/__main__.py` & `cikuu-2022.8.3/sbert/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/sbert/hello.py` & `cikuu-2022.8.3/sbert/hello.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/sbert/redis-sntvec.py` & `cikuu-2022.8.3/sbert/redis-sntvec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/sbert/sntvec-so.py` & `cikuu-2022.8.3/sbert/sntvec-so.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/sbert/sntvec.py` & `cikuu-2022.8.3/sbert/sntvec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/setup.py` & `cikuu-2022.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 # Created Time: 2022-2-13
 #############################################
  
 from setuptools import setup, find_packages
  
 setup(
   name = "cikuu",
-  version = "2022.8.2",
+  version = "2022.8.3",
   keywords = ("pip"),
   description = "cikuu tools",
   long_description = "add replace into soinit",
   license = "MIT Licence",
  
   url = "http://www.cikuu.com",
   author = "cikuu",
   author_email = "info@cikuu.com",
  
   packages = find_packages(),
   include_package_data = True,
   platforms = "any", #"pymysql","pika","fastapi","uvicorn","click==7.1.2", "fire","elasticsearch","marisa_trie",
-  install_requires = ["redis","requests"]  #>=2.27.1
+  install_requires = ["requests"]  #>=2.27.1
 )
```

### Comparing `cikuu-2022.8.2/so/__init__.py` & `cikuu-2022.8.3/so/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,36 +118,47 @@
 			"np": { "type": "text", "analyzer": "postag_ana","fielddata":"true"},
 			"ske": { "type": "text", "analyzer": "postag_ana","fielddata":"true"},
 			"i": { "type": "integer", "index": "false"},
 			"start": { "type": "integer", "index": "false"},
 			"end": { "type": "integer", "index": "false"},
 			"head": { "type": "integer", "index": "false"},
 			"score": { "type": "float"},
+			"idf": { "type": "float"},
 			"ratio": { "type": "float", "index": "false"},
 			"memo": { "type": "keyword", "index": "false"}, # to store some memo info, for show only
 			"sent": { "type": "keyword", "index": "false"},
 			"offset": { "type": "float"},
 			"final_score": { "type": "float"},
 			"sid": { "type": "keyword"},
 			"sntid": { "type": "keyword"},
+			"level": { "type": "keyword"},  # awl,gsl1,gsl2
 			"pid": { "type": "keyword"}, # parentid 
 			"paraid": { "type": "keyword"}, # paragraph
 			"id": { "type": "keyword"},
 			"rid": { "type": "keyword"},
-			"did": { "type": "keyword"},
+			"did": { "type": "keyword"}, # update keyword -> integer,  in didlist 
+			"didver": { "type": "float"},
 			"vpat": { "type": "keyword"},
 			"ibeg": { "type": "integer"},
 			"iend": { "type": "integer"},
 			"len": { "type": "integer"}, # [start, start + len) 
 			"docid": { "type": "keyword"},
 			"uid": { "type": "keyword"},
 			"eid": { "type": "keyword"},
 			"sntnum": { "type": "integer"},
 			"wordnum": { "type": "integer"},
 			"awl": { "type": "float"},
+			"ttr1": { "type": "float"},
+			"word_diff_avg": { "type": "float"},
+			"ast": { "type": "float"},
+			"cl_ratio": { "type": "float"},
+			"doc_tc": { "type": "float"},
+			"para_num": { "type": "float"},
+			"spell_correct_ratio": { "type": "float"},
+			"grammar_correct_ri": { "type": "float"},
 			"cnt": { "type": "long"},
 			"vers": { "type": "integer"},
 			"ver": { "type": "integer"},
 			"ct": { "type": "integer"},
 			"lem": { "type": "keyword"},
 			"frame": { "type": "keyword"}, # flair/frame 
 			"lempos": { "type": "keyword"}, # for wordattr , ie: open/VERB 
@@ -504,41 +515,19 @@
 def sntbr(essay): # added 2023.5.2
 	import spacy
 	from spacy.lang import en
 	if not hasattr(sntbr, 'inst'): 
 		sntbr.inst = (inst := en.English(), inst.add_pipe("sentencizer"))[0]
 	return sntbr.inst(essay) 
 
-def dskindex(idxname, did, dsk_or_essay):
-	''' (sntid, did, snt, ... ) , 2023.5.2 '''
-	import gecdsk 
-	dsk = gecdsk.parse({"essay":dsk_or_essay}) if isinstance(dsk_or_essay, str) else dsk_or_essay
-	info = dsk['info'] 
-
-	if not requests.es.exists(index=idxname, id=f"{did}:snts" ):  # return  # already exists 
-		snts = [ mkf['meta']['snt'].strip() for mkf in dsk['snt'] ]
-		esindex(idxname, f"{did}:snts", {"id": f"{did}:snts", 'did': did, 'type':'snts', 'snts': snts, 'sntnum':len(snts) })
-	
-	if not requests.es.exists(index=idxname, id=f"{did}:dims"):
-		esindex(idxname, f"{did}:dims", {"id": f"{did}:dims", 'did': did, 'type':'dims', 'dims': json.dumps(dsk['doc'] ) })
-	
-	for i,mkf in enumerate(dsk['snt']): 
-		snt = mkf['meta']['snt'].strip() 	
-		sid = f"{did}:snt-{i}"
-		esindex(idxname, sid, {"did": did,'sntid': sid, 'type':'snt', 'snt': snt, 'rid': info.get('rid',0), 'uid': info.get('uid',0), 'tc': mkf['meta'].get('tc',0)} )
-		for k, item in mkf['feedback'].items():
-			cate = item.get('cate','')
-			if cate.startswith("e_") or cate.startswith("w_"):
-				esindex(idxname, f"{sid}:{k}", {"did": did, 'sntid': sid, 'rid': info.get('rid',0), 'uid': info.get('uid',0), 'type':'sntfd', 'kp': item['kp'], 'cate': cate, 'short_msg':item.get('short_msg',''), 'sent':snt})
-
-def update(idxname, id, arr): # arr = {"tags":"VIP"}
+def esupdate(idxname, id, arr): # arr = {"tags":"VIP"}
 	try:
 		return requests.post(f"http://{requests.eshost}/{idxname}/_doc/{id}/_update", json={"doc":arr }).json() 
 	except Exception as ex:
-		print(">>update ex:", ex)
+		print(">>esupdate ex:", ex)
 
 def drop(idxname): 
 	try:
 		requests.es.indices.delete(index=idxname)
 	except Exception as ex:
 		print(">>drop index ex:", ex)
 
@@ -566,28 +555,36 @@
 	''' 2023.5.5 '''
 	for root, dirs, files in os.walk(folder):
 		for file in files: 
 			if file.endswith(pattern):
 				text = open(f"{folder}/{file}", 'r').read().strip() 
 				yield (file, text)  #{"folder":folder, "filename":file, "content":text}
 
+fire.actions = []
+def addaction(arr, batch:int=10000): #{'_op_type':'index', '_index':index, '_id': sntid, '_source': source }
+	fire.actions.append( arr )
+	if len(fire.actions) >= batch: 
+		helpers.bulk(client=requests.es,actions=fire.actions, raise_on_error=False)
+		print (fire.actions[-1], flush=True) 
+		fire.actions = []
+submit_actions = lambda : helpers.bulk(client=requests.es,actions=fire.actions, raise_on_error=False) if fire.actions else None	
+
 def testana(index:str='test'):
 	requests.eshost	= os.getenv("eshost", "sntvec.wrask.com:9200") 
 	requests.es		= Elasticsearch([ f"http://{requests.eshost}" ])  
 	init( index ) 
 	arr = requests.post(f"http://sntvec.wrask.com:9200/{index}/_analyze", json={
   "analyzer": "postag_ana",
   "text": "booked_book_VERB_VBN_NP5"
 }).json()
 	for t in arr['tokens']:
 		print (t) 
 
 if __name__ == "__main__": 
 	import platform
-	#testana()
 	print( lemlist()) if platform.system() in ('Windows') else fire.Fire({"init":init,"test":testana}) 
 	
 '''
 {'tokens': [{'token': 'booked', 'start_offset': 0, 'end_offset': 22, 'type': 'word', 'position': 0}, 
 {'token': 'd', 'start_offset': 0, 'end_offset': 22, 'type': 'word', 'position': 0}, 
 {'token': '_book', 'start_offset': 0, 'end_offset': 22, 'type': 'word', 'position': 0}, 
 {'token': '_,', 'start_offset': 0, 'end_offset': 22, 'type': 'word', 'position': 0}]}
@@ -797,9 +794,8 @@
     "aggs" : {
         "termrank" : {
             "terms" : { "field" : "lem", "size":1000  } 
             
         }
     }
 }
-
 '''
```

### Comparing `cikuu-2022.8.2/so/__main__.py` & `cikuu-2022.8.3/so/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/so/dis-eev.py` & `cikuu-2022.8.3/so/dis-eev.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 	start = time.time()
 	with open(outfile if outfile is not None else infile.split('.')[0] + ".dis-jsonl", 'w') as fw : 
 		for i, line in enumerate(fileinput.input(infile,openhook=fileinput.hook_compressed)): 
 			if i % 100 == 0: print (f"[dis-eev] {infile}:\t", i, flush=True)
 			arr = json.loads(line.replace('"essay_id"','"eid"').replace('"request_id"','"rid"').replace('"user_id"','"uid"') ) 
 			if arr['essay'] is None: continue # :null => None
 			essay = arr['essay'] 
-			doc = nlp(essay)
+			doc = nlp(essay.strip())
 			dsk = gecdsk.parse({"essay":essay})
-			fw.write(json.dumps({'info':arr, 'dsk': dsk, 'spacy': doc.to_json()}) + "\n")
+			snts = [sp.as_doc().to_json() for sp in doc.sents ] # docs
+			fw.write(json.dumps({'info':arr, 'dsk': dsk, 'snts': snts }) + "\n")
+			#fw.write(json.dumps({'info':arr, 'dsk': dsk, 'spacy': doc.to_json()}) + "\n")
 	print(f"finished: {infile}, \t| using: ", time.time() - start) 
 
 if __name__ == '__main__': 	#run('testdoc', debug=True)
 	fire.Fire(run)
 
 '''
 ubuntu@dicvec-scivec-jukuu-com-flair-64-245:/data/cikuu/pypi/so$ nohup python dis-eev.py nju.2023.jsonl.gz &
```

### Comparing `cikuu-2022.8.2/so/dis-essays.py` & `cikuu-2022.8.3/so/dis-essays.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/so/dis-folder.py` & `cikuu-2022.8.3/so/dis-folder.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/so/dsk.py` & `cikuu-2022.8.3/so/dsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/so/folder.py` & `cikuu-2022.8.3/so/folder.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/so/load.py` & `cikuu-2022.8.3/so/load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/so/loades.py` & `cikuu-2022.8.3/so/loades.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/sqlite/__init__.py` & `cikuu-2022.8.3/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/__init__.py` & `cikuu-2022.8.3/util/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -61,14 +61,24 @@
 		G2 = round(2 * ((a * ln(a / E1)) + (b * ln(b / E2))), 2)
 		if minus or  (minus is None and a * d < b * c): G2 = 0 - G2 #if minus or  (minus is None and a/c < b/d): G2 = 0 - G2
 		return round(G2,1)
 	except Exception as e:
 		print ("likelihood ex:",e, a,b,c,d)
 		return 0
 
+def keyness(srcrows:list=[['one',5],['two',7]], srcsum:int=None, tgtrows:list=[['one',5],['three',17]], tgtsum:int=None, topk:int=30):
+	''' srcrows is the es result, 2023.5.10 '''
+	srcsum	= sum([i for s,i in srcrows]) + 0.01 if srcsum is None else srcsum + 0.01
+	tgtsum	= sum([i for s,i in tgtrows]) + 0.01 if tgtsum is None else tgtsum + 0.01
+	dic1    = dict(tgtrows)
+	rows	= [ {"word":s, "src": i, "tgt": dic1.get(s,0), "srcper":round(100.0 * i/srcsum,1), "tgtper":round(100.0 * dic1.get(s,0)/tgtsum,1), 
+				"keyness": likelihood( i, dic1.get(s,0), srcsum, tgtsum ) } for s,i in srcrows ] 
+	rows.sort(key=lambda a:a['keyness'], reverse =True)
+	return rows[0:topk]	
+
 has_zh = lambda s : any([c for c in s if ord(c) > 255])
 
 def logdice(xy, x, y): # https://www.fi.muni.cz/usr/sojka/download/raslan2008/13.pdf
 	return round(14  + ln ( 2 * xy/ (x+y), 2),1)
 #print (logdice( 1, 23, 56) )
 
 def lexlist( lemma='open', sepa="|"):
@@ -143,8 +153,8 @@
   else:
       if t.label() == label: f(t)  # or do something else
       else:
           for child in t: 
               traverse(child, label, f)
 
 if __name__ == '__main__': 
-	print( cands_product()) 
+	print( keyness())
```

### Comparing `cikuu-2022.8.2/util/__main__.py` & `cikuu-2022.8.3/util/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/annotate.py` & `cikuu-2022.8.3/util/annotate.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/bcp.py` & `cikuu-2022.8.3/util/bcp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/c4data.py` & `cikuu-2022.8.3/util/c4data.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/client-blpop.py` & `cikuu-2022.8.3/util/client-blpop.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/client-xwps.py` & `cikuu-2022.8.3/util/client-xwps.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/clientx.py` & `cikuu-2022.8.3/util/clientx.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/dsk-util.py` & `cikuu-2022.8.3/util/dsk-util.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/kvr.py` & `cikuu-2022.8.3/util/kvr.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/mq.py` & `cikuu-2022.8.3/util/mq.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/nldp.py` & `cikuu-2022.8.3/util/nldp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/pubsub-sync.py` & `cikuu-2022.8.3/util/pubsub-sync.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/pubsub2api.py` & `cikuu-2022.8.3/util/pubsub2api.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/spider.py` & `cikuu-2022.8.3/util/spider.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/sqlitedict-load.py` & `cikuu-2022.8.3/util/sqlitedict-load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/wps-blpop.py` & `cikuu-2022.8.3/util/wps-blpop.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/wps.py` & `cikuu-2022.8.3/util/wps.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/xsnt-spacy.py` & `cikuu-2022.8.3/util/xsnt-spacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/xstream.py` & `cikuu-2022.8.3/util/xstream.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/xtest-params.py` & `cikuu-2022.8.3/util/xtest-params.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/util/xtest.py` & `cikuu-2022.8.3/util/xtest.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uviapp/__init__.py` & `cikuu-2022.8.3/uviapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/Jinja2-test.py` & `cikuu-2022.8.3/uvirun/Jinja2-test.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/__init__.py` & `cikuu-2022.8.3/uvirun/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/__main__.py` & `cikuu-2022.8.3/uvirun/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/c4es.py` & `cikuu-2022.8.3/uvirun/c4es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/c4gramsi.py` & `cikuu-2022.8.3/uvirun/c4gramsi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/cos_fastapi.py` & `cikuu-2022.8.3/uvirun/cos_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/demo_fastapi.py` & `cikuu-2022.8.3/uvirun/demo_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/dsk_fastapi.py` & `cikuu-2022.8.3/uvirun/dsk_fastapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -302,14 +302,28 @@
 				"chunks": [ {"start":sp.start, "end": sp.end,"type":"NP", "lem": doc[sp.end-1].lemma_, "text":sp.text} for sp in doc.noun_chunks ],
 				} 
 		for t in doc:
 			sntdic[sntkey][f'toks-{t.i}'] =  {'i':t.i, "head":t.head.i, 'lex':t.text, 'lem':t.lemma_, 'pos':t.pos_, 'tag':t.tag_, 'dep':t.dep_, "gpos":t.head.pos_, "glem":t.head.lemma_}
 	
 	return {"hdoc": arr, "hsnts": sntdic} 
 
+@app.get("/gecdsk/paravs", tags=["dsk"])
+def para_vs( essay:str='The quick fox jumped over the lazy dog. She has ready.', snt: str='She has ready.', num:int=5, apihost:str="api.jukuu.com"):
+	''' added 2023.5.11 '''
+	import gecdsk, requests
+	res = [( snt, gecdsk.parse({"essay":essay})['info']['final_score'] )]
+	for row in requests.get(f"http://{apihost}/paraphrase",params={"snt":snt, "num_return_sequences":num}).json(): #[{"id":0,"snt":"She is prepared."},{"id":1,"snt":"Her readiness is complete."},{"id":2,"snt":"She has got it."},{"id":3,"snt":"She's prepared."},{"id":4,"snt":"Her preparation has been completed."}]
+		try:
+			txt = essay.replace(snt, row['snt'])
+			dsk = gecdsk.parse({"essay":txt})
+			res.append( ( row['snt'], dsk['info']['final_score'] ) )
+		except Exception as ex:
+			print(">>para_vs ex:", ex)
+	return res
+
 if __name__ == '__main__':  #uvicorn.run(app, host='0.0.0.0', port=80)
 	#print (dsk_wrapper("[\u8bd1\u6587]The 55-kilometre Hong Kong Zhuhai-Macau Bridge is an extraordinary engineering. It is the world's longest sea-crossing transportation system combining bridges and tunnels, which joins the three cities of Hong Kong Zhuhai and Macao, cutting the travelling time among them from 3 hours to 30 minutes. The reinforced concrete bridge with huge spans fully not only proves that China has the ability to complete the record-breaking mega-construction, but also will enhance the regional integration and boost the economic growth. It plays a crucial role in the overall plan to develop China’s Great Bay Area, which China intends to turn into one rivaling those of San Francisco, New York and Tokyo in terms of technological innovation and economic prosperity.", JSONEachRow=True))
 	#print (sntbr("[\u8bd1\u6587]The 55-kilometre Hong Kong Zhuhai-Macau Bridge is an extraordinary engineering. It is the world's longest sea-crossing transportation system combining bridges and tunnels, which joins the three cities of Hong Kong Zhuhai and Macao, cutting the travelling time among them from 3 hours to 30 minutes. The reinforced concrete bridge with huge spans fully not only proves that China has the ability to complete the record-breaking mega-construction, but also will enhance the regional integration and boost the economic growth. It plays a crucial role in the overall plan to develop China’s Great Bay Area, which China intends to turn into one rivaling those of San Francisco, New York and Tokyo in terms of technological innovation and economic prosperity."))
 	print ( xdsk_with_pid()) 
 
 def topk_info(snts, docs,  topk, default_dims = {"internal_sim":0.2} ): 
 	''' info computing with topk snts, upon those long essay '''
```

### Comparing `cikuu-2022.8.2/uvirun/echart_fastapi.py` & `cikuu-2022.8.3/uvirun/echart_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/elastic_fastapi.py` & `cikuu-2022.8.3/uvirun/elastic_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/errant/__init__.py` & `cikuu-2022.8.3/uvirun/errant/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/errant/alignment.py` & `cikuu-2022.8.3/uvirun/errant/alignment.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/errant/annotator.py` & `cikuu-2022.8.3/uvirun/errant/annotator.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/errant/commands/compare_m2.py` & `cikuu-2022.8.3/uvirun/errant/commands/compare_m2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/errant/commands/m2_to_m2.py` & `cikuu-2022.8.3/uvirun/errant/commands/m2_to_m2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/errant/commands/parallel_to_m2.py` & `cikuu-2022.8.3/uvirun/errant/commands/parallel_to_m2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/errant/edit.py` & `cikuu-2022.8.3/uvirun/errant/edit.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/errant/en/classifier.py` & `cikuu-2022.8.3/uvirun/errant/en/classifier.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/errant/en/lancaster.py` & `cikuu-2022.8.3/uvirun/errant/en/lancaster.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/errant/en/merger.py` & `cikuu-2022.8.3/uvirun/errant/en/merger.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/errant_fastapi.py` & `cikuu-2022.8.3/uvirun/errant_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/es1_fastapi.py` & `cikuu-2022.8.3/uvirun/es1_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/es_fastapi.py` & `cikuu-2022.8.3/uvirun/es_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/essay_fastapi.py` & `cikuu-2022.8.3/uvirun/essay_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/exchunk_fastapi.py` & `cikuu-2022.8.3/uvirun/exchunk_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/feishu_fastapi.py` & `cikuu-2022.8.3/uvirun/feishu_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/flair_fastapi.py` & `cikuu-2022.8.3/uvirun/flair_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/ftp.py` & `cikuu-2022.8.3/uvirun/ftp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/fusion_fastapi.py` & `cikuu-2022.8.3/uvirun/fusion_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/gec_fastapi.py` & `cikuu-2022.8.3/uvirun/gec_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/gec_fastapi_33000.py` & `cikuu-2022.8.3/uvirun/gec_fastapi_33000.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/gensim_fastapi.py` & `cikuu-2022.8.3/uvirun/gensim_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/gramx_fastapi.py` & `cikuu-2022.8.3/uvirun/gramx_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/hnswlib_fastapi.py` & `cikuu-2022.8.3/uvirun/hnswlib_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/kenlm_fastapi.py` & `cikuu-2022.8.3/uvirun/kenlm_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/kpsi_fastapi.py` & `cikuu-2022.8.3/uvirun/kpsi_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/kvr_dskdm.py` & `cikuu-2022.8.3/uvirun/kvr_dskdm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/kvr_dskdm1230.py` & `cikuu-2022.8.3/uvirun/kvr_dskdm1230.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/nldp_fastapi.py` & `cikuu-2022.8.3/uvirun/nldp_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/nltk_fastapi.py` & `cikuu-2022.8.3/uvirun/nltk_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/nsp_fastapi.py` & `cikuu-2022.8.3/uvirun/nsp_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/penlykvr.py` & `cikuu-2022.8.3/uvirun/penlykvr.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/sbert_fastapi.py` & `cikuu-2022.8.3/uvirun/sbert_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/spacy_fastapi.py` & `cikuu-2022.8.3/uvirun/spacy_fastapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,15 +329,15 @@
 		if sp.end - sp.start > 1:
 			toks[sp.start] = f"<u>{toks[sp.start]}"
 			toks[sp.end-1] = f"{toks[sp.end-1]}</u>"
 	html =  "".join(toks) 
 	return HTMLResponse(content=html)  if ashtml else html
 
 @app.post('/spacy/colored', tags=["spacy"])
-def spacy_colored_snts(snts:str=["She has ready.","It are ok."]): 
+def spacy_colored_snts(snts:list=["She has ready.","It are ok."]): 
 	''' 2023.4.28 '''
 	return [ {"id":i, "snt":  spacy_colored_snt(snt, False)} for i,snt in enumerate(snts)]
 
 @app.get('/spacy/highlight', tags=["spacy"])
 def doc_highlight(text:str='And the quick fox hit the lazy dog.', as_html:bool=False): #, pos:str='ADJ'
 	''' return html, with pos highlighted ''' 
 	doc = spacy.nlp(text)
```

### Comparing `cikuu-2022.8.2/uvirun/textacy_fastapi.py` & `cikuu-2022.8.3/uvirun/textacy_fastapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 
 @app.get('/textacy/keyword_in_context', tags=["textacy"])
 def keyword_in_context(text:str="The quick fox jumped over the lazy dog.", keyword:str="jumped", window_width:int=25, pad_context:bool=True): 
 	''' 2022.1.28	'''
 	from textacy import extract
 	return list(extract.keyword_in_context(text, keyword, window_width=window_width, pad_context=pad_context))
 
+@app.post('/textacy/kwic', tags=["textacy"])
+def textacy_kwic(snts:list=["The quick fox jumped over the lazy dog.","I jumped over the dog."], keyword:str="jumped", window_width:int=25, pad_context:bool=True): 
+	''' 2023.5.10	'''
+	return [ keyword_in_context(snt, keyword,window_width,pad_context)[0]  for snt in snts]
+
 @app.get('/textacy/ngrams', tags=["textacy"])
 def ngrams(text:str="The quick fox jumped over the lazy dog.",n:int=3,filter_stops:bool=True, filter_punct:bool=True, filter_nums:bool=False, min_freq:int=1): 
 	''' 2022.1.28	'''
 	doc = spacy.nlp(text)
 	return list(textacy.extract.ngrams(
 	   doc, n, filter_stops=filter_stops, filter_punct=filter_punct, filter_nums=filter_nums,min_freq=min_freq))
```

### Comparing `cikuu-2022.8.2/uvirun/trans_fastapi.py` & `cikuu-2022.8.3/uvirun/trans_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/unmasker_fastapi.py` & `cikuu-2022.8.3/uvirun/unmasker_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/util_fastapi.py` & `cikuu-2022.8.3/uvirun/util_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/uviredis.py` & `cikuu-2022.8.3/uvirun/uviredis.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.2/uvirun/yulk-nac.py` & `cikuu-2022.8.3/uvirun/yulk-nac.py`

 * *Files identical despite different names*

