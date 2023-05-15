# Comparing `tmp/breds-1.0.0.tar.gz` & `tmp/breds-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breds-1.0.0.tar", last modified: Sat May  6 23:25:00 2023, max compression
+gzip compressed data, was "breds-1.0.1.tar", last modified: Mon May 15 13:17:32 2023, max compression
```

## Comparing `breds-1.0.0.tar` & `breds-1.0.1.tar`

### file list

```diff
@@ -1,53 +1,52 @@
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-06 23:25:00.491989 breds-1.0.0/
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-06 23:25:00.482188 breds-1.0.0/.github/
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-06 23:25:00.484832 breds-1.0.0/.github/workflows/
--rw-r--r--   0 dsbatista   (501) staff       (20)     1152 2023-05-04 21:39:29.000000 breds-1.0.0/.github/workflows/code_checks.yml
--rw-r--r--   0 dsbatista   (501) staff       (20)     1265 2023-04-22 09:49:17.000000 breds-1.0.0/.gitignore
--rw-r--r--   0 dsbatista   (501) staff       (20)     7651 2023-05-06 14:41:19.000000 breds-1.0.0/LICENSE.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)      555 2023-05-04 21:39:29.000000 breds-1.0.0/Makefile
--rw-r--r--   0 dsbatista   (501) staff       (20)    19983 2023-05-06 23:25:00.492155 breds-1.0.0/PKG-INFO
--rw-r--r--   0 dsbatista   (501) staff       (20)    10266 2023-05-06 23:22:11.000000 breds-1.0.0/README.md
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-06 23:25:00.485292 breds-1.0.0/automatic-evaluation/
--rw-r--r--   0 dsbatista   (501) staff       (20)     1489 2023-04-16 13:51:29.000000 breds-1.0.0/automatic-evaluation/README.md
--rwxr-xr-x   0 dsbatista   (501) staff       (20)    39514 2023-04-22 09:49:17.000000 breds-1.0.0/automatic-evaluation/large-scale-evaluation-freebase.py
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-06 23:25:00.486584 breds-1.0.0/automatic-evaluation/pre_processing_KB/
--rw-r--r--   0 dsbatista   (501) staff       (20)     5131 2023-04-22 09:49:17.000000 breds-1.0.0/automatic-evaluation/pre_processing_KB/Sentence.py
--rw-r--r--   0 dsbatista   (501) staff       (20)        0 2023-04-16 13:51:29.000000 breds-1.0.0/automatic-evaluation/pre_processing_KB/__init__.py
--rwxr-xr-x   0 dsbatista   (501) staff       (20)     3223 2023-04-22 09:49:17.000000 breds-1.0.0/automatic-evaluation/pre_processing_KB/easy_freebase_clean.py
--rwxr-xr-x   0 dsbatista   (501) staff       (20)     2436 2023-04-22 09:49:17.000000 breds-1.0.0/automatic-evaluation/pre_processing_KB/index_whoosh.py
--rwxr-xr-x   0 dsbatista   (501) staff       (20)     1631 2023-04-22 09:49:17.000000 breds-1.0.0/automatic-evaluation/pre_processing_KB/read_high_pmi_relationships.py
--rwxr-xr-x   0 dsbatista   (501) staff       (20)     7403 2023-04-22 09:49:17.000000 breds-1.0.0/automatic-evaluation/pre_processing_KB/select_sentences.py
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-06 23:25:00.489748 breds-1.0.0/breds/
--rw-r--r--   0 dsbatista   (501) staff       (20)    15028 2023-05-06 23:23:57.000000 breds-1.0.0/breds/bootstrapping.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     5121 2023-05-04 21:39:29.000000 breds-1.0.0/breds/breds_tuple.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     2506 2023-05-06 15:34:23.000000 breds-1.0.0/breds/cli.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      263 2023-05-04 21:39:29.000000 breds-1.0.0/breds/commons.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     7034 2023-05-06 23:14:43.000000 breds-1.0.0/breds/config.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      815 2023-05-06 23:01:12.000000 breds-1.0.0/breds/parameters.cfg
--rw-r--r--   0 dsbatista   (501) staff       (20)     3266 2023-05-04 21:39:29.000000 breds-1.0.0/breds/pattern.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      525 2023-05-04 21:39:29.000000 breds-1.0.0/breds/pyproject.toml
--rw-r--r--   0 dsbatista   (501) staff       (20)    12002 2023-05-04 21:39:29.000000 breds-1.0.0/breds/reverb.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      490 2023-05-04 21:39:29.000000 breds-1.0.0/breds/seed.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     6658 2023-05-04 21:39:29.000000 breds-1.0.0/breds/sentence.py
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-06 23:25:00.490563 breds-1.0.0/breds.egg-info/
--rw-r--r--   0 dsbatista   (501) staff       (20)    19983 2023-05-06 23:25:00.000000 breds-1.0.0/breds.egg-info/PKG-INFO
--rw-r--r--   0 dsbatista   (501) staff       (20)     1132 2023-05-06 23:25:00.000000 breds-1.0.0/breds.egg-info/SOURCES.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)        1 2023-05-06 23:25:00.000000 breds-1.0.0/breds.egg-info/dependency_links.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)       41 2023-05-06 23:25:00.000000 breds-1.0.0/breds.egg-info/entry_points.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)       40 2023-05-06 23:25:00.000000 breds-1.0.0/breds.egg-info/requires.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)        6 2023-05-06 23:25:00.000000 breds-1.0.0/breds.egg-info/top_level.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)      239 2023-04-29 18:38:44.000000 breds-1.0.0/mypy.ini
--rw-r--r--   0 dsbatista   (501) staff       (20)      414 2023-05-04 20:44:10.000000 breds-1.0.0/pylint.cfg
--rw-r--r--   0 dsbatista   (501) staff       (20)      996 2023-05-06 14:37:05.000000 breds-1.0.0/pyproject.toml
--rw-r--r--   0 dsbatista   (501) staff       (20)       65 2023-04-22 09:49:17.000000 breds-1.0.0/requirements.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)      137 2023-05-01 15:05:05.000000 breds-1.0.0/requirements_dev.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)      566 2023-05-06 23:25:00.492518 breds-1.0.0/setup.cfg
--rw-r--r--   0 dsbatista   (501) staff       (20)       38 2023-05-04 21:39:29.000000 breds-1.0.0/setup.py
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-06 23:25:00.491872 breds-1.0.0/tests/
--rw-r--r--   0 dsbatista   (501) staff       (20)      115 2023-04-22 09:49:18.000000 breds-1.0.0/tests/__init__.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      568 2023-05-01 15:05:05.000000 breds-1.0.0/tests/test_breds_tuple.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      537 2023-05-01 15:05:05.000000 breds-1.0.0/tests/test_commons.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     1883 2023-05-01 15:05:05.000000 breds-1.0.0/tests/test_pattern.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      346 2023-05-01 15:05:05.000000 breds-1.0.0/tests/test_relationship.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      508 2023-04-26 21:53:59.000000 breds-1.0.0/tests/test_seed.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     3493 2023-05-01 15:05:05.000000 breds-1.0.0/tests/test_sentence.py
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-15 13:17:32.909556 breds-1.0.1/
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-15 13:17:32.899951 breds-1.0.1/.github/
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-15 13:17:32.902123 breds-1.0.1/.github/workflows/
+-rw-r--r--   0 dsbatista   (501) staff       (20)     1152 2023-05-06 23:42:36.000000 breds-1.0.1/.github/workflows/code_checks.yml
+-rw-r--r--   0 dsbatista   (501) staff       (20)     1265 2023-05-06 23:42:36.000000 breds-1.0.1/.gitignore
+-rw-r--r--   0 dsbatista   (501) staff       (20)     7651 2023-05-06 23:42:36.000000 breds-1.0.1/LICENSE.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)      724 2023-05-15 13:16:30.000000 breds-1.0.1/Makefile
+-rw-r--r--   0 dsbatista   (501) staff       (20)    10963 2023-05-15 13:17:32.909686 breds-1.0.1/PKG-INFO
+-rw-r--r--   0 dsbatista   (501) staff       (20)    10208 2023-05-14 09:49:55.000000 breds-1.0.1/README.md
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-15 13:17:32.902733 breds-1.0.1/automatic-evaluation/
+-rw-r--r--   0 dsbatista   (501) staff       (20)     1489 2023-04-16 13:51:29.000000 breds-1.0.1/automatic-evaluation/README.md
+-rwxr-xr-x   0 dsbatista   (501) staff       (20)    39514 2023-05-06 23:42:36.000000 breds-1.0.1/automatic-evaluation/large-scale-evaluation-freebase.py
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-15 13:17:32.906860 breds-1.0.1/automatic-evaluation/pre_processing_KB/
+-rw-r--r--   0 dsbatista   (501) staff       (20)     5131 2023-05-06 23:42:36.000000 breds-1.0.1/automatic-evaluation/pre_processing_KB/Sentence.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)        0 2023-04-16 13:51:29.000000 breds-1.0.1/automatic-evaluation/pre_processing_KB/__init__.py
+-rwxr-xr-x   0 dsbatista   (501) staff       (20)     3223 2023-05-06 23:42:36.000000 breds-1.0.1/automatic-evaluation/pre_processing_KB/easy_freebase_clean.py
+-rwxr-xr-x   0 dsbatista   (501) staff       (20)     2436 2023-05-06 23:42:36.000000 breds-1.0.1/automatic-evaluation/pre_processing_KB/index_whoosh.py
+-rwxr-xr-x   0 dsbatista   (501) staff       (20)     1631 2023-05-06 23:42:36.000000 breds-1.0.1/automatic-evaluation/pre_processing_KB/read_high_pmi_relationships.py
+-rwxr-xr-x   0 dsbatista   (501) staff       (20)     7403 2023-05-06 23:42:36.000000 breds-1.0.1/automatic-evaluation/pre_processing_KB/select_sentences.py
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-15 13:17:32.908048 breds-1.0.1/breds/
+-rw-r--r--   0 dsbatista   (501) staff       (20)    15028 2023-05-06 23:42:36.000000 breds-1.0.1/breds/bootstrapping.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     5121 2023-05-06 23:42:36.000000 breds-1.0.1/breds/breds_tuple.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     2506 2023-05-06 23:42:36.000000 breds-1.0.1/breds/cli.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      263 2023-05-06 23:42:36.000000 breds-1.0.1/breds/commons.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     7034 2023-05-06 23:42:36.000000 breds-1.0.1/breds/config.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      815 2023-05-06 23:42:36.000000 breds-1.0.1/breds/parameters.cfg
+-rw-r--r--   0 dsbatista   (501) staff       (20)     3266 2023-05-06 23:42:36.000000 breds-1.0.1/breds/pattern.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)    12002 2023-05-06 23:42:36.000000 breds-1.0.1/breds/reverb.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      490 2023-05-06 23:42:36.000000 breds-1.0.1/breds/seed.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     6658 2023-05-06 23:42:36.000000 breds-1.0.1/breds/sentence.py
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-15 13:17:32.908729 breds-1.0.1/breds.egg-info/
+-rw-r--r--   0 dsbatista   (501) staff       (20)    10963 2023-05-15 13:17:32.000000 breds-1.0.1/breds.egg-info/PKG-INFO
+-rw-r--r--   0 dsbatista   (501) staff       (20)     1111 2023-05-15 13:17:32.000000 breds-1.0.1/breds.egg-info/SOURCES.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)        1 2023-05-15 13:17:32.000000 breds-1.0.1/breds.egg-info/dependency_links.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)       41 2023-05-15 13:17:32.000000 breds-1.0.1/breds.egg-info/entry_points.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)       40 2023-05-15 13:17:32.000000 breds-1.0.1/breds.egg-info/requires.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)        6 2023-05-15 13:17:32.000000 breds-1.0.1/breds.egg-info/top_level.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)      239 2023-05-06 23:42:36.000000 breds-1.0.1/mypy.ini
+-rw-r--r--   0 dsbatista   (501) staff       (20)      414 2023-05-06 23:42:36.000000 breds-1.0.1/pylint.cfg
+-rw-r--r--   0 dsbatista   (501) staff       (20)      994 2023-05-15 13:16:53.000000 breds-1.0.1/pyproject.toml
+-rw-r--r--   0 dsbatista   (501) staff       (20)       65 2023-05-06 23:42:36.000000 breds-1.0.1/requirements.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)      137 2023-05-06 23:42:36.000000 breds-1.0.1/requirements_dev.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)      566 2023-05-15 13:17:32.910054 breds-1.0.1/setup.cfg
+-rw-r--r--   0 dsbatista   (501) staff       (20)       38 2023-05-06 23:42:36.000000 breds-1.0.1/setup.py
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-15 13:17:32.909468 breds-1.0.1/tests/
+-rw-r--r--   0 dsbatista   (501) staff       (20)      115 2023-05-06 23:42:36.000000 breds-1.0.1/tests/__init__.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      568 2023-05-06 23:42:36.000000 breds-1.0.1/tests/test_breds_tuple.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      537 2023-05-06 23:42:36.000000 breds-1.0.1/tests/test_commons.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     1883 2023-05-06 23:42:36.000000 breds-1.0.1/tests/test_pattern.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      346 2023-05-06 23:42:36.000000 breds-1.0.1/tests/test_relationship.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      508 2023-05-06 23:42:36.000000 breds-1.0.1/tests/test_seed.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     3493 2023-05-06 23:42:36.000000 breds-1.0.1/tests/test_sentence.py
```

### Comparing `breds-1.0.0/.github/workflows/code_checks.yml` & `breds-1.0.1/.github/workflows/code_checks.yml`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/.gitignore` & `breds-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/LICENSE.txt` & `breds-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/Makefile` & `breds-1.0.1/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -17,12 +17,20 @@
 	PYTHONPATH=. coverage report --rcfile=setup.cfg
 
 
 clean:
 	rm -rf build dist *.egg-info .coverage .pytest_cache .mypy_cache .pytest_cache src/*.egg-info
 
 
+publish:
+	make all
+	python -m pip install --upgrade build
+	python -m build
+	python -m pip install --upgrade twine
+	python -m twine upload --repository testpypi dist/*
+
+
 all:
 	make clean
 	make lint
 	make typing
 	make test
```

### Comparing `breds-1.0.0/README.md` & `breds-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,45 +4,46 @@
 &nbsp;
 ![code coverage](https://raw.githubusercontent.com/davidsbatista/BREDS/coverage-badge/coverage.svg?raw=true)
 &nbsp;
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 &nbsp;
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 &nbsp;
-[![Pull Requests Welcome](https://img.shields.io/badge/pull%20requests-welcome-brightgreen.svg)](https://github.com/davidsbatista/BREDS/blob/main/CONTRIBUTING.md)
-&nbsp;
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+&nbsp;
+[![Pull Requests Welcome](https://img.shields.io/badge/pull%20requests-welcome-brightgreen.svg)](https://github.com/davidsbatista/BREDS/blob/main/CONTRIBUTING.md)
+
 
 # BREDS
 
 BREDS extracts relationships using a bootstrapping/semi-supervised approach, it relies on an initial set of 
 seeds, i.e. paris of named-entities representing relationship type to be extracted.  
 
 The algorithm expands the initial set of seeds using distributional semantics to generalize the relationship while 
 limiting the semantic drift.
 
 
 ## Extracting companies headquarters:
 
 The input text needs to have the named-entities tagged, like show in the example bellow:
  
-```
+```yaml
 The tech company <ORG>Soundcloud</ORG> is based in <LOC>Berlin</LOC>, capital of Germany.
 <ORG>Pfizer</ORG> says it has hired <ORG>Morgan Stanley</ORG> to conduct the review.
 <ORG>Allianz</ORG>, based in <LOC>Munich</LOC>, said net income rose to EUR 1.32 billion.
 <LOC>Switzerland</LOC> and <LOC>South Africa</LOC> are co-chairing the meeting.
 <LOC>Ireland</LOC> beat <LOC>Italy</LOC> , then lost 43-31 to <LOC>France</LOC>.
 <ORG>Pfizer</ORG>, based in <LOC>New York City</LOC> , employs about 90,000 workers.
 <PER>Burton</PER> 's engine passed <ORG>NASCAR</ORG> inspection following the qualifying session.
 ```
 
 We need to give seeds to boostrap the extraction process, specifying the type of each named-entity and 
 relationships examples that should also be present in the input text:
 
-```   
+```yaml
 e1:ORG
 e2:LOC
 
 Lufthansa;Cologne
 Nokia;Espoo
 Google;Mountain View
 DoubleClick;New York
@@ -56,30 +57,29 @@
 - afp_apw_xin_embeddings.bin
 - sentences_short.txt.bz2
 - seeds_positive.txt
 ```
 
 Install BREDS using pip
 
-```
+```sh
 pip install breads
 ```
 
 Run the following command:
 
-```
+```sh
 breds --word2vec=afp_apw_xin_embeddings.bin --sentences=sentences_short.txt --positive_seeds=seeds_positive.txt --similarity=0.6 --confidence=0.6
-
 ```
 
 After the  process is terminated an output file `relationships.jsonl` is generated containing the extracted  relationships. 
 
 You can pretty print it's content to the terminal with: `jq '.' < relationships.jsonl`: 
 
-```
+```json
 {
   "entity_1": "Medtronic",
   "entity_2": "Minneapolis",
   "confidence": 0.9982486865148862,
   "sentence": "<ORG>Medtronic</ORG> , based in <LOC>Minneapolis</LOC> , is the nation 's largest independent medical device maker . ",
   "bef_words": "",
   "bet_words": ", based in",
@@ -110,49 +110,50 @@
 }
 ```
 <br>
 
 BREDS has several parameters to tune the extraction process, in the example above it uses the default values, but these 
 can be set in the configuration file: `parameters.cfg`
 
-    max_tokens_away=6           # maximum number of tokens between the two entities
-    min_tokens_away=1           # minimum number of tokens between the two entities
-    context_window_size=2       # number of tokens to the left and right of each entity
-
-    alpha=0.2                   # weight of the BEF context in the similarity function
-    beta=0.6                    # weight of the BET context in the similarity function
-    gamma=0.2                   # weight of the AFT context in the similarity function
-
-    wUpdt=0.5                   # < 0.5 trusts new examples less on each iteration
-    number_iterations=4         # number of bootstrap iterations
-    wUnk=0.1                    # weight given to unknown extracted relationship instances
-    wNeg=2                      # weight given to extracted relationship instances
-    min_pattern_support=2       # minimum number of instances in a cluster to be considered a pattern
-
+```yaml
+max_tokens_away=6           # maximum number of tokens between the two entities
+min_tokens_away=1           # minimum number of tokens between the two entities
+context_window_size=2       # number of tokens to the left and right of each entity
+
+alpha=0.2                   # weight of the BEF context in the similarity function
+beta=0.6                    # weight of the BET context in the similarity function
+gamma=0.2                   # weight of the AFT context in the similarity function
+
+wUpdt=0.5                   # < 0.5 trusts new examples less on each iteration
+number_iterations=4         # number of bootstrap iterations
+wUnk=0.1                    # weight given to unknown extracted relationship instances
+wNeg=2                      # weight given to extracted relationship instances
+min_pattern_support=2       # minimum number of instances in a cluster to be considered a pattern
+```
 
 and passed with the argument `--config=parameters.cfg`.
 
 The full command line parameters are:
 
-```
+```sh
   -h, --help            show this help message and exit
   --config CONFIG       file with bootstrapping configuration parameters
   --word2vec WORD2VEC   an embedding model based on word2vec, in the format of a .bin file
   --sentences SENTENCES
                         a text file with a sentence per line, and with at least two entities per sentence
   --positive_seeds POSITIVE_SEEDS
                         a text file with a seed per line, in the format, e.g.: 'Nokia;Espoo'
   --negative_seeds NEGATIVE_SEEDS
                         a text file with a seed per line, in the format, e.g.: 'Microsoft;San Francisco'
   --similarity SIMILARITY
                         the minimum similarity between tuples and patterns to be considered a match
   --confidence CONFIDENCE
                         the minimum confidence score for a match to be considered a true positive
   --number_iterations NUMBER_ITERATIONS
-                        the minimum confidence score for a match to be considered a true positive
+                        the number of iterations the run
 ```
 
 Please, refer to the section [References and Citations](#references-and-citations) for details on the parameters.
 
 In the first step BREDS pre-processes the input file `sentences.txt` generating word vector representations of  
 relationships (i.e.: `processed_tuples.pkl`). 
 
@@ -160,48 +161,43 @@
 generating word vectors representations. Just pass the argument `--sentences=processed_tuples.pkl` instead to skip 
 this generation step.
 
 ---
 
 # References and Citations
 [Semi-Supervised Bootstrapping of Relationship Extractors with Distributional Semantics, EMNLP'15](https://aclanthology.org/D15-1056/)
-```
+```BibTeX
 @inproceedings{batista-etal-2015-semi,
     title = "Semi-Supervised Bootstrapping of Relationship Extractors with Distributional Semantics",
     author = "Batista, David S.  and Martins, Bruno  and Silva, M{\'a}rio J.",
     booktitle = "Proceedings of the 2015 Conference on Empirical Methods in Natural Language Processing",
     month = sep,
     year = "2015",
     address = "Lisbon, Portugal",
     publisher = "Association for Computational Linguistics",
     url = "https://aclanthology.org/D15-1056",
     doi = "10.18653/v1/D15-1056",
     pages = "499--504",
 }
 ```
 ["Large-Scale Semantic Relationship Extraction for Information Discovery" - Chapter 5, David S Batista, Ph.D. Thesis](http://davidsbatista.net/assets/documents/publications/dsbatista-phd-thesis-2016.pdf)
-```
+```BibTeX
 @incollection{phd-dsbatista2016
   title = {Large-Scale Semantic Relationship Extraction for Information Discovery},
     author = {Batista, David S.},
   school = {Instituto Superior Técnico, Universidade de Lisboa},
   year = {2016}
 }
 ```
 
 # Presenting BREDS at PyData Berlin 2017
 [![Presentation at PyData Berlin 2017](https://img.youtube.com/vi/Ra15lX-wojg/hqdefault.jpg)](https://www.youtube.com/watch?v=Ra15lX-wojg)
 
-
-<br>
-
 ---
 
-<br>
-
 # Contributing to BREDS
 
 Improvements, adding new features and bug fixes are welcome. If you wish to participate in the development of BREDS, 
 please read the following guidelines.
 
 ## The contribution process at a glance
 
@@ -215,15 +211,15 @@
 
 
 ## Preparing the development environment
 
 Make sure you have Python3.9 installed on your system
 
 macOs
-```
+```sh
 brew install python@3.9
 python3.9 -m pip install --user --upgrade pip
 python3.9 -m pip install virtualenv
 ```
 
 Clone the repository and prepare the development environment:
```

### Comparing `breds-1.0.0/automatic-evaluation/README.md` & `breds-1.0.1/automatic-evaluation/README.md`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/automatic-evaluation/large-scale-evaluation-freebase.py` & `breds-1.0.1/automatic-evaluation/large-scale-evaluation-freebase.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/automatic-evaluation/pre_processing_KB/Sentence.py` & `breds-1.0.1/automatic-evaluation/pre_processing_KB/Sentence.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/automatic-evaluation/pre_processing_KB/easy_freebase_clean.py` & `breds-1.0.1/automatic-evaluation/pre_processing_KB/easy_freebase_clean.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/automatic-evaluation/pre_processing_KB/index_whoosh.py` & `breds-1.0.1/automatic-evaluation/pre_processing_KB/index_whoosh.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/automatic-evaluation/pre_processing_KB/read_high_pmi_relationships.py` & `breds-1.0.1/automatic-evaluation/pre_processing_KB/read_high_pmi_relationships.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/automatic-evaluation/pre_processing_KB/select_sentences.py` & `breds-1.0.1/automatic-evaluation/pre_processing_KB/select_sentences.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/breds/bootstrapping.py` & `breds-1.0.1/breds/bootstrapping.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/breds/breds_tuple.py` & `breds-1.0.1/breds/breds_tuple.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/breds/cli.py` & `breds-1.0.1/breds/cli.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/breds/config.py` & `breds-1.0.1/breds/config.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/breds/parameters.cfg` & `breds-1.0.1/breds/parameters.cfg`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/breds/pattern.py` & `breds-1.0.1/breds/pattern.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/breds/reverb.py` & `breds-1.0.1/breds/reverb.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/breds/sentence.py` & `breds-1.0.1/breds/sentence.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/breds.egg-info/SOURCES.txt` & `breds-1.0.1/breds.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 breds/bootstrapping.py
 breds/breds_tuple.py
 breds/cli.py
 breds/commons.py
 breds/config.py
 breds/parameters.cfg
 breds/pattern.py
-breds/pyproject.toml
 breds/reverb.py
 breds/seed.py
 breds/sentence.py
 breds.egg-info/PKG-INFO
 breds.egg-info/SOURCES.txt
 breds.egg-info/dependency_links.txt
 breds.egg-info/entry_points.txt
```

### Comparing `breds-1.0.0/pyproject.toml` & `breds-1.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "breds"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{name = "David S. Batista", email = "dsbatista@gmail.com"}]
 description = "Bootstrapping Relationship Extraction with Distributional Semantics"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["nlp", "semantic relationship extraction", "bootstrapping", "emnlp",
     "vector representations", "word embeddings", "word2vec", "phrase embeddings"]
-license = {file = "LICENSE.txt"}
+license = {text = "GNU GPLv3"}
 classifiers = [
     "Topic :: Text Processing :: Linguistic",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "gensim >= 3.7.3",
     "nltk >= 3.4.1",
```

### Comparing `breds-1.0.0/setup.cfg` & `breds-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/tests/test_breds_tuple.py` & `breds-1.0.1/tests/test_breds_tuple.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/tests/test_commons.py` & `breds-1.0.1/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/tests/test_pattern.py` & `breds-1.0.1/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `breds-1.0.0/tests/test_sentence.py` & `breds-1.0.1/tests/test_sentence.py`

 * *Files identical despite different names*

