# Comparing `tmp/pyriksprot-2023.4.3.tar.gz` & `tmp/pyriksprot-2023.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksprot-2023.4.3.tar", max compression
+gzip compressed data, was "pyriksprot-2023.4.4.tar", max compression
```

## Comparing `pyriksprot-2023.4.3.tar` & `pyriksprot-2023.4.4.tar`

### file list

```diff
@@ -1,90 +1,97 @@
--rw-r--r--   0        0        0     1080 2022-03-14 19:05:38.857587 pyriksprot-2023.4.3/LICENSE
--rw-r--r--   0        0        0     7547 2023-04-13 10:55:09.499216 pyriksprot-2023.4.3/README.md
--rw-r--r--   0        0        0     3536 2023-04-19 09:23:02.948346 pyriksprot-2023.4.3/pyproject.toml
--rw-r--r--   0        0        0     1250 2023-04-17 14:57:52.426931 pyriksprot-2023.4.3/pyriksprot/__init__.py
--rw-r--r--   0        0        0      152 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/corpus/__init__.py
--rw-r--r--   0        0        0     4111 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/corpus_index.py
--rw-r--r--   0        0        0    11973 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/iterate.py
--rw-r--r--   0        0        0      243 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/__init__.py
--rw-r--r--   0        0        0     3528 2023-04-17 14:57:52.426931 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/convert.py
--rw-r--r--   0        0        0     2467 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/iterate.py
--rw-r--r--   0        0        0     5365 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/parse.py
--rw-r--r--   0        0        0        0 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/__init__.py
--rw-r--r--   0        0        0      244 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/templates/__init__.py
--rw-r--r--   0        0        0      330 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.txt.jinja
--rw-r--r--   0        0        0      447 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.xml.jinja
--rw-r--r--   0        0        0      352 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/templates/speeches.cdata.xml.jinja
--rw-r--r--   0        0        0      278 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/templates/speeches.txt.jinja
--rw-r--r--   0        0        0      342 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/templates/speeches.xml.jinja
--rw-r--r--   0        0        0     1779 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt
--rw-r--r--   0        0        0     1578 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt
--rw-r--r--   0        0        0     1201 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt
--rw-r--r--   0        0        0     2266 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/tf.py
--rw-r--r--   0        0        0      170 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/tagged/__init__.py
--rw-r--r--   0        0        0     1630 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/tagged/iterate.py
--rw-r--r--   0        0        0     5790 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/tagged/persist.py
--rw-r--r--   0        0        0     1515 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/utility.py
--rw-r--r--   0        0        0      113 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/dehyphenation/__init__.py
--rw-r--r--   0        0        0     1693 2022-03-14 19:05:38.861587 pyriksprot-2023.4.3/pyriksprot/dehyphenation/flair_dehyphen.py
--rw-r--r--   0        0        0     8642 2023-04-19 09:21:24.587202 pyriksprot-2023.4.3/pyriksprot/dehyphenation/swe_dehyphen.py
--rw-r--r--   0        0        0      843 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/dehyphenation/utility.py
--rw-r--r--   0        0        0      438 2023-01-24 09:13:07.490512 pyriksprot-2023.4.3/pyriksprot/dispatch/__init__.py
--rw-r--r--   0        0        0    21577 2023-04-19 09:21:24.587202 pyriksprot-2023.4.3/pyriksprot/dispatch/dispatch.py
--rw-r--r--   0        0        0     2100 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/dispatch/item.py
--rw-r--r--   0        0        0     4594 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/dispatch/merge.py
--rw-r--r--   0        0        0     4908 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/dispatch/utility.py
--rw-r--r--   0        0        0       40 2022-03-14 19:05:38.861587 pyriksprot-2023.4.3/pyriksprot/foss/README.md
--rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.3/pyriksprot/foss/__init__.py
--rw-r--r--   0        0        0     2335 2022-03-14 19:05:38.861587 pyriksprot-2023.4.3/pyriksprot/foss/bettertokenizer.sv
--rw-r--r--   0        0        0      945 2022-03-14 19:05:38.861587 pyriksprot-2023.4.3/pyriksprot/foss/bettertokenizer.sv.saldo-tokens
--rw-r--r--   0        0        0    12236 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/foss/pos_tags.py
--rw-r--r--   0        0        0     7546 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/foss/sparv_tokenize.py
--rw-r--r--   0        0        0     1420 2022-03-14 19:05:38.861587 pyriksprot-2023.4.3/pyriksprot/foss/stopwords.py
--rw-r--r--   0        0        0     6119 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/foss/untangle.py
--rw-r--r--   0        0        0     3582 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/gitchen.py
--rw-r--r--   0        0        0    13080 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/interface.py
--rw-r--r--   0        0        0      769 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/metadata/__init__.py
--rw-r--r--   0        0        0     5145 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/codecs.py
--rw-r--r--   0        0        0    12475 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/config.py
--rw-r--r--   0        0        0     7737 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/generate.py
--rw-r--r--   0        0        0    14671 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/person.py
--rw-r--r--   0        0        0     3125 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/repository.py
--rw-r--r--   0        0        0     2373 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/subset.py
--rw-r--r--   0        0        0     6384 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/utility.py
--rw-r--r--   0        0        0     1461 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/utterance.py
--rw-r--r--   0        0        0     4296 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/verify.py
--rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.3/pyriksprot/scripts/__init__.py
--rw-r--r--   0        0        0     1596 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/scripts/csv2pgsql.py
--rw-r--r--   0        0        0     1648 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/scripts/fix_speaker_notes.py
--rw-r--r--   0        0        0     3543 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/scripts/metadata2db.py
--rw-r--r--   0        0        0     2789 2023-04-19 09:21:24.587202 pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2speech.py
--rw-r--r--   0        0        0     3475 2023-04-19 09:07:54.192237 pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2speech_text.py
--rw-r--r--   0        0        0     2902 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2tagged.py
--rw-r--r--   0        0        0     4650 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2text.py
--rw-r--r--   0        0        0      487 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2tfs.py
--rwxr-xr-x   0        0        0      680 2023-01-24 09:13:07.494512 pyriksprot-2023.4.3/pyriksprot/scripts/speaker_note2csv
--rw-r--r--   0        0        0     2568 2023-01-24 09:13:07.494512 pyriksprot-2023.4.3/pyriksprot/scripts/speech_index.py
--rw-r--r--   0        0        0     1162 2023-04-19 09:21:24.591202 pyriksprot-2023.4.3/pyriksprot/scripts/subset_corpus.py
--rw-r--r--   0        0        0     5266 2023-01-24 09:13:07.494512 pyriksprot-2023.4.3/pyriksprot/scripts/utils.py
--rwxr-xr-x   0        0        0      541 2023-01-24 09:13:07.494512 pyriksprot-2023.4.3/pyriksprot/scripts/xml2csv
--rw-r--r--   0        0        0      599 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/00_rename.sql
--rw-r--r--   0        0        0     4522 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/01_data_updates.sql
--rw-r--r--   0        0        0     2592 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/02_code_tables.sql
--rw-r--r--   0        0        0     2199 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/03_persons_of_interest.sql
--rw-r--r--   0        0        0     5973 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/04_terms_of_office.sql
--rw-r--r--   0        0        0     2818 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/05_person_party.sql
--rw-r--r--   0        0        0     1707 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/06_unknown.sql
--rw-r--r--   0        0        0     1344 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/09_cleanup.sql
--rw-r--r--   0        0        0      204 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/__init__.py
--rw-r--r--   0        0        0     7144 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/to_speech.py
--rw-r--r--   0        0        0    12974 2023-04-17 14:57:52.426931 pyriksprot-2023.4.3/pyriksprot/utility.py
--rw-r--r--   0        0        0      250 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/workflows/__init__.py
--rw-r--r--   0        0        0     1415 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/workflows/_extract_speech_ids.py
--rw-r--r--   0        0        0     4425 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/workflows/extract_speech_text.py
--rw-r--r--   0        0        0     6449 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/workflows/extract_tags.py
--rw-r--r--   0        0        0     4552 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/workflows/extract_text.py
--rw-r--r--   0        0        0     3254 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/workflows/speech_index.py
--rw-r--r--   0        0        0     2230 2023-04-13 13:53:26.190262 pyriksprot-2023.4.3/pyriksprot/workflows/subset_corpus.py
--rw-r--r--   0        0        0     6123 2023-04-19 09:21:24.591202 pyriksprot-2023.4.3/pyriksprot/workflows/tag.py
--rw-r--r--   0        0        0     4159 2023-04-19 09:21:24.591202 pyriksprot-2023.4.3/pyriksprot/workflows/tf.py
--rw-r--r--   0        0        0     8732 1970-01-01 00:00:00.000000 pyriksprot-2023.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-03-14 19:05:38.857587 pyriksprot-2023.4.4/LICENSE
+-rw-r--r--   0        0        0     7547 2023-04-13 10:55:09.499216 pyriksprot-2023.4.4/README.md
+-rw-r--r--   0        0        0     3597 2023-05-15 14:39:35.617625 pyriksprot-2023.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1248 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/__init__.py
+-rw-r--r--   0        0        0      122 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/configuration/__init__.py
+-rw-r--r--   0        0        0     5905 2023-05-15 14:37:02.779664 pyriksprot-2023.4.4/pyriksprot/configuration/config.py
+-rw-r--r--   0        0        0     4915 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/configuration/inject.py
+-rw-r--r--   0        0        0     2599 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/configuration/registry.py
+-rw-r--r--   0        0        0      152 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/corpus/__init__.py
+-rw-r--r--   0        0        0     4111 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/corpus/corpus_index.py
+-rw-r--r--   0        0        0    11973 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/corpus/iterate.py
+-rw-r--r--   0        0        0      220 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/__init__.py
+-rw-r--r--   0        0        0     2770 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/convert.py
+-rw-r--r--   0        0        0     2467 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/iterate.py
+-rw-r--r--   0        0        0     5368 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/parse.py
+-rw-r--r--   0        0        0        0 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/__init__.py
+-rw-r--r--   0        0        0      244 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/templates/__init__.py
+-rw-r--r--   0        0        0      330 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.txt.jinja
+-rw-r--r--   0        0        0      447 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.xml.jinja
+-rw-r--r--   0        0        0      352 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/templates/speeches.cdata.xml.jinja
+-rw-r--r--   0        0        0      278 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/templates/speeches.txt.jinja
+-rw-r--r--   0        0        0      342 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/templates/speeches.xml.jinja
+-rw-r--r--   0        0        0     1779 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt
+-rw-r--r--   0        0        0     1578 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt
+-rw-r--r--   0        0        0     1201 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt
+-rw-r--r--   0        0        0     2302 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/tf.py
+-rw-r--r--   0        0        0      170 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/tagged/__init__.py
+-rw-r--r--   0        0        0     1630 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/corpus/tagged/iterate.py
+-rw-r--r--   0        0        0     5790 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/corpus/tagged/persist.py
+-rw-r--r--   0        0        0     1515 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/corpus/utility.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/cwb/__init__.py
+-rw-r--r--   0        0        0      113 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/dehyphenation/__init__.py
+-rw-r--r--   0        0        0     1693 2022-03-14 19:05:38.861587 pyriksprot-2023.4.4/pyriksprot/dehyphenation/flair_dehyphen.py
+-rw-r--r--   0        0        0     8902 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/dehyphenation/swe_dehyphen.py
+-rw-r--r--   0        0        0      843 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/dehyphenation/utility.py
+-rw-r--r--   0        0        0      438 2023-01-24 09:13:07.490512 pyriksprot-2023.4.4/pyriksprot/dispatch/__init__.py
+-rw-r--r--   0        0        0    21600 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/dispatch/dispatch.py
+-rw-r--r--   0        0        0     2100 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/dispatch/item.py
+-rw-r--r--   0        0        0     4594 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/dispatch/merge.py
+-rw-r--r--   0        0        0     4908 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/dispatch/utility.py
+-rw-r--r--   0        0        0       40 2022-03-14 19:05:38.861587 pyriksprot-2023.4.4/pyriksprot/foss/README.md
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.4/pyriksprot/foss/__init__.py
+-rw-r--r--   0        0        0    12236 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/foss/pos_tags.py
+-rw-r--r--   0        0        0     2335 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/foss/resources/bettertokenizer.sv
+-rw-r--r--   0        0        0      945 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/foss/resources/bettertokenizer.sv.saldo-tokens
+-rw-r--r--   0        0        0  3493683 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/foss/resources/punkt-nltk-svenska.pickle
+-rw-r--r--   0        0        0    13495 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/foss/sparv_tokenize.py
+-rw-r--r--   0        0        0     1420 2022-03-14 19:05:38.861587 pyriksprot-2023.4.4/pyriksprot/foss/stopwords.py
+-rw-r--r--   0        0        0     6119 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/foss/untangle.py
+-rw-r--r--   0        0        0     3582 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/gitchen.py
+-rw-r--r--   0        0        0    13080 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/interface.py
+-rw-r--r--   0        0        0      769 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/metadata/__init__.py
+-rw-r--r--   0        0        0     5145 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/codecs.py
+-rw-r--r--   0        0        0    12475 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/config.py
+-rw-r--r--   0        0        0     7737 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/generate.py
+-rw-r--r--   0        0        0    14671 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/person.py
+-rw-r--r--   0        0        0     3125 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/repository.py
+-rw-r--r--   0        0        0     2373 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/subset.py
+-rw-r--r--   0        0        0     6384 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/utility.py
+-rw-r--r--   0        0        0     1461 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/utterance.py
+-rw-r--r--   0        0        0     4296 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/verify.py
+-rw-r--r--   0        0        0     1657 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/preprocess.py
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.4/pyriksprot/scripts/__init__.py
+-rw-r--r--   0        0        0     1596 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/scripts/csv2pgsql.py
+-rw-r--r--   0        0        0     1648 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/scripts/fix_speaker_notes.py
+-rw-r--r--   0        0        0     3543 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/scripts/metadata2db.py
+-rw-r--r--   0        0        0     2789 2023-04-19 09:21:24.587202 pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2speech.py
+-rw-r--r--   0        0        0     3475 2023-04-19 09:07:54.192237 pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2speech_text.py
+-rw-r--r--   0        0        0     2902 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2tagged.py
+-rw-r--r--   0        0        0     4650 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2text.py
+-rw-r--r--   0        0        0      487 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2tfs.py
+-rwxr-xr-x   0        0        0      680 2023-01-24 09:13:07.494512 pyriksprot-2023.4.4/pyriksprot/scripts/speaker_note2csv
+-rw-r--r--   0        0        0     2568 2023-01-24 09:13:07.494512 pyriksprot-2023.4.4/pyriksprot/scripts/speech_index.py
+-rw-r--r--   0        0        0     1162 2023-04-19 09:21:24.591202 pyriksprot-2023.4.4/pyriksprot/scripts/subset_corpus.py
+-rw-r--r--   0        0        0     5266 2023-01-24 09:13:07.494512 pyriksprot-2023.4.4/pyriksprot/scripts/utils.py
+-rwxr-xr-x   0        0        0      541 2023-01-24 09:13:07.494512 pyriksprot-2023.4.4/pyriksprot/scripts/xml2csv
+-rw-r--r--   0        0        0      599 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/00_rename.sql
+-rw-r--r--   0        0        0     4522 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/01_data_updates.sql
+-rw-r--r--   0        0        0     2592 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/02_code_tables.sql
+-rw-r--r--   0        0        0     2199 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/03_persons_of_interest.sql
+-rw-r--r--   0        0        0     5973 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/04_terms_of_office.sql
+-rw-r--r--   0        0        0     2818 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/05_person_party.sql
+-rw-r--r--   0        0        0     1707 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/06_unknown.sql
+-rw-r--r--   0        0        0     1344 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/09_cleanup.sql
+-rw-r--r--   0        0        0      204 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/__init__.py
+-rw-r--r--   0        0        0     7144 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/to_speech.py
+-rw-r--r--   0        0        0    14138 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/utility.py
+-rw-r--r--   0        0        0      266 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/workflows/__init__.py
+-rw-r--r--   0        0        0     1415 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/workflows/_extract_speech_ids.py
+-rw-r--r--   0        0        0     4429 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/workflows/extract_speech_text.py
+-rw-r--r--   0        0        0     6449 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/workflows/extract_tags.py
+-rw-r--r--   0        0        0     4556 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/workflows/extract_text.py
+-rw-r--r--   0        0        0     3254 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/workflows/speech_index.py
+-rw-r--r--   0        0        0     2230 2023-04-13 13:53:26.190262 pyriksprot-2023.4.4/pyriksprot/workflows/subset_corpus.py
+-rw-r--r--   0        0        0     7476 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/workflows/tag.py
+-rw-r--r--   0        0        0     4159 2023-04-19 09:21:24.591202 pyriksprot-2023.4.4/pyriksprot/workflows/tf.py
+-rw-r--r--   0        0        0     8856 1970-01-01 00:00:00.000000 pyriksprot-2023.4.4/PKG-INFO
```

### Comparing `pyriksprot-2023.4.3/LICENSE` & `pyriksprot-2023.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/README.md` & `pyriksprot-2023.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyproject.toml` & `pyriksprot-2023.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyriksprot"
-version = "2023.4.3"
+version = "2023.4.4"
 description = "Python API for Riksdagens Protokoll"
 authors = ["Roger Mähler <roger.mahler@hotmail.com>"]
 packages = [
     { include = "pyriksprot" },
 ]
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
@@ -32,14 +32,17 @@
 pyarrow = "*"
 more-itertools = "*"
 python-dotenv = "*"
 unidecode = "^1.3.6"
 pygit2 = "^1.11.1"
 sqlalchemy = "^2.0.6"
 psycopg2-binary = "^2.9.5"
+nltk = "^3.8.1"
+dynaconf = "^3.1.12"
+pathvalidate = "^2.5.2"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 coverage = "*"
 flake8 = "*"
 flake8-black = "*"
 isort = "*"
```

### Comparing `pyriksprot-2023.4.3/pyriksprot/__init__.py` & `pyriksprot-2023.4.4/pyriksprot/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # type: ignore
 
 from . import metadata
 from .corpus.corpus_index import CorpusSourceIndex, ICorpusSourceItem
 from .corpus.iterate import ProtocolSegment, ProtocolSegmentIterator
-from .corpus.parlaclarin import pretokenize
 from .dehyphenation import SwedishDehyphenator
 from .dispatch import DispatchItem, SegmentMerger, create_grouping_hashcoder
 from .interface import ParlaClarinError, Protocol, SegmentLevel, Speech, Utterance
+from .preprocess import dedent, dehyphen, pretokenize
 from .to_speech import MergerFactory, MergeStrategyType, to_speeches
 from .utility import (
     compose,
-    dedent,
     deprecated,
     dget,
     dotget,
     ensure_path,
     flatten,
     hasattr_path,
     is_empty,
```

### Comparing `pyriksprot-2023.4.3/pyriksprot/corpus/corpus_index.py` & `pyriksprot-2023.4.4/pyriksprot/corpus/corpus_index.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/corpus/iterate.py` & `pyriksprot-2023.4.4/pyriksprot/corpus/iterate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/iterate.py` & `pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/iterate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/parse.py` & `pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Any, Iterable
 
 from loguru import logger
 
 from pyriksprot import interface
 from pyriksprot.foss import untangle
-from pyriksprot.utility import dedent as dedent_text
+from pyriksprot.preprocess import dedent as dedent_text
 
 XML_ID: str = '{http://www.w3.org/XML/1998/namespace}id'
 
 # pylint: disable=too-many-statements
 
 
 class ProtocolMapper(interface.IProtocolParser):
```

### Comparing `pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt` & `pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt` & `pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt` & `pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/tf.py` & `pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/tf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pickle
 from collections import defaultdict
 from typing import Any, Callable, Dict, Iterable, List, Union
 
 from tqdm.auto import tqdm
 
-from pyriksprot.foss.sparv_tokenize import default_tokenize
+from pyriksprot.foss.sparv_tokenize import SegmenterRepository
 
 from .iterate import XmlProtocolSegmentIterator, XmlUntangleSegmentIterator
 
 
 class TermFrequencyCounter:
     """Term frequency container.
 
@@ -19,15 +19,15 @@
     def __init__(self, tokenizer: Callable[[str], List[str]] = None, do_lower_case: bool = True, progress: bool = True):
         """
         Args:
             tokenizer (Callable[[str], List[str]], optional): Tokenizer to use when ingesting tokens. Defaults to None.
             do_lower_case (bool, optional): [description]. Defaults to True.
         """
 
-        self._tokenize: Callable[[Any], List[str]] = tokenizer or default_tokenize
+        self._tokenize: Callable[[Any], List[str]] = tokenizer or SegmenterRepository.create_tokenize(False, False)
         self._do_lower_case: bool = do_lower_case
         self._progress: bool = progress
 
         self.frequencies: Dict[str, int] = defaultdict(int)
 
     def ingest(self, value: Union[str, Iterable[str], XmlUntangleSegmentIterator]) -> "TermFrequencyCounter":
         """Update term frequencies with term counts in `value`"""
```

### Comparing `pyriksprot-2023.4.3/pyriksprot/corpus/tagged/iterate.py` & `pyriksprot-2023.4.4/pyriksprot/corpus/tagged/iterate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/corpus/tagged/persist.py` & `pyriksprot-2023.4.4/pyriksprot/corpus/tagged/persist.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/corpus/utility.py` & `pyriksprot-2023.4.4/pyriksprot/corpus/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/dehyphenation/flair_dehyphen.py` & `pyriksprot-2023.4.4/pyriksprot/dehyphenation/flair_dehyphen.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/dehyphenation/swe_dehyphen.py` & `pyriksprot-2023.4.4/pyriksprot/dehyphenation/swe_dehyphen.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from dataclasses import dataclass, field
 from enum import IntEnum
 from os.path import isfile, join
 from typing import Callable
 
 from loguru import logger
 
+from ..configuration import ConfigValue, inject_config
 from .utility import load_dict, load_token_set, store_dict, store_token_set
 
 PARAGRAPH_MARKER = '##PARAGRAPH##'
 
 # pylint: disable=too-many-arguments
 jj = join
 
@@ -70,20 +71,23 @@
     MergeIfWordsOnlySeparatedByTwoNewlines = (1,)
     MergeAll = 2
 
 
 WORD_FREQUENCIES_NAME: str = 'word-frequencies.pkl'
 
 
+@inject_config
 @dataclass
 class SwedishDehyphenator:
     """Dehyphens Swedish text"""
 
-    data_folder: str
-    word_frequencies: dict[str, int] | str
+    data_folder: str | ConfigValue = ConfigValue.create_field(key="dehyphen:folder", default="/data")
+    word_frequencies: dict[str, int] | str | ConfigValue = ConfigValue.create_field(
+        key="dehyphen:tf_filename,tf_filename", default=None
+    )
 
     # Internal data
     whitelist: set[str] = field(default_factory=set)
     whitelist_log: dict[str, int] = field(default_factory=dict)
     unresolved: set[str] = field(default_factory=set)
 
     paragraph_merge_strategy: ParagraphMergeStrategy = 0
```

### Comparing `pyriksprot-2023.4.3/pyriksprot/dehyphenation/utility.py` & `pyriksprot-2023.4.4/pyriksprot/dehyphenation/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/dispatch/dispatch.py` & `pyriksprot-2023.4.4/pyriksprot/dispatch/dispatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import pandas as pd
 from loguru import logger
 
 from pyriksprot.corpus.iterate import ProtocolSegment
 from pyriksprot.dispatch.item import DispatchItem
 from pyriksprot.dispatch.utility import decode_protocol_segment_filename, to_temporal_category
 from pyriksprot.foss.pos_tags import PoS_Tag_Scheme, PoS_TAGS_SCHEMES
-from pyriksprot.foss.sparv_tokenize import default_tokenize
+from pyriksprot.foss.sparv_tokenize import SegmenterRepository
 from pyriksprot.foss.stopwords import STOPWORDS
 from pyriksprot.metadata import Codecs
 
 from .. import utility
 from ..interface import IDispatchItem, SegmentLevel
 
 jj = os.path.join
@@ -282,15 +282,15 @@
             segments: list[ProtocolSegment] = getattr(item, "protocol_segments")
             if len(segments) > 0:
                 return segments[0]
 
         raise ValueError(f"{type(self).__name__}: item has no protocol segments")
 
     def _dispatch_index_item(self, item: IDispatchItem) -> None:
-        tokens: list[str] = default_tokenize(item.text)
+        tokens: list[str] = SegmenterRepository.default_tokenize(item.text)
         tokens = [t for t in tokens if len(t) > 1 or t not in string.punctuation]
         item.n_tokens = len(tokens)
         return super()._dispatch_index_item(item)
 
     def _dispatch_item(self, item: IDispatchItem) -> None:
         speech: ProtocolSegment = self.to_speech_segment(item)
```

### Comparing `pyriksprot-2023.4.3/pyriksprot/dispatch/item.py` & `pyriksprot-2023.4.4/pyriksprot/dispatch/item.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/dispatch/merge.py` & `pyriksprot-2023.4.4/pyriksprot/dispatch/merge.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/dispatch/utility.py` & `pyriksprot-2023.4.4/pyriksprot/dispatch/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/foss/bettertokenizer.sv` & `pyriksprot-2023.4.4/pyriksprot/foss/resources/bettertokenizer.sv`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/foss/bettertokenizer.sv.saldo-tokens` & `pyriksprot-2023.4.4/pyriksprot/foss/resources/bettertokenizer.sv.saldo-tokens`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/foss/pos_tags.py` & `pyriksprot-2023.4.4/pyriksprot/foss/pos_tags.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/foss/stopwords.py` & `pyriksprot-2023.4.4/pyriksprot/foss/stopwords.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/foss/untangle.py` & `pyriksprot-2023.4.4/pyriksprot/foss/untangle.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/gitchen.py` & `pyriksprot-2023.4.4/pyriksprot/gitchen.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/interface.py` & `pyriksprot-2023.4.4/pyriksprot/interface.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/metadata/__init__.py` & `pyriksprot-2023.4.4/pyriksprot/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/metadata/codecs.py` & `pyriksprot-2023.4.4/pyriksprot/metadata/codecs.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/metadata/config.py` & `pyriksprot-2023.4.4/pyriksprot/metadata/config.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/metadata/generate.py` & `pyriksprot-2023.4.4/pyriksprot/metadata/generate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/metadata/person.py` & `pyriksprot-2023.4.4/pyriksprot/metadata/person.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/metadata/repository.py` & `pyriksprot-2023.4.4/pyriksprot/metadata/repository.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/metadata/subset.py` & `pyriksprot-2023.4.4/pyriksprot/metadata/subset.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/metadata/utility.py` & `pyriksprot-2023.4.4/pyriksprot/metadata/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/metadata/utterance.py` & `pyriksprot-2023.4.4/pyriksprot/metadata/utterance.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/metadata/verify.py` & `pyriksprot-2023.4.4/pyriksprot/metadata/verify.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/scripts/csv2pgsql.py` & `pyriksprot-2023.4.4/pyriksprot/scripts/csv2pgsql.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/scripts/fix_speaker_notes.py` & `pyriksprot-2023.4.4/pyriksprot/scripts/fix_speaker_notes.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/scripts/metadata2db.py` & `pyriksprot-2023.4.4/pyriksprot/scripts/metadata2db.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2speech.py` & `pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2speech.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2speech_text.py` & `pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2speech_text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2tagged.py` & `pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2tagged.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2text.py` & `pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/scripts/speaker_note2csv` & `pyriksprot-2023.4.4/pyriksprot/scripts/speaker_note2csv`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/scripts/speech_index.py` & `pyriksprot-2023.4.4/pyriksprot/scripts/speech_index.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/scripts/subset_corpus.py` & `pyriksprot-2023.4.4/pyriksprot/scripts/subset_corpus.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/scripts/utils.py` & `pyriksprot-2023.4.4/pyriksprot/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/scripts/xml2csv` & `pyriksprot-2023.4.4/pyriksprot/scripts/xml2csv`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/sql/00_rename.sql` & `pyriksprot-2023.4.4/pyriksprot/sql/00_rename.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/sql/01_data_updates.sql` & `pyriksprot-2023.4.4/pyriksprot/sql/01_data_updates.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/sql/02_code_tables.sql` & `pyriksprot-2023.4.4/pyriksprot/sql/02_code_tables.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/sql/03_persons_of_interest.sql` & `pyriksprot-2023.4.4/pyriksprot/sql/03_persons_of_interest.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/sql/04_terms_of_office.sql` & `pyriksprot-2023.4.4/pyriksprot/sql/04_terms_of_office.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/sql/05_person_party.sql` & `pyriksprot-2023.4.4/pyriksprot/sql/05_person_party.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/sql/06_unknown.sql` & `pyriksprot-2023.4.4/pyriksprot/sql/06_unknown.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/sql/09_cleanup.sql` & `pyriksprot-2023.4.4/pyriksprot/sql/09_cleanup.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/to_speech.py` & `pyriksprot-2023.4.4/pyriksprot/to_speech.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/utility.py` & `pyriksprot-2023.4.4/pyriksprot/utility.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,48 +34,74 @@
 
 def norm_join(a: str, *paths: str):
     """Joins paths and normalizes resulting path to current platform (i.e. sep)"""
     return normpath(jj(a, *paths))
 
 
 class dotdict(dict):
-    """dot.notation access to dictionary attributes"""
+    """dot.notation access to  dictionary attributes"""
 
     def __getattr__(self, *args):
         value = self.get(*args)
         return dotdict(value) if isinstance(value, dict) else value
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
 
-def dotget(data: dict, path: str | list[str], default: Any = None) -> Any:
+def dget(data: dict, *path: str | list[str], default: Any = None) -> Any:
     if path is None or not data:
         return default
 
     ps: list[str] = path if isinstance(path, (list, tuple)) else [path]
 
     d = None
 
     for p in ps:
-        d = data
-        for attr in p.split('.'):
-            d: dict = d.get(attr) if isinstance(d, dict) else None
-
-            if d is None:
-                break
+        d = dotget(data, p)
 
         if d is not None:
             return d
 
     return d or default
 
 
-def dget(data: dict, *paths: list[str], default: Any = None) -> Any:
-    return dotget(data, paths, default)
+def dotexists(data: dict, *paths: list[str]) -> bool:
+    for path in paths:
+        if dotget(data, path, default="@@") != "@@":
+            return True
+    return False
+
+
+def dotexpand(path: str) -> list[str]:
+    """Expands paths with ',' and ':'."""
+    paths = []
+    for p in path.replace(' ', '').split(','):
+        if not p:
+            continue
+        if ':' in p:
+            paths.extend([p.replace(":", "."), p.replace(":", "_")])
+        else:
+            paths.append(p)
+    return paths
+
+
+def dotget(data: dict, path: str, default: Any = None) -> Any:
+    """Gets element from dict. Path can be x.y.y or x_y_y or x:y:y.
+    if path is x:y:y then element is search using borh x.y.y or x_y_y."""
+
+    for key in dotexpand(path):
+        d: dict = data
+        for attr in key.split('.'):
+            d: dict = d.get(attr) if isinstance(d, dict) else None
+            if d is None:
+                break
+        if d is not None:
+            return d
+    return default
 
 
 def sync_delta_names(
     source_folder: str, source_extension: str, target_folder: str, target_extension: str, delete: bool = False
 ) -> Set(str):
     """Returns basenames in targat_folder that doesn't exist in source folder (with respectively extensions)"""
 
@@ -331,19 +357,14 @@
 def compose(*fns: Sequence[Callable[[str], str]]) -> Callable[[str], str]:
     """Create a composed function from a list of function. Return function."""
     if len(fns) == 0:
         return None
     return functools.reduce(lambda f, g: lambda *args: f(g(*args)), fns)
 
 
-def dedent(text: str) -> str:
-    """Remove whitespaces before and after newlines"""
-    return '\n'.join(x.strip() for x in text.split('\n'))
-
-
 def is_empty(filename: str) -> bool:
     """Check if file is empty."""
     return os.path.exists(filename) and os.stat(filename).st_size == 0
 
 
 def strip_csv_header(csv_str: str, sep: str = '\n') -> str:
     """Remove header line from `csv_str`"""
@@ -429,7 +450,32 @@
 
 def revdict(d: dict) -> dict:
     return {v: k for k, v in d.items()}
 
 
 def props(cls: Type) -> list[str]:
     return [i for i in cls.__dict__.keys() if i[:1] != '_']
+
+
+# def register(registry: dict | Type[Any], key: str = None):
+#     if not isinstance(registry, dict):
+#         if not hasattr(registry, "registry"):
+#             registry.registry = {}
+#             registry = registry.registry
+
+#     def registrar(func):
+#         registry[key or func.__name__] = func
+#         return func
+
+#     return registrar
+
+
+# class Registry:
+#     items: dict = {}
+
+#     @classmethod
+#     def register(cls, args):
+#         def decorator(fn):
+#             cls.items[fn.__name__] = args
+#             return fn
+
+#         return decorator
```

### Comparing `pyriksprot-2023.4.3/pyriksprot/workflows/_extract_speech_ids.py` & `pyriksprot-2023.4.4/pyriksprot/workflows/_extract_speech_ids.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/workflows/extract_speech_text.py` & `pyriksprot-2023.4.4/pyriksprot/workflows/extract_speech_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pyriksprot.corpus.iterate import ProtocolSegment
 from pyriksprot.corpus.parlaclarin import iterate
 
 from .. import dehyphenation
 from .. import dispatch as sd
 from .. import interface
 from .. import metadata as md
-from .. import utility
+from .. import preprocess as pp
 from ..corpus import corpus_index
 
 # pylint: disable=too-many-arguments
 
 jj = os.path.join
 
 
@@ -71,15 +71,15 @@
     dehypenator: dehyphenation.SwedishDehyphenator = (
         dehyphenation.SwedishDehyphenator(data_folder=data_path, word_frequencies=None) if dehyphen else None
     )
     speaker_service: md.SpeakerInfoService = md.SpeakerInfoService(database_filename=metadata_filename)
 
     def preprocess(item: ProtocolSegment) -> None:
         if dedent:
-            item.data = utility.dedent(item.data)
+            item.data = pp.dedent(item.data)
 
         if dehypenator:
             item.data = dehypenator(item.data)  # pylint: disable=not-callable
 
         item.speaker_info = speaker_service.get_speaker_info(u_id=item.u_id, person_id=item.who, year=item.year)
 
     segments: iterate.XmlUntangleSegmentIterator = iterate.XmlUntangleSegmentIterator(
```

### Comparing `pyriksprot-2023.4.3/pyriksprot/workflows/extract_tags.py` & `pyriksprot-2023.4.4/pyriksprot/workflows/extract_tags.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/workflows/extract_text.py` & `pyriksprot-2023.4.4/pyriksprot/workflows/extract_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from loguru import logger
 
 from pyriksprot.corpus.iterate import ProtocolSegment
 from pyriksprot.corpus.parlaclarin import iterate
 
 from .. import dehyphenation, interface
 from .. import metadata as md
-from .. import utility
+from .. import preprocess as pp
 from ..corpus import corpus_index
 from ..dispatch import dispatch, merge
 
 # pylint: disable=too-many-arguments
 
 
 def extract_corpus_text(
@@ -66,15 +66,15 @@
     dehypenator: dehyphenation.SwedishDehyphenator = (
         dehyphenation.SwedishDehyphenator(data_folder=data_path, word_frequencies=None) if dehyphen else None
     )
     speaker_service: md.SpeakerInfoService = md.SpeakerInfoService(database_filename=metadata_filename)
 
     def preprocess(item: ProtocolSegment) -> None:
         if dedent:
-            item.data = utility.dedent(item.data)
+            item.data = pp.dedent(item.data)
 
         if dehypenator:
             item.data = dehypenator(item.data)  # pylint: disable=not-callable
 
         if segment_level not in ('protocol', None):
             item.speaker_info = speaker_service.get_speaker_info(u_id=item.u_id, person_id=item.who, year=item.year)
```

### Comparing `pyriksprot-2023.4.3/pyriksprot/workflows/speech_index.py` & `pyriksprot-2023.4.4/pyriksprot/workflows/speech_index.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/workflows/subset_corpus.py` & `pyriksprot-2023.4.4/pyriksprot/workflows/subset_corpus.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/pyriksprot/workflows/tag.py` & `pyriksprot-2023.4.4/pyriksprot/workflows/tag.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 import abc
-import itertools
+import importlib
 from functools import reduce
 from glob import glob
 from os.path import dirname, getmtime, isfile, join, split
 from typing import Any, Callable, List, Mapping, Type, Union
 
 from loguru import logger
 from tqdm import tqdm
 
 from pyriksprot.corpus.parlaclarin import parse
 from pyriksprot.corpus.tagged import persist
 
 from .. import interface
+from .. import preprocess as pp
+from ..configuration import ConfigValue, inject_config
 from ..utility import ensure_path, strip_path_and_extension, touch, unlink
 
 METADATA_FILENAME: str = 'metadata.json'
 
 TaggedDocument = Mapping[str, List[str]]
 
 
@@ -27,15 +29,15 @@
     @abc.abstractmethod
     def create(self) -> "ITagger":
         ...
 
 
 class ITagger(abc.ABC):
     def __init__(self, preprocessors: Callable[[str], str] = None):
-        self.preprocessors: Callable[[str], str] = preprocessors or []
+        self.preprocessors: Callable[[str], str] = self.resolve_preprocessors(preprocessors)
 
     def tag(self, text: Union[str, List[str]], preprocess: bool = True) -> List[TaggedDocument]:
         """Tag text. Return dict if lists."""
         if isinstance(text, str):
             text = [text]
 
         if not isinstance(text, list):
@@ -58,34 +60,62 @@
     @abc.abstractmethod
     def _to_dict(self, tagged_document: Any) -> TaggedDocument:
         return {}
 
     @staticmethod
     def to_csv(tagged_document: TaggedDocument, sep='\t') -> str:
         """Converts a TaggedDocument to a TSV string"""
-
-        tokens, lemmas, pos, xpos = (
-            tagged_document['token'],
-            tagged_document['lemma'],
-            tagged_document['pos'],
-            tagged_document['xpos'],
-        )
-        csv_str = '\n'.join(
-            itertools.chain(
-                [f"token{sep}lemma{sep}pos{sep}xpos"],
-                (f"{tokens[i]}{sep}{lemmas[i]}{sep}{pos[i]}{sep}{xpos[i]}" for i in range(0, len(tokens))),
+        columns: list[str] = [c for c in ['token', 'lemma', 'pos', 'xpos', 'sentence_id'] if c in tagged_document]
+        csv_str: str = (
+            sep.join(columns)
+            + '\n'
+            + '\n'.join(
+                sep.join(str(tagged_document[c][i]) for c in columns) for i in range(0, len(tagged_document['token']))
             )
         )
         return csv_str
 
     def preprocess(self, text: str) -> str:
         """Transform `text` with preprocessors."""
         text: str = reduce(lambda res, f: f(res), self.preprocessors, text)
         return text
 
+    def resolve_preprocessors(self, preprocessors: str | list[Callable[[str], str] | str]):
+        if isinstance(preprocessors, str):
+            preprocessors = preprocessors.split(",")
+
+        if not any(isinstance(p, str) for p in preprocessors):
+            return preprocessors
+
+        self.is_satisfied(preprocessors)
+
+        return [pp.Registry.items.get(p) if isinstance(p, str) else p for p in preprocessors]
+
+    def is_satisfied(self, preprocessors: str | list[Callable[[str], str] | str]) -> bool:
+        keys: list[str] = [p for p in preprocessors if isinstance(p, str)]
+        unknown_keys: list[str] = [p for p in keys if not p in pp.Registry.items]
+        if unknown_keys:
+            raise ValueError(f"unknown preprocessor: {', '.join(unknown_keys)}")
+        return True
+
+
+class TaggerProvider:
+    @inject_config
+    @staticmethod
+    def tagger_factory(
+        module_name: str | ConfigValue = ConfigValue(key="tagger:module"),
+    ) -> ITaggerFactory:
+        if module_name is None:
+            return None
+        tagger_module = importlib.import_module(module_name)
+        abstract_factory = getattr(tagger_module, "tagger_factory")
+        if abstract_factory is None:
+            raise ValueError(f"Module {module_name} does not implement `tagger_factory`.")
+        return abstract_factory()
+
 
 class TaggerRegistry:
     """Simple tagger cache since somee taggers are expensive to setup"""
 
     instances: Mapping[Type[ITagger], ITagger] = {}
 
     @staticmethod
```

### Comparing `pyriksprot-2023.4.3/pyriksprot/workflows/tf.py` & `pyriksprot-2023.4.4/pyriksprot/workflows/tf.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.3/PKG-INFO` & `pyriksprot-2023.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriksprot
-Version: 2023.4.3
+Version: 2023.4.4
 Summary: Python API for Riksdagens Protokoll
 Home-page: https://westac.se
 License: Apache-2.0
 Author: Roger Mähler
 Author-email: roger.mahler@hotmail.com
 Requires-Python: >=3.11.0,<3.12.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,18 +13,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Dist: Jinja2
 Requires-Dist: click
+Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: loguru
 Requires-Dist: lz4
 Requires-Dist: more-itertools
+Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: pandas
+Requires-Dist: pathvalidate (>=2.5.2,<3.0.0)
 Requires-Dist: pdoc
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: pyarrow
 Requires-Dist: pygit2 (>=1.11.1,<2.0.0)
 Requires-Dist: python-dotenv
 Requires-Dist: requests
 Requires-Dist: sqlalchemy (>=2.0.6,<3.0.0)
```

