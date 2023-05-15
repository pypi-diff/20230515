# Comparing `tmp/indic_nlp_library-0.90.tar.gz` & `tmp/indic_nlp_library-0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indic_nlp_library-0.90.tar", last modified: Tue Mar 14 16:22:32 2023, max compression
+gzip compressed data, was "indic_nlp_library-0.91.tar", last modified: Wed Mar 15 03:07:41 2023, max compression
```

## Comparing `indic_nlp_library-0.90.tar` & `indic_nlp_library-0.91.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:22:32.255116 indic_nlp_library-0.90/
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     1082 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/LICENSE
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     5610 2023-03-14 16:22:32.255116 indic_nlp_library-0.90/PKG-INFO
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     4923 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/README.md
-drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:22:32.245116 indic_nlp_library-0.90/indic_nlp_library.egg-info/
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     5610 2023-03-14 16:22:32.000000 indic_nlp_library-0.90/indic_nlp_library.egg-info/PKG-INFO
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     1126 2023-03-14 16:22:32.000000 indic_nlp_library-0.90/indic_nlp_library.egg-info/SOURCES.txt
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        1 2023-03-14 16:22:32.000000 indic_nlp_library-0.90/indic_nlp_library.egg-info/dependency_links.txt
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)       56 2023-03-14 16:22:32.000000 indic_nlp_library-0.90/indic_nlp_library.egg-info/requires.txt
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        9 2023-03-14 16:22:32.000000 indic_nlp_library-0.90/indic_nlp_library.egg-info/top_level.txt
-drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:22:32.245116 indic_nlp_library-0.90/indicnlp/
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)      238 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/__init__.py
-drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:22:32.245116 indic_nlp_library-0.90/indicnlp/cli/
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/cli/__init__.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     9102 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/cli/cliparser.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     1546 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/common.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)    11285 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/langinfo.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     1000 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/loader.py
-drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:22:32.245116 indic_nlp_library-0.90/indicnlp/morph/
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/morph/__init__.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     4556 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/morph/unsupervised_morph.py
-drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:22:32.245116 indic_nlp_library-0.90/indicnlp/normalize/
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/normalize/__init__.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)    37295 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/normalize/indic_normalize.py
-drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:22:32.245116 indic_nlp_library-0.90/indicnlp/script/
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/script/__init__.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     3974 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/script/english_script.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     8770 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/script/indic_scripts.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     1870 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/script/phonetic_sim.py
-drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:22:32.245116 indic_nlp_library-0.90/indicnlp/syllable/
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/syllable/__init__.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     9571 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/syllable/syllabifier.py
-drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:22:32.245116 indic_nlp_library-0.90/indicnlp/test/
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/test/__init__.py
-drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:22:32.255116 indic_nlp_library-0.90/indicnlp/test/unit/
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/test/unit/__init__.py
-drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:22:32.255116 indic_nlp_library-0.90/indicnlp/tokenize/
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/tokenize/__init__.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     3426 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/tokenize/indic_detokenize.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     3615 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/tokenize/indic_tokenize.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     7549 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/tokenize/sentence_tokenize.py
-drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:22:32.255116 indic_nlp_library-0.90/indicnlp/transliterate/
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/transliterate/__init__.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     2337 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/transliterate/acronym_transliterator.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     6439 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/transliterate/script_unifier.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     5664 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/transliterate/sinhala_transliterator.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)    12626 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/indicnlp/transliterate/unicode_transliterate.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)       21 2023-03-14 16:22:31.000000 indic_nlp_library-0.90/indicnlp/version.py
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)       38 2023-03-14 16:22:32.255116 indic_nlp_library-0.90/setup.cfg
--rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     1744 2023-03-14 16:10:24.000000 indic_nlp_library-0.90/setup.py
+drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-15 03:07:41.702372 indic_nlp_library-0.91/
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     1082 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/LICENSE
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     5610 2023-03-15 03:07:41.702372 indic_nlp_library-0.91/PKG-INFO
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     4923 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/README.md
+drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-15 03:07:41.692372 indic_nlp_library-0.91/indic_nlp_library.egg-info/
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     5610 2023-03-15 03:07:41.000000 indic_nlp_library-0.91/indic_nlp_library.egg-info/PKG-INFO
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     1126 2023-03-15 03:07:41.000000 indic_nlp_library-0.91/indic_nlp_library.egg-info/SOURCES.txt
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        1 2023-03-15 03:07:41.000000 indic_nlp_library-0.91/indic_nlp_library.egg-info/dependency_links.txt
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)       56 2023-03-15 03:07:41.000000 indic_nlp_library-0.91/indic_nlp_library.egg-info/requires.txt
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        9 2023-03-15 03:07:41.000000 indic_nlp_library-0.91/indic_nlp_library.egg-info/top_level.txt
+drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-15 03:07:41.692372 indic_nlp_library-0.91/indicnlp/
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)      238 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/__init__.py
+drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-15 03:07:41.692372 indic_nlp_library-0.91/indicnlp/cli/
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/cli/__init__.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     9102 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/cli/cliparser.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     1546 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/common.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)    11285 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/langinfo.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     1000 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/loader.py
+drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-15 03:07:41.692372 indic_nlp_library-0.91/indicnlp/morph/
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/morph/__init__.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     4556 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/morph/unsupervised_morph.py
+drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-15 03:07:41.692372 indic_nlp_library-0.91/indicnlp/normalize/
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/normalize/__init__.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)    37295 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/normalize/indic_normalize.py
+drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-15 03:07:41.692372 indic_nlp_library-0.91/indicnlp/script/
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/script/__init__.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     3974 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/script/english_script.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     8770 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/script/indic_scripts.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     1870 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/script/phonetic_sim.py
+drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-15 03:07:41.702372 indic_nlp_library-0.91/indicnlp/syllable/
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/syllable/__init__.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     9571 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/syllable/syllabifier.py
+drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-15 03:07:41.702372 indic_nlp_library-0.91/indicnlp/test/
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/test/__init__.py
+drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-15 03:07:41.702372 indic_nlp_library-0.91/indicnlp/test/unit/
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/test/unit/__init__.py
+drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-15 03:07:41.702372 indic_nlp_library-0.91/indicnlp/tokenize/
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/tokenize/__init__.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     3426 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/tokenize/indic_detokenize.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     3615 2023-03-15 03:04:53.000000 indic_nlp_library-0.91/indicnlp/tokenize/indic_tokenize.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     7549 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/tokenize/sentence_tokenize.py
+drwxr-xr-x   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-15 03:07:41.702372 indic_nlp_library-0.91/indicnlp/transliterate/
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)        0 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/transliterate/__init__.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     2337 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/transliterate/acronym_transliterator.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     6439 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/transliterate/script_unifier.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     5664 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/transliterate/sinhala_transliterator.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)    12626 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/indicnlp/transliterate/unicode_transliterate.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)       21 2023-03-15 03:07:41.000000 indic_nlp_library-0.91/indicnlp/version.py
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)       38 2023-03-15 03:07:41.702372 indic_nlp_library-0.91/setup.cfg
+-rw-r--r--   0 ankunchu  (1000) ankunchu  (1000)     1744 2023-03-14 16:10:24.000000 indic_nlp_library-0.91/setup.py
```

### Comparing `indic_nlp_library-0.90/LICENSE` & `indic_nlp_library-0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/PKG-INFO` & `indic_nlp_library-0.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indic_nlp_library
-Version: 0.90
+Version: 0.91
 Summary: The goal of the Indic NLP Library is to build Python based libraries for common text processing and Natural Language Processing in Indian languages.
 Home-page: https://github.com/anoopkunchukuttan/indic_nlp_library
 Download-URL: https://github.com/anoopkunchukuttan/indic_nlp_library/archive/master.zip
 Author: Anoop Kunchukuttan
 Author-email: anoop.kunchukuttan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
```

### Comparing `indic_nlp_library-0.90/README.md` & `indic_nlp_library-0.91/README.md`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indic_nlp_library.egg-info/PKG-INFO` & `indic_nlp_library-0.91/indic_nlp_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indic-nlp-library
-Version: 0.90
+Version: 0.91
 Summary: The goal of the Indic NLP Library is to build Python based libraries for common text processing and Natural Language Processing in Indian languages.
 Home-page: https://github.com/anoopkunchukuttan/indic_nlp_library
 Download-URL: https://github.com/anoopkunchukuttan/indic_nlp_library/archive/master.zip
 Author: Anoop Kunchukuttan
 Author-email: anoop.kunchukuttan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
```

### Comparing `indic_nlp_library-0.90/indic_nlp_library.egg-info/SOURCES.txt` & `indic_nlp_library-0.91/indic_nlp_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/cli/cliparser.py` & `indic_nlp_library-0.91/indicnlp/cli/cliparser.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/common.py` & `indic_nlp_library-0.91/indicnlp/common.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/langinfo.py` & `indic_nlp_library-0.91/indicnlp/langinfo.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/loader.py` & `indic_nlp_library-0.91/indicnlp/loader.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/morph/unsupervised_morph.py` & `indic_nlp_library-0.91/indicnlp/morph/unsupervised_morph.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/normalize/indic_normalize.py` & `indic_nlp_library-0.91/indicnlp/normalize/indic_normalize.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/script/english_script.py` & `indic_nlp_library-0.91/indicnlp/script/english_script.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/script/indic_scripts.py` & `indic_nlp_library-0.91/indicnlp/script/indic_scripts.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/script/phonetic_sim.py` & `indic_nlp_library-0.91/indicnlp/script/phonetic_sim.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/syllable/syllabifier.py` & `indic_nlp_library-0.91/indicnlp/syllable/syllabifier.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/tokenize/indic_detokenize.py` & `indic_nlp_library-0.91/indicnlp/tokenize/indic_detokenize.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/tokenize/indic_tokenize.py` & `indic_nlp_library-0.91/indicnlp/tokenize/indic_tokenize.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
     Returns:
         list: list of tokens
     """
     # tok_str=triv_tokenizer_urdu_pat.sub(r' \1 ',text.replace('\t',' '))
     # return re.sub(r'[ ]+',' ',tok_str).strip(' ').split(' ')
     from urduhack.tokenization import word_tokenizer
-    return word_tokenizer(sent)
+    return word_tokenizer(text)
 
 def trivial_tokenize(text,lang='hi'): 
     """trivial tokenizer for Indian languages using Brahmi for Arabic scripts
 
     A trivial tokenizer which just tokenizes on the punctuation boundaries. 
     Major punctuations specific to Indian langauges are handled. 
     These punctuations characters were identified from the Unicode database.
```

### Comparing `indic_nlp_library-0.90/indicnlp/tokenize/sentence_tokenize.py` & `indic_nlp_library-0.91/indicnlp/tokenize/sentence_tokenize.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/transliterate/acronym_transliterator.py` & `indic_nlp_library-0.91/indicnlp/transliterate/acronym_transliterator.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/transliterate/script_unifier.py` & `indic_nlp_library-0.91/indicnlp/transliterate/script_unifier.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/transliterate/sinhala_transliterator.py` & `indic_nlp_library-0.91/indicnlp/transliterate/sinhala_transliterator.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/indicnlp/transliterate/unicode_transliterate.py` & `indic_nlp_library-0.91/indicnlp/transliterate/unicode_transliterate.py`

 * *Files identical despite different names*

### Comparing `indic_nlp_library-0.90/setup.py` & `indic_nlp_library-0.91/setup.py`

 * *Files identical despite different names*

