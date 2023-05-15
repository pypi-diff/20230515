# Comparing `tmp/mocodo-3.1.2.tar.gz` & `tmp/mocodo-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocodo-3.1.2.tar", max compression
+gzip compressed data, was "mocodo-3.2.0.tar", max compression
```

## Comparing `mocodo-3.1.2.tar` & `mocodo-3.2.0.tar`

### file list

```diff
@@ -1,97 +1,98 @@
--rw-r--r--   0        0        0     1072 2017-09-06 13:23:36.000000 mocodo-3.1.2/LICENSE
--rw-r--r--   0        0        0     5502 2023-05-11 17:23:34.304546 mocodo-3.1.2/README.md
--rw-r--r--   0        0        0       75 2022-09-05 13:09:15.074760 mocodo-3.1.2/mocodo/__init__.py
--rwxr-xr-x   0        0        0     3798 2022-11-02 08:58:46.486058 mocodo-3.1.2/mocodo/__main__.py
--rwxr-xr-x   0        0        0    16632 2023-01-28 11:18:09.584553 mocodo-3.1.2/mocodo/argument_parser.py
--rwxr-xr-x   0        0        0     8988 2022-09-29 15:13:08.365059 mocodo-3.1.2/mocodo/arrange_bb.py
--rwxr-xr-x   0        0        0     5511 2022-09-22 13:40:19.000000 mocodo-3.1.2/mocodo/arrange_ga.py
--rwxr-xr-x   0        0        0    21157 2022-11-18 08:55:22.092728 mocodo-3.1.2/mocodo/association.py
--rwxr-xr-x   0        0        0     3903 2022-09-05 13:09:15.079105 mocodo-3.1.2/mocodo/attribute.py
--rwxr-xr-x   0        0        0     5886 2023-01-28 11:16:39.787010 mocodo-3.1.2/mocodo/common.py
--rwxr-xr-x   0        0        0     1437 2022-09-05 13:09:15.080189 mocodo-3.1.2/mocodo/cross.py
--rw-r--r--   0        0        0     1991 2022-09-05 13:09:15.080684 mocodo-3.1.2/mocodo/damerau_levenshtein.py
--rwxr-xr-x   0        0        0     4484 2022-09-05 13:09:15.081151 mocodo-3.1.2/mocodo/diagram_link.py
--rwxr-xr-x   0        0        0     6558 2022-12-12 09:58:24.000000 mocodo-3.1.2/mocodo/entity.py
--rwxr-xr-x   0        0        0      228 2022-09-05 13:09:15.082116 mocodo-3.1.2/mocodo/file_helpers.py
--rwxr-xr-x   0        0        0     1280 2022-09-05 13:09:15.082712 mocodo-3.1.2/mocodo/fitness.py
--rwxr-xr-x   0        0        0     1110 2023-01-28 11:16:39.787918 mocodo-3.1.2/mocodo/font_metrics.py
--rwxr-xr-x   0        0        0     1957 2022-09-05 13:09:15.083736 mocodo-3.1.2/mocodo/grid.py
--rwxr-xr-x   0        0        0    22715 2022-09-18 13:16:09.863651 mocodo-3.1.2/mocodo/leg.py
--rw-r--r--   0        0        0     5334 2022-12-12 12:51:27.098572 mocodo-3.1.2/mocodo/magic_command.py
--rwxr-xr-x   0        0        0    22987 2023-01-28 11:18:09.585379 mocodo-3.1.2/mocodo/mcd.py
--rw-r--r--   0        0        0    10653 2023-01-28 11:18:09.586112 mocodo-3.1.2/mocodo/mcd_to_svg.py
--rwxr-xr-x   0        0        0      630 2022-09-18 17:39:21.116186 mocodo-3.1.2/mocodo/mocodo_error.py
--rwxr-xr-x   0        0        0     4172 2022-09-22 13:40:20.000000 mocodo-3.1.2/mocodo/obfuscate.py
--rwxr-xr-x   0        0        0      542 2022-09-05 13:09:15.088019 mocodo-3.1.2/mocodo/phantom.py
--rwxr-xr-x   0        0        0     1639 2022-09-12 10:44:29.393788 mocodo-3.1.2/mocodo/pluralize_fr.py
--rwxr-xr-x   0        0        0     4535 2023-01-28 11:16:39.790562 mocodo-3.1.2/mocodo/read_template.py
--rwxr-xr-x   0        0        0    35235 2023-01-28 11:16:39.791270 mocodo-3.1.2/mocodo/relations.py
--rw-r--r--   0        0        0      537 2022-09-05 13:09:15.089872 mocodo-3.1.2/mocodo/resources/colors/blank.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.090314 mocodo-3.1.2/mocodo/resources/colors/brewer+1.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.090722 mocodo-3.1.2/mocodo/resources/colors/brewer+2.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.090974 mocodo-3.1.2/mocodo/resources/colors/brewer+3.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.091207 mocodo-3.1.2/mocodo/resources/colors/brewer+4.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.091422 mocodo-3.1.2/mocodo/resources/colors/brewer+5.json
--rw-r--r--   0        0        0      574 2022-09-05 13:09:15.091816 mocodo-3.1.2/mocodo/resources/colors/brewer+6.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.092123 mocodo-3.1.2/mocodo/resources/colors/brewer+7.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.092664 mocodo-3.1.2/mocodo/resources/colors/brewer+8.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.093089 mocodo-3.1.2/mocodo/resources/colors/brewer+9.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.093664 mocodo-3.1.2/mocodo/resources/colors/brewer-1.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.093912 mocodo-3.1.2/mocodo/resources/colors/brewer-2.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.094140 mocodo-3.1.2/mocodo/resources/colors/brewer-3.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.094377 mocodo-3.1.2/mocodo/resources/colors/brewer-4.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.094632 mocodo-3.1.2/mocodo/resources/colors/brewer-5.json
--rw-r--r--   0        0        0      574 2022-09-05 13:09:15.094880 mocodo-3.1.2/mocodo/resources/colors/brewer-6.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.095161 mocodo-3.1.2/mocodo/resources/colors/brewer-7.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.095777 mocodo-3.1.2/mocodo/resources/colors/brewer-8.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.096030 mocodo-3.1.2/mocodo/resources/colors/brewer-9.json
--rw-r--r--   0        0        0      545 2022-12-08 07:24:06.000000 mocodo-3.1.2/mocodo/resources/colors/bw-alpha.json
--rw-r--r--   0        0        0      547 2022-12-08 07:24:30.000000 mocodo-3.1.2/mocodo/resources/colors/bw.json
--rw-r--r--   0        0        0      587 2022-09-05 13:09:15.097008 mocodo-3.1.2/mocodo/resources/colors/desert.json
--rw-r--r--   0        0        0      545 2022-09-05 13:09:15.097312 mocodo-3.1.2/mocodo/resources/colors/gray.json
--rw-r--r--   0        0        0      577 2022-09-05 13:09:15.097927 mocodo-3.1.2/mocodo/resources/colors/keepsake.json
--rw-r--r--   0        0        0      593 2022-09-05 13:09:15.098329 mocodo-3.1.2/mocodo/resources/colors/mondrian.json
--rw-r--r--   0        0        0      587 2022-09-05 13:09:15.098577 mocodo-3.1.2/mocodo/resources/colors/ocean.json
--rw-r--r--   0        0        0      587 2022-09-05 13:09:15.098954 mocodo-3.1.2/mocodo/resources/colors/pond.json
--rw-r--r--   0        0        0      550 2022-09-05 13:09:15.099350 mocodo-3.1.2/mocodo/resources/colors/wb.json
--rw-r--r--   0        0        0      592 2022-09-05 13:09:15.099599 mocodo-3.1.2/mocodo/resources/colors/xinnian.json
--rw-r--r--   0        0        0    99839 2022-09-05 13:09:15.100146 mocodo-3.1.2/mocodo/resources/font_metrics.json
--rw-r--r--   0        0        0    64345 2022-09-05 13:09:15.100633 mocodo-3.1.2/mocodo/resources/lorem/disparition.txt
--rw-r--r--   0        0        0     3200 2022-09-05 13:09:15.100777 mocodo-3.1.2/mocodo/resources/lorem/four_letter_words.txt
--rw-r--r--   0        0        0     2051 2022-09-05 13:09:15.100888 mocodo-3.1.2/mocodo/resources/lorem/lorem_ipsum.txt
--rw-r--r--   0        0        0      434 2023-05-11 16:54:02.232226 mocodo-3.1.2/mocodo/resources/pristine_sandbox.mcd
--rw-r--r--   0        0        0     3237 2022-12-11 18:28:56.187987 mocodo-3.1.2/mocodo/resources/relation_templates/debug.json
--rw-r--r--   0        0        0     1137 2023-01-28 11:16:39.791612 mocodo-3.1.2/mocodo/resources/relation_templates/dependencies.json
--rw-r--r--   0        0        0      973 2022-12-12 15:29:58.319997 mocodo-3.1.2/mocodo/resources/relation_templates/diagram.json
--rw-r--r--   0        0        0     1362 2022-12-13 17:17:49.267440 mocodo-3.1.2/mocodo/resources/relation_templates/html.json
--rw-r--r--   0        0        0    18311 2022-12-12 15:29:58.320955 mocodo-3.1.2/mocodo/resources/relation_templates/html_verbose.json
--rw-r--r--   0        0        0     7363 2022-12-12 15:29:58.321361 mocodo-3.1.2/mocodo/resources/relation_templates/json.json
--rw-r--r--   0        0        0     1253 2022-12-12 15:29:58.321750 mocodo-3.1.2/mocodo/resources/relation_templates/latex.json
--rw-r--r--   0        0        0      104 2023-01-28 11:16:39.792002 mocodo-3.1.2/mocodo/resources/relation_templates/latex_without_def.json
--rw-r--r--   0        0        0      421 2022-12-12 15:29:58.322622 mocodo-3.1.2/mocodo/resources/relation_templates/markdown.json
--rw-r--r--   0        0        0     1441 2022-12-12 15:29:58.323069 mocodo-3.1.2/mocodo/resources/relation_templates/markdown_data_dict.json
--rw-r--r--   0        0        0    14169 2022-12-12 15:29:58.323618 mocodo-3.1.2/mocodo/resources/relation_templates/markdown_verbose.json
--rw-r--r--   0        0        0     5065 2022-12-12 15:29:58.323968 mocodo-3.1.2/mocodo/resources/relation_templates/mysql.json
--rw-r--r--   0        0        0     5104 2022-12-12 15:29:58.324305 mocodo-3.1.2/mocodo/resources/relation_templates/oracle.json
--rw-r--r--   0        0        0     4918 2022-12-12 15:29:58.324644 mocodo-3.1.2/mocodo/resources/relation_templates/postgresql.json
--rw-r--r--   0        0        0     5311 2022-12-12 15:29:58.325008 mocodo-3.1.2/mocodo/resources/relation_templates/sqlite.json
--rw-r--r--   0        0        0       25 2023-01-28 11:16:39.792840 mocodo-3.1.2/mocodo/resources/relation_templates/text.json
--rw-r--r--   0        0        0      347 2022-12-12 09:58:24.000000 mocodo-3.1.2/mocodo/resources/relation_templates/txt2tags.json
--rw-r--r--   0        0        0     4777 2022-09-05 13:09:15.107446 mocodo-3.1.2/mocodo/resources/res/messages_de.mo
--rw-r--r--   0        0        0     8632 2023-01-28 11:16:39.793231 mocodo-3.1.2/mocodo/resources/res/messages_fr.mo
--rw-r--r--   0        0        0    10357 2023-01-28 11:16:39.793653 mocodo-3.1.2/mocodo/resources/res/messages_fr.po
--rw-r--r--   0        0        0     4048 2022-09-05 13:09:15.109006 mocodo-3.1.2/mocodo/resources/res/messages_zh.mo
--rw-r--r--   0        0        0     1213 2022-09-05 13:09:15.109826 mocodo-3.1.2/mocodo/resources/shapes/arial.json
--rw-r--r--   0        0        0     1215 2022-09-05 13:09:15.110327 mocodo-3.1.2/mocodo/resources/shapes/copperplate.json
--rw-r--r--   0        0        0     1205 2022-09-05 13:09:15.110856 mocodo-3.1.2/mocodo/resources/shapes/georgia.json
--rw-r--r--   0        0        0     1345 2022-09-05 13:09:15.111318 mocodo-3.1.2/mocodo/resources/shapes/mondrian.json
--rw-r--r--   0        0        0     1260 2022-09-05 13:09:15.112005 mocodo-3.1.2/mocodo/resources/shapes/sans.json
--rw-r--r--   0        0        0     1267 2022-09-05 13:09:15.112359 mocodo-3.1.2/mocodo/resources/shapes/serif.json
--rw-r--r--   0        0        0     1245 2022-09-05 13:09:15.112640 mocodo-3.1.2/mocodo/resources/shapes/times.json
--rw-r--r--   0        0        0     1230 2022-09-05 13:09:15.112988 mocodo-3.1.2/mocodo/resources/shapes/trebuchet.json
--rw-r--r--   0        0        0     1333 2022-09-05 13:09:15.113325 mocodo-3.1.2/mocodo/resources/shapes/verdana.json
--rw-r--r--   0        0        0     1245 2022-09-05 13:09:15.113890 mocodo-3.1.2/mocodo/resources/shapes/xinnian.json
--rw-r--r--   0        0        0       18 2023-05-11 17:20:56.321498 mocodo-3.1.2/mocodo/version_number.py
--rw-r--r--   0        0        0     1216 2023-05-11 17:20:56.246865 mocodo-3.1.2/pyproject.toml
--rw-r--r--   0        0        0     7291 1970-01-01 00:00:00.000000 mocodo-3.1.2/setup.py
--rw-r--r--   0        0        0     6712 1970-01-01 00:00:00.000000 mocodo-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2017-09-06 13:23:36.000000 mocodo-3.2.0/LICENSE
+-rw-r--r--   0        0        0     6729 2023-05-15 17:40:57.109268 mocodo-3.2.0/README.md
+-rw-r--r--   0        0        0       75 2022-09-05 13:09:15.074760 mocodo-3.2.0/mocodo/__init__.py
+-rwxr-xr-x   0        0        0     3798 2022-11-02 08:58:46.486058 mocodo-3.2.0/mocodo/__main__.py
+-rwxr-xr-x   0        0        0    16632 2023-01-28 11:18:09.584553 mocodo-3.2.0/mocodo/argument_parser.py
+-rwxr-xr-x   0        0        0     8988 2022-09-29 15:13:08.365059 mocodo-3.2.0/mocodo/arrange_bb.py
+-rwxr-xr-x   0        0        0     5511 2022-09-22 13:40:19.000000 mocodo-3.2.0/mocodo/arrange_ga.py
+-rwxr-xr-x   0        0        0    21404 2023-05-15 13:04:54.384907 mocodo-3.2.0/mocodo/association.py
+-rwxr-xr-x   0        0        0     3903 2022-09-05 13:09:15.079105 mocodo-3.2.0/mocodo/attribute.py
+-rwxr-xr-x   0        0        0     5886 2023-01-28 11:16:39.787010 mocodo-3.2.0/mocodo/common.py
+-rwxr-xr-x   0        0        0     4418 2023-05-15 17:43:30.305592 mocodo-3.2.0/mocodo/constraint.py
+-rwxr-xr-x   0        0        0     1437 2022-09-05 13:09:15.080189 mocodo-3.2.0/mocodo/cross.py
+-rw-r--r--   0        0        0     1991 2022-09-05 13:09:15.080684 mocodo-3.2.0/mocodo/damerau_levenshtein.py
+-rwxr-xr-x   0        0        0     4484 2022-09-05 13:09:15.081151 mocodo-3.2.0/mocodo/diagram_link.py
+-rwxr-xr-x   0        0        0     6558 2022-12-12 09:58:24.000000 mocodo-3.2.0/mocodo/entity.py
+-rwxr-xr-x   0        0        0      228 2022-09-05 13:09:15.082116 mocodo-3.2.0/mocodo/file_helpers.py
+-rwxr-xr-x   0        0        0     1280 2022-09-05 13:09:15.082712 mocodo-3.2.0/mocodo/fitness.py
+-rwxr-xr-x   0        0        0     1110 2023-01-28 11:16:39.787918 mocodo-3.2.0/mocodo/font_metrics.py
+-rwxr-xr-x   0        0        0     1957 2022-09-05 13:09:15.083736 mocodo-3.2.0/mocodo/grid.py
+-rwxr-xr-x   0        0        0    25987 2023-05-15 15:42:56.641165 mocodo-3.2.0/mocodo/leg.py
+-rw-r--r--   0        0        0     5334 2022-12-12 12:51:27.098572 mocodo-3.2.0/mocodo/magic_command.py
+-rwxr-xr-x   0        0        0    24808 2023-05-15 16:00:16.400968 mocodo-3.2.0/mocodo/mcd.py
+-rw-r--r--   0        0        0    11367 2023-05-15 14:17:26.992323 mocodo-3.2.0/mocodo/mcd_to_svg.py
+-rwxr-xr-x   0        0        0      630 2022-09-18 17:39:21.116186 mocodo-3.2.0/mocodo/mocodo_error.py
+-rwxr-xr-x   0        0        0     4807 2023-05-15 15:25:26.108679 mocodo-3.2.0/mocodo/obfuscate.py
+-rwxr-xr-x   0        0        0      542 2022-09-05 13:09:15.088019 mocodo-3.2.0/mocodo/phantom.py
+-rwxr-xr-x   0        0        0     1639 2022-09-12 10:44:29.393788 mocodo-3.2.0/mocodo/pluralize_fr.py
+-rwxr-xr-x   0        0        0     4535 2023-01-28 11:16:39.790562 mocodo-3.2.0/mocodo/read_template.py
+-rwxr-xr-x   0        0        0    35235 2023-01-28 11:16:39.791270 mocodo-3.2.0/mocodo/relations.py
+-rw-r--r--   0        0        0      650 2023-05-15 17:14:17.009755 mocodo-3.2.0/mocodo/resources/colors/blank.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.899518 mocodo-3.2.0/mocodo/resources/colors/brewer+1.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.907572 mocodo-3.2.0/mocodo/resources/colors/brewer+2.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.905622 mocodo-3.2.0/mocodo/resources/colors/brewer+3.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.903628 mocodo-3.2.0/mocodo/resources/colors/brewer+4.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.903285 mocodo-3.2.0/mocodo/resources/colors/brewer+5.json
+-rw-r--r--   0        0        0      693 2023-05-15 14:44:57.900653 mocodo-3.2.0/mocodo/resources/colors/brewer+6.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.900431 mocodo-3.2.0/mocodo/resources/colors/brewer+7.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.904370 mocodo-3.2.0/mocodo/resources/colors/brewer+8.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.902137 mocodo-3.2.0/mocodo/resources/colors/brewer+9.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.899761 mocodo-3.2.0/mocodo/resources/colors/brewer-1.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.905982 mocodo-3.2.0/mocodo/resources/colors/brewer-2.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.907245 mocodo-3.2.0/mocodo/resources/colors/brewer-3.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.901837 mocodo-3.2.0/mocodo/resources/colors/brewer-4.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.904980 mocodo-3.2.0/mocodo/resources/colors/brewer-5.json
+-rw-r--r--   0        0        0      693 2023-05-15 14:44:57.900217 mocodo-3.2.0/mocodo/resources/colors/brewer-6.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.901531 mocodo-3.2.0/mocodo/resources/colors/brewer-7.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.902965 mocodo-3.2.0/mocodo/resources/colors/brewer-8.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.903848 mocodo-3.2.0/mocodo/resources/colors/brewer-9.json
+-rw-r--r--   0        0        0      656 2023-05-15 17:13:10.230401 mocodo-3.2.0/mocodo/resources/colors/bw-alpha.json
+-rw-r--r--   0        0        0      660 2023-05-15 14:44:57.899228 mocodo-3.2.0/mocodo/resources/colors/bw.json
+-rw-r--r--   0        0        0      706 2023-05-15 17:13:10.207409 mocodo-3.2.0/mocodo/resources/colors/desert.json
+-rw-r--r--   0        0        0      658 2023-05-15 17:13:10.207350 mocodo-3.2.0/mocodo/resources/colors/gray.json
+-rw-r--r--   0        0        0      686 2023-05-15 17:13:10.206133 mocodo-3.2.0/mocodo/resources/colors/keepsake.json
+-rw-r--r--   0        0        0      715 2023-05-15 14:44:57.901018 mocodo-3.2.0/mocodo/resources/colors/mondrian.json
+-rw-r--r--   0        0        0      706 2023-05-15 17:13:44.139095 mocodo-3.2.0/mocodo/resources/colors/ocean.json
+-rw-r--r--   0        0        0      706 2023-05-15 17:13:07.899644 mocodo-3.2.0/mocodo/resources/colors/pond.json
+-rw-r--r--   0        0        0      663 2023-05-15 14:44:57.906877 mocodo-3.2.0/mocodo/resources/colors/wb.json
+-rw-r--r--   0        0        0      714 2023-05-15 14:44:57.907841 mocodo-3.2.0/mocodo/resources/colors/xinnian.json
+-rw-r--r--   0        0        0    99839 2022-09-05 13:09:15.100146 mocodo-3.2.0/mocodo/resources/font_metrics.json
+-rw-r--r--   0        0        0    64345 2022-09-05 13:09:15.100633 mocodo-3.2.0/mocodo/resources/lorem/disparition.txt
+-rw-r--r--   0        0        0     3200 2022-09-05 13:09:15.100777 mocodo-3.2.0/mocodo/resources/lorem/four_letter_words.txt
+-rw-r--r--   0        0        0     2051 2022-09-05 13:09:15.100888 mocodo-3.2.0/mocodo/resources/lorem/lorem_ipsum.txt
+-rw-r--r--   0        0        0      741 2023-05-15 17:23:22.354970 mocodo-3.2.0/mocodo/resources/pristine_sandbox.mcd
+-rw-r--r--   0        0        0     3237 2022-12-11 18:28:56.187987 mocodo-3.2.0/mocodo/resources/relation_templates/debug.json
+-rw-r--r--   0        0        0     1137 2023-01-28 11:16:39.791612 mocodo-3.2.0/mocodo/resources/relation_templates/dependencies.json
+-rw-r--r--   0        0        0      973 2022-12-12 15:29:58.319997 mocodo-3.2.0/mocodo/resources/relation_templates/diagram.json
+-rw-r--r--   0        0        0     1362 2022-12-13 17:17:49.267440 mocodo-3.2.0/mocodo/resources/relation_templates/html.json
+-rw-r--r--   0        0        0    18311 2022-12-12 15:29:58.320955 mocodo-3.2.0/mocodo/resources/relation_templates/html_verbose.json
+-rw-r--r--   0        0        0     7363 2022-12-12 15:29:58.321361 mocodo-3.2.0/mocodo/resources/relation_templates/json.json
+-rw-r--r--   0        0        0     1253 2022-12-12 15:29:58.321750 mocodo-3.2.0/mocodo/resources/relation_templates/latex.json
+-rw-r--r--   0        0        0      104 2023-01-28 11:16:39.792002 mocodo-3.2.0/mocodo/resources/relation_templates/latex_without_def.json
+-rw-r--r--   0        0        0      421 2022-12-12 15:29:58.322622 mocodo-3.2.0/mocodo/resources/relation_templates/markdown.json
+-rw-r--r--   0        0        0     1441 2022-12-12 15:29:58.323069 mocodo-3.2.0/mocodo/resources/relation_templates/markdown_data_dict.json
+-rw-r--r--   0        0        0    14169 2022-12-12 15:29:58.323618 mocodo-3.2.0/mocodo/resources/relation_templates/markdown_verbose.json
+-rw-r--r--   0        0        0     5065 2022-12-12 15:29:58.323968 mocodo-3.2.0/mocodo/resources/relation_templates/mysql.json
+-rw-r--r--   0        0        0     5104 2022-12-12 15:29:58.324305 mocodo-3.2.0/mocodo/resources/relation_templates/oracle.json
+-rw-r--r--   0        0        0     4918 2022-12-12 15:29:58.324644 mocodo-3.2.0/mocodo/resources/relation_templates/postgresql.json
+-rw-r--r--   0        0        0     5311 2022-12-12 15:29:58.325008 mocodo-3.2.0/mocodo/resources/relation_templates/sqlite.json
+-rw-r--r--   0        0        0       25 2023-01-28 11:16:39.792840 mocodo-3.2.0/mocodo/resources/relation_templates/text.json
+-rw-r--r--   0        0        0      347 2022-12-12 09:58:24.000000 mocodo-3.2.0/mocodo/resources/relation_templates/txt2tags.json
+-rw-r--r--   0        0        0     4777 2022-09-05 13:09:15.107446 mocodo-3.2.0/mocodo/resources/res/messages_de.mo
+-rw-r--r--   0        0        0     9078 2023-05-15 17:26:46.559028 mocodo-3.2.0/mocodo/resources/res/messages_fr.mo
+-rw-r--r--   0        0        0    10357 2023-01-28 11:16:39.793653 mocodo-3.2.0/mocodo/resources/res/messages_fr.po
+-rw-r--r--   0        0        0     4048 2022-09-05 13:09:15.109006 mocodo-3.2.0/mocodo/resources/res/messages_zh.mo
+-rw-r--r--   0        0        0     1451 2023-05-15 14:49:17.550663 mocodo-3.2.0/mocodo/resources/shapes/arial.json
+-rw-r--r--   0        0        0     1450 2023-05-15 16:37:09.601570 mocodo-3.2.0/mocodo/resources/shapes/copperplate.json
+-rw-r--r--   0        0        0     1441 2023-05-15 14:48:07.012008 mocodo-3.2.0/mocodo/resources/shapes/georgia.json
+-rw-r--r--   0        0        0     1599 2023-05-15 14:50:47.803027 mocodo-3.2.0/mocodo/resources/shapes/mondrian.json
+-rw-r--r--   0        0        0     1506 2023-05-15 14:41:58.295545 mocodo-3.2.0/mocodo/resources/shapes/sans.json
+-rw-r--r--   0        0        0     1514 2023-05-15 14:41:58.296140 mocodo-3.2.0/mocodo/resources/shapes/serif.json
+-rw-r--r--   0        0        0     1481 2023-05-15 14:51:53.188174 mocodo-3.2.0/mocodo/resources/shapes/times.json
+-rw-r--r--   0        0        0     1466 2023-05-15 14:52:43.367466 mocodo-3.2.0/mocodo/resources/shapes/trebuchet.json
+-rw-r--r--   0        0        0     1591 2023-05-15 14:55:47.087364 mocodo-3.2.0/mocodo/resources/shapes/verdana.json
+-rw-r--r--   0        0        0     1487 2023-05-15 14:56:47.062651 mocodo-3.2.0/mocodo/resources/shapes/xinnian.json
+-rw-r--r--   0        0        0       18 2023-05-15 16:44:12.700272 mocodo-3.2.0/mocodo/version_number.py
+-rw-r--r--   0        0        0     1216 2023-05-15 16:44:24.208663 mocodo-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8543 1970-01-01 00:00:00.000000 mocodo-3.2.0/setup.py
+-rw-r--r--   0        0        0     7939 1970-01-01 00:00:00.000000 mocodo-3.2.0/PKG-INFO
```

### Comparing `mocodo-3.1.2/LICENSE` & `mocodo-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/__main__.py` & `mocodo-3.2.0/mocodo/__main__.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/argument_parser.py` & `mocodo-3.2.0/mocodo/argument_parser.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/arrange_bb.py` & `mocodo-3.2.0/mocodo/arrange_bb.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/arrange_ga.py` & `mocodo-3.2.0/mocodo/arrange_ga.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/association.py` & `mocodo-3.2.0/mocodo/association.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 kind = "forced_table"
             name = name.replace("\\", "")
             name_view = (name[:-1] if name[-1:].isdigit() else name)
             return (name, name_view, kind)
         
         def clean_up_legs_and_attributes(
             legs_and_attributes,
-            match_leg = re.compile(r"((?:_11|/..|..)[<>]?\s+(?:\[.+?\]\s+)?)(.+)").match,
+            match_leg = re.compile(r"(-?(?:_11|/..|..)[<>]?\s+(?:\[.+?\]\s+)?)(.+)").match,
         ):
             (legs, attributes) = (legs_and_attributes.split(":", 1) + [""])[:2]
             (cards, entity_names) = ([], [])
             for leg in legs.split(","):
                 leg = leg.strip().replace("\\", "")
                 m = match_leg(leg)
                 if m:
@@ -80,19 +80,19 @@
                 elif cards[0][0] == "<":
                     cards[0] = cards[0][:2] + ">" + cards[0][2:]
             self.kind = f"inheritance: {cards[0][:2]}"
         elif kind == "forced_table":
             self.kind = kind
         else:
             candidate_peg_count = sum(card.startswith("/") for card in cards)
-            valid_peg_count = sum(card in ("/0N", "/1N") for card in cards)
+            valid_peg_count = sum(card.startswith(("/0N", "/1N")) for card in cards)
             if candidate_peg_count > valid_peg_count:
                 raise MocodoError(26, _('Only cardinalities "/0N" or "/1N" are permitted to start with a "/" character.').format(name=self.name)) # fmt: skip
             if valid_peg_count > 0:
-                valid_leg_count = sum(card in ("0N", "1N") for card in cards)
+                valid_leg_count = sum(card.startswith(("0N", "1N")) for card in cards)
                 if valid_leg_count < 1:
                     raise MocodoError(27, _('To become a cluster, association "{name}" must have at least one cardinality "0N" or "1N" (without "/").').format(name=self.name)) # fmt: skip
                 if valid_leg_count + valid_peg_count < len(cards):
                     raise MocodoError(28, _('''To become a cluster, association "{name}"'s cardinalities must all be "0N", "1N", "/0N" or "/1N".''').format(name=self.name)) # fmt: skip
                 self.kind = "cluster"
             else:
                 self.kind = "association"
@@ -101,18 +101,22 @@
         for (i, (card, name)) in enumerate(zip(cards, entity_names)):
             leg = Leg(self, card, name, **params)
             mutiplicity = entity_names.count(name)
             rank = entity_names[:i].count(name)
             leg.set_spin_strategy(0 if mutiplicity == 1 else 2 * rank / (mutiplicity - 1) - 1)
             self.legs.append(leg)
 
-
     def register_boxes(self, boxes):
         self.boxes = boxes
 
+    def register_mcd_has_cif(self, mcd_has_cif):
+        self.mcd_has_cif = mcd_has_cif
+        for leg in self.legs:
+            leg.register_mcd_has_cif(mcd_has_cif)
+
     def calculate_size(self, style, get_font_metrics):
         cartouche_font = get_font_metrics(style["association_cartouche_font"])
         self.get_cartouche_string_width = cartouche_font.get_pixel_width
         self.cartouche_height = cartouche_font.get_pixel_height()
         attribute_font = get_font_metrics(style["association_attribute_font"])
         self.attribute_height = attribute_font.get_pixel_height()
         self.calculate_size_depending_on_kind(style, get_font_metrics)
@@ -208,14 +212,16 @@
                         "family": style["association_cartouche_font"]["family"],
                         "size": style["association_cartouche_font"]["size"],
                     },
                 ),
             ]
         
         def optional_description_for_cluster(style):
+            if self.mcd_has_cif:
+                return []
             clustered_entities = [leg.entity for leg in self.legs if leg.kind == "cluster_leg"]
             if len(clustered_entities) == 2:
                 (e1, e2) = clustered_entities
             elif len(clustered_entities) == 1:
                 e1 = e2 = clustered_entities[0]
             else:
                 return []
```

### Comparing `mocodo-3.1.2/mocodo/attribute.py` & `mocodo-3.2.0/mocodo/attribute.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/common.py` & `mocodo-3.2.0/mocodo/common.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/cross.py` & `mocodo-3.2.0/mocodo/cross.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/damerau_levenshtein.py` & `mocodo-3.2.0/mocodo/damerau_levenshtein.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/diagram_link.py` & `mocodo-3.2.0/mocodo/diagram_link.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/entity.py` & `mocodo-3.2.0/mocodo/entity.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/fitness.py` & `mocodo-3.2.0/mocodo/fitness.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/font_metrics.py` & `mocodo-3.2.0/mocodo/font_metrics.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/grid.py` & `mocodo-3.2.0/mocodo/grid.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/leg.py` & `mocodo-3.2.0/mocodo/leg.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,21 +16,25 @@
 
 class Leg:
     def __init__(
         self,
         association,
         card,
         entity_name,
-        match_card=re.compile(r"(_11|/0N|/1N|..)([<>]?)\s*(?:\[(.+?)\])?").match,
+        match_card=re.compile(r"(-?(?:_11|/0N|/1N|..))([<>]?)\s*(?:\[(.+?)\])?").match,
         **params,
     ):
         params["strengthen_card"] = params.get("strengthen_card", "_1,1_")
         params["card_format"] = params.get("card_format", "{min_card},{max_card}")
         (card, arrow, note) = match_card(card).groups()
         kind = "leg"
+        is_masked = False
+        if card.startswith("-"):
+            card = card[1:]
+            is_masked = True
         if card == "_11":
             kind = "strengthening"
             card = "11"
             card_view = params["strengthen_card"]
         elif association.kind == "cluster":
             if card.startswith("/"):
                 kind = "cluster_peg"
@@ -48,26 +52,31 @@
             else:
                 card_view = "     "
         elif card.startswith("XX"):
             card_view = "     "
         else:
             card = auto_correction.get(card, card)
             card_view = params["card_format"].format(min_card=card[0], max_card=card[1])
+        if is_masked:
+            card_view = "     "
         self.card = card
         self.arrow = arrow
         self.kind = kind
         self.card_view = card_view
         self.note = note and note.replace("<<<safe-comma>>>", ",").replace("<<<safe-colon>>>", ":")
         self.association = association
         self.entity_name = entity_name
         self.twist = False
         self.identifier = None
 
     def register_entity(self, entity):
         self.entity = entity
+    
+    def register_mcd_has_cif(self, mcd_has_cif):
+        self.mcd_has_cif = mcd_has_cif
 
     def calculate_size(self, style, get_font_metrics):
         font = get_font_metrics(style["card_font"])
         self.h = font.get_pixel_height()
         self.w = font.get_pixel_width(self.card_view.strip("_"))
 
     def set_spin_strategy(self, spin):
@@ -90,15 +99,15 @@
         card_margin = style["card_margin"]
         cw = self.w + 2 * card_margin
         ch = self.h + 2 * card_margin
         leg = straight_leg_factory(ex, ey, ew, eh, ax, ay, aw, ah, cw, ch, card_margin)
         if self.kind == "cluster_peg":
             result.append(
                 (
-                    "dash_line",
+                    "line" if self.mcd_has_cif else "dash_line",
                     {
                         "x0": ex,
                         "y0": ey,
                         "x1": ax,
                         "y1": ay,
                         "stroke_color": style["leg_stroke_color"],
                         "stroke_depth": style["leg_stroke_depth"],
@@ -305,14 +314,95 @@
                         "stroke_color": style["leg_stroke_color"],
                     },
                 ),
             )
         return result
 
 
+class ConstraintLeg:
+
+    def __init__(self, constraint, kind, box_name):
+        self.constraint = constraint
+        self.kind = kind
+        self.box_name = box_name
+        self.identifier = None
+    
+    def register_box(self, box):
+        self.box = box
+    
+    def description(self, style, geo):
+        if self.kind == "": # a phantom leg, useful to tweak the barycenter
+            return []
+        result = []
+        bx = self.box.cx
+        by = self.box.cy
+        bw = self.box.w // 2
+        bh = self.box.h // 2
+        cx = self.constraint.cx
+        cy = self.constraint.cy
+        cw = self.constraint.w // 2
+        ch = self.constraint.h // 2
+        leg = straight_leg_factory(bx, by, bw, bh, cx, cy, cw, ch)
+        kind = self.kind
+        for direction in "<>":
+            if direction in self.kind:
+                (x, y, a, b) = leg.arrow_pos(direction, 1)
+                c = hypot(a, b) or 1
+                (cos, sin) = (a / c, b / c)
+                result.append(
+                    (
+                        "arrow",
+                        {
+                            "x0": x,
+                            "y0": y,
+                            "x1": x + style["arrow_width"] * cos - style["arrow_half_height"] * sin,
+                            "y1": y - style["arrow_half_height"] * cos - style["arrow_width"] * sin,
+                            "x2": x + style["arrow_axis"] * cos,
+                            "y2": y - style["arrow_axis"] * sin,
+                            "x3": x + style["arrow_width"] * cos + style["arrow_half_height"] * sin,
+                            "y3": y + style["arrow_half_height"] * cos - style["arrow_width"] * sin,
+                            "stroke_color": style["constraint_stroke_color"],
+                        },
+                    ),
+                )
+                kind = kind.replace(direction, "")
+        if kind[:1] == "-":
+            result.append(
+                (
+                    "line",
+                    {
+                        "x0": bx,
+                        "y0": by,
+                        "x1": cx,
+                        "y1": cy,
+                        "stroke_color": style["constraint_stroke_color"],
+                        "stroke_depth": style["constraint_stroke_depth"],
+                    }
+                )
+            )
+        elif kind[:1] == ".":
+            result.append(
+                (
+                    "dot_line",
+                    {
+                        "x0": bx,
+                        "y0": by,
+                        "x1": cx,
+                        "y1": cy,
+                        "stroke_color": style["constraint_stroke_color"],
+                        "stroke_depth": style["constraint_dot_stroke_depth"],
+                        "dash_gap": style["constraint_dot_gap_width"],
+                    }
+                )
+            )
+        else:
+            raise NotImplementedError
+        return result
+
+
 class DiagramLink:
     def __init__(self, entities, foreign_entity, foreign_key):
         self.foreign_entity = foreign_entity
         self.foreign_key = foreign_key
         try:
             self.primary_entity = entities[foreign_key.primary_entity_name]
         except KeyError:
@@ -422,15 +512,15 @@
     y = ey + (ay - ey) * (x - ex) / (ax - ex)
     if abs(y - ey) > h:
         y = ey + cmp(ay, ey) * h
         x = ex + (ax - ex) * (y - ey) / (ay - ey)
     return (x, y)
 
 
-def straight_leg_factory(ex, ey, ew, eh, ax, ay, aw, ah, cw, ch, card_margin):
+def straight_leg_factory(ex, ey, ew, eh, ax, ay, aw, ah, cw=0, ch=0, card_margin=0):
     def card_pos(twist, shift):
         compare = operator.lt if twist else operator.le
         correction = 1 - abs(abs(ax - ex) - abs(ay - ey)) / hypot(ax - ex, ay - ey)
         correction = card_margin * 1.4142 * correction - shift
         (xg, yg) = line_intersection(ex, ey, ew, eh + ch, ax, ay)
         (xb, yb) = line_intersection(ex, ey, ew + cw, eh, ax, ay)
         if compare(xg, xb):
```

### Comparing `mocodo-3.1.2/mocodo/magic_command.py` & `mocodo-3.2.0/mocodo/magic_command.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/mcd.py` & `mocodo-3.2.0/mocodo/mcd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from email.policy import default
 import itertools
 import re
 from collections import defaultdict
 from hashlib import md5
 
 from .association import Association
+from .constraint import Constraint
 from .diagram_link import DiagramLink
 from .entity import Entity
 from .grid import Grid
 from .mocodo_error import MocodoError
 from .phantom import Phantom
 
 def cmp(x, y):
@@ -26,35 +27,46 @@
                 return f"{h[:8]}_{params['uid_suffix']}"
             else:
                 return h[:8]
 
         def parse_clauses():
             self.entities = {}
             self.associations = {}
+            self.constraints = []
+            mcd_has_cif = False
+            self.commented_lines = []
+            self.constraint_clauses = []
             seen = set()
             self.rows = [[]]
-            self.header = ""
             pages = defaultdict(list)
             for clause in clauses:
                 indentation = len(clause) - len(clause.lstrip())
                 clause = clause.strip(" \n\r\t")
                 if not clause:
                     self.rows.append([])
                     continue
                 if clause.startswith("%"):
                     if not self.rows[-1]:
-                        self.header += "%s\n" % clause
+                        self.commented_lines.append(clause)
                     continue
                 if clause == ":" * len(clause):
                     self.rows[-1].extend(Phantom(next(phantom_counter)) for _ in clause)
                     continue
                 if clause.startswith(":"):
                     raise MocodoError(19, _('The clause "{clause}" starts with a colon.').format(clause=clause)) # fmt: skip
-                clause = re.sub("\[.+?\]", substitute_forbidden_symbols_between_brackets, clause)
-                if "," in clause.split(":", 1)[0] or re.match(r"\s*(/\w*\\)", clause):
+                clause = re.sub(r"\[.+?\]", substitute_forbidden_symbols_between_brackets, clause)
+                if re.match(r"\s*\(.{0,3}\)", clause):
+                    element = Constraint(clause)
+                    if element.name == "CIF":
+                        mcd_has_cif = True
+                    self.constraints.append(element)
+                    pages[indentation].append(element)
+                    self.constraint_clauses.append(clause)
+                    continue
+                elif "," in clause.split(":", 1)[0] or re.match(r"\s*(/\w*\\)", clause):
                     element = Association(clause, **params)
                     if element.name in self.associations:
                         raise MocodoError(7, _('Duplicate association "{name}". If you want to make two associations appear with the same name, you must suffix it with a number.').format(name=element.name)) # fmt: skip
                     self.associations[element.name] = element
                     pages[indentation].append(element)
                 elif ":" in clause:
                     element = Entity(clause)
@@ -73,26 +85,38 @@
             self.rows = [row for row in self.rows if row]
             self.col_count = max(len(row) for row in self.rows)
             self.row_count = len(self.rows)
             self.page_count = len(pages)
             for (i, (indentation, elements)) in enumerate(sorted(pages.items(), key=lambda x: x[0])):
                 for element in elements:
                     element.page = i
+            self.header = "\n".join(self.commented_lines) + "\n\n" if self.commented_lines else ""
+            self.footer = "\n\n" + "\n".join(self.constraint_clauses) if self.constraint_clauses else ""
+            for association in self.associations.values():
+                association.register_mcd_has_cif(mcd_has_cif)
         
         def add_legs():
             for association in self.associations.values():
                 for leg in association.legs:
-                    try:
+                    if leg.entity_name in self.entities:
                         entity = self.entities[leg.entity_name]
-                    except KeyError:
-                        if leg.entity_name in self.associations:
-                            raise MocodoError(20, _('Association "{association}" linked to another association "{entity}"!').format(association=association.name, entity=leg.entity_name)) # fmt: skip
-                        else:
-                            raise MocodoError(1, _('Association "{association}" linked to an unknown entity "{entity}"!').format(association=association.name, entity=leg.entity_name)) # fmt: skip
+                    elif leg.entity_name in self.associations:
+                        raise MocodoError(20, _('Association "{association}" linked to another association "{entity}"!').format(association=association.name, entity=leg.entity_name)) # fmt: skip
+                    else:
+                        raise MocodoError(1, _('Association "{association}" linked to an unknown entity "{entity}"!').format(association=association.name, entity=leg.entity_name)) # fmt: skip
                     leg.register_entity(entity)
+            for constraint in self.constraints:
+                for leg in constraint.legs:
+                    if leg.box_name in self.associations:
+                        box = self.associations[leg.box_name]
+                    elif leg.box_name in self.entities:
+                        box = self.entities[leg.box_name]
+                    else:
+                        raise MocodoError(40, _('Constraint "{constraint}" linked to an unknown entity or association "{box}"!').format(constraint=constraint.name, box=leg.box_name)) # fmt: skip
+                    leg.register_box(box)
         
         def add_attributes():
             legs_to_strengthen = dict((entity_name, []) for entity_name in self.entities)
             children = set()
             for association in self.associations.values():
                 for leg in association.legs:
                     if association.kind.startswith("inheritance") and leg.card == "XX":
@@ -266,24 +290,24 @@
     
     def get_clauses(self):
         result = self.header
         if self.associations:
             result += "\n\n".join(self.get_row_text(row) for row in self.rows)
         else:
             result += "\n\n".join(":\n" + "\n:\n".join(self.get_row_text(row).split("\n")) + "\n:" for row in self.rows)
-        return result
+        return result + self.footer
     
     def get_clauses_horizontal_mirror(self):
-        return self.header + "\n\n".join(self.get_row_text(row) for row in self.rows[::-1])
+        return self.header + "\n\n".join(self.get_row_text(row) for row in self.rows[::-1]) + self.footer
     
     def get_clauses_vertical_mirror(self):
-        return self.header + "\n\n".join(self.get_row_text(row[::-1]) for row in self.rows)
+        return self.header + "\n\n".join(self.get_row_text(row[::-1]) for row in self.rows) + self.footer
     
     def get_clauses_diagonal_mirror(self):
-        return self.header + "\n\n".join(self.get_row_text(row) for row in zip(*self.rows))
+        return self.header + "\n\n".join(self.get_row_text(row) for row in zip(*self.rows)) + self.footer
     
     def get_reformatted_clauses(self, nth_fit):
         grid = Grid(len(self.boxes) + 100) # make sure there are enough precalculated grids
         start = len(self.entities) + len(self.associations) # number of nonempty boxes
         if nth_fit < 0:
             if (self.col_count, self.row_count) in grid: # the current grid is among precalculated ones
                 start = self.col_count * self.row_count # start from the completed grid
@@ -297,15 +321,15 @@
                     result.append("")
                 result.append("  " * box.page + box.clause)
                 i += 1
         for i in range(i, col_count * row_count):
             if i % col_count == 0 and i:
                 result.append("")
             result.append(":")
-        return self.header + "\n".join(result)
+        return self.header + "\n".join(result) + self.footer
     
     def calculate_size(self, style):
 
         def increase_margins_in_presence_of_clusters():
             for association in self.associations.values():
                 if association.kind == "cluster":
                     style["margin"] *= 2
@@ -323,14 +347,16 @@
         def calculate_sizes():
             for row in self.rows:
                 for (i, box) in enumerate(row):
                     box.calculate_size(style, self.get_font_metrics)
                     max_box_width_per_column[i] = max(box.w, max_box_width_per_column[i])
             for diagram_link in self.diagram_links:
                 diagram_link.calculate_size(style, self.get_font_metrics)
+            for constraint in self.constraints:
+                constraint.calculate_size(style, self.get_font_metrics)
         #
         def make_horizontal_layout():
             self.w = style["margin"]
             for row in self.rows:
                 horizontal_offset = style["margin"]
                 for (i, box) in enumerate(row):
                     box.x = horizontal_offset + (max_box_width_per_column[i] - box.w) // 2
@@ -387,21 +413,25 @@
         compress_horizontally()
         make_vertical_layout()
         compress_vertically()
     
     def description(self, style, geo):
         for box in self.boxes:
             box.register_center(geo)
+        for constraint in self.constraints:
+            constraint.register_center(geo)
         result = []
         for element in self.entities.values():
             result.extend(element.description(style, geo))
         for element in self.associations.values():
             result.extend(element.description(style, geo))
         for element in self.diagram_links:
             result.extend(element.description(style, geo))
+        for element in self.constraints:
+            result.extend(element.description(style, geo))
         result.append(("comment", {"text": "Notes"}))
         result.append(
             (
                 "notes",
                 {
                     "height_threshold": geo["height"] - style["note_overlay_height"] - style["card_margin"],
                     "overlay_height": style["note_overlay_height"],
```

### Comparing `mocodo-3.1.2/mocodo/mcd_to_svg.py` & `mocodo-3.2.0/mocodo/mcd_to_svg.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,23 @@
                 "background_color": style["background_color"],
             }
         ),
         *mcd.description(style, geo),
     ]
     has_note_card = False
     tabs = 0
-    categories = {"": [], "Association": [], "Entity": [], "Link": [], "Notes": [], "Pager": []}
+    categories = { # the order is that of the drawing in the SVG
+        "": [],
+        "Constraint": [],
+        "Association": [],
+        "Entity": [],
+        "Link": [],
+        "Notes": [],
+        "Pager": [],
+    }
     category = ""
     for (key, mapping) in description:
         mapping["mcd_uid"] = mcd.uid
         has_note_card |= key.endswith("with_note")
         if key == "comment":
             category = mapping["text"].partition(" ")[0]
         for (k, v) in mapping.items():
@@ -102,22 +110,25 @@
     "preamble":         """<?xml version="1.0" encoding="utf-8"?>\n<svg width="{width}" height="{total_height}" viewBox="0 0 {width} {total_height}" xmlns="http://www.w3.org/2000/svg">""",
     "background":       """<rect id="frame" x="0" y="0" width="{width}" height="{height}" fill="{background_color}" stroke="none" stroke-width="0"/>""",
     "comment":          """\n<!-- {text} -->""",
     "begin_component":  """<g class="page_{page}_{mcd_uid} diagram_page" visibility="{visibility}">""",
     "begin_group":      """<g>""",
     "end":              """</g>""",
     "text":             """<text x="{x}" y="{y}" fill="{text_color}" font-family="{family}" font-size="{size}">{text}</text>""",
+    "text_above_note":  """<text x="{x}" y="{y}" fill="{text_color}" font-family="{family}" font-size="{size}" style="pointer-events: none;">{text}</text>""",
     "text_with_note":   """<text x="{x}" y="{y}" fill="{text_color}" font-family="{family}" font-size="{size}" onmouseover="show_{mcd_uid}(evt,'{note}')" onmouseout="hide_{mcd_uid}(evt)" style="cursor: pointer;">{text}</text>""",
     "line":             """<line x1="{x0}" y1="{y0}" x2="{x1}" y2="{y1}" stroke="{stroke_color}" stroke-width="{stroke_depth}"/>""",
     "dash_line":        """<line x1="{x0}" y1="{y0}" x2="{x1}" y2="{y1}" stroke="{stroke_color}" stroke-width="{stroke_depth}" stroke-dasharray="{dash_width}"/>""",
+    "dot_line":         """<line x1="{x0}" y1="{y0}" x2="{x1}" y2="{y1}" stroke="{stroke_color}" stroke-width="{stroke_depth}"  stroke-dasharray="0,{dash_gap}" stroke-linecap="round"/>""",
     "rect":             """<rect x="{x}" y="{y}" width="{w}" height="{h}" fill="{color}" stroke="{stroke_color}" stroke-width="{stroke_depth}" opacity="{opacity}"/>""",
     "dash_rect":        """<rect x="{x}" y="{y}" width="{w}" height="{h}" fill="{color}" stroke="{stroke_color}" stroke-width="{stroke_depth}" stroke-dasharray="{dash_width}"/>""",
     "polygon":          """<polygon points="{points}" fill="{color}" stroke="{stroke_color}" stroke-width="{stroke_depth}" opacity="{opacity}"/>""",
     "dot_polygon":      """<polygon points="{points}" fill="{color}" stroke="{stroke_color}" stroke-width="{stroke_depth}" stroke-dasharray="0,{dash_gap}" stroke-linecap="round"/>""",
     "circle":           """<circle cx="{cx}" cy="{cy}" r="{r}" stroke="{stroke_color}" stroke-width="{stroke_depth}" fill="{color}"/>""",
+    "circle_with_note": """<circle cx="{cx}" cy="{cy}" r="{r}" stroke="{stroke_color}" stroke-width="{stroke_depth}" fill="{color}" onmouseover="show_{mcd_uid}(evt,'{note}')" onmouseout="hide_{mcd_uid}(evt)" style="cursor: pointer;"/>""",
     "pager_dot":        """<circle cx="{cx}" cy="{cy}" r="{r}" fill="{color}" id="pager_dot_{page}_{mcd_uid}" class="pager_dot" stroke-width="0" onclick="switch_page_visibility_{mcd_uid}(evt,{page})" style="cursor: pointer;"/>""",
     "triangle":         """<polygon points="{x1} {y1} {x2} {y2} {x3} {y3}" stroke="{stroke_color}" stroke-width="{stroke_depth}" fill="{color}"/>""",
     "arrow":            """<polygon points="{x0} {y0} {x1} {y1} {x2} {y2} {x3} {y3}" fill="{stroke_color}" stroke-width="0"/>""",
     "curve":            """<path d="M{x0} {y0} C{x1} {y1} {x2} {y2} {x3} {y3}" fill="none" stroke="{stroke_color}" stroke-width="{stroke_depth}"/>""",
     "round_rect":       """<rect x="{x}" y="{y}" width="{w}" height="{h}" fill="{color}" rx="{radius}" stroke="{stroke_color}" stroke-width="{stroke_depth}"/>""",
     "upper_round_rect": """<path d="M{x0} {y0} a{r} {r} 90 0 1 {r} {r} V{y1} h-{w} V{y2} a{r} {r} 90 0 1 {r} -{r}" fill="{color}" stroke="{stroke_color}" stroke-width="{stroke_depth}"/>""",
     "lower_round_rect": """<path d="M{x0} {y0} v{y1} a{r} {r} 90 0 1 -{r} {r} H{x1} a{r} {r} 90 0 1 -{r} -{r} V{y0} H{w}" fill="{color}" stroke="{stroke_color}" stroke-width="{stroke_depth}"/>""",
```

### Comparing `mocodo-3.1.2/mocodo/mocodo_error.py` & `mocodo-3.2.0/mocodo/mocodo_error.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/obfuscate.py` & `mocodo-3.2.0/mocodo/obfuscate.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,23 +23,26 @@
             previous_words.add(word)
 
 def obfuscate(clauses, params):
     
     cache = {"": ""}
     def obfuscate_label(label):
         if label not in cache:
-            try:
-                new_label = next(random_word)
-            except StopIteration:
-                raise MocodoError(12, _('Obfuscation failed. Not enough substitution words in "{filename}". You may decrease the `obfuscation_min_distance` option values.').format(filename=lorem_filename)) # fmt: skip
-            if label.isupper():
-                new_label = new_label.upper()
-            elif label == label.capitalize():
-                new_label = new_label.capitalize()
-            cache[label] = new_label
+            if label.isdigit():
+                cache[label] = label
+            else:
+                try:
+                    new_label = next(random_word)
+                except StopIteration:
+                    raise MocodoError(12, _('Obfuscation failed. Not enough substitution words in "{filename}". You may decrease the `obfuscation_min_distance` option values.').format(filename=lorem_filename)) # fmt: skip
+                if label.isupper():
+                    new_label = new_label.upper()
+                elif label == label.capitalize():
+                    new_label = new_label.capitalize()
+                cache[label] = new_label
         return cache[label]
 
     random.seed(params["seed"])
     lorem_filename = params["obfuscate"] or ""
     try:
         lorem_text = read_contents(lorem_filename)
     except IOError:
@@ -53,48 +56,64 @@
     header = [comment + "\n" for comment in itertools.takewhile(lambda line: line.startswith("%"), clauses)]
     clauses = "\n".join(clauses[len(header):])
     clauses = re.sub(r"(?m)^([ \t]*)\[(.+?)\]", r"\1<<<safe-left-bracket>>>\2<<<safe-right-bracket>>>", clauses)
     clauses = re.sub(r"\[.+?\]", "", clauses)
     clauses = clauses.replace("<<<safe-left-bracket>>>", "[")
     clauses = clauses.replace("<<<safe-right-bracket>>>", "]")
     clauses = re.sub(r"(?m)^%.*\n?", "", clauses)
-    elements = re.split(r"([ \t\]]*(?:[:,\n]+|/[XT]*\\|=>|<=|->|<-)[ \t_\[]*)", clauses) + ['']
+    elements = re.split(r"([ \t\]]*(?:[:,\n]+|/[XT]*\\|\(.*?\)|=>|<=|->|<-|(?<= )<?[-.]+>?)[ \t_\[]*)", clauses) + ['']
     after_first_comma = False
     before_colon = True
+    constraint = False
     for (i, element) in enumerate(elements):
         if i % 2:
             if "\n" in element:
                 after_first_comma = False
                 before_colon = True
                 inheritance = False
+                constraint = False
             elif element.startswith("/"):
                 inheritance = True
+            elif element.startswith("("):
+                constraint = True
             elif "," in element:
                 after_first_comma = True
             elif ":" in element:
                 before_colon = False
         else:
-            if after_first_comma and before_colon and not inheritance:
+            if element and after_first_comma and before_colon and not inheritance and not constraint:
                 (card, entity_name) = element.split(" ", 1)
                 entity_name = entity_name.strip()
                 elements[i-1] += card + " "
                 elements[i] = entity_name
             elements[i] = obfuscate_label(elements[i])
     return "".join(header + elements).strip()
 
 
 if __name__=="__main__":
     # launch with:
     # python -m mocodo.obfuscate
     from .argument_parser import parsed_arguments
     clauses = """
-        CLIENT: Réf. client, Nom, Prénom, Adresse
-        PASSER, 0N CLIENT, /11 COMMANDE
-        COMMANDE: Num commande, Date, Montant
-        INCLURE, 1N [foobar] COMMANDE, 0N PRODUIT: Quantité
-        PRODUIT: Réf. produit, Libellé, Prix unitaire
-        [AVOIR COLORIS], 01 PRODUIT, 0N COLORIS
-        COLORIS: coloris
+        Projet: num. projet, nom projet
+        :
+        Fournir, 1N Projet, 1N Pièce, 1N Fournisseur
+        Fournisseur: num. fournisseur, raison sociale
+            
+        Requérir, 1N Projet, 0N Pièce: quantité
+        :
+        Pièce: réf. pièce, libellé pièce
+
+        Date: Date
+        Réserver, /1N Client, 1N Chambre, 0N Date: Durée
+        Chambre: Numéro, Prix
+
+        :
+            
+        Client: Id. client
+
+        (CIF) [Même date, même chambre => un seul client] --Chambre, --Date, ->Client, ..Réserver: 20, 80
+        (X) [Toute pièce fournie doit avoir été requise.] ..Pièce, ->Requérir, --Fournir, Projet
     """.replace("  ", "").split("\n")
     params = parsed_arguments()
     params["obfuscate"] = "four_letter_words.txt"
     print(obfuscate(clauses, params))
```

### Comparing `mocodo-3.1.2/mocodo/phantom.py` & `mocodo-3.2.0/mocodo/phantom.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/pluralize_fr.py` & `mocodo-3.2.0/mocodo/pluralize_fr.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/read_template.py` & `mocodo-3.2.0/mocodo/read_template.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/relations.py` & `mocodo-3.2.0/mocodo/relations.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/colors/blank.json` & `mocodo-3.2.0/mocodo/resources/colors/wb.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4473684210526316%*

 * *Differences: {"'association_attribute_text_color'": "'#FFF'",*

 * * "'association_cartouche_color'": "'#000'",*

 * * "'association_cartouche_text_color'": "'#FFF'",*

 * * "'association_color'": "'#000'",*

 * * "'association_stroke_color'": "'#FFF'",*

 * * "'background_color'": "'#FFF'",*

 * * "'card_text_color'": "'#000'",*

 * * "'constraint_background_color'": "'#FFF'",*

 * * "'constraint_stroke_color'": "'#FFF'",*

 * * "'constraint_text_color'": "'#FFF'",*

 * * "'entity_attribute_text_color'": "'#FFF'",*

 * * "'entity_cartouche_color'": "'#000'",*

 * * "'entity_cartouche_text_ […]*

```diff
@@ -1,18 +1,21 @@
 {
-    "association_attribute_text_color": null,
-    "association_cartouche_color": "#FFF",
-    "association_cartouche_text_color": "#000",
-    "association_color": "#FFF",
-    "association_stroke_color": "#000",
-    "background_color": null,
-    "card_text_color": null,
-    "entity_attribute_text_color": null,
-    "entity_cartouche_color": "#FFF",
-    "entity_cartouche_text_color": "#000",
-    "entity_color": "#FFF",
-    "entity_stroke_color": "#000",
+    "association_attribute_text_color": "#FFF",
+    "association_cartouche_color": "#000",
+    "association_cartouche_text_color": "#FFF",
+    "association_color": "#000",
+    "association_stroke_color": "#FFF",
+    "background_color": "#FFF",
+    "card_text_color": "#000",
+    "constraint_background_color": "#FFF",
+    "constraint_stroke_color": "#FFF",
+    "constraint_text_color": "#FFF",
+    "entity_attribute_text_color": "#FFF",
+    "entity_cartouche_color": "#000",
+    "entity_cartouche_text_color": "#FFF",
+    "entity_color": "#000",
+    "entity_stroke_color": "#FFF",
     "leg_stroke_color": "#000",
-    "note_color": "#000",
-    "note_opacity": 0,
-    "note_text_color": "#FFF"
+    "note_color": "#FFFF00",
+    "note_opacity": 0.9,
+    "note_text_color": "#000"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer+1.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer-6.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5526315789473685%*

 * *Differences: {"'association_cartouche_color'": "'#bababa'",*

 * * "'association_color'": "'#e0e0e0'",*

 * * "'association_stroke_color'": "'#878787'",*

 * * "'background_color'": "'#fff'",*

 * * "'card_text_color'": "'#b2182b'",*

 * * "'constraint_background_color'": "'#fff'",*

 * * "'constraint_stroke_color'": "'#878787'",*

 * * "'constraint_text_color'": "'#878787'",*

 * * "'entity_cartouche_color'": "'#f4a582'",*

 * * "'entity_color'": "'#fddbc7'",*

 * * "'entity_stroke_color'": "'#d6604d'",*

 * * "'leg_stroke_color'": "'#878787'",*

 * * "'note_color'": "'#4d4d4d'",*

 * * "'note_t […]*

```diff
@@ -1,18 +1,21 @@
 {
     "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#dfc27d",
+    "association_cartouche_color": "#bababa",
     "association_cartouche_text_color": "#000",
-    "association_color": "#f6e8c3",
-    "association_stroke_color": "#bf812d",
-    "background_color": "#f5f5f5",
-    "card_text_color": "#01665e",
+    "association_color": "#e0e0e0",
+    "association_stroke_color": "#878787",
+    "background_color": "#fff",
+    "card_text_color": "#b2182b",
+    "constraint_background_color": "#fff",
+    "constraint_stroke_color": "#878787",
+    "constraint_text_color": "#878787",
     "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#80cdc1",
+    "entity_cartouche_color": "#f4a582",
     "entity_cartouche_text_color": "#000",
-    "entity_color": "#c7eae5",
-    "entity_stroke_color": "#35978f",
-    "leg_stroke_color": "#bf812d",
-    "note_color": "#8c510a",
+    "entity_color": "#fddbc7",
+    "entity_stroke_color": "#d6604d",
+    "leg_stroke_color": "#878787",
+    "note_color": "#4d4d4d",
     "note_opacity": 0.9,
-    "note_text_color": "#f5f5f5"
+    "note_text_color": "#fff"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer+2.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer+2.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8421052631578947%*

 * *Differences: {"'constraint_background_color'": "'#f7f7f7'",*

 * * "'constraint_stroke_color'": "'#de77ae'",*

 * * "'constraint_text_color'": "'#de77ae'"}*

```diff
@@ -2,14 +2,17 @@
     "association_attribute_text_color": "#000",
     "association_cartouche_color": "#f1b6da",
     "association_cartouche_text_color": "#000",
     "association_color": "#fde0ef",
     "association_stroke_color": "#de77ae",
     "background_color": "#f7f7f7",
     "card_text_color": "#4d9221",
+    "constraint_background_color": "#f7f7f7",
+    "constraint_stroke_color": "#de77ae",
+    "constraint_text_color": "#de77ae",
     "entity_attribute_text_color": "#000",
     "entity_cartouche_color": "#b8e186",
     "entity_cartouche_text_color": "#000",
     "entity_color": "#e6f5d0",
     "entity_stroke_color": "#7fbc41",
     "leg_stroke_color": "#de77ae",
     "note_color": "#c51b7d",
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer+3.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer-3.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6052631578947368%*

 * *Differences: {"'association_cartouche_color'": "'#a6dba0'",*

 * * "'association_color'": "'#d9f0d3'",*

 * * "'association_stroke_color'": "'#5aae61'",*

 * * "'card_text_color'": "'#762a83'",*

 * * "'constraint_background_color'": "'#f7f7f7'",*

 * * "'constraint_stroke_color'": "'#5aae61'",*

 * * "'constraint_text_color'": "'#5aae61'",*

 * * "'entity_cartouche_color'": "'#c2a5cf'",*

 * * "'entity_color'": "'#e7d4e8'",*

 * * "'entity_stroke_color'": "'#9970ab'",*

 * * "'leg_stroke_color'": "'#5aae61'",*

 * * "'note_color'": "'#1b7837'"}*

```diff
@@ -1,18 +1,21 @@
 {
     "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#c2a5cf",
+    "association_cartouche_color": "#a6dba0",
     "association_cartouche_text_color": "#000",
-    "association_color": "#e7d4e8",
-    "association_stroke_color": "#9970ab",
+    "association_color": "#d9f0d3",
+    "association_stroke_color": "#5aae61",
     "background_color": "#f7f7f7",
-    "card_text_color": "#1b7837",
+    "card_text_color": "#762a83",
+    "constraint_background_color": "#f7f7f7",
+    "constraint_stroke_color": "#5aae61",
+    "constraint_text_color": "#5aae61",
     "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#a6dba0",
+    "entity_cartouche_color": "#c2a5cf",
     "entity_cartouche_text_color": "#000",
-    "entity_color": "#d9f0d3",
-    "entity_stroke_color": "#5aae61",
-    "leg_stroke_color": "#9970ab",
-    "note_color": "#762a83",
+    "entity_color": "#e7d4e8",
+    "entity_stroke_color": "#9970ab",
+    "leg_stroke_color": "#5aae61",
+    "note_color": "#1b7837",
     "note_opacity": 0.9,
     "note_text_color": "#f7f7f7"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer+4.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer+4.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8421052631578947%*

 * *Differences: {"'constraint_background_color'": "'#f7f7f7'",*

 * * "'constraint_stroke_color'": "'#e08214'",*

 * * "'constraint_text_color'": "'#e08214'"}*

```diff
@@ -2,14 +2,17 @@
     "association_attribute_text_color": "#000",
     "association_cartouche_color": "#fdb863",
     "association_cartouche_text_color": "#000",
     "association_color": "#fee0b6",
     "association_stroke_color": "#e08214",
     "background_color": "#f7f7f7",
     "card_text_color": "#542788",
+    "constraint_background_color": "#f7f7f7",
+    "constraint_stroke_color": "#e08214",
+    "constraint_text_color": "#e08214",
     "entity_attribute_text_color": "#000",
     "entity_cartouche_color": "#b2abd2",
     "entity_cartouche_text_color": "#000",
     "entity_color": "#d8daeb",
     "entity_stroke_color": "#8073ac",
     "leg_stroke_color": "#e08214",
     "note_color": "#b35806",
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer+5.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer-2.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6052631578947368%*

 * *Differences: {"'association_cartouche_color'": "'#b8e186'",*

 * * "'association_color'": "'#e6f5d0'",*

 * * "'association_stroke_color'": "'#7fbc41'",*

 * * "'card_text_color'": "'#c51b7d'",*

 * * "'constraint_background_color'": "'#f7f7f7'",*

 * * "'constraint_stroke_color'": "'#7fbc41'",*

 * * "'constraint_text_color'": "'#7fbc41'",*

 * * "'entity_cartouche_color'": "'#f1b6da'",*

 * * "'entity_color'": "'#fde0ef'",*

 * * "'entity_stroke_color'": "'#de77ae'",*

 * * "'leg_stroke_color'": "'#7fbc41'",*

 * * "'note_color'": "'#4d9221'"}*

```diff
@@ -1,18 +1,21 @@
 {
     "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#f4a582",
+    "association_cartouche_color": "#b8e186",
     "association_cartouche_text_color": "#000",
-    "association_color": "#fddbc7",
-    "association_stroke_color": "#d6604d",
+    "association_color": "#e6f5d0",
+    "association_stroke_color": "#7fbc41",
     "background_color": "#f7f7f7",
-    "card_text_color": "#2166ac",
+    "card_text_color": "#c51b7d",
+    "constraint_background_color": "#f7f7f7",
+    "constraint_stroke_color": "#7fbc41",
+    "constraint_text_color": "#7fbc41",
     "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#92c5de",
+    "entity_cartouche_color": "#f1b6da",
     "entity_cartouche_text_color": "#000",
-    "entity_color": "#d1e5f0",
-    "entity_stroke_color": "#4393c3",
-    "leg_stroke_color": "#d6604d",
-    "note_color": "#b2182b",
+    "entity_color": "#fde0ef",
+    "entity_stroke_color": "#de77ae",
+    "leg_stroke_color": "#7fbc41",
+    "note_color": "#4d9221",
     "note_opacity": 0.9,
     "note_text_color": "#f7f7f7"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer+6.json` & `mocodo-3.2.0/mocodo/resources/colors/pond.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.42105263157894735%*

 * *Differences: {"'association_attribute_text_color'": "'#3d484a'",*

 * * "'association_cartouche_color'": "'#9ebd6d'",*

 * * "'association_cartouche_text_color'": "'#3d484a'",*

 * * "'association_color'": "'#c3dbbb'",*

 * * "'association_stroke_color'": "'#8ea243'",*

 * * "'background_color'": 'None',*

 * * "'card_text_color'": "'#2f494e'",*

 * * "'constraint_background_color'": "'#FFF'",*

 * * "'constraint_stroke_color'": "'#8ea243'",*

 * * "'constraint_text_color'": "'#8ea243'",*

 * * "'entity_attribute_text_color'": "'#1b5343'",*

 * * "'entity_cartouche_color'": "'#7ecb9a' […]*

```diff
@@ -1,18 +1,21 @@
 {
-    "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#f4a582",
-    "association_cartouche_text_color": "#000",
-    "association_color": "#fddbc7",
-    "association_stroke_color": "#d6604d",
-    "background_color": "#fff",
-    "card_text_color": "#4d4d4d",
-    "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#bababa",
-    "entity_cartouche_text_color": "#000",
-    "entity_color": "#e0e0e0",
-    "entity_stroke_color": "#878787",
-    "leg_stroke_color": "#d6604d",
-    "note_color": "#b2182b",
-    "note_opacity": 0.9,
-    "note_text_color": "#fff"
+    "association_attribute_text_color": "#3d484a",
+    "association_cartouche_color": "#9ebd6d",
+    "association_cartouche_text_color": "#3d484a",
+    "association_color": "#c3dbbb",
+    "association_stroke_color": "#8ea243",
+    "background_color": null,
+    "card_text_color": "#2f494e",
+    "constraint_background_color": "#FFF",
+    "constraint_stroke_color": "#8ea243",
+    "constraint_text_color": "#8ea243",
+    "entity_attribute_text_color": "#1b5343",
+    "entity_cartouche_color": "#7ecb9a",
+    "entity_cartouche_text_color": "#1b5343",
+    "entity_color": "#a6efb3",
+    "entity_stroke_color": "#387252",
+    "leg_stroke_color": "#476062",
+    "note_color": "#0A2019",
+    "note_opacity": 0.7,
+    "note_text_color": "#E3FFD9"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer+7.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer-8.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6052631578947368%*

 * *Differences: {"'association_cartouche_color'": "'#a6d96a'",*

 * * "'association_color'": "'#d9ef8b'",*

 * * "'association_stroke_color'": "'#66bd63'",*

 * * "'card_text_color'": "'#d73027'",*

 * * "'constraint_background_color'": "'#ffffbf'",*

 * * "'constraint_stroke_color'": "'#66bd63'",*

 * * "'constraint_text_color'": "'#66bd63'",*

 * * "'entity_cartouche_color'": "'#fdae61'",*

 * * "'entity_color'": "'#fee08b'",*

 * * "'entity_stroke_color'": "'#f46d43'",*

 * * "'leg_stroke_color'": "'#66bd63'",*

 * * "'note_color'": "'#1a9850'"}*

```diff
@@ -1,18 +1,21 @@
 {
     "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#fdae61",
+    "association_cartouche_color": "#a6d96a",
     "association_cartouche_text_color": "#000",
-    "association_color": "#fee090",
-    "association_stroke_color": "#f46d43",
+    "association_color": "#d9ef8b",
+    "association_stroke_color": "#66bd63",
     "background_color": "#ffffbf",
-    "card_text_color": "#4575b4",
+    "card_text_color": "#d73027",
+    "constraint_background_color": "#ffffbf",
+    "constraint_stroke_color": "#66bd63",
+    "constraint_text_color": "#66bd63",
     "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#abd9e9",
+    "entity_cartouche_color": "#fdae61",
     "entity_cartouche_text_color": "#000",
-    "entity_color": "#e0f3f8",
-    "entity_stroke_color": "#74add1",
-    "leg_stroke_color": "#f46d43",
-    "note_color": "#d73027",
+    "entity_color": "#fee08b",
+    "entity_stroke_color": "#f46d43",
+    "leg_stroke_color": "#66bd63",
+    "note_color": "#1a9850",
     "note_opacity": 0.9,
     "note_text_color": "#ffffbf"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer+8.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer+8.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8421052631578947%*

 * *Differences: {"'constraint_background_color'": "'#ffffbf'",*

 * * "'constraint_stroke_color'": "'#f46d43'",*

 * * "'constraint_text_color'": "'#f46d43'"}*

```diff
@@ -2,14 +2,17 @@
     "association_attribute_text_color": "#000",
     "association_cartouche_color": "#fdae61",
     "association_cartouche_text_color": "#000",
     "association_color": "#fee08b",
     "association_stroke_color": "#f46d43",
     "background_color": "#ffffbf",
     "card_text_color": "#1a9850",
+    "constraint_background_color": "#ffffbf",
+    "constraint_stroke_color": "#f46d43",
+    "constraint_text_color": "#f46d43",
     "entity_attribute_text_color": "#000",
     "entity_cartouche_color": "#a6d96a",
     "entity_cartouche_text_color": "#000",
     "entity_color": "#d9ef8b",
     "entity_stroke_color": "#66bd63",
     "leg_stroke_color": "#f46d43",
     "note_color": "#d73027",
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer+9.json` & `mocodo-3.2.0/mocodo/resources/colors/desert.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.42105263157894735%*

 * *Differences: {"'association_attribute_text_color'": "'#7F5D3B'",*

 * * "'association_cartouche_color'": "'#CE9F6F'",*

 * * "'association_cartouche_text_color'": "'#7F5D3B'",*

 * * "'association_color'": "'#E2BE9F'",*

 * * "'association_stroke_color'": "'#896C39'",*

 * * "'background_color'": 'None',*

 * * "'card_text_color'": "'#5C4827'",*

 * * "'constraint_background_color'": "'#FFF'",*

 * * "'constraint_stroke_color'": "'#896C39'",*

 * * "'constraint_text_color'": "'#896C39'",*

 * * "'entity_attribute_text_color'": "'#645530'",*

 * * "'entity_cartouche_color'": "'#FAA945' […]*

```diff
@@ -1,18 +1,21 @@
 {
-    "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#fdae61",
-    "association_cartouche_text_color": "#000",
-    "association_color": "#fee08b",
-    "association_stroke_color": "#f46d43",
-    "background_color": "#ffffbf",
-    "card_text_color": "#3288bd",
-    "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#abdda4",
-    "entity_cartouche_text_color": "#000",
-    "entity_color": "#e6f598",
-    "entity_stroke_color": "#66c2a5",
-    "leg_stroke_color": "#f46d43",
-    "note_color": "#d53e4f",
-    "note_opacity": 0.9,
-    "note_text_color": "#ffffbf"
+    "association_attribute_text_color": "#7F5D3B",
+    "association_cartouche_color": "#CE9F6F",
+    "association_cartouche_text_color": "#7F5D3B",
+    "association_color": "#E2BE9F",
+    "association_stroke_color": "#896C39",
+    "background_color": null,
+    "card_text_color": "#5C4827",
+    "constraint_background_color": "#FFF",
+    "constraint_stroke_color": "#896C39",
+    "constraint_text_color": "#896C39",
+    "entity_attribute_text_color": "#645530",
+    "entity_cartouche_color": "#FAA945",
+    "entity_cartouche_text_color": "#645530",
+    "entity_color": "#FFB94E",
+    "entity_stroke_color": "#CB7E1F",
+    "leg_stroke_color": "#4C3D30",
+    "note_color": "#18180B",
+    "note_opacity": 0.7,
+    "note_text_color": "#FFFFD0"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer-1.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer-1.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8421052631578947%*

 * *Differences: {"'constraint_background_color'": "'#f5f5f5'",*

 * * "'constraint_stroke_color'": "'#35978f'",*

 * * "'constraint_text_color'": "'#35978f'"}*

```diff
@@ -2,14 +2,17 @@
     "association_attribute_text_color": "#000",
     "association_cartouche_color": "#80cdc1",
     "association_cartouche_text_color": "#000",
     "association_color": "#c7eae5",
     "association_stroke_color": "#35978f",
     "background_color": "#f5f5f5",
     "card_text_color": "#8c510a",
+    "constraint_background_color": "#f5f5f5",
+    "constraint_stroke_color": "#35978f",
+    "constraint_text_color": "#35978f",
     "entity_attribute_text_color": "#000",
     "entity_cartouche_color": "#dfc27d",
     "entity_cartouche_text_color": "#000",
     "entity_color": "#f6e8c3",
     "entity_stroke_color": "#bf812d",
     "leg_stroke_color": "#35978f",
     "note_color": "#01665e",
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer-2.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer+6.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5526315789473685%*

 * *Differences: {"'association_cartouche_color'": "'#f4a582'",*

 * * "'association_color'": "'#fddbc7'",*

 * * "'association_stroke_color'": "'#d6604d'",*

 * * "'background_color'": "'#fff'",*

 * * "'card_text_color'": "'#4d4d4d'",*

 * * "'constraint_background_color'": "'#fff'",*

 * * "'constraint_stroke_color'": "'#d6604d'",*

 * * "'constraint_text_color'": "'#d6604d'",*

 * * "'entity_cartouche_color'": "'#bababa'",*

 * * "'entity_color'": "'#e0e0e0'",*

 * * "'entity_stroke_color'": "'#878787'",*

 * * "'leg_stroke_color'": "'#d6604d'",*

 * * "'note_color'": "'#b2182b'",*

 * * "'note_t […]*

```diff
@@ -1,18 +1,21 @@
 {
     "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#b8e186",
+    "association_cartouche_color": "#f4a582",
     "association_cartouche_text_color": "#000",
-    "association_color": "#e6f5d0",
-    "association_stroke_color": "#7fbc41",
-    "background_color": "#f7f7f7",
-    "card_text_color": "#c51b7d",
+    "association_color": "#fddbc7",
+    "association_stroke_color": "#d6604d",
+    "background_color": "#fff",
+    "card_text_color": "#4d4d4d",
+    "constraint_background_color": "#fff",
+    "constraint_stroke_color": "#d6604d",
+    "constraint_text_color": "#d6604d",
     "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#f1b6da",
+    "entity_cartouche_color": "#bababa",
     "entity_cartouche_text_color": "#000",
-    "entity_color": "#fde0ef",
-    "entity_stroke_color": "#de77ae",
-    "leg_stroke_color": "#7fbc41",
-    "note_color": "#4d9221",
+    "entity_color": "#e0e0e0",
+    "entity_stroke_color": "#878787",
+    "leg_stroke_color": "#d6604d",
+    "note_color": "#b2182b",
     "note_opacity": 0.9,
-    "note_text_color": "#f7f7f7"
+    "note_text_color": "#fff"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer-3.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer-4.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6052631578947368%*

 * *Differences: {"'association_cartouche_color'": "'#b2abd2'",*

 * * "'association_color'": "'#d8daeb'",*

 * * "'association_stroke_color'": "'#8073ac'",*

 * * "'card_text_color'": "'#b35806'",*

 * * "'constraint_background_color'": "'#f7f7f7'",*

 * * "'constraint_stroke_color'": "'#8073ac'",*

 * * "'constraint_text_color'": "'#8073ac'",*

 * * "'entity_cartouche_color'": "'#fdb863'",*

 * * "'entity_color'": "'#fee0b6'",*

 * * "'entity_stroke_color'": "'#e08214'",*

 * * "'leg_stroke_color'": "'#8073ac'",*

 * * "'note_color'": "'#542788'"}*

```diff
@@ -1,18 +1,21 @@
 {
     "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#a6dba0",
+    "association_cartouche_color": "#b2abd2",
     "association_cartouche_text_color": "#000",
-    "association_color": "#d9f0d3",
-    "association_stroke_color": "#5aae61",
+    "association_color": "#d8daeb",
+    "association_stroke_color": "#8073ac",
     "background_color": "#f7f7f7",
-    "card_text_color": "#762a83",
+    "card_text_color": "#b35806",
+    "constraint_background_color": "#f7f7f7",
+    "constraint_stroke_color": "#8073ac",
+    "constraint_text_color": "#8073ac",
     "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#c2a5cf",
+    "entity_cartouche_color": "#fdb863",
     "entity_cartouche_text_color": "#000",
-    "entity_color": "#e7d4e8",
-    "entity_stroke_color": "#9970ab",
-    "leg_stroke_color": "#5aae61",
-    "note_color": "#1b7837",
+    "entity_color": "#fee0b6",
+    "entity_stroke_color": "#e08214",
+    "leg_stroke_color": "#8073ac",
+    "note_color": "#542788",
     "note_opacity": 0.9,
     "note_text_color": "#f7f7f7"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer-4.json` & `mocodo-3.2.0/mocodo/resources/colors/ocean.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.42105263157894735%*

 * *Differences: {"'association_attribute_text_color'": "'#607734'",*

 * * "'association_cartouche_color'": "'#b2bba4'",*

 * * "'association_cartouche_text_color'": "'#27360c'",*

 * * "'association_color'": "'#ccd6ba'",*

 * * "'association_stroke_color'": "'#85956b'",*

 * * "'background_color'": 'None',*

 * * "'card_text_color'": "'#726f83'",*

 * * "'constraint_background_color'": "'#FFF'",*

 * * "'constraint_stroke_color'": "'#85956b'",*

 * * "'constraint_text_color'": "'#85956b'",*

 * * "'entity_attribute_text_color'": "'#3e3c42'",*

 * * "'entity_cartouche_color'": "'#97b8ff' […]*

```diff
@@ -1,18 +1,21 @@
 {
-    "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#b2abd2",
-    "association_cartouche_text_color": "#000",
-    "association_color": "#d8daeb",
-    "association_stroke_color": "#8073ac",
-    "background_color": "#f7f7f7",
-    "card_text_color": "#b35806",
-    "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#fdb863",
-    "entity_cartouche_text_color": "#000",
-    "entity_color": "#fee0b6",
-    "entity_stroke_color": "#e08214",
-    "leg_stroke_color": "#8073ac",
-    "note_color": "#542788",
-    "note_opacity": 0.9,
-    "note_text_color": "#f7f7f7"
+    "association_attribute_text_color": "#607734",
+    "association_cartouche_color": "#b2bba4",
+    "association_cartouche_text_color": "#27360c",
+    "association_color": "#ccd6ba",
+    "association_stroke_color": "#85956b",
+    "background_color": null,
+    "card_text_color": "#726f83",
+    "constraint_background_color": "#FFF",
+    "constraint_stroke_color": "#85956b",
+    "constraint_text_color": "#85956b",
+    "entity_attribute_text_color": "#3e3c42",
+    "entity_cartouche_color": "#97b8ff",
+    "entity_cartouche_text_color": "#131114",
+    "entity_color": "#c0d4ff",
+    "entity_stroke_color": "#578dff",
+    "leg_stroke_color": "#726f83",
+    "note_color": "#060707",
+    "note_opacity": 0.7,
+    "note_text_color": "#E2EED0"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer-5.json` & `mocodo-3.2.0/mocodo/resources/colors/keepsake.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.42105263157894735%*

 * *Differences: {"'association_attribute_text_color'": "'#57483d'",*

 * * "'association_cartouche_color'": "'#c6aea5'",*

 * * "'association_cartouche_text_color'": "'#422f2c'",*

 * * "'association_color'": "'#d3b5b2'",*

 * * "'association_stroke_color'": 'None',*

 * * "'background_color'": 'None',*

 * * "'card_text_color'": "'#57483d'",*

 * * "'constraint_background_color'": "'#FFF'",*

 * * "'constraint_stroke_color'": 'None',*

 * * "'constraint_text_color'": 'None',*

 * * "'entity_attribute_text_color'": "'#57483d'",*

 * * "'entity_cartouche_color'": "'#cbcbb5'",*

 * * "'entity_ca […]*

```diff
@@ -1,18 +1,21 @@
 {
-    "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#92c5de",
-    "association_cartouche_text_color": "#000",
-    "association_color": "#d1e5f0",
-    "association_stroke_color": "#4393c3",
-    "background_color": "#f7f7f7",
-    "card_text_color": "#b2182b",
-    "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#f4a582",
-    "entity_cartouche_text_color": "#000",
-    "entity_color": "#fddbc7",
-    "entity_stroke_color": "#d6604d",
-    "leg_stroke_color": "#4393c3",
-    "note_color": "#2166ac",
-    "note_opacity": 0.9,
-    "note_text_color": "#f7f7f7"
+    "association_attribute_text_color": "#57483d",
+    "association_cartouche_color": "#c6aea5",
+    "association_cartouche_text_color": "#422f2c",
+    "association_color": "#d3b5b2",
+    "association_stroke_color": null,
+    "background_color": null,
+    "card_text_color": "#57483d",
+    "constraint_background_color": "#FFF",
+    "constraint_stroke_color": null,
+    "constraint_text_color": null,
+    "entity_attribute_text_color": "#57483d",
+    "entity_cartouche_color": "#cbcbb5",
+    "entity_cartouche_text_color": "#422f2c",
+    "entity_color": "#e4e3b4",
+    "entity_stroke_color": null,
+    "leg_stroke_color": "#57483d",
+    "note_color": "#0F0F0A",
+    "note_opacity": 0.7,
+    "note_text_color": "#FFFFD7"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer-6.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer-9.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5526315789473685%*

 * *Differences: {"'association_cartouche_color'": "'#abdda4'",*

 * * "'association_color'": "'#e6f598'",*

 * * "'association_stroke_color'": "'#66c2a5'",*

 * * "'background_color'": "'#ffffbf'",*

 * * "'card_text_color'": "'#d53e4f'",*

 * * "'constraint_background_color'": "'#ffffbf'",*

 * * "'constraint_stroke_color'": "'#66c2a5'",*

 * * "'constraint_text_color'": "'#66c2a5'",*

 * * "'entity_cartouche_color'": "'#fdae61'",*

 * * "'entity_color'": "'#fee08b'",*

 * * "'entity_stroke_color'": "'#f46d43'",*

 * * "'leg_stroke_color'": "'#66c2a5'",*

 * * "'note_color'": "'#3288bd'",*

 * * "' […]*

```diff
@@ -1,18 +1,21 @@
 {
     "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#bababa",
+    "association_cartouche_color": "#abdda4",
     "association_cartouche_text_color": "#000",
-    "association_color": "#e0e0e0",
-    "association_stroke_color": "#878787",
-    "background_color": "#fff",
-    "card_text_color": "#b2182b",
+    "association_color": "#e6f598",
+    "association_stroke_color": "#66c2a5",
+    "background_color": "#ffffbf",
+    "card_text_color": "#d53e4f",
+    "constraint_background_color": "#ffffbf",
+    "constraint_stroke_color": "#66c2a5",
+    "constraint_text_color": "#66c2a5",
     "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#f4a582",
+    "entity_cartouche_color": "#fdae61",
     "entity_cartouche_text_color": "#000",
-    "entity_color": "#fddbc7",
-    "entity_stroke_color": "#d6604d",
-    "leg_stroke_color": "#878787",
-    "note_color": "#4d4d4d",
+    "entity_color": "#fee08b",
+    "entity_stroke_color": "#f46d43",
+    "leg_stroke_color": "#66c2a5",
+    "note_color": "#3288bd",
     "note_opacity": 0.9,
-    "note_text_color": "#fff"
+    "note_text_color": "#ffffbf"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer-7.json` & `mocodo-3.2.0/mocodo/resources/colors/gray.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5263157894736842%*

 * *Differences: {"'association_cartouche_color'": "'#FFF'",*

 * * "'association_color'": "'#FFF'",*

 * * "'association_stroke_color'": "'#000'",*

 * * "'background_color'": 'None',*

 * * "'card_text_color'": "'#000'",*

 * * "'constraint_background_color'": "'#FFF'",*

 * * "'constraint_stroke_color'": "'#000'",*

 * * "'constraint_text_color'": "'#000'",*

 * * "'entity_cartouche_color'": "'#DDD'",*

 * * "'entity_color'": "'#EEE'",*

 * * "'entity_stroke_color'": "'#000'",*

 * * "'leg_stroke_color'": "'#000'",*

 * * "'note_color'": "'#000'",*

 * * "'note_opacity'": '0.7',*

 * * "'note_text_color […]*

```diff
@@ -1,18 +1,21 @@
 {
     "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#abd9e9",
+    "association_cartouche_color": "#FFF",
     "association_cartouche_text_color": "#000",
-    "association_color": "#e0f3f8",
-    "association_stroke_color": "#74add1",
-    "background_color": "#ffffbf",
-    "card_text_color": "#d73027",
+    "association_color": "#FFF",
+    "association_stroke_color": "#000",
+    "background_color": null,
+    "card_text_color": "#000",
+    "constraint_background_color": "#FFF",
+    "constraint_stroke_color": "#000",
+    "constraint_text_color": "#000",
     "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#fdae61",
+    "entity_cartouche_color": "#DDD",
     "entity_cartouche_text_color": "#000",
-    "entity_color": "#fee090",
-    "entity_stroke_color": "#f46d43",
-    "leg_stroke_color": "#74add1",
-    "note_color": "#4575b4",
-    "note_opacity": 0.9,
-    "note_text_color": "#ffffbf"
+    "entity_color": "#EEE",
+    "entity_stroke_color": "#000",
+    "leg_stroke_color": "#000",
+    "note_color": "#000",
+    "note_opacity": 0.7,
+    "note_text_color": "#FFF"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer-8.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer+1.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5526315789473685%*

 * *Differences: {"'association_cartouche_color'": "'#dfc27d'",*

 * * "'association_color'": "'#f6e8c3'",*

 * * "'association_stroke_color'": "'#bf812d'",*

 * * "'background_color'": "'#f5f5f5'",*

 * * "'card_text_color'": "'#01665e'",*

 * * "'constraint_background_color'": "'#f5f5f5'",*

 * * "'constraint_stroke_color'": "'#bf812d'",*

 * * "'constraint_text_color'": "'#bf812d'",*

 * * "'entity_cartouche_color'": "'#80cdc1'",*

 * * "'entity_color'": "'#c7eae5'",*

 * * "'entity_stroke_color'": "'#35978f'",*

 * * "'leg_stroke_color'": "'#bf812d'",*

 * * "'note_color'": "'#8c510a'",*

 * * "' […]*

```diff
@@ -1,18 +1,21 @@
 {
     "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#a6d96a",
+    "association_cartouche_color": "#dfc27d",
     "association_cartouche_text_color": "#000",
-    "association_color": "#d9ef8b",
-    "association_stroke_color": "#66bd63",
-    "background_color": "#ffffbf",
-    "card_text_color": "#d73027",
+    "association_color": "#f6e8c3",
+    "association_stroke_color": "#bf812d",
+    "background_color": "#f5f5f5",
+    "card_text_color": "#01665e",
+    "constraint_background_color": "#f5f5f5",
+    "constraint_stroke_color": "#bf812d",
+    "constraint_text_color": "#bf812d",
     "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#fdae61",
+    "entity_cartouche_color": "#80cdc1",
     "entity_cartouche_text_color": "#000",
-    "entity_color": "#fee08b",
-    "entity_stroke_color": "#f46d43",
-    "leg_stroke_color": "#66bd63",
-    "note_color": "#1a9850",
+    "entity_color": "#c7eae5",
+    "entity_stroke_color": "#35978f",
+    "leg_stroke_color": "#bf812d",
+    "note_color": "#8c510a",
     "note_opacity": 0.9,
-    "note_text_color": "#ffffbf"
+    "note_text_color": "#f5f5f5"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/brewer-9.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer+3.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5526315789473685%*

 * *Differences: {"'association_cartouche_color'": "'#c2a5cf'",*

 * * "'association_color'": "'#e7d4e8'",*

 * * "'association_stroke_color'": "'#9970ab'",*

 * * "'background_color'": "'#f7f7f7'",*

 * * "'card_text_color'": "'#1b7837'",*

 * * "'constraint_background_color'": "'#f7f7f7'",*

 * * "'constraint_stroke_color'": "'#9970ab'",*

 * * "'constraint_text_color'": "'#9970ab'",*

 * * "'entity_cartouche_color'": "'#a6dba0'",*

 * * "'entity_color'": "'#d9f0d3'",*

 * * "'entity_stroke_color'": "'#5aae61'",*

 * * "'leg_stroke_color'": "'#9970ab'",*

 * * "'note_color'": "'#762a83'",*

 * * "' […]*

```diff
@@ -1,18 +1,21 @@
 {
     "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#abdda4",
+    "association_cartouche_color": "#c2a5cf",
     "association_cartouche_text_color": "#000",
-    "association_color": "#e6f598",
-    "association_stroke_color": "#66c2a5",
-    "background_color": "#ffffbf",
-    "card_text_color": "#d53e4f",
+    "association_color": "#e7d4e8",
+    "association_stroke_color": "#9970ab",
+    "background_color": "#f7f7f7",
+    "card_text_color": "#1b7837",
+    "constraint_background_color": "#f7f7f7",
+    "constraint_stroke_color": "#9970ab",
+    "constraint_text_color": "#9970ab",
     "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#fdae61",
+    "entity_cartouche_color": "#a6dba0",
     "entity_cartouche_text_color": "#000",
-    "entity_color": "#fee08b",
-    "entity_stroke_color": "#f46d43",
-    "leg_stroke_color": "#66c2a5",
-    "note_color": "#3288bd",
+    "entity_color": "#d9f0d3",
+    "entity_stroke_color": "#5aae61",
+    "leg_stroke_color": "#9970ab",
+    "note_color": "#762a83",
     "note_opacity": 0.9,
-    "note_text_color": "#ffffbf"
+    "note_text_color": "#f7f7f7"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/bw-alpha.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer-5.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5263157894736842%*

 * *Differences: {"'association_cartouche_color'": "'#92c5de'",*

 * * "'association_color'": "'#d1e5f0'",*

 * * "'association_stroke_color'": "'#4393c3'",*

 * * "'background_color'": "'#f7f7f7'",*

 * * "'card_text_color'": "'#b2182b'",*

 * * "'constraint_background_color'": "'#f7f7f7'",*

 * * "'constraint_stroke_color'": "'#4393c3'",*

 * * "'constraint_text_color'": "'#4393c3'",*

 * * "'entity_cartouche_color'": "'#f4a582'",*

 * * "'entity_color'": "'#fddbc7'",*

 * * "'entity_stroke_color'": "'#d6604d'",*

 * * "'leg_stroke_color'": "'#4393c3'",*

 * * "'note_color'": "'#2166ac'",*

 * * "' […]*

```diff
@@ -1,18 +1,21 @@
 {
     "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#FFF",
+    "association_cartouche_color": "#92c5de",
     "association_cartouche_text_color": "#000",
-    "association_color": "#FFF",
-    "association_stroke_color": "#000",
-    "background_color": null,
-    "card_text_color": "#000",
+    "association_color": "#d1e5f0",
+    "association_stroke_color": "#4393c3",
+    "background_color": "#f7f7f7",
+    "card_text_color": "#b2182b",
+    "constraint_background_color": "#f7f7f7",
+    "constraint_stroke_color": "#4393c3",
+    "constraint_text_color": "#4393c3",
     "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#FFF",
+    "entity_cartouche_color": "#f4a582",
     "entity_cartouche_text_color": "#000",
-    "entity_color": "#FFF",
-    "entity_stroke_color": "#000",
-    "leg_stroke_color": "#000",
-    "note_color": "#000",
-    "note_opacity": 0.7,
-    "note_text_color": "#FFF"
+    "entity_color": "#fddbc7",
+    "entity_stroke_color": "#d6604d",
+    "leg_stroke_color": "#4393c3",
+    "note_color": "#2166ac",
+    "note_opacity": 0.9,
+    "note_text_color": "#f7f7f7"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/bw.json` & `mocodo-3.2.0/mocodo/resources/colors/bw.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8421052631578947%*

 * *Differences: {"'constraint_background_color'": "'#FFF'",*

 * * "'constraint_stroke_color'": "'#000'",*

 * * "'constraint_text_color'": "'#000'"}*

```diff
@@ -2,14 +2,17 @@
     "association_attribute_text_color": "#000",
     "association_cartouche_color": "#FFF",
     "association_cartouche_text_color": "#000",
     "association_color": "#FFF",
     "association_stroke_color": "#000",
     "background_color": "#FFF",
     "card_text_color": "#000",
+    "constraint_background_color": "#FFF",
+    "constraint_stroke_color": "#000",
+    "constraint_text_color": "#000",
     "entity_attribute_text_color": "#000",
     "entity_cartouche_color": "#FFF",
     "entity_cartouche_text_color": "#000",
     "entity_color": "#FFF",
     "entity_stroke_color": "#000",
     "leg_stroke_color": "#000",
     "note_color": "#000",
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/desert.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer+7.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.42105263157894735%*

 * *Differences: {"'association_attribute_text_color'": "'#000'",*

 * * "'association_cartouche_color'": "'#fdae61'",*

 * * "'association_cartouche_text_color'": "'#000'",*

 * * "'association_color'": "'#fee090'",*

 * * "'association_stroke_color'": "'#f46d43'",*

 * * "'background_color'": "'#ffffbf'",*

 * * "'card_text_color'": "'#4575b4'",*

 * * "'constraint_background_color'": "'#ffffbf'",*

 * * "'constraint_stroke_color'": "'#f46d43'",*

 * * "'constraint_text_color'": "'#f46d43'",*

 * * "'entity_attribute_text_color'": "'#000'",*

 * * "'entity_cartouche_color'": "'#abd9e9'" […]*

```diff
@@ -1,18 +1,21 @@
 {
-    "association_attribute_text_color": "#7F5D3B",
-    "association_cartouche_color": "#CE9F6F",
-    "association_cartouche_text_color": "#7F5D3B",
-    "association_color": "#E2BE9F",
-    "association_stroke_color": "#896C39",
-    "background_color": null,
-    "card_text_color": "#5C4827",
-    "entity_attribute_text_color": "#645530",
-    "entity_cartouche_color": "#FAA945",
-    "entity_cartouche_text_color": "#645530",
-    "entity_color": "#FFB94E",
-    "entity_stroke_color": "#CB7E1F",
-    "leg_stroke_color": "#4C3D30",
-    "note_color": "#18180B",
-    "note_opacity": 0.7,
-    "note_text_color": "#FFFFD0"
+    "association_attribute_text_color": "#000",
+    "association_cartouche_color": "#fdae61",
+    "association_cartouche_text_color": "#000",
+    "association_color": "#fee090",
+    "association_stroke_color": "#f46d43",
+    "background_color": "#ffffbf",
+    "card_text_color": "#4575b4",
+    "constraint_background_color": "#ffffbf",
+    "constraint_stroke_color": "#f46d43",
+    "constraint_text_color": "#f46d43",
+    "entity_attribute_text_color": "#000",
+    "entity_cartouche_color": "#abd9e9",
+    "entity_cartouche_text_color": "#000",
+    "entity_color": "#e0f3f8",
+    "entity_stroke_color": "#74add1",
+    "leg_stroke_color": "#f46d43",
+    "note_color": "#d73027",
+    "note_opacity": 0.9,
+    "note_text_color": "#ffffbf"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/gray.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer-7.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5263157894736842%*

 * *Differences: {"'association_cartouche_color'": "'#abd9e9'",*

 * * "'association_color'": "'#e0f3f8'",*

 * * "'association_stroke_color'": "'#74add1'",*

 * * "'background_color'": "'#ffffbf'",*

 * * "'card_text_color'": "'#d73027'",*

 * * "'constraint_background_color'": "'#ffffbf'",*

 * * "'constraint_stroke_color'": "'#74add1'",*

 * * "'constraint_text_color'": "'#74add1'",*

 * * "'entity_cartouche_color'": "'#fdae61'",*

 * * "'entity_color'": "'#fee090'",*

 * * "'entity_stroke_color'": "'#f46d43'",*

 * * "'leg_stroke_color'": "'#74add1'",*

 * * "'note_color'": "'#4575b4'",*

 * * "' […]*

```diff
@@ -1,18 +1,21 @@
 {
     "association_attribute_text_color": "#000",
-    "association_cartouche_color": "#FFF",
+    "association_cartouche_color": "#abd9e9",
     "association_cartouche_text_color": "#000",
-    "association_color": "#FFF",
-    "association_stroke_color": "#000",
-    "background_color": null,
-    "card_text_color": "#000",
+    "association_color": "#e0f3f8",
+    "association_stroke_color": "#74add1",
+    "background_color": "#ffffbf",
+    "card_text_color": "#d73027",
+    "constraint_background_color": "#ffffbf",
+    "constraint_stroke_color": "#74add1",
+    "constraint_text_color": "#74add1",
     "entity_attribute_text_color": "#000",
-    "entity_cartouche_color": "#DDD",
+    "entity_cartouche_color": "#fdae61",
     "entity_cartouche_text_color": "#000",
-    "entity_color": "#EEE",
-    "entity_stroke_color": "#000",
-    "leg_stroke_color": "#000",
-    "note_color": "#000",
-    "note_opacity": 0.7,
-    "note_text_color": "#FFF"
+    "entity_color": "#fee090",
+    "entity_stroke_color": "#f46d43",
+    "leg_stroke_color": "#74add1",
+    "note_color": "#4575b4",
+    "note_opacity": 0.9,
+    "note_text_color": "#ffffbf"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/keepsake.json` & `mocodo-3.2.0/mocodo/resources/colors/bw-alpha.json`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 00000000: 7b0a 2020 2261 7373 6f63 6961 7469 6f6e  {.  "association
 00000010: 5f61 7474 7269 6275 7465 5f74 6578 745f  _attribute_text_
-00000020: 636f 6c6f 7222 3a20 2223 3537 3438 3364  color": "#57483d
-00000030: 222c 0a20 2022 6173 736f 6369 6174 696f  ",.  "associatio
-00000040: 6e5f 6361 7274 6f75 6368 655f 636f 6c6f  n_cartouche_colo
-00000050: 7222 3a20 2223 6336 6165 6135 222c 0a20  r": "#c6aea5",. 
-00000060: 2022 6173 736f 6369 6174 696f 6e5f 6361   "association_ca
-00000070: 7274 6f75 6368 655f 7465 7874 5f63 6f6c  rtouche_text_col
-00000080: 6f72 223a 2022 2334 3232 6632 6322 2c0a  or": "#422f2c",.
-00000090: 2020 2261 7373 6f63 6961 7469 6f6e 5f63    "association_c
-000000a0: 6f6c 6f72 223a 2022 2364 3362 3562 3222  olor": "#d3b5b2"
-000000b0: 2c0a 2020 2261 7373 6f63 6961 7469 6f6e  ,.  "association
-000000c0: 5f73 7472 6f6b 655f 636f 6c6f 7222 3a20  _stroke_color": 
-000000d0: 6e75 6c6c 2c0a 2020 2262 6163 6b67 726f  null,.  "backgro
-000000e0: 756e 645f 636f 6c6f 7222 3a20 6e75 6c6c  und_color": null
-000000f0: 2c0a 2020 2263 6172 645f 7465 7874 5f63  ,.  "card_text_c
-00000100: 6f6c 6f72 223a 2022 2335 3734 3833 6422  olor": "#57483d"
-00000110: 2c0a 2020 2265 6e74 6974 795f 6174 7472  ,.  "entity_attr
-00000120: 6962 7574 655f 7465 7874 5f63 6f6c 6f72  ibute_text_color
-00000130: 223a 2022 2335 3734 3833 6422 2c0a 2020  ": "#57483d",.  
-00000140: 2265 6e74 6974 795f 6361 7274 6f75 6368  "entity_cartouch
-00000150: 655f 636f 6c6f 7222 3a20 2223 6362 6362  e_color": "#cbcb
-00000160: 6235 222c 0a20 2022 656e 7469 7479 5f63  b5",.  "entity_c
-00000170: 6172 746f 7563 6865 5f74 6578 745f 636f  artouche_text_co
-00000180: 6c6f 7222 3a20 2223 3432 3266 3263 222c  lor": "#422f2c",
-00000190: 0a20 2022 656e 7469 7479 5f63 6f6c 6f72  .  "entity_color
-000001a0: 223a 2022 2365 3465 3362 3422 2c0a 2020  ": "#e4e3b4",.  
-000001b0: 2265 6e74 6974 795f 7374 726f 6b65 5f63  "entity_stroke_c
-000001c0: 6f6c 6f72 223a 206e 756c 6c2c 0a20 2022  olor": null,.  "
-000001d0: 6c65 675f 7374 726f 6b65 5f63 6f6c 6f72  leg_stroke_color
-000001e0: 223a 2022 2335 3734 3833 6422 2c0a 2020  ": "#57483d",.  
-000001f0: 226e 6f74 655f 636f 6c6f 7222 3a20 2223  "note_color": "#
-00000200: 3046 3046 3041 222c 0a20 2022 6e6f 7465  0F0F0A",.  "note
-00000210: 5f6f 7061 6369 7479 223a 2030 2e37 2c0a  _opacity": 0.7,.
-00000220: 2020 226e 6f74 655f 7465 7874 5f63 6f6c    "note_text_col
-00000230: 6f72 223a 2022 2346 4646 4644 3722 0a7d  or": "#FFFFD7".}
-00000240: 0a                                       .
+00000020: 636f 6c6f 7222 3a20 2223 3030 3022 2c0a  color": "#000",.
+00000030: 2020 2261 7373 6f63 6961 7469 6f6e 5f63    "association_c
+00000040: 6172 746f 7563 6865 5f63 6f6c 6f72 223a  artouche_color":
+00000050: 2022 2346 4646 222c 0a20 2022 6173 736f   "#FFF",.  "asso
+00000060: 6369 6174 696f 6e5f 6361 7274 6f75 6368  ciation_cartouch
+00000070: 655f 7465 7874 5f63 6f6c 6f72 223a 2022  e_text_color": "
+00000080: 2330 3030 222c 0a20 2022 6173 736f 6369  #000",.  "associ
+00000090: 6174 696f 6e5f 636f 6c6f 7222 3a20 2223  ation_color": "#
+000000a0: 4646 4622 2c0a 2020 2261 7373 6f63 6961  FFF",.  "associa
+000000b0: 7469 6f6e 5f73 7472 6f6b 655f 636f 6c6f  tion_stroke_colo
+000000c0: 7222 3a20 2223 3030 3022 2c0a 2020 2262  r": "#000",.  "b
+000000d0: 6163 6b67 726f 756e 645f 636f 6c6f 7222  ackground_color"
+000000e0: 3a20 6e75 6c6c 2c0a 2020 2263 6172 645f  : null,.  "card_
+000000f0: 7465 7874 5f63 6f6c 6f72 223a 2022 2330  text_color": "#0
+00000100: 3030 222c 0a20 2022 636f 6e73 7472 6169  00",.  "constrai
+00000110: 6e74 5f62 6163 6b67 726f 756e 645f 636f  nt_background_co
+00000120: 6c6f 7222 3a20 2346 4646 2c0a 2020 2263  lor": #FFF,.  "c
+00000130: 6f6e 7374 7261 696e 745f 7374 726f 6b65  onstraint_stroke
+00000140: 5f63 6f6c 6f72 223a 2022 2330 3030 222c  _color": "#000",
+00000150: 0a20 2022 636f 6e73 7472 6169 6e74 5f74  .  "constraint_t
+00000160: 6578 745f 636f 6c6f 7222 3a20 2223 3030  ext_color": "#00
+00000170: 3022 2c0a 2020 2265 6e74 6974 795f 6174  0",.  "entity_at
+00000180: 7472 6962 7574 655f 7465 7874 5f63 6f6c  tribute_text_col
+00000190: 6f72 223a 2022 2330 3030 222c 0a20 2022  or": "#000",.  "
+000001a0: 656e 7469 7479 5f63 6172 746f 7563 6865  entity_cartouche
+000001b0: 5f63 6f6c 6f72 223a 2022 2346 4646 222c  _color": "#FFF",
+000001c0: 0a20 2022 656e 7469 7479 5f63 6172 746f  .  "entity_carto
+000001d0: 7563 6865 5f74 6578 745f 636f 6c6f 7222  uche_text_color"
+000001e0: 3a20 2223 3030 3022 2c0a 2020 2265 6e74  : "#000",.  "ent
+000001f0: 6974 795f 636f 6c6f 7222 3a20 2223 4646  ity_color": "#FF
+00000200: 4622 2c0a 2020 2265 6e74 6974 795f 7374  F",.  "entity_st
+00000210: 726f 6b65 5f63 6f6c 6f72 223a 2022 2330  roke_color": "#0
+00000220: 3030 222c 0a20 2022 6c65 675f 7374 726f  00",.  "leg_stro
+00000230: 6b65 5f63 6f6c 6f72 223a 2022 2330 3030  ke_color": "#000
+00000240: 222c 0a20 2022 6e6f 7465 5f63 6f6c 6f72  ",.  "note_color
+00000250: 223a 2022 2330 3030 222c 0a20 2022 6e6f  ": "#000",.  "no
+00000260: 7465 5f6f 7061 6369 7479 223a 2030 2e37  te_opacity": 0.7
+00000270: 2c0a 2020 226e 6f74 655f 7465 7874 5f63  ,.  "note_text_c
+00000280: 6f6c 6f72 223a 2022 2346 4646 220a 7d0a  olor": "#FFF".}.
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/ocean.json` & `mocodo-3.2.0/mocodo/resources/colors/brewer+5.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.42105263157894735%*

 * *Differences: {"'association_attribute_text_color'": "'#000'",*

 * * "'association_cartouche_color'": "'#f4a582'",*

 * * "'association_cartouche_text_color'": "'#000'",*

 * * "'association_color'": "'#fddbc7'",*

 * * "'association_stroke_color'": "'#d6604d'",*

 * * "'background_color'": "'#f7f7f7'",*

 * * "'card_text_color'": "'#2166ac'",*

 * * "'constraint_background_color'": "'#f7f7f7'",*

 * * "'constraint_stroke_color'": "'#d6604d'",*

 * * "'constraint_text_color'": "'#d6604d'",*

 * * "'entity_attribute_text_color'": "'#000'",*

 * * "'entity_cartouche_color'": "'#92c5de'" […]*

```diff
@@ -1,18 +1,21 @@
 {
-    "association_attribute_text_color": "#607734",
-    "association_cartouche_color": "#b2bba4",
-    "association_cartouche_text_color": "#27360c",
-    "association_color": "#ccd6ba",
-    "association_stroke_color": "#85956b",
-    "background_color": null,
-    "card_text_color": "#726f83",
-    "entity_attribute_text_color": "#3e3c42",
-    "entity_cartouche_color": "#97b8ff",
-    "entity_cartouche_text_color": "#131114",
-    "entity_color": "#c0d4ff",
-    "entity_stroke_color": "#578dff",
-    "leg_stroke_color": "#726f83",
-    "note_color": "#060707",
-    "note_opacity": 0.7,
-    "note_text_color": "#E2EED0"
+    "association_attribute_text_color": "#000",
+    "association_cartouche_color": "#f4a582",
+    "association_cartouche_text_color": "#000",
+    "association_color": "#fddbc7",
+    "association_stroke_color": "#d6604d",
+    "background_color": "#f7f7f7",
+    "card_text_color": "#2166ac",
+    "constraint_background_color": "#f7f7f7",
+    "constraint_stroke_color": "#d6604d",
+    "constraint_text_color": "#d6604d",
+    "entity_attribute_text_color": "#000",
+    "entity_cartouche_color": "#92c5de",
+    "entity_cartouche_text_color": "#000",
+    "entity_color": "#d1e5f0",
+    "entity_stroke_color": "#4393c3",
+    "leg_stroke_color": "#d6604d",
+    "note_color": "#b2182b",
+    "note_opacity": 0.9,
+    "note_text_color": "#f7f7f7"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/pond.json` & `mocodo-3.2.0/mocodo/resources/colors/blank.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4473684210526316%*

 * *Differences: {"'association_attribute_text_color'": 'None',*

 * * "'association_cartouche_color'": "'#FFF'",*

 * * "'association_cartouche_text_color'": "'#000'",*

 * * "'association_color'": "'#FFF'",*

 * * "'association_stroke_color'": "'#000'",*

 * * "'card_text_color'": 'None',*

 * * "'constraint_background_color'": "'#FFF'",*

 * * "'constraint_stroke_color'": "'#000'",*

 * * "'constraint_text_color'": "'#000'",*

 * * "'entity_attribute_text_color'": 'None',*

 * * "'entity_cartouche_color'": "'#FFF'",*

 * * "'entity_cartouche_text_color'": "'#000'",*

 * * "'entity_color'": " […]*

```diff
@@ -1,18 +1,21 @@
 {
-    "association_attribute_text_color": "#3d484a",
-    "association_cartouche_color": "#9ebd6d",
-    "association_cartouche_text_color": "#3d484a",
-    "association_color": "#c3dbbb",
-    "association_stroke_color": "#8ea243",
+    "association_attribute_text_color": null,
+    "association_cartouche_color": "#FFF",
+    "association_cartouche_text_color": "#000",
+    "association_color": "#FFF",
+    "association_stroke_color": "#000",
     "background_color": null,
-    "card_text_color": "#2f494e",
-    "entity_attribute_text_color": "#1b5343",
-    "entity_cartouche_color": "#7ecb9a",
-    "entity_cartouche_text_color": "#1b5343",
-    "entity_color": "#a6efb3",
-    "entity_stroke_color": "#387252",
-    "leg_stroke_color": "#476062",
-    "note_color": "#0A2019",
-    "note_opacity": 0.7,
-    "note_text_color": "#E3FFD9"
+    "card_text_color": null,
+    "constraint_background_color": "#FFF",
+    "constraint_stroke_color": "#000",
+    "constraint_text_color": "#000",
+    "entity_attribute_text_color": null,
+    "entity_cartouche_color": "#FFF",
+    "entity_cartouche_text_color": "#000",
+    "entity_color": "#FFF",
+    "entity_stroke_color": "#000",
+    "leg_stroke_color": "#000",
+    "note_color": "#000",
+    "note_opacity": 0,
+    "note_text_color": "#FFF"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/wb.json` & `mocodo-3.2.0/mocodo/resources/colors/xinnian.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.42105263157894735%*

 * *Differences: {"'association_attribute_text_color'": "'#ffcf00'",*

 * * "'association_cartouche_color'": "'#fd0400'",*

 * * "'association_cartouche_text_color'": "'#ffcf00'",*

 * * "'association_color'": "'#fd0400'",*

 * * "'association_stroke_color'": "'#ffcf00'",*

 * * "'background_color'": "'#d30300'",*

 * * "'card_text_color'": "'#ffcf00'",*

 * * "'constraint_background_color'": "'#d30300'",*

 * * "'constraint_stroke_color'": "'#ffcf00'",*

 * * "'constraint_text_color'": "'#ffcf00'",*

 * * "'entity_attribute_text_color'": "'#ffcf00'",*

 * * "'entity_cartouche_color'": "' […]*

```diff
@@ -1,18 +1,21 @@
 {
-    "association_attribute_text_color": "#FFF",
-    "association_cartouche_color": "#000",
-    "association_cartouche_text_color": "#FFF",
-    "association_color": "#000",
-    "association_stroke_color": "#FFF",
-    "background_color": "#FFF",
-    "card_text_color": "#000",
-    "entity_attribute_text_color": "#FFF",
-    "entity_cartouche_color": "#000",
-    "entity_cartouche_text_color": "#FFF",
-    "entity_color": "#000",
-    "entity_stroke_color": "#FFF",
-    "leg_stroke_color": "#000",
-    "note_color": "#FFFF00",
-    "note_opacity": 0.9,
-    "note_text_color": "#000"
+    "association_attribute_text_color": "#ffcf00",
+    "association_cartouche_color": "#fd0400",
+    "association_cartouche_text_color": "#ffcf00",
+    "association_color": "#fd0400",
+    "association_stroke_color": "#ffcf00",
+    "background_color": "#d30300",
+    "card_text_color": "#ffcf00",
+    "constraint_background_color": "#d30300",
+    "constraint_stroke_color": "#ffcf00",
+    "constraint_text_color": "#ffcf00",
+    "entity_attribute_text_color": "#ffcf00",
+    "entity_cartouche_color": "#fd0400",
+    "entity_cartouche_text_color": "#ffcf00",
+    "entity_color": "#fd0400",
+    "entity_stroke_color": "#ffcf00",
+    "leg_stroke_color": "#ffcf00",
+    "note_color": "#535300",
+    "note_opacity": 0.7,
+    "note_text_color": "#FFFF00"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/colors/xinnian.json` & `mocodo-3.2.0/mocodo/resources/colors/mondrian.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.42105263157894735%*

 * *Differences: {"'association_attribute_text_color'": "'#060100'",*

 * * "'association_cartouche_color'": "'#081a84'",*

 * * "'association_cartouche_text_color'": "'#fefeec'",*

 * * "'association_color'": "'#fefeec'",*

 * * "'association_stroke_color'": "'#060100'",*

 * * "'background_color'": "'#fefeec'",*

 * * "'card_text_color'": "'#060100'",*

 * * "'constraint_background_color'": "'#fefeec'",*

 * * "'constraint_stroke_color'": "'#060100'",*

 * * "'constraint_text_color'": "'#060100'",*

 * * "'entity_attribute_text_color'": "'#060100'",*

 * * "'entity_cartouche_color'": "' […]*

```diff
@@ -1,18 +1,21 @@
 {
-    "association_attribute_text_color": "#ffcf00",
-    "association_cartouche_color": "#fd0400",
-    "association_cartouche_text_color": "#ffcf00",
-    "association_color": "#fd0400",
-    "association_stroke_color": "#ffcf00",
-    "background_color": "#d30300",
-    "card_text_color": "#ffcf00",
-    "entity_attribute_text_color": "#ffcf00",
-    "entity_cartouche_color": "#fd0400",
-    "entity_cartouche_text_color": "#ffcf00",
-    "entity_color": "#fd0400",
-    "entity_stroke_color": "#ffcf00",
-    "leg_stroke_color": "#ffcf00",
-    "note_color": "#535300",
-    "note_opacity": 0.7,
-    "note_text_color": "#FFFF00"
+    "association_attribute_text_color": "#060100",
+    "association_cartouche_color": "#081a84",
+    "association_cartouche_text_color": "#fefeec",
+    "association_color": "#fefeec",
+    "association_stroke_color": "#060100",
+    "background_color": "#fefeec",
+    "card_text_color": "#060100",
+    "constraint_background_color": "#fefeec",
+    "constraint_stroke_color": "#060100",
+    "constraint_text_color": "#060100",
+    "entity_attribute_text_color": "#060100",
+    "entity_cartouche_color": "#c6281b",
+    "entity_cartouche_text_color": "#fefeec",
+    "entity_color": "#fced5f",
+    "entity_stroke_color": "#060100",
+    "leg_stroke_color": "#060100",
+    "note_color": "#066A6A",
+    "note_opacity": 0.85,
+    "note_text_color": "#FFFF22"
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/font_metrics.json` & `mocodo-3.2.0/mocodo/resources/font_metrics.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/lorem/disparition.txt` & `mocodo-3.2.0/mocodo/resources/lorem/disparition.txt`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/lorem/four_letter_words.txt` & `mocodo-3.2.0/mocodo/resources/lorem/four_letter_words.txt`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/lorem/lorem_ipsum.txt` & `mocodo-3.2.0/mocodo/resources/lorem/lorem_ipsum.txt`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/relation_templates/debug.json` & `mocodo-3.2.0/mocodo/resources/relation_templates/debug.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/relation_templates/dependencies.json` & `mocodo-3.2.0/mocodo/resources/relation_templates/dependencies.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/relation_templates/diagram.json` & `mocodo-3.2.0/mocodo/resources/relation_templates/diagram.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/relation_templates/html.json` & `mocodo-3.2.0/mocodo/resources/relation_templates/html.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/relation_templates/html_verbose.json` & `mocodo-3.2.0/mocodo/resources/relation_templates/html_verbose.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/relation_templates/json.json` & `mocodo-3.2.0/mocodo/resources/relation_templates/json.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/relation_templates/latex.json` & `mocodo-3.2.0/mocodo/resources/relation_templates/latex.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/relation_templates/markdown_data_dict.json` & `mocodo-3.2.0/mocodo/resources/relation_templates/markdown_data_dict.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/relation_templates/markdown_verbose.json` & `mocodo-3.2.0/mocodo/resources/relation_templates/markdown_verbose.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/relation_templates/mysql.json` & `mocodo-3.2.0/mocodo/resources/relation_templates/mysql.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/relation_templates/oracle.json` & `mocodo-3.2.0/mocodo/resources/relation_templates/oracle.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/relation_templates/postgresql.json` & `mocodo-3.2.0/mocodo/resources/relation_templates/postgresql.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/relation_templates/sqlite.json` & `mocodo-3.2.0/mocodo/resources/relation_templates/sqlite.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/res/messages_de.mo` & `mocodo-3.2.0/mocodo/resources/res/messages_de.mo`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/res/messages_fr.mo` & `mocodo-3.2.0/mocodo/resources/res/messages_fr.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,29 +1,30 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: mocodo\n"
-"POT-Creation-Date: 2022-12-14 18:28+0100\n"
+"POT-Creation-Date: 2023-05-15 18:03+0200\n"
 "PO-Revision-Date: 2015-08-16 07:00+0000\n"
-"Last-Translator: Aristide Grange <chewingword@wingi.net>, 2015-2016,2022\n"
-"Language-Team: French (http://www.transifex.com/aristide/mocodo/language/"
+"Last-Translator: Aristide Grange <chewingword@wingi.net>, "
+"2015-2016,2022-2023\n"
+"Language-Team: French (http://app.transifex.com/aristide/mocodo/language/"
 "fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid ""
 "\"{clause}\" does not constitute a valid declaration of an entity or "
 "association."
 msgstr ""
-"« {clause} » ne constitue pas une déclaration d'entité ou d'association "
-"valide."
+"« {clause} » ne constitue pas une déclaration d'entité, d'association ou de "
+"contrainte valide."
 
 msgid "- Leg “{b1} — {b2}” overlaps “{b3}”."
 msgstr "- La patte « {b1} — {b2} » chevauche « {b3} »."
 
 msgid "- Legs “{b1} — {b2}” and “{b3} — {b4}” overlap."
 msgstr "- Les pattes  « {b1} — {b2} » et « {b3} — {b4} » se chevauchent."
 
@@ -53,14 +54,21 @@
 "L'attribut « {attribute} » de l'entité « {entity_1} » fait référence à une "
 "entité « {entity_2} » inconnue."
 
 msgid "Circular inheritance in template \"{name}.json\" of \"{folder}."
 msgstr ""
 "Héritage circulaire dans le gabarit « {name}.json » du dossier « {folder} »."
 
+msgid ""
+"Constraint \"{constraint}\" linked to an unknown entity or association "
+"\"{box}\"!"
+msgstr ""
+"Une contrainte « {constraint} » est liée à une entité ou association "
+"inconnue « {box} »."
+
 msgid "Cycle of weak entities in {entities}."
 msgstr "Cycle d'entités faibles dans {entities}."
 
 msgid ""
 "Duplicate association \"{name}\". If you want to make two associations "
 "appear with the same name, you must suffix it with a number."
 msgstr ""
@@ -80,14 +88,20 @@
 
 msgid "Generated by Mocodo {version} on {date}"
 msgstr "Généré par Mocodo {version} ({date})."
 
 msgid "Layout calculation time exceeded."
 msgstr "Dépassement du temps maximum alloué pour le calcul de la mise en page."
 
+msgid "Malformed constraint ratios \"{ratios}\"."
+msgstr ""
+"Pour positionner le centre d'une contrainte, terminez la clause par un deux-"
+"points suivi d'un ou deux entiers séparés par des virgules.  "
+"« {ratios} » n'est pas correct."
+
 msgid "Missing cardinalities on leg \"{leg}\" of association \"{name}\"."
 msgstr ""
 "Cardinalités manquantes sur la patte « {leg} » de l'association « {name} »."
 
 msgid "Missing leg in association \"{name}\"."
 msgstr "Patte manquante dans  association « {name} »."
 
@@ -204,15 +218,15 @@
 "doit avoir au moins une cardinalité 0N ou 1N (sans barre oblique)."
 
 msgid ""
 "To become a cluster, association \"{name}\"'s cardinalities must all be "
 "\"0N\", \"1N\", \"/0N\" or \"/1N\"."
 msgstr ""
 "Pour devenir une pseudo-entité (ou agrégation), l'association « {name} » ne "
-"peut avoir d'autres cardinalités que 0N, 1N, /ON ou /1N."
+"peut avoir d'autres cardinalités que 0N, 1N, /0N ou /1N."
 
 msgid ""
 "Totality (/T\\ or /XT\\) is mandatory for \"=>\" inheritance of parent "
 "{name}."
 msgstr ""
 "La totalité (/T\\ or /XT\\) est requise pour définir l'héritage « => » sur "
 "l'entité-mère « {name} »."
```

### Comparing `mocodo-3.1.2/mocodo/resources/res/messages_fr.po` & `mocodo-3.2.0/mocodo/resources/res/messages_fr.po`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/res/messages_zh.mo` & `mocodo-3.2.0/mocodo/resources/res/messages_zh.mo`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.2/mocodo/resources/shapes/arial.json` & `mocodo-3.2.0/mocodo/resources/shapes/arial.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8461538461538461%*

 * *Differences: {"'constraint_dot_gap_width'": '5.0',*

 * * "'constraint_dot_stroke_depth'": '2.5',*

 * * "'constraint_font'": "OrderedDict([('family', 'Arial'), ('size', 12)])",*

 * * "'constraint_margin'": '5',*

 * * "'constraint_stroke_depth'": '1.5',*

 * * "'constraint_text_height_tweak'": '0.3'}*

```diff
@@ -18,14 +18,23 @@
         "size": 12
     },
     "card_margin": 6,
     "card_text_height_ratio": 0.85,
     "card_underline_depth": 1.2,
     "card_underline_skip_height": -3,
     "cartouche_text_height_ratio": 0.85,
+    "constraint_dot_gap_width": 5.0,
+    "constraint_dot_stroke_depth": 2.5,
+    "constraint_font": {
+        "family": "Arial",
+        "size": 12
+    },
+    "constraint_margin": 5,
+    "constraint_stroke_depth": 1.5,
+    "constraint_text_height_tweak": 0.3,
     "dash_width": 4,
     "df_text_height_ratio": 1.0,
     "entity_attribute_font": {
         "family": "Arial",
         "size": 14
     },
     "entity_cartouche_font": {
```

### Comparing `mocodo-3.1.2/mocodo/resources/shapes/copperplate.json` & `mocodo-3.2.0/mocodo/resources/shapes/georgia.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7115384615384616%*

 * *Differences: {"'association_attribute_font'": "{'family': 'Georgia', 'size': 14}",*

 * * "'association_cartouche_font'": "{'family': 'Georgia', 'size': 14}",*

 * * "'attribute_text_height_ratio'": '0.85',*

 * * "'card_font'": "{'family': 'Verdana', 'size': 12}",*

 * * "'constraint_dot_gap_width'": '5.0',*

 * * "'constraint_dot_stroke_depth'": '2',*

 * * "'constraint_font'": "OrderedDict([('family', 'Verdana'), ('size', 12)])",*

 * * "'constraint_margin'": '5',*

 * * "'constraint_stroke_depth'": '1',*

 * * "'constraint_text_height_tweak'": '0.3',*

 * * "'df_text_height_ […]*

```diff
@@ -1,56 +1,65 @@
 {
     "arrow_axis": 8,
     "arrow_half_height": 6,
     "arrow_width": 12,
     "association_attribute_font": {
-        "family": "Gill Sans",
-        "size": 15
+        "family": "Georgia",
+        "size": 14
     },
     "association_cartouche_font": {
-        "family": "Copperplate",
-        "size": 18
+        "family": "Georgia",
+        "size": 14
     },
-    "attribute_text_height_ratio": 0.65,
+    "attribute_text_height_ratio": 0.85,
     "box_stroke_depth": 1.5,
     "card_baseline": 3,
     "card_font": {
-        "family": "Futura",
-        "size": 11
+        "family": "Verdana",
+        "size": 12
     },
     "card_margin": 5,
     "card_text_height_ratio": 0.85,
     "card_underline_depth": 1,
     "card_underline_skip_height": -2,
     "cartouche_text_height_ratio": 0.85,
+    "constraint_dot_gap_width": 5.0,
+    "constraint_dot_stroke_depth": 2,
+    "constraint_font": {
+        "family": "Verdana",
+        "size": 12
+    },
+    "constraint_margin": 5,
+    "constraint_stroke_depth": 1,
+    "constraint_text_height_tweak": 0.3,
     "dash_width": 4,
-    "df_text_height_ratio": 1.1,
+    "df_text_height_ratio": 1.0,
     "entity_attribute_font": {
-        "family": "Gill Sans",
-        "size": 15
+        "family": "Georgia",
+        "size": 14
     },
     "entity_cartouche_font": {
-        "family": "Copperplate",
-        "size": 18
+        "family": "Georgia",
+        "size": 14
     },
-    "inner_stroke_depth": 1.5,
+    "inner_stroke_depth": 1,
     "label_font": {
-        "family": "Futura",
-        "size": 11
+        "family": "Verdana",
+        "size": 12
     },
     "leg_stroke_depth": 1,
-    "line_skip_height": 0,
+    "line_skip_height": 2,
     "margin": 9,
     "note_baseline": 24,
     "note_font": {
-        "family": "Futura",
-        "size": 16
+        "family": "Georgia",
+        "size": 15
     },
     "note_overlay_height": 40,
-    "rect_margin_height": 6,
-    "rect_margin_width": 8,
+    "rect_margin_height": 5,
+    "rect_margin_width": 5,
     "round_corner_radius": 14,
     "round_rect_margin_height": 5,
     "round_rect_margin_width": 7,
     "underline_depth": 1,
-    "underline_skip_height": -3
+    "underline_skip_height": 0.0
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/shapes/georgia.json` & `mocodo-3.2.0/mocodo/resources/shapes/copperplate.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7115384615384616%*

 * *Differences: {"'association_attribute_font'": "{'family': 'Gill Sans', 'size': 15}",*

 * * "'association_cartouche_font'": "{'family': 'Copperplate', 'size': 18}",*

 * * "'attribute_text_height_ratio'": '0.65',*

 * * "'card_font'": "{'family': 'Futura', 'size': 11}",*

 * * "'constraint_dot_gap_width'": '5.0',*

 * * "'constraint_dot_stroke_depth'": '2',*

 * * "'constraint_font'": "OrderedDict([('family', 'Futura'), ('size', 11)])",*

 * * "'constraint_margin'": '5',*

 * * "'constraint_stroke_depth'": '1',*

 * * "'constraint_text_height_tweak'": '0.3',*

 * * "'df_text_hei […]*

```diff
@@ -1,56 +1,65 @@
 {
     "arrow_axis": 8,
     "arrow_half_height": 6,
     "arrow_width": 12,
     "association_attribute_font": {
-        "family": "Georgia",
-        "size": 14
+        "family": "Gill Sans",
+        "size": 15
     },
     "association_cartouche_font": {
-        "family": "Georgia",
-        "size": 14
+        "family": "Copperplate",
+        "size": 18
     },
-    "attribute_text_height_ratio": 0.85,
+    "attribute_text_height_ratio": 0.65,
     "box_stroke_depth": 1.5,
     "card_baseline": 3,
     "card_font": {
-        "family": "Verdana",
-        "size": 12
+        "family": "Futura",
+        "size": 11
     },
     "card_margin": 5,
     "card_text_height_ratio": 0.85,
     "card_underline_depth": 1,
     "card_underline_skip_height": -2,
     "cartouche_text_height_ratio": 0.85,
+    "constraint_dot_gap_width": 5.0,
+    "constraint_dot_stroke_depth": 2,
+    "constraint_font": {
+        "family": "Futura",
+        "size": 11
+    },
+    "constraint_margin": 5,
+    "constraint_stroke_depth": 1,
+    "constraint_text_height_tweak": 0.3,
     "dash_width": 4,
-    "df_text_height_ratio": 1.0,
+    "df_text_height_ratio": 1.1,
     "entity_attribute_font": {
-        "family": "Georgia",
-        "size": 14
+        "family": "Gill Sans",
+        "size": 15
     },
     "entity_cartouche_font": {
-        "family": "Georgia",
-        "size": 14
+        "family": "Copperplate",
+        "size": 18
     },
-    "inner_stroke_depth": 1,
+    "inner_stroke_depth": 1.5,
     "label_font": {
-        "family": "Verdana",
-        "size": 12
+        "family": "Futura",
+        "size": 11
     },
     "leg_stroke_depth": 1,
-    "line_skip_height": 2,
+    "line_skip_height": 0,
     "margin": 9,
     "note_baseline": 24,
     "note_font": {
-        "family": "Georgia",
-        "size": 15
+        "family": "Futura",
+        "size": 16
     },
     "note_overlay_height": 40,
-    "rect_margin_height": 5,
-    "rect_margin_width": 5,
+    "rect_margin_height": 6,
+    "rect_margin_width": 8,
     "round_corner_radius": 14,
     "round_rect_margin_height": 5,
     "round_rect_margin_width": 7,
     "underline_depth": 1,
-    "underline_skip_height": 0.0
+    "underline_skip_height": -3
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/shapes/mondrian.json` & `mocodo-3.2.0/mocodo/resources/shapes/serif.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.517094017094017%*

 * *Differences: {"'arrow_axis'": '8',*

 * * "'arrow_half_height'": '6',*

 * * "'arrow_width'": '12',*

 * * "'association_attribute_font'": "{'family': 'Liberation Serif', 'size': 14, delete: ['weight']}",*

 * * "'association_cartouche_font'": "{'family': 'Liberation Serif', 'size': 14, delete: ['weight']}",*

 * * "'box_stroke_depth'": '1.5',*

 * * "'card_baseline'": '3',*

 * * "'card_font'": "{'family': 'Liberation Serif', 'size': 12, delete: ['weight']}",*

 * * "'card_margin'": '5',*

 * * "'card_underline_depth'": '1',*

 * * "'card_underline_skip_height'": '1',*

 * * "'constr […]*

```diff
@@ -1,63 +1,65 @@
 {
-    "arrow_axis": 12,
-    "arrow_half_height": 9,
-    "arrow_width": 18,
+    "arrow_axis": 8,
+    "arrow_half_height": 6,
+    "arrow_width": 12,
     "association_attribute_font": {
-        "family": "Skia",
-        "size": 18,
-        "weight": "bold"
+        "family": "Liberation Serif",
+        "size": 14
     },
     "association_cartouche_font": {
-        "family": "Skia",
-        "size": 20,
-        "weight": "bold"
+        "family": "Liberation Serif",
+        "size": 14
     },
     "attribute_text_height_ratio": 0.85,
-    "box_stroke_depth": 5,
-    "card_baseline": 4,
+    "box_stroke_depth": 1.5,
+    "card_baseline": 3,
     "card_font": {
-        "family": "Skia",
-        "size": 18,
-        "weight": "bold"
+        "family": "Liberation Serif",
+        "size": 12
     },
-    "card_margin": 8,
+    "card_margin": 5,
     "card_text_height_ratio": 0.85,
-    "card_underline_depth": 1.2,
-    "card_underline_skip_height": -3,
+    "card_underline_depth": 1,
+    "card_underline_skip_height": 1,
     "cartouche_text_height_ratio": 0.85,
-    "dash_width": 2,
+    "constraint_dot_gap_width": 5.0,
+    "constraint_dot_stroke_depth": 2,
+    "constraint_font": {
+        "family": "Liberation Serif",
+        "size": 12
+    },
+    "constraint_margin": 2.5,
+    "constraint_stroke_depth": 1,
+    "constraint_text_height_tweak": 0.3,
+    "dash_width": 4,
     "df_text_height_ratio": 1.0,
     "entity_attribute_font": {
-        "family": "Skia",
-        "size": 18,
-        "weight": "bold"
+        "family": "Liberation Serif",
+        "size": 14
     },
     "entity_cartouche_font": {
-        "family": "Skia",
-        "size": 20,
-        "weight": "bold"
+        "family": "Liberation Serif",
+        "size": 14
     },
-    "inner_stroke_depth": 5,
+    "inner_stroke_depth": 1,
     "label_font": {
-        "family": "Skia",
-        "size": 18,
-        "weight": "bold"
-    },
-    "leg_stroke_depth": 5,
-    "line_skip_height": 1,
-    "margin": 25,
-    "note_baseline": 32,
+        "family": "Liberation Serif",
+        "size": 12
+    },
+    "leg_stroke_depth": 1,
+    "line_skip_height": 2,
+    "margin": 9,
+    "note_baseline": 24,
     "note_font": {
-        "family": "Skia",
-        "size": 20,
-        "weight": "bold"
-    },
-    "note_overlay_height": 50,
-    "rect_margin_height": 10,
-    "rect_margin_width": 10,
-    "round_corner_radius": 2,
-    "round_rect_margin_height": 10,
-    "round_rect_margin_width": 10,
-    "underline_depth": 1.2,
+        "family": "Liberation Serif",
+        "size": 14
+    },
+    "note_overlay_height": 40,
+    "rect_margin_height": 5,
+    "rect_margin_width": 5,
+    "round_corner_radius": 14,
+    "round_rect_margin_height": 5,
+    "round_rect_margin_width": 7,
+    "underline_depth": 1,
     "underline_skip_height": 0.0
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/shapes/sans.json` & `mocodo-3.2.0/mocodo/resources/shapes/sans.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8461538461538461%*

 * *Differences: {"'constraint_dot_gap_width'": '5.0',*

 * * "'constraint_dot_stroke_depth'": '2',*

 * * "'constraint_font'": "OrderedDict([('family', 'Liberation Sans'), ('size', 12)])",*

 * * "'constraint_margin'": '2.5',*

 * * "'constraint_stroke_depth'": '1',*

 * * "'constraint_text_height_tweak'": '0.3'}*

```diff
@@ -18,14 +18,23 @@
         "size": 12
     },
     "card_margin": 5,
     "card_text_height_ratio": 0.85,
     "card_underline_depth": 1,
     "card_underline_skip_height": 1,
     "cartouche_text_height_ratio": 0.85,
+    "constraint_dot_gap_width": 5.0,
+    "constraint_dot_stroke_depth": 2,
+    "constraint_font": {
+        "family": "Liberation Sans",
+        "size": 12
+    },
+    "constraint_margin": 2.5,
+    "constraint_stroke_depth": 1,
+    "constraint_text_height_tweak": 0.3,
     "dash_width": 4,
     "df_text_height_ratio": 1.0,
     "entity_attribute_font": {
         "family": "Liberation Sans",
         "size": 14
     },
     "entity_cartouche_font": {
```

### Comparing `mocodo-3.1.2/mocodo/resources/shapes/serif.json` & `mocodo-3.2.0/mocodo/resources/shapes/times.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7948717948717948%*

 * *Differences: {"'association_attribute_font'": "{'family': 'Times New Roman'}",*

 * * "'association_cartouche_font'": "{'family': 'Times New Roman'}",*

 * * "'card_font'": "{'family': 'Verdana'}",*

 * * "'card_underline_skip_height'": '-2',*

 * * "'constraint_dot_gap_width'": '5.0',*

 * * "'constraint_dot_stroke_depth'": '2',*

 * * "'constraint_font'": "OrderedDict([('family', 'Verdana'), ('size', 12)])",*

 * * "'constraint_margin'": '5',*

 * * "'constraint_stroke_depth'": '1',*

 * * "'constraint_text_height_tweak'": '0.3',*

 * * "'df_text_height_ratio'": '1.1',*

 * * "'enti […]*

```diff
@@ -1,53 +1,62 @@
 {
     "arrow_axis": 8,
     "arrow_half_height": 6,
     "arrow_width": 12,
     "association_attribute_font": {
-        "family": "Liberation Serif",
+        "family": "Times New Roman",
         "size": 14
     },
     "association_cartouche_font": {
-        "family": "Liberation Serif",
+        "family": "Times New Roman",
         "size": 14
     },
     "attribute_text_height_ratio": 0.85,
     "box_stroke_depth": 1.5,
     "card_baseline": 3,
     "card_font": {
-        "family": "Liberation Serif",
+        "family": "Verdana",
         "size": 12
     },
     "card_margin": 5,
     "card_text_height_ratio": 0.85,
     "card_underline_depth": 1,
-    "card_underline_skip_height": 1,
+    "card_underline_skip_height": -2,
     "cartouche_text_height_ratio": 0.85,
+    "constraint_dot_gap_width": 5.0,
+    "constraint_dot_stroke_depth": 2,
+    "constraint_font": {
+        "family": "Verdana",
+        "size": 12
+    },
+    "constraint_margin": 5,
+    "constraint_stroke_depth": 1,
+    "constraint_text_height_tweak": 0.3,
     "dash_width": 4,
-    "df_text_height_ratio": 1.0,
+    "df_text_height_ratio": 1.1,
     "entity_attribute_font": {
-        "family": "Liberation Serif",
+        "family": "Times New Roman",
         "size": 14
     },
     "entity_cartouche_font": {
-        "family": "Liberation Serif",
+        "family": "Times New Roman",
         "size": 14
     },
     "inner_stroke_depth": 1,
     "label_font": {
-        "family": "Liberation Serif",
+        "family": "Verdana",
         "size": 12
     },
     "leg_stroke_depth": 1,
     "line_skip_height": 2,
     "margin": 9,
     "note_baseline": 24,
     "note_font": {
-        "family": "Liberation Serif",
-        "size": 14
+        "family": "Times New Roman",
+        "size": 16
     },
     "note_overlay_height": 40,
     "rect_margin_height": 5,
     "rect_margin_width": 5,
     "round_corner_radius": 14,
     "round_rect_margin_height": 5,
     "round_rect_margin_width": 7,
```

### Comparing `mocodo-3.1.2/mocodo/resources/shapes/times.json` & `mocodo-3.2.0/mocodo/resources/shapes/trebuchet.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8141025641025641%*

 * *Differences: {"'association_attribute_font'": "{'family': 'Trebuchet MS'}",*

 * * "'association_cartouche_font'": "{'family': 'Trebuchet MS'}",*

 * * "'constraint_dot_gap_width'": '5.0',*

 * * "'constraint_dot_stroke_depth'": '2',*

 * * "'constraint_font'": "OrderedDict([('family', 'Verdana'), ('size', 12)])",*

 * * "'constraint_margin'": '5',*

 * * "'constraint_stroke_depth'": '1',*

 * * "'constraint_text_height_tweak'": '0.3',*

 * * "'df_text_height_ratio'": '0.9',*

 * * "'entity_attribute_font'": "{'family': 'Trebuchet MS'}",*

 * * "'entity_cartouche_font'": "{'fami […]*

```diff
@@ -1,53 +1,62 @@
 {
     "arrow_axis": 8,
     "arrow_half_height": 6,
     "arrow_width": 12,
     "association_attribute_font": {
-        "family": "Times New Roman",
+        "family": "Trebuchet MS",
         "size": 14
     },
     "association_cartouche_font": {
-        "family": "Times New Roman",
+        "family": "Trebuchet MS",
         "size": 14
     },
     "attribute_text_height_ratio": 0.85,
     "box_stroke_depth": 1.5,
     "card_baseline": 3,
     "card_font": {
         "family": "Verdana",
         "size": 12
     },
     "card_margin": 5,
     "card_text_height_ratio": 0.85,
     "card_underline_depth": 1,
     "card_underline_skip_height": -2,
     "cartouche_text_height_ratio": 0.85,
+    "constraint_dot_gap_width": 5.0,
+    "constraint_dot_stroke_depth": 2,
+    "constraint_font": {
+        "family": "Verdana",
+        "size": 12
+    },
+    "constraint_margin": 5,
+    "constraint_stroke_depth": 1,
+    "constraint_text_height_tweak": 0.3,
     "dash_width": 4,
-    "df_text_height_ratio": 1.1,
+    "df_text_height_ratio": 0.9,
     "entity_attribute_font": {
-        "family": "Times New Roman",
+        "family": "Trebuchet MS",
         "size": 14
     },
     "entity_cartouche_font": {
-        "family": "Times New Roman",
+        "family": "Trebuchet MS",
         "size": 14
     },
     "inner_stroke_depth": 1,
     "label_font": {
         "family": "Verdana",
         "size": 12
     },
     "leg_stroke_depth": 1,
     "line_skip_height": 2,
     "margin": 9,
     "note_baseline": 24,
     "note_font": {
-        "family": "Times New Roman",
-        "size": 16
+        "family": "Trebuchet MS",
+        "size": 14
     },
     "note_overlay_height": 40,
     "rect_margin_height": 5,
     "rect_margin_width": 5,
     "round_corner_radius": 14,
     "round_rect_margin_height": 5,
     "round_rect_margin_width": 7,
```

### Comparing `mocodo-3.1.2/mocodo/resources/shapes/trebuchet.json` & `mocodo-3.2.0/mocodo/resources/shapes/xinnian.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5705128205128205%*

 * *Differences: {"'arrow_axis'": '12',*

 * * "'arrow_half_height'": '9',*

 * * "'arrow_width'": '18',*

 * * "'association_attribute_font'": "{'family': 'Arial Black'}",*

 * * "'association_cartouche_font'": "{'family': 'Arial Black'}",*

 * * "'attribute_text_height_ratio'": '0.5',*

 * * "'box_stroke_depth'": '5',*

 * * "'card_baseline'": '5',*

 * * "'card_font'": "{'family': 'Comic Sans MS', 'size': 14}",*

 * * "'card_margin'": '10',*

 * * "'card_underline_skip_height'": '-4.0',*

 * * "'constraint_dot_gap_width'": '8',*

 * * "'constraint_dot_stroke_depth'": '4',*

 * * "'constraint_font' […]*

```diff
@@ -1,56 +1,65 @@
 {
-    "arrow_axis": 8,
-    "arrow_half_height": 6,
-    "arrow_width": 12,
+    "arrow_axis": 12,
+    "arrow_half_height": 9,
+    "arrow_width": 18,
     "association_attribute_font": {
-        "family": "Trebuchet MS",
+        "family": "Arial Black",
         "size": 14
     },
     "association_cartouche_font": {
-        "family": "Trebuchet MS",
+        "family": "Arial Black",
         "size": 14
     },
-    "attribute_text_height_ratio": 0.85,
-    "box_stroke_depth": 1.5,
-    "card_baseline": 3,
+    "attribute_text_height_ratio": 0.5,
+    "box_stroke_depth": 5,
+    "card_baseline": 5,
     "card_font": {
-        "family": "Verdana",
-        "size": 12
+        "family": "Comic Sans MS",
+        "size": 14
     },
-    "card_margin": 5,
+    "card_margin": 10,
     "card_text_height_ratio": 0.85,
     "card_underline_depth": 1,
-    "card_underline_skip_height": -2,
+    "card_underline_skip_height": -4.0,
     "cartouche_text_height_ratio": 0.85,
+    "constraint_dot_gap_width": 8,
+    "constraint_dot_stroke_depth": 4,
+    "constraint_font": {
+        "family": "Comic Sans MS",
+        "size": 14
+    },
+    "constraint_margin": 5.0,
+    "constraint_stroke_depth": 2,
+    "constraint_text_height_tweak": 0.3,
     "dash_width": 4,
-    "df_text_height_ratio": 0.9,
+    "df_text_height_ratio": 1.0,
     "entity_attribute_font": {
-        "family": "Trebuchet MS",
+        "family": "Arial Black",
         "size": 14
     },
     "entity_cartouche_font": {
-        "family": "Trebuchet MS",
+        "family": "Arial Black",
         "size": 14
     },
-    "inner_stroke_depth": 1,
+    "inner_stroke_depth": 0.5,
     "label_font": {
-        "family": "Verdana",
-        "size": 12
+        "family": "Comic Sans MS",
+        "size": 14
     },
-    "leg_stroke_depth": 1,
+    "leg_stroke_depth": 2,
     "line_skip_height": 2,
-    "margin": 9,
+    "margin": 20,
     "note_baseline": 24,
     "note_font": {
-        "family": "Trebuchet MS",
-        "size": 14
+        "family": "Arial Black",
+        "size": 16
     },
     "note_overlay_height": 40,
-    "rect_margin_height": 5,
-    "rect_margin_width": 5,
-    "round_corner_radius": 14,
-    "round_rect_margin_height": 5,
-    "round_rect_margin_width": 7,
-    "underline_depth": 1,
-    "underline_skip_height": 0.0
+    "rect_margin_height": 9,
+    "rect_margin_width": 14,
+    "round_corner_radius": 30,
+    "round_rect_margin_height": 10,
+    "round_rect_margin_width": 14,
+    "underline_depth": 2,
+    "underline_skip_height": -5.0
 }
```

### Comparing `mocodo-3.1.2/mocodo/resources/shapes/verdana.json` & `mocodo-3.2.0/mocodo/resources/shapes/verdana.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8461538461538461%*

 * *Differences: {"'constraint_dot_gap_width'": '6',*

 * * "'constraint_dot_stroke_depth'": '3',*

 * * "'constraint_font'": "OrderedDict([('family', 'Verdana'), ('size', 12), ('weight', 'bold')])",*

 * * "'constraint_margin'": '5',*

 * * "'constraint_stroke_depth'": '1.5',*

 * * "'constraint_text_height_tweak'": '0.3'}*

```diff
@@ -21,14 +21,24 @@
         "weight": "bold"
     },
     "card_margin": 5,
     "card_text_height_ratio": 0.85,
     "card_underline_depth": 1,
     "card_underline_skip_height": -2,
     "cartouche_text_height_ratio": 0.85,
+    "constraint_dot_gap_width": 6,
+    "constraint_dot_stroke_depth": 3,
+    "constraint_font": {
+        "family": "Verdana",
+        "size": 12,
+        "weight": "bold"
+    },
+    "constraint_margin": 5,
+    "constraint_stroke_depth": 1.5,
+    "constraint_text_height_tweak": 0.3,
     "dash_width": 4,
     "df_text_height_ratio": 1.0,
     "entity_attribute_font": {
         "family": "Verdana",
         "size": 12,
         "weight": "bold"
     },
```

### Comparing `mocodo-3.1.2/pyproject.toml` & `mocodo-3.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mocodo"
-version = "3.1.2"
+version = "3.2.0"
 description = "Modélisation Conceptuelle de Données. Nickel. Ni souris."
 authors = ["Aristide Grange"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.mocodo.net"
 repository = "https://github.com/laowantong/mocodo/"
 keywords = ["education",
```

### Comparing `mocodo-3.1.2/setup.py` & `mocodo-3.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,17 +32,17 @@
             'resources/shapes/*']}
 
 entry_points = \
 {'console_scripts': ['mocodo = mocodo.__main__:main']}
 
 setup_kwargs = {
     'name': 'mocodo',
-    'version': '3.1.2',
+    'version': '3.2.0',
     'description': 'Modélisation Conceptuelle de Données. Nickel. Ni souris.',
-    'long_description': "**11 mai 2023.** Ajout d'un tutoriel / galerie d'exemples dans la [version en ligne](https://www.mocodo.net) de Mocodo 3.1.2.\n\n**24 décembre 2022.** Mocodo 3.1.1 corrige la [gestion des collisions des SVG interactifs](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Éviter-qu'une-interaction-sur-un-SVG-ne-s'applique-à-un-autre).\n\n**14 décembre 2022.** Mocodo 3.1 améliore le passage au relationnel\xa0: prise en charge de [gabarits personnels dérivés des gabarits existants](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Dérivation-de-gabarits), traitement des [tables indépendantes réduites à leur clé primaire](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Suppression-des-tables-indépendantes-réduites-à-leur-clé-primaire), génération d'un [graphe des dépendances](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Graphe-des-dépendances) pour le tri topologique des tables, [etc](https://github.com/laowantong/mocodo/releases/tag/3.1.0).\n\n**11 septembre 2022.** Mocodo 3.0 introduit l'[héritage](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), l'[agrégation](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Agrégation-(ou-pseudo-entité)), les [calques](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), les [sorties PDF et PNG](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), [etc](https://github.com/laowantong/mocodo/releases/tag/3.0).\n\n------\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/logos/banner.svg)\n\nMocodo est un logiciel d'aide à l'enseignement et à la conception des [bases de données relationnelles](https://fr.wikipedia.org/wiki/Base_de_données_relationnelle).\n\n- En entrée, il prend une description textuelle des entités et associations du modèle conceptuel de données ([MCD](https://fr.wikipedia.org/wiki/Modèle_entité-association)).\n- En sortie, il produit son diagramme entité-association en [SVG](https://fr.wikipedia.org/wiki/Scalable_Vector_Graphics) et son schéma relationnel ([MLD](\nhttps://fr.wikipedia.org/wiki/Merise_%28informatique%29#MLD_:_mod.C3.A8le_logique_des_donn.C3.A9es)) en [SQL](https://fr.wikipedia.org/wiki/Structured_Query_Language), [LaTeX](https://fr.wikipedia.org/wiki/LaTeX), [Markdown](https://fr.wikipedia.org/wiki/Markdown), etc.\n\nCi-dessous, un exemple sous [Jupyter Notebook](https://jupyter.org). L'appel du programme se fait en première ligne, sur un texte d'entrée donné lignes suivantes.\n\n```\n%%mocodo --mld --colors brewer+1 --shapes copperplate --relations diagram markdown_data_dict\nDF, 11 Élève, 1N Classe\nClasse: Num. classe, Num. salle\nFaire Cours, 1N Classe, 1N Prof: Vol. horaire\nCatégorie: Code catégorie, Nom catégorie\n\nÉlève: Num. élève, Nom élève\nNoter, 1N Élève, 0N Prof, 0N Matière, 1N Date: Note\nProf: Num. prof, Nom prof\nRelever, 0N Catégorie, 11 Prof\n\nDate: Date\nMatière: Libellé matière\nEnseigner, 11 Prof, 1N Matière\n```\n\nEn sortie, le MCD (diagramme conceptuel) et le MLD (schéma relationnel) correspondants:\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/doc/readme_1.svg)\n\n**Catégorie** (<ins>Code catégorie</ins>, Nom catégorie)<br>\n**Classe** (<ins>Num. classe</ins>, Num. salle)<br>\n**Faire Cours** (<ins>_#Num. classe_</ins>, <ins>_#Num. prof_</ins>, Vol. horaire)<br>\n**Noter** (<ins>_#Num. élève_</ins>, <ins>_#Num. prof_</ins>, <ins>_#Libellé matière_</ins>, <ins>_#Date_</ins>, Note)<br>\n**Prof** (<ins>Num. prof</ins>, Nom prof, _#Code catégorie_, _#Libellé matière_)<br>\n**Élève** (<ins>Num. élève</ins>, Nom élève, _#Num. classe_)\n\nL'appel ci-dessus a également construit le dictionnaire des données:\n\n- Num. classe\n- Num. salle\n- Vol. horaire\n- Code catégorie\n- Nom catégorie\n- Num. élève\n- Nom élève\n- Note\n- Num. prof\n- Nom prof\n- Date\n- Libellé matière\n\nAinsi que le diagramme relationnel, qui peut être visualisé par un nouvel appel:\n\n```\n%mocodo --input mocodo_notebook/sandbox.mld --colors brewer+1\n```\n\n![](https://cdn.rawgit.com/laowantong/mocodo/f06f70a/doc/readme_2.svg)\n\nLa devise de Mocodo, «\xa0nickel, ni souris\xa0», en résume les principaux points forts:\n\n- description textuelle des données. L'utilisateur n'a pas à renseigner, placer et déplacer des éléments comme avec une lessive ordinaire. Il ne fournit rien de plus que les informations définissant son MCD. L'outil s'occupe tout seul du plongement;\n- propreté du rendu. La sortie se fait en vectoriel, prête à être affichée, imprimée, agrandie, exportée dans une multitude de formats sans perte de qualité;\n- rapidité des retouches. L'utilisateur rectifie les alignements en insérant des éléments invisibles, en dupliquant des coordonnées ou en ajustant des facteurs mutiplicatifs: là encore, il travaille sur une description textuelle, et non directement sur le dessin.\n\nMocodo est libre, gratuit et multiplateforme. Si vous l'aimez, répandez la bonne nouvelle en incluant l'un de ses logos dans votre support: cela multipliera ses chances d'attirer des contributeurs qui le feront évoluer.\n\nPour vous familiariser avec Mocodo, le mieux est d'utiliser [sa version en ligne](https://www.mocodo.net).\n\nPour en savoir plus, lisez la documentation [au format HTML](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html) ou téléchargez-la [au format Jupyter Notebook](doc/fr_refman.ipynb).\n",
+    'long_description': "**15 mai 2023.** Mocodo 3.2.0 prend en charge la [visualisation des contraintes sur associations](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Visualisation-des-contraintes-sur-associations).\n\n**11 mai 2023.** Ajout d'un tutoriel / galerie d'exemples dans la [version en ligne](https://www.mocodo.net) de Mocodo 3.1.2.\n\n**24 décembre 2022.** Mocodo 3.1.1 corrige la [gestion des collisions des SVG interactifs](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Éviter-qu'une-interaction-sur-un-SVG-ne-s'applique-à-un-autre).\n\n**14 décembre 2022.** Mocodo 3.1 améliore le passage au relationnel\xa0: prise en charge de [gabarits personnels dérivés des gabarits existants](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Dérivation-de-gabarits), traitement des [tables indépendantes réduites à leur clé primaire](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Suppression-des-tables-indépendantes-réduites-à-leur-clé-primaire), génération d'un [graphe des dépendances](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Graphe-des-dépendances) pour le tri topologique des tables, [etc](https://github.com/laowantong/mocodo/releases/tag/3.1.0).\n\n**11 septembre 2022.** Mocodo 3.0 introduit l'[héritage](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), l'[agrégation](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Agrégation-(ou-pseudo-entité)), les [calques](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), les [sorties PDF et PNG](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), [etc](https://github.com/laowantong/mocodo/releases/tag/3.0).\n\n------\n\nDocumentation [au format HTML](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html) ou sous forme de [notebook](doc/fr_refman.ipynb) Jupyter.\n\n----\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/logos/banner.svg)\n\nMocodo est un logiciel d'aide à l'enseignement et à la conception des [bases de données relationnelles](https://fr.wikipedia.org/wiki/Base_de_données_relationnelle).\n\n- En entrée, il prend une description textuelle des entités et associations du modèle conceptuel de données ([MCD](https://fr.wikipedia.org/wiki/Modèle_entité-association)).\n- En sortie, il produit son diagramme entité-association en [SVG](https://fr.wikipedia.org/wiki/Scalable_Vector_Graphics) et son schéma relationnel ([MLD](\nhttps://fr.wikipedia.org/wiki/Merise_%28informatique%29#MLD_:_mod.C3.A8le_logique_des_donn.C3.A9es)) en [SQL](https://fr.wikipedia.org/wiki/Structured_Query_Language), [LaTeX](https://fr.wikipedia.org/wiki/LaTeX), [Markdown](https://fr.wikipedia.org/wiki/Markdown), etc.\n\nCi-dessous, un exemple d'utilisation sous [Jupyter Notebook](https://jupyter.org). L'appel du programme est en première ligne, sur un texte d'entrée donné lignes suivantes. Le cas est adapté de l'article fondateur de Peter Chen, [_The entity-relationship model—toward a unified view of data_](https://doi.org/10.1145/320434.320440) (ACM Trans. Database Syst. 1, 1, March 1976, pp. 9–36), avec en bonus une association de type hiérarchique et une contrainte d'inclusion.\n\n```\n%%mocodo --mld --colors brewer+1 --shapes copperplate --relations diagram markdown_data_dict\n\nAyant-droit: nom ayant-droit, lien\nDiriger, 0N Employé, 01 Projet\nRequérir, 1N Projet, 0N Pièce: qté requise\nPièce: réf. pièce, libellé pièce\nComposer, 0N [composée] Pièce, 0N [composante] Pièce: quantité\n\nDF1, _11 Ayant-droit, 0N Employé\nEmployé: matricule, nom employé\nProjet: num. projet, nom projet\nFournir, 1N Projet, 1N Pièce, 1N Société: qté fournie\n\nDépartement: num. département, nom département\nEmployer, 11 Employé, 1N Département\nTravailler, 0N Employé, 1N Projet\nSociété: num. société, raison sociale\nContrôler, 0N< [filiale] Société, 01 [mère] Société\n\n(I) --Fournir, ->Requérir, ..Pièce, Projet\n```\n\nEn sortie, le MCD (diagramme conceptuel) et le MLD (schéma relationnel) correspondants:\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/doc/readme_1.png)\n\n**Ayant-droit** (<ins>_#matricule_</ins>, <ins>nom ayant-droit</ins>, lien)<br>\n**Composer** (<ins>_#réf. pièce composée_</ins>, <ins>_#réf. pièce composante_</ins>, quantité)<br>\n**Département** (<ins>num. département</ins>, nom département)<br>\n**Employé** (<ins>matricule</ins>, nom employé, _#num. département_)<br>\n**Fournir** (<ins>_#num. projet_</ins>, <ins>_#réf. pièce_</ins>, <ins>_#num. société_</ins>, qté fournie)<br>\n**Pièce** (<ins>réf. pièce</ins>, libellé pièce)<br>\n**Projet** (<ins>num. projet</ins>, nom projet, _#matricule_)<br>\n**Requérir** (<ins>_#num. projet_</ins>, <ins>_#réf. pièce_</ins>, qté requise)<br>\n**Société** (<ins>num. société</ins>, raison sociale, _#num. société mère_)<br>\n**Travailler** (<ins>_#matricule_</ins>, <ins>_#num. projet_</ins>)\n\nL'appel précédent a également créé un fichier `mocodo_notebook/sandbox_data_dict.md` contenant le dictionnaire des données :\n\n- nom ayant-droit\n- lien\n- quantité\n- num. département\n- nom département\n- matricule\n- nom employé\n- qté fournie\n- réf. pièce\n- libellé pièce\n- num. projet\n- nom projet\n- qté requise\n- num. société\n- raison sociale\n\nAinsi que le diagramme relationnel, qui peut être visualisé par un nouvel appel:\n\n```\n%mocodo --input mocodo_notebook/sandbox.mld --colors brewer+1\n```\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/doc/readme_2.png)\n\nLa devise de Mocodo, «\xa0nickel, ni souris\xa0», en résume les principaux points forts:\n\n- description textuelle des données. L'utilisateur n'a pas à renseigner, placer et déplacer des éléments comme avec une lessive ordinaire. Il ne fournit rien de plus que les informations définissant son MCD. L'outil s'occupe tout seul du plongement\xa0;\n- propreté du rendu. La sortie se fait en vectoriel, prête à être affichée, imprimée, agrandie, exportée dans une multitude de formats sans perte de qualité\xa0;\n- rapidité des retouches. L'utilisateur rectifie les alignements en insérant des éléments invisibles, en dupliquant des coordonnées ou en ajustant des facteurs mutiplicatifs\xa0: là encore, il travaille sur une description textuelle, et non directement sur le dessin.\n\nMocodo est libre, gratuit et multiplateforme. Si vous l'aimez, répandez la bonne nouvelle en incluant l'un de ses logos dans votre support\xa0: cela augmentera ses chances d'attirer des contributeurs qui le feront évoluer.\n\nPour vous familiariser avec Mocodo, le mieux est d'utiliser [sa version en ligne](https://www.mocodo.net).\n",
     'author': 'Aristide Grange',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.mocodo.net',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mocodo-3.1.2/PKG-INFO` & `mocodo-3.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,99 @@
-Metadata-Version: 2.1
-Name: mocodo
-Version: 3.1.2
-Summary: Modélisation Conceptuelle de Données. Nickel. Ni souris.
-Home-page: https://www.mocodo.net
-License: MIT
-Keywords: education,relational,database,drawing,ERD,SVG,Merise
-Author: Aristide Grange
-Requires-Python: >=3.6.1,<4.0.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Framework :: IPython
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Database
-Classifier: Topic :: Education
-Project-URL: Repository, https://github.com/laowantong/mocodo/
-Project-URL: issues, https://github.com/laowantong/mocodo/issues
-Description-Content-Type: text/markdown
+**15 mai 2023.** Mocodo 3.2.0 prend en charge la [visualisation des contraintes sur associations](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Visualisation-des-contraintes-sur-associations).
 
 **11 mai 2023.** Ajout d'un tutoriel / galerie d'exemples dans la [version en ligne](https://www.mocodo.net) de Mocodo 3.1.2.
 
 **24 décembre 2022.** Mocodo 3.1.1 corrige la [gestion des collisions des SVG interactifs](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Éviter-qu'une-interaction-sur-un-SVG-ne-s'applique-à-un-autre).
 
 **14 décembre 2022.** Mocodo 3.1 améliore le passage au relationnel : prise en charge de [gabarits personnels dérivés des gabarits existants](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Dérivation-de-gabarits), traitement des [tables indépendantes réduites à leur clé primaire](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Suppression-des-tables-indépendantes-réduites-à-leur-clé-primaire), génération d'un [graphe des dépendances](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Graphe-des-dépendances) pour le tri topologique des tables, [etc](https://github.com/laowantong/mocodo/releases/tag/3.1.0).
 
 **11 septembre 2022.** Mocodo 3.0 introduit l'[héritage](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), l'[agrégation](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Agrégation-(ou-pseudo-entité)), les [calques](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), les [sorties PDF et PNG](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), [etc](https://github.com/laowantong/mocodo/releases/tag/3.0).
 
 ------
 
+Documentation [au format HTML](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html) ou sous forme de [notebook](doc/fr_refman.ipynb) Jupyter.
+
+----
+
 ![](https://cdn.rawgit.com/laowantong/mocodo/master/logos/banner.svg)
 
 Mocodo est un logiciel d'aide à l'enseignement et à la conception des [bases de données relationnelles](https://fr.wikipedia.org/wiki/Base_de_données_relationnelle).
 
 - En entrée, il prend une description textuelle des entités et associations du modèle conceptuel de données ([MCD](https://fr.wikipedia.org/wiki/Modèle_entité-association)).
 - En sortie, il produit son diagramme entité-association en [SVG](https://fr.wikipedia.org/wiki/Scalable_Vector_Graphics) et son schéma relationnel ([MLD](
 https://fr.wikipedia.org/wiki/Merise_%28informatique%29#MLD_:_mod.C3.A8le_logique_des_donn.C3.A9es)) en [SQL](https://fr.wikipedia.org/wiki/Structured_Query_Language), [LaTeX](https://fr.wikipedia.org/wiki/LaTeX), [Markdown](https://fr.wikipedia.org/wiki/Markdown), etc.
 
-Ci-dessous, un exemple sous [Jupyter Notebook](https://jupyter.org). L'appel du programme se fait en première ligne, sur un texte d'entrée donné lignes suivantes.
+Ci-dessous, un exemple d'utilisation sous [Jupyter Notebook](https://jupyter.org). L'appel du programme est en première ligne, sur un texte d'entrée donné lignes suivantes. Le cas est adapté de l'article fondateur de Peter Chen, [_The entity-relationship model—toward a unified view of data_](https://doi.org/10.1145/320434.320440) (ACM Trans. Database Syst. 1, 1, March 1976, pp. 9–36), avec en bonus une association de type hiérarchique et une contrainte d'inclusion.
 
 ```
 %%mocodo --mld --colors brewer+1 --shapes copperplate --relations diagram markdown_data_dict
-DF, 11 Élève, 1N Classe
-Classe: Num. classe, Num. salle
-Faire Cours, 1N Classe, 1N Prof: Vol. horaire
-Catégorie: Code catégorie, Nom catégorie
-
-Élève: Num. élève, Nom élève
-Noter, 1N Élève, 0N Prof, 0N Matière, 1N Date: Note
-Prof: Num. prof, Nom prof
-Relever, 0N Catégorie, 11 Prof
-
-Date: Date
-Matière: Libellé matière
-Enseigner, 11 Prof, 1N Matière
+
+Ayant-droit: nom ayant-droit, lien
+Diriger, 0N Employé, 01 Projet
+Requérir, 1N Projet, 0N Pièce: qté requise
+Pièce: réf. pièce, libellé pièce
+Composer, 0N [composée] Pièce, 0N [composante] Pièce: quantité
+
+DF1, _11 Ayant-droit, 0N Employé
+Employé: matricule, nom employé
+Projet: num. projet, nom projet
+Fournir, 1N Projet, 1N Pièce, 1N Société: qté fournie
+
+Département: num. département, nom département
+Employer, 11 Employé, 1N Département
+Travailler, 0N Employé, 1N Projet
+Société: num. société, raison sociale
+Contrôler, 0N< [filiale] Société, 01 [mère] Société
+
+(I) --Fournir, ->Requérir, ..Pièce, Projet
 ```
 
 En sortie, le MCD (diagramme conceptuel) et le MLD (schéma relationnel) correspondants:
 
-![](https://cdn.rawgit.com/laowantong/mocodo/master/doc/readme_1.svg)
+![](https://cdn.rawgit.com/laowantong/mocodo/master/doc/readme_1.png)
 
-**Catégorie** (<ins>Code catégorie</ins>, Nom catégorie)<br>
-**Classe** (<ins>Num. classe</ins>, Num. salle)<br>
-**Faire Cours** (<ins>_#Num. classe_</ins>, <ins>_#Num. prof_</ins>, Vol. horaire)<br>
-**Noter** (<ins>_#Num. élève_</ins>, <ins>_#Num. prof_</ins>, <ins>_#Libellé matière_</ins>, <ins>_#Date_</ins>, Note)<br>
-**Prof** (<ins>Num. prof</ins>, Nom prof, _#Code catégorie_, _#Libellé matière_)<br>
-**Élève** (<ins>Num. élève</ins>, Nom élève, _#Num. classe_)
-
-L'appel ci-dessus a également construit le dictionnaire des données:
-
-- Num. classe
-- Num. salle
-- Vol. horaire
-- Code catégorie
-- Nom catégorie
-- Num. élève
-- Nom élève
-- Note
-- Num. prof
-- Nom prof
-- Date
-- Libellé matière
+**Ayant-droit** (<ins>_#matricule_</ins>, <ins>nom ayant-droit</ins>, lien)<br>
+**Composer** (<ins>_#réf. pièce composée_</ins>, <ins>_#réf. pièce composante_</ins>, quantité)<br>
+**Département** (<ins>num. département</ins>, nom département)<br>
+**Employé** (<ins>matricule</ins>, nom employé, _#num. département_)<br>
+**Fournir** (<ins>_#num. projet_</ins>, <ins>_#réf. pièce_</ins>, <ins>_#num. société_</ins>, qté fournie)<br>
+**Pièce** (<ins>réf. pièce</ins>, libellé pièce)<br>
+**Projet** (<ins>num. projet</ins>, nom projet, _#matricule_)<br>
+**Requérir** (<ins>_#num. projet_</ins>, <ins>_#réf. pièce_</ins>, qté requise)<br>
+**Société** (<ins>num. société</ins>, raison sociale, _#num. société mère_)<br>
+**Travailler** (<ins>_#matricule_</ins>, <ins>_#num. projet_</ins>)
+
+L'appel précédent a également créé un fichier `mocodo_notebook/sandbox_data_dict.md` contenant le dictionnaire des données :
+
+- nom ayant-droit
+- lien
+- quantité
+- num. département
+- nom département
+- matricule
+- nom employé
+- qté fournie
+- réf. pièce
+- libellé pièce
+- num. projet
+- nom projet
+- qté requise
+- num. société
+- raison sociale
 
 Ainsi que le diagramme relationnel, qui peut être visualisé par un nouvel appel:
 
 ```
 %mocodo --input mocodo_notebook/sandbox.mld --colors brewer+1
 ```
 
-![](https://cdn.rawgit.com/laowantong/mocodo/f06f70a/doc/readme_2.svg)
+![](https://cdn.rawgit.com/laowantong/mocodo/master/doc/readme_2.png)
 
 La devise de Mocodo, « nickel, ni souris », en résume les principaux points forts:
 
-- description textuelle des données. L'utilisateur n'a pas à renseigner, placer et déplacer des éléments comme avec une lessive ordinaire. Il ne fournit rien de plus que les informations définissant son MCD. L'outil s'occupe tout seul du plongement;
-- propreté du rendu. La sortie se fait en vectoriel, prête à être affichée, imprimée, agrandie, exportée dans une multitude de formats sans perte de qualité;
-- rapidité des retouches. L'utilisateur rectifie les alignements en insérant des éléments invisibles, en dupliquant des coordonnées ou en ajustant des facteurs mutiplicatifs: là encore, il travaille sur une description textuelle, et non directement sur le dessin.
+- description textuelle des données. L'utilisateur n'a pas à renseigner, placer et déplacer des éléments comme avec une lessive ordinaire. Il ne fournit rien de plus que les informations définissant son MCD. L'outil s'occupe tout seul du plongement ;
+- propreté du rendu. La sortie se fait en vectoriel, prête à être affichée, imprimée, agrandie, exportée dans une multitude de formats sans perte de qualité ;
+- rapidité des retouches. L'utilisateur rectifie les alignements en insérant des éléments invisibles, en dupliquant des coordonnées ou en ajustant des facteurs mutiplicatifs : là encore, il travaille sur une description textuelle, et non directement sur le dessin.
 
-Mocodo est libre, gratuit et multiplateforme. Si vous l'aimez, répandez la bonne nouvelle en incluant l'un de ses logos dans votre support: cela multipliera ses chances d'attirer des contributeurs qui le feront évoluer.
+Mocodo est libre, gratuit et multiplateforme. Si vous l'aimez, répandez la bonne nouvelle en incluant l'un de ses logos dans votre support : cela augmentera ses chances d'attirer des contributeurs qui le feront évoluer.
 
 Pour vous familiariser avec Mocodo, le mieux est d'utiliser [sa version en ligne](https://www.mocodo.net).
-
-Pour en savoir plus, lisez la documentation [au format HTML](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html) ou téléchargez-la [au format Jupyter Notebook](doc/fr_refman.ipynb).
-
```

