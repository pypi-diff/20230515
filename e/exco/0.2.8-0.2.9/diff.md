# Comparing `tmp/exco-0.2.8.tar.gz` & `tmp/exco-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/exco-0.2.8.tar", last modified: Wed Sep  7 10:11:44 2022, max compression
+gzip compressed data, was "exco-0.2.9.tar", last modified: Mon Jan 23 04:00:34 2023, max compression
```

## Comparing `exco-0.2.8.tar` & `exco-0.2.9.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/
--rw-r--r--   0 piti       (501) staff       (20)    15436 2022-09-07 10:11:44.000000 exco-0.2.8/PKG-INFO
--rw-r--r--   0 piti       (501) staff       (20)    12210 2022-09-07 10:10:25.000000 exco-0.2.8/README.md
--rw-r--r--   0 piti       (501) staff       (20)       92 2022-09-07 10:11:44.000000 exco-0.2.8/setup.cfg
--rw-r--r--   0 piti       (501) staff       (20)     1418 2020-12-04 17:40:35.000000 exco-0.2.8/setup.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/
--rw-r--r--   0 piti       (501) staff       (20)      689 2020-11-12 05:29:52.000000 exco-0.2.8/src/exco/__init__.py
--rw-r--r--   0 piti       (501) staff       (20)       18 2022-09-07 10:10:37.000000 exco-0.2.8/src/exco/__version__.py
--rw-r--r--   0 piti       (501) staff       (20)     1447 2020-12-02 20:18:26.000000 exco-0.2.8/src/exco/cell_full_path.py
--rw-r--r--   0 piti       (501) staff       (20)     3844 2022-08-26 03:51:31.000000 exco-0.2.8/src/exco/cell_location.py
--rw-r--r--   0 piti       (501) staff       (20)     2902 2020-12-04 17:40:35.000000 exco-0.2.8/src/exco/dereferator.py
--rw-r--r--   0 piti       (501) staff       (20)      296 2020-11-08 15:57:52.000000 exco-0.2.8/src/exco/excel_extraction_scope.py
--rw-r--r--   0 piti       (501) staff       (20)     1236 2020-12-02 21:11:37.000000 exco-0.2.8/src/exco/exception.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/exco_template/
--rw-r--r--   0 piti       (501) staff       (20)      114 2020-11-12 05:29:52.000000 exco-0.2.8/src/exco/exco_template/__init__.py
--rw-r--r--   0 piti       (501) staff       (20)     6844 2021-07-14 01:49:20.000000 exco-0.2.8/src/exco/exco_template/exco_block.py
--rw-r--r--   0 piti       (501) staff       (20)     8217 2020-12-04 17:40:35.000000 exco-0.2.8/src/exco/exco_template/exco_template.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/exco_watch/
--rw-r--r--   0 piti       (501) staff       (20)     2350 2021-07-14 03:52:28.000000 exco-0.2.8/src/exco/exco_watch/__init__.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/extractor/
--rw-r--r--   0 piti       (501) staff       (20)      329 2020-11-12 05:29:52.000000 exco-0.2.8/src/exco/extractor/__init__.py
--rw-r--r--   0 piti       (501) staff       (20)      220 2020-11-08 15:43:47.000000 exco-0.2.8/src/exco/extractor/actor.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/extractor/assumption/
--rw-r--r--   0 piti       (501) staff       (20)        0 2020-11-08 15:43:47.000000 exco-0.2.8/src/exco/extractor/assumption/__init__.py
--rw-r--r--   0 piti       (501) staff       (20)      371 2020-11-12 05:29:52.000000 exco-0.2.8/src/exco/extractor/assumption/assumption.py
--rw-r--r--   0 piti       (501) staff       (20)      817 2022-08-26 07:57:15.000000 exco-0.2.8/src/exco/extractor/assumption/assumption_factory.py
--rw-r--r--   0 piti       (501) staff       (20)      421 2020-11-08 15:43:47.000000 exco-0.2.8/src/exco/extractor/assumption/assumption_result.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/extractor/assumption/built_in/
--rw-r--r--   0 piti       (501) staff       (20)        0 2020-11-08 15:43:47.000000 exco-0.2.8/src/exco/extractor/assumption/built_in/__init__.py
--rw-r--r--   0 piti       (501) staff       (20)      609 2020-11-12 05:29:52.000000 exco-0.2.8/src/exco/extractor/assumption/built_in/left_cell_match_assumption.py
--rw-r--r--   0 piti       (501) staff       (20)     2905 2020-12-02 21:11:37.000000 exco-0.2.8/src/exco/extractor/base_factory.py
--rw-r--r--   0 piti       (501) staff       (20)     5627 2020-12-04 17:40:35.000000 exco-0.2.8/src/exco/extractor/cell_extraction_task.py
--rw-r--r--   0 piti       (501) staff       (20)    10667 2022-08-26 07:57:15.000000 exco-0.2.8/src/exco/extractor/excel_processor.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/extractor/locator/
--rw-r--r--   0 piti       (501) staff       (20)        0 2020-11-08 15:43:47.000000 exco-0.2.8/src/exco/extractor/locator/__init__.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/extractor/locator/built_in/
--rw-r--r--   0 piti       (501) staff       (20)        0 2020-11-08 15:43:47.000000 exco-0.2.8/src/exco/extractor/locator/built_in/__init__.py
--rw-r--r--   0 piti       (501) staff       (20)      432 2020-11-12 05:29:52.000000 exco-0.2.8/src/exco/extractor/locator/built_in/at_comment_cell_locator.py
--rw-r--r--   0 piti       (501) staff       (20)     1146 2022-08-26 03:51:31.000000 exco-0.2.8/src/exco/extractor/locator/built_in/below_of_locator.py
--rw-r--r--   0 piti       (501) staff       (20)     1195 2022-09-07 10:10:25.000000 exco-0.2.8/src/exco/extractor/locator/built_in/below_of_regex_locator.py
--rw-r--r--   0 piti       (501) staff       (20)     1124 2022-08-26 03:51:31.000000 exco-0.2.8/src/exco/extractor/locator/built_in/right_of_locator.py
--rw-r--r--   0 piti       (501) staff       (20)     1202 2022-09-07 10:10:25.000000 exco-0.2.8/src/exco/extractor/locator/built_in/right_of_regex_locator.py
--rw-r--r--   0 piti       (501) staff       (20)     1469 2022-08-26 03:51:31.000000 exco-0.2.8/src/exco/extractor/locator/built_in/search_below_of_locator.py
--rw-r--r--   0 piti       (501) staff       (20)     1451 2022-08-26 03:51:31.000000 exco-0.2.8/src/exco/extractor/locator/built_in/search_right_of_locator.py
--rw-r--r--   0 piti       (501) staff       (20)     2652 2022-09-07 10:10:25.000000 exco-0.2.8/src/exco/extractor/locator/built_in/within_locator.py
--rw-r--r--   0 piti       (501) staff       (20)      618 2020-11-12 05:29:52.000000 exco-0.2.8/src/exco/extractor/locator/locating_result.py
--rw-r--r--   0 piti       (501) staff       (20)      441 2020-11-12 05:29:52.000000 exco-0.2.8/src/exco/extractor/locator/locator.py
--rw-r--r--   0 piti       (501) staff       (20)     1566 2022-09-07 10:10:25.000000 exco-0.2.8/src/exco/extractor/locator/locator_factory.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/extractor/parser/
--rw-r--r--   0 piti       (501) staff       (20)        0 2020-11-08 15:43:47.000000 exco-0.2.8/src/exco/extractor/parser/__init__.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/extractor/parser/built_in/
--rw-r--r--   0 piti       (501) staff       (20)        0 2020-11-08 15:43:47.000000 exco-0.2.8/src/exco/extractor/parser/built_in/__init__.py
--rw-r--r--   0 piti       (501) staff       (20)      445 2020-11-08 18:12:28.000000 exco-0.2.8/src/exco/extractor/parser/built_in/date_parser.py
--rw-r--r--   0 piti       (501) staff       (20)      434 2020-11-10 02:31:13.000000 exco-0.2.8/src/exco/extractor/parser/built_in/float_parser.py
--rw-r--r--   0 piti       (501) staff       (20)      449 2020-11-10 02:05:22.000000 exco-0.2.8/src/exco/extractor/parser/built_in/int_parser.py
--rw-r--r--   0 piti       (501) staff       (20)     1199 2022-08-26 03:51:31.000000 exco-0.2.8/src/exco/extractor/parser/built_in/link_parser.py
--rw-r--r--   0 piti       (501) staff       (20)      263 2020-11-12 05:29:52.000000 exco-0.2.8/src/exco/extractor/parser/built_in/string_parser.py
--rw-r--r--   0 piti       (501) staff       (20)      817 2020-11-12 05:29:52.000000 exco-0.2.8/src/exco/extractor/parser/built_in/value_parser.py
--rw-r--r--   0 piti       (501) staff       (20)      422 2020-12-02 21:11:37.000000 exco-0.2.8/src/exco/extractor/parser/parser.py
--rw-r--r--   0 piti       (501) staff       (20)     1121 2022-08-26 07:57:15.000000 exco-0.2.8/src/exco/extractor/parser/parser_factory.py
--rw-r--r--   0 piti       (501) staff       (20)      706 2020-11-12 05:29:52.000000 exco-0.2.8/src/exco/extractor/parser/parsing_result.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/extractor/table_end_conditions/
--rw-r--r--   0 piti       (501) staff       (20)        0 2020-11-10 02:05:22.000000 exco-0.2.8/src/exco/extractor/table_end_conditions/__init__.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/extractor/table_end_conditions/built_in/
--rw-r--r--   0 piti       (501) staff       (20)        0 2020-11-10 02:05:22.000000 exco-0.2.8/src/exco/extractor/table_end_conditions/built_in/__init__.py
--rw-r--r--   0 piti       (501) staff       (20)      923 2020-11-10 08:26:44.000000 exco-0.2.8/src/exco/extractor/table_end_conditions/built_in/all_blank_table_end_condition.py
--rw-r--r--   0 piti       (501) staff       (20)      972 2022-08-26 03:51:31.000000 exco-0.2.8/src/exco/extractor/table_end_conditions/built_in/cell_value_table_end_condition.py
--rw-r--r--   0 piti       (501) staff       (20)      976 2020-11-10 08:26:44.000000 exco-0.2.8/src/exco/extractor/table_end_conditions/built_in/max_row_table_end_condition.py
--rw-r--r--   0 piti       (501) staff       (20)      568 2020-11-10 08:26:44.000000 exco-0.2.8/src/exco/extractor/table_end_conditions/table_end_condition.py
--rw-r--r--   0 piti       (501) staff       (20)     1564 2022-08-26 07:57:15.000000 exco-0.2.8/src/exco/extractor/table_end_conditions/table_end_condition_factory.py
--rw-r--r--   0 piti       (501) staff       (20)      356 2020-11-10 08:26:44.000000 exco-0.2.8/src/exco/extractor/table_end_conditions/table_end_condition_param.py
--rw-r--r--   0 piti       (501) staff       (20)     1615 2020-12-02 21:11:37.000000 exco-0.2.8/src/exco/extractor/table_end_conditions/table_end_condition_result.py
--rw-r--r--   0 piti       (501) staff       (20)     8345 2021-07-14 01:49:20.000000 exco-0.2.8/src/exco/extractor/table_extraction_task.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/extractor/validator/
--rw-r--r--   0 piti       (501) staff       (20)        0 2020-11-08 15:43:47.000000 exco-0.2.8/src/exco/extractor/validator/__init__.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/extractor/validator/built_in/
--rw-r--r--   0 piti       (501) staff       (20)        0 2020-11-08 15:43:47.000000 exco-0.2.8/src/exco/extractor/validator/built_in/__init__.py
--rw-r--r--   0 piti       (501) staff       (20)      286 2020-11-08 17:23:47.000000 exco-0.2.8/src/exco/extractor/validator/built_in/between_validator.py
--rw-r--r--   0 piti       (501) staff       (20)      243 2020-12-02 21:11:37.000000 exco-0.2.8/src/exco/extractor/validator/built_in/is_not_blank_validator.py
--rw-r--r--   0 piti       (501) staff       (20)      617 2020-11-12 05:29:52.000000 exco-0.2.8/src/exco/extractor/validator/built_in/value_validator.py
--rw-r--r--   0 piti       (501) staff       (20)      489 2020-11-08 15:43:47.000000 exco-0.2.8/src/exco/extractor/validator/validation_result.py
--rw-r--r--   0 piti       (501) staff       (20)      338 2020-11-08 15:58:42.000000 exco-0.2.8/src/exco/extractor/validator/validator.py
--rw-r--r--   0 piti       (501) staff       (20)      904 2022-08-26 07:57:15.000000 exco-0.2.8/src/exco/extractor/validator/validator_factory.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco/extractor_spec/
--rw-r--r--   0 piti       (501) staff       (20)      335 2020-11-12 05:29:52.000000 exco-0.2.8/src/exco/extractor_spec/__init__.py
--rw-r--r--   0 piti       (501) staff       (20)     2207 2020-12-04 17:40:35.000000 exco-0.2.8/src/exco/extractor_spec/apv_spec.py
--rw-r--r--   0 piti       (501) staff       (20)      940 2020-12-02 21:11:37.000000 exco-0.2.8/src/exco/extractor_spec/assumption_spec.py
--rw-r--r--   0 piti       (501) staff       (20)     2418 2020-12-02 21:11:37.000000 exco-0.2.8/src/exco/extractor_spec/cell_extraction_spec.py
--rw-r--r--   0 piti       (501) staff       (20)     4064 2020-12-02 21:11:37.000000 exco-0.2.8/src/exco/extractor_spec/excel_processor_spec.py
--rw-r--r--   0 piti       (501) staff       (20)      916 2020-12-02 21:11:37.000000 exco-0.2.8/src/exco/extractor_spec/locator_spec.py
--rw-r--r--   0 piti       (501) staff       (20)     1027 2020-12-02 21:11:37.000000 exco-0.2.8/src/exco/extractor_spec/parser_spec.py
--rw-r--r--   0 piti       (501) staff       (20)      363 2020-12-02 21:11:37.000000 exco-0.2.8/src/exco/extractor_spec/spec_source.py
--rw-r--r--   0 piti       (501) staff       (20)     4630 2020-12-04 17:40:35.000000 exco-0.2.8/src/exco/extractor_spec/table_extraction_spec.py
--rw-r--r--   0 piti       (501) staff       (20)      143 2020-11-10 02:05:22.000000 exco-0.2.8/src/exco/extractor_spec/type.py
--rw-r--r--   0 piti       (501) staff       (20)     1120 2020-12-02 21:11:37.000000 exco-0.2.8/src/exco/extractor_spec/validator_spec.py
--rw-r--r--   0 piti       (501) staff       (20)      756 2020-12-04 17:40:35.000000 exco-0.2.8/src/exco/setting.py
--rw-r--r--   0 piti       (501) staff       (20)      304 2022-08-26 03:51:31.000000 exco-0.2.8/src/exco/sheet_name_alias.py
--rw-r--r--   0 piti       (501) staff       (20)     2200 2022-08-26 07:57:15.000000 exco-0.2.8/src/exco/shortcut.py
--rw-r--r--   0 piti       (501) staff       (20)     8001 2022-09-07 10:10:25.000000 exco-0.2.8/src/exco/util.py
-drwxr-xr-x   0 piti       (501) staff       (20)        0 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco.egg-info/
--rw-r--r--   0 piti       (501) staff       (20)    15436 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco.egg-info/PKG-INFO
--rw-r--r--   0 piti       (501) staff       (20)     3895 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco.egg-info/SOURCES.txt
--rw-r--r--   0 piti       (501) staff       (20)        1 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco.egg-info/dependency_links.txt
--rw-r--r--   0 piti       (501) staff       (20)       70 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco.egg-info/entry_points.txt
--rw-r--r--   0 piti       (501) staff       (20)        1 2020-11-08 15:50:23.000000 exco-0.2.8/src/exco.egg-info/not-zip-safe
--rw-r--r--   0 piti       (501) staff       (20)      131 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco.egg-info/requires.txt
--rw-r--r--   0 piti       (501) staff       (20)        5 2022-09-07 10:11:44.000000 exco-0.2.8/src/exco.egg-info/top_level.txt
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.120519 exco-0.2.9/
+-rw-r--r--   0 piti       (501) staff       (20)     1085 2022-08-17 10:32:40.000000 exco-0.2.9/LICENSE
+-rw-r--r--   0 piti       (501) staff       (20)    12821 2023-01-23 04:00:34.120594 exco-0.2.9/PKG-INFO
+-rw-r--r--   0 piti       (501) staff       (20)    12499 2023-01-23 03:58:34.000000 exco-0.2.9/README.md
+-rw-r--r--   0 piti       (501) staff       (20)       92 2023-01-23 04:00:34.120859 exco-0.2.9/setup.cfg
+-rw-r--r--   0 piti       (501) staff       (20)     1418 2022-08-17 10:32:40.000000 exco-0.2.9/setup.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.105747 exco-0.2.9/src/
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.109489 exco-0.2.9/src/exco/
+-rw-r--r--   0 piti       (501) staff       (20)      689 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/__init__.py
+-rw-r--r--   0 piti       (501) staff       (20)       18 2023-01-23 03:58:34.000000 exco-0.2.9/src/exco/__version__.py
+-rw-r--r--   0 piti       (501) staff       (20)     1447 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/cell_full_path.py
+-rw-r--r--   0 piti       (501) staff       (20)     3844 2022-08-25 09:33:36.000000 exco-0.2.9/src/exco/cell_location.py
+-rw-r--r--   0 piti       (501) staff       (20)     2902 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/dereferator.py
+-rw-r--r--   0 piti       (501) staff       (20)      296 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/excel_extraction_scope.py
+-rw-r--r--   0 piti       (501) staff       (20)     1236 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/exception.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.111117 exco-0.2.9/src/exco/exco_template/
+-rw-r--r--   0 piti       (501) staff       (20)      114 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/exco_template/__init__.py
+-rw-r--r--   0 piti       (501) staff       (20)     6844 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/exco_template/exco_block.py
+-rw-r--r--   0 piti       (501) staff       (20)     8217 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/exco_template/exco_template.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.111273 exco-0.2.9/src/exco/exco_watch/
+-rw-r--r--   0 piti       (501) staff       (20)     2350 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/exco_watch/__init__.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.112233 exco-0.2.9/src/exco/extractor/
+-rw-r--r--   0 piti       (501) staff       (20)      329 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/__init__.py
+-rw-r--r--   0 piti       (501) staff       (20)      220 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/actor.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.112824 exco-0.2.9/src/exco/extractor/assumption/
+-rw-r--r--   0 piti       (501) staff       (20)        0 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/assumption/__init__.py
+-rw-r--r--   0 piti       (501) staff       (20)      371 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/assumption/assumption.py
+-rw-r--r--   0 piti       (501) staff       (20)      817 2023-01-23 03:58:34.000000 exco-0.2.9/src/exco/extractor/assumption/assumption_factory.py
+-rw-r--r--   0 piti       (501) staff       (20)      421 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/assumption/assumption_result.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.113052 exco-0.2.9/src/exco/extractor/assumption/built_in/
+-rw-r--r--   0 piti       (501) staff       (20)        0 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/assumption/built_in/__init__.py
+-rw-r--r--   0 piti       (501) staff       (20)      609 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/assumption/built_in/left_cell_match_assumption.py
+-rw-r--r--   0 piti       (501) staff       (20)     2905 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/base_factory.py
+-rw-r--r--   0 piti       (501) staff       (20)     5627 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/cell_extraction_task.py
+-rw-r--r--   0 piti       (501) staff       (20)    12062 2023-01-23 03:58:34.000000 exco-0.2.9/src/exco/extractor/excel_processor.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.113796 exco-0.2.9/src/exco/extractor/locator/
+-rw-r--r--   0 piti       (501) staff       (20)        0 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/locator/__init__.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.115109 exco-0.2.9/src/exco/extractor/locator/built_in/
+-rw-r--r--   0 piti       (501) staff       (20)        0 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/locator/built_in/__init__.py
+-rw-r--r--   0 piti       (501) staff       (20)      432 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/locator/built_in/at_comment_cell_locator.py
+-rw-r--r--   0 piti       (501) staff       (20)     1146 2022-08-25 09:33:36.000000 exco-0.2.9/src/exco/extractor/locator/built_in/below_of_locator.py
+-rw-r--r--   0 piti       (501) staff       (20)     1196 2023-01-23 03:58:34.000000 exco-0.2.9/src/exco/extractor/locator/built_in/below_of_regex_locator.py
+-rw-r--r--   0 piti       (501) staff       (20)     1124 2022-08-25 09:33:36.000000 exco-0.2.9/src/exco/extractor/locator/built_in/right_of_locator.py
+-rw-r--r--   0 piti       (501) staff       (20)     1202 2023-01-23 03:58:34.000000 exco-0.2.9/src/exco/extractor/locator/built_in/right_of_regex_locator.py
+-rw-r--r--   0 piti       (501) staff       (20)     1469 2022-08-25 09:33:36.000000 exco-0.2.9/src/exco/extractor/locator/built_in/search_below_of_locator.py
+-rw-r--r--   0 piti       (501) staff       (20)     1451 2022-08-25 09:33:36.000000 exco-0.2.9/src/exco/extractor/locator/built_in/search_right_of_locator.py
+-rw-r--r--   0 piti       (501) staff       (20)     2652 2023-01-23 03:58:34.000000 exco-0.2.9/src/exco/extractor/locator/built_in/within_locator.py
+-rw-r--r--   0 piti       (501) staff       (20)      618 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/locator/locating_result.py
+-rw-r--r--   0 piti       (501) staff       (20)      441 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/locator/locator.py
+-rw-r--r--   0 piti       (501) staff       (20)     1566 2023-01-23 03:58:34.000000 exco-0.2.9/src/exco/extractor/locator/locator_factory.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.115713 exco-0.2.9/src/exco/extractor/parser/
+-rw-r--r--   0 piti       (501) staff       (20)        0 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/parser/__init__.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.116725 exco-0.2.9/src/exco/extractor/parser/built_in/
+-rw-r--r--   0 piti       (501) staff       (20)        0 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/parser/built_in/__init__.py
+-rw-r--r--   0 piti       (501) staff       (20)      445 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/parser/built_in/date_parser.py
+-rw-r--r--   0 piti       (501) staff       (20)      434 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/parser/built_in/float_parser.py
+-rw-r--r--   0 piti       (501) staff       (20)      449 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/parser/built_in/int_parser.py
+-rw-r--r--   0 piti       (501) staff       (20)     1199 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/parser/built_in/link_parser.py
+-rw-r--r--   0 piti       (501) staff       (20)      263 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/parser/built_in/string_parser.py
+-rw-r--r--   0 piti       (501) staff       (20)      817 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/parser/built_in/value_parser.py
+-rw-r--r--   0 piti       (501) staff       (20)      422 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/parser/parser.py
+-rw-r--r--   0 piti       (501) staff       (20)     1121 2023-01-23 03:58:34.000000 exco-0.2.9/src/exco/extractor/parser/parser_factory.py
+-rw-r--r--   0 piti       (501) staff       (20)      706 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/parser/parsing_result.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.117335 exco-0.2.9/src/exco/extractor/table_end_conditions/
+-rw-r--r--   0 piti       (501) staff       (20)        0 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/table_end_conditions/__init__.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.117832 exco-0.2.9/src/exco/extractor/table_end_conditions/built_in/
+-rw-r--r--   0 piti       (501) staff       (20)        0 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/table_end_conditions/built_in/__init__.py
+-rw-r--r--   0 piti       (501) staff       (20)      923 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/table_end_conditions/built_in/all_blank_table_end_condition.py
+-rw-r--r--   0 piti       (501) staff       (20)      972 2022-08-25 09:33:36.000000 exco-0.2.9/src/exco/extractor/table_end_conditions/built_in/cell_value_table_end_condition.py
+-rw-r--r--   0 piti       (501) staff       (20)      976 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/table_end_conditions/built_in/max_row_table_end_condition.py
+-rw-r--r--   0 piti       (501) staff       (20)      568 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/table_end_conditions/table_end_condition.py
+-rw-r--r--   0 piti       (501) staff       (20)     1564 2023-01-23 03:58:34.000000 exco-0.2.9/src/exco/extractor/table_end_conditions/table_end_condition_factory.py
+-rw-r--r--   0 piti       (501) staff       (20)      356 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/table_end_conditions/table_end_condition_param.py
+-rw-r--r--   0 piti       (501) staff       (20)     1615 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/table_end_conditions/table_end_condition_result.py
+-rw-r--r--   0 piti       (501) staff       (20)     8345 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/table_extraction_task.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.118306 exco-0.2.9/src/exco/extractor/validator/
+-rw-r--r--   0 piti       (501) staff       (20)        0 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/validator/__init__.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.118776 exco-0.2.9/src/exco/extractor/validator/built_in/
+-rw-r--r--   0 piti       (501) staff       (20)        0 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/validator/built_in/__init__.py
+-rw-r--r--   0 piti       (501) staff       (20)      286 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/validator/built_in/between_validator.py
+-rw-r--r--   0 piti       (501) staff       (20)      243 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/validator/built_in/is_not_blank_validator.py
+-rw-r--r--   0 piti       (501) staff       (20)      617 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/validator/built_in/value_validator.py
+-rw-r--r--   0 piti       (501) staff       (20)      489 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/validator/validation_result.py
+-rw-r--r--   0 piti       (501) staff       (20)      338 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor/validator/validator.py
+-rw-r--r--   0 piti       (501) staff       (20)      904 2023-01-23 03:58:34.000000 exco-0.2.9/src/exco/extractor/validator/validator_factory.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.120393 exco-0.2.9/src/exco/extractor_spec/
+-rw-r--r--   0 piti       (501) staff       (20)      335 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor_spec/__init__.py
+-rw-r--r--   0 piti       (501) staff       (20)     2207 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor_spec/apv_spec.py
+-rw-r--r--   0 piti       (501) staff       (20)      940 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor_spec/assumption_spec.py
+-rw-r--r--   0 piti       (501) staff       (20)     2418 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor_spec/cell_extraction_spec.py
+-rw-r--r--   0 piti       (501) staff       (20)     4064 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor_spec/excel_processor_spec.py
+-rw-r--r--   0 piti       (501) staff       (20)      916 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor_spec/locator_spec.py
+-rw-r--r--   0 piti       (501) staff       (20)     1027 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor_spec/parser_spec.py
+-rw-r--r--   0 piti       (501) staff       (20)      363 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor_spec/spec_source.py
+-rw-r--r--   0 piti       (501) staff       (20)     4630 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor_spec/table_extraction_spec.py
+-rw-r--r--   0 piti       (501) staff       (20)      143 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor_spec/type.py
+-rw-r--r--   0 piti       (501) staff       (20)     1120 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/extractor_spec/validator_spec.py
+-rw-r--r--   0 piti       (501) staff       (20)      756 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/setting.py
+-rw-r--r--   0 piti       (501) staff       (20)      304 2022-08-17 10:32:40.000000 exco-0.2.9/src/exco/sheet_name_alias.py
+-rw-r--r--   0 piti       (501) staff       (20)     2506 2023-01-23 03:58:34.000000 exco-0.2.9/src/exco/shortcut.py
+-rw-r--r--   0 piti       (501) staff       (20)     8001 2023-01-23 03:58:34.000000 exco-0.2.9/src/exco/util.py
+drwxr-xr-x   0 piti       (501) staff       (20)        0 2023-01-23 04:00:34.110630 exco-0.2.9/src/exco.egg-info/
+-rw-r--r--   0 piti       (501) staff       (20)    12821 2023-01-23 04:00:34.000000 exco-0.2.9/src/exco.egg-info/PKG-INFO
+-rw-r--r--   0 piti       (501) staff       (20)     3903 2023-01-23 04:00:34.000000 exco-0.2.9/src/exco.egg-info/SOURCES.txt
+-rw-r--r--   0 piti       (501) staff       (20)        1 2023-01-23 04:00:34.000000 exco-0.2.9/src/exco.egg-info/dependency_links.txt
+-rw-r--r--   0 piti       (501) staff       (20)       69 2023-01-23 04:00:34.000000 exco-0.2.9/src/exco.egg-info/entry_points.txt
+-rw-r--r--   0 piti       (501) staff       (20)        1 2022-08-17 10:33:14.000000 exco-0.2.9/src/exco.egg-info/not-zip-safe
+-rw-r--r--   0 piti       (501) staff       (20)      131 2023-01-23 04:00:34.000000 exco-0.2.9/src/exco.egg-info/requires.txt
+-rw-r--r--   0 piti       (501) staff       (20)        5 2023-01-23 04:00:34.000000 exco-0.2.9/src/exco.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `exco-0.2.8/PKG-INFO` & `exco-0.2.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,376 +1,384 @@
 Metadata-Version: 2.1
 Name: exco
-Version: 0.2.8
+Version: 0.2.9
 Summary: Excel Comment Orm
 Home-page: https://github.com/thegangtechnology/exco
 Author: Piti Ongmongkolkul
 Author-email: piti118@gmail.com
 License: Private
-Description: # Exco
-        
-        [![Build](https://github.com/thegangtechnology/exco/workflows/Build/badge.svg)](https://github.com/thegangtechnology/exco/actions?query=workflow%3ABuild)
-        [![Sonarqube](https://github.com/thegangtechnology/exco/workflows/Sonarqube/badge.svg)](https://github.com/thegangtechnology/exco/actions?query=workflow%3ASonarqube)
-        [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=thegangtechnology_exco&metric=alert_status)](https://sonarcloud.io/dashboard?id=thegangtechnology_exco)
-        [![CodeQL](https://github.com/thegangtechnology/exco/workflows/CodeQL/badge.svg)](https://github.com/thegangtechnology/exco/actions?query=workflow%3ACodeQL)
-        [![codecov](https://codecov.io/gh/thegangtechnology/exco/branch/master/graph/badge.svg?token=8BrjxREw2O)](https://codecov.io/gh/thegangtechnology/exco)
-        [![PyPI version](https://badge.fury.io/py/exco.svg)](https://badge.fury.io/py/exco)
-        
-        Excel Comment ORM. Declare ORM Spec descriptively right on the excel file.
-        
-        # What it does
-        
-        The package allows you to declare orm mapping right in the excel file in the comments
-         then use it to extract data from other similar files.
-         
-        An example of a template is shown below.
-        
-        ![Template](notebooks/quickstart/template.png)
-        
-        Dynamic Location, Validation, Assumptions, custom Parser are also supported.
-        
-        
-        # Installation
-        
-        ```
-        pip install exco
-        ```
-        
-        # Simple Usage
-        
-        ```
-        import exco
-        processor = exco.from_excel('./quickstart_template.xlsx')
-        result = processor.process_excel('./quickstart_data_file.xlsx')
-        print(result.to_dict())
-        ```
-        
-        See Also [Quick Start Notebook](notebooks/quickstart/0%20Quick%20Start.ipynb)
-        
-        # Exco Block
-        
-        Exco relies on yml blocks inside excel comment to build a spec.
-        Each comment can contain multiple blocks.
-        There are three types of echo block: a cell block, a table block, and a column block.
-        
-        ## Cell Block
-        
-        A cellblock is a block of yml that is surrounded by `{{--` and `--}}`
-        ```
-        {{--
-        key: some_int
-        parser: int
-        --}}
-        ```
-        
-        This means that parse this cell as `int` and put it in the result with key `some_int`.
-        
-        
-        
-        Other advance features like, fallback, locator, assumptions, validator are optional.
-        The full specification is shown below.
-        
-        ```
-        {{--
-        key: some_value
-        # Optional default at_comment_cell
-        locator: {name: at_comment_cell} 
-        assumptions: # Optional
-            - {key: right_of, name: right_of, label: marker}
-        parser: int
-        # Optional
-        fallback: 7 
-        # Optional. Dict[name, value].
-        params: {} 
-        validators: # Optional
-            - {key: between, name: between, low: 5, high: 10 }
-        metadata: {unit: km}
-        --}}
-        ```
-        
-        ### Processing Flow.
-        
-        The cell processing flow is
-        
-        1. Locating the Cell
-        2. Check Assumption
-        3. Parse
-        4. Validation
-        
-        ### Features
-        
-        #### `key`
-        Key where the result will be put. This is required.
-        
-        #### `fallback`
-        
-        This is the most useful one where if the cell is failed locating, testing assumption, parsing.
-        The fallback value is assumed. If it is not specified, the value None is used. (yml's none is `null`).
-        
-        #### `locator`
-        Locator is a dictionary. The key `name` is the class name to be used to locate the cell. Other parameters
-        can be flattened and put in the same dictionary. These parameters will be pass through the constructor
-        of such class.
-        
-        If the locator is left out, it is assumed to be `at_comment_cell` which locate the cell with exactly
-        the same coordinate as the commented cell in the template.
-        
-        #### `assumptions`
-        List of dictionaries. The `key` is the name of the check. `name` is the name of the class to be used in
-        testing an assumption. Other parameters can be flattened and included in the same dictionary.
-        
-        #### `parser`
-        Required. Name of the parser class.
-        
-        #### `params`
-        Optional. Dictionary of the parameter name to its value. The spread values are passed through the parser
-        constructor.
-        
-        #### `validations`
-        Optional. List of Dictionary. Each dictionary must have `key` for the validation key and `name`,
-        validator's class name, specified. Other parameters to be passed to the validator constructor can be flattened and specified in this dictionary as well.
-        
-        ### `metadata`
-        Optional. Metadata. Dictionary of any object can be put here. The object will be parsed on to the result.
-        
-        ## Table Block
-        A table block is for specifying the properties of the table. The table block is surrounded by
-        `{{--table` and `--}}`. The simplest table block is
-        ```
-        {{--table
-        key: some_table
-        --}}
-        ```
-        This is typically what you need. A more complicated example is shown below:
-        
-        ```
-        {{--table
-        key: some_table
-        # optional. default at_comment_cell
-        locator: {name: at_comment_cell}
-        # optional. default downward
-        item_direction: downward
-        end_conditions:
-            - {name: all_blank}
-            - {name: max_row, n: 10, inclusive: true}
-        --}}
-        ```
-        ### Features
-        #### `key`
-        where the table will be put in the result. The output for the table is a list of dictionaries
-        where the key in the dictionaries is the column name specified in column blocks.
-        
-        #### `locator`
-        Optional. Default at_comment_cell. Locator for the table anchor cell. Same as a cell block.
-        
-        #### `item_direction`
-        Optional Direction for items in the table. Default downward. (rightward or downward)
-        
-        #### `end_conditions`
-        A list of dictionary specifying each termination condition. The dictionary contains `name` and flattened
-        parameters.
-        
-        If any of the end condition is met then the parsing for the table terminates. Depending on the end condition's
-        class, it may or may not include the matching row.
-        
-        ## Column Block
-        
-        Column block specifications are very similar to the cell block. The simplest example is shown below.
-        ```
-        {{--col
-        table_key: some_table
-        key: some_col
-        parser: int
-        }}
-        ```
-        The column block is very similar to the cell block. It is the cell block with `table_key` and without
-        `locator`. The `table_key` tells which table it belongs to. It must match one of the table's `key` defined in the table block.
-        
-        The position of the column cell when extracting value is computed from the relative position to the table
-         block in the template.
-         
-         All other features like fallback, assumptions, validations are also supported in the same
-         fashion as the cell block.
-        
-        # Built-in Functions
-        
-        ## Locator
-        ### `at_comment_cell`
-        Locate the cell right at the comment cell's coordinate in the template.
-        
-        ### `right_of`
-        Locate the cell to the right of the cell or merged cell with the given label.
-        In the case of a merged cell, right_of will pick the rightmost column and 
-        topmost row of the merged cell togo to the right of.
-        
-        Parameters:
-        - `label` label to match.
-        - `n` Optional. Default value is 1. Indicates the number of columns to move from label cell to located cell.
-        
-        ### `search_right_of`
-        Searches for non-empty cell right of the cell with the given value.
-        
-        Parameters:
-        - `label` label to match.
-        - `max_empty_col_search` Indicates the maximum number of columns to search for non-empty cell right of label.
-        ### `right_of_regex`
-        Locate the cell to the right of the cell with a regex match.
-        Similarly, in the case of a merged cell, right_of_regex will 
-        pick the rightmost column and topmost row of the merged cell 
-        togo to the right of.
-        
-        Parameters:
-        - `regex` string for the regular expression.
-        - `n` Optional. Default value is 1. Indicates the number of columns to move from regex matched cell to located cell.
-        
-        ### `below_of`
-        Locate the cell below of the cell with the given label.
-        In the case of a merged cell, below_of will pick the 
-        bottommost row and leftmost column of the merged cell togo 
-        to the bottom of.
-        
-        Parameters:
-        - `label` label to match.
-        - `n` Optional. Default value is 1. Indicates the number of rows to skip from label cell to located cell.
-        
-        ### `search_below_of`
-        Searches for non-empty cell below of the cell with the given label.
-        
-        Parameters:
-        - `label` label to match.
-        - `max_empty_row_search` Indicates the maximum number of rows to search for non-empty cell below of label.
-        
-        ### `below_of_regex`
-        Locate the cell below of the cell with a regex match.
-        Similarly, in the case of a merged cell, below_of_regex will 
-        pick the bottommost row and leftmost row of the merged cell 
-        togo to the bottom of.
-        
-        Parameters:
-        - `regex` string for the regular expression.
-        - `n` Optional. Default value is 1. Indicates the number of rows to move from regex matched cell to located cell.
-        
-        
-        ### `within`
-        Locate the cell between a cell with the given label.
-        This function searches to the right of or below of the
-        cell with the given label. If it is to the right of, the function
-        searches row by row while staying in between the column ranges
-        of the cell with the given label. If it is below of, similarly,
-        we search row by row while staying in between the row ranges of
-        the cell with the given label. On top of this you have the option
-        on how to pick your data (to the right of or beneath of) once you have found your desired key within
-        the cell range.
-        
-        Parameters:
-        - `label` label of cell you want to search in between
-        - `find` the name of the cell you want to find in between the cell with that label's range
-        - `direction` direction you want to search for your value, choices are:
-          - `right_of` this will search the right of the cell between the columns row wise
-          - `below_of` this will search the beneath the cell between the rows row wise
-        - `perform` the action you want to perform to fetch your data, your options are:
-          - `right_of` fetch the value to the right of the cell labeled in `find`
-          - `below_of` fetch the value to beneath of the cell labeled in `find`
-        - `n` pick the value n values away in the specified perform direction (right_of or below_of)
-        
-        
-        ## Assumption
-        
-        ### `left_cell_match`
-        This is useful in batch processing allowing us to check that we have the correct label to the left.
-        
-        Parameters:
-        
-        - `label` string to check that it matches.
-        
-        ## Parser
-        ### `string`
-        parse value as string.
-        
-        ### `int`
-        parse the value as an integer. 
-        
-        ### `float`
-        parse the value as float
-        
-        ### `date`
-        parser the value as a date.
-        
-        ## Validator
-        
-        ### `between`
-        valid if the value is between(inclusively) `high` and `low`
-        
-        #### Parameters
-        
-        - `high` upper bound value.
-        - `low` lower bound value
-        
-        ## TableEndCondition
-        
-        ### `all_blank`
-        Evaluate to true if all columns are blank.
-        
-        ### `max_row`
-        Evaluate to true if the row number(start from 1) including the parsing row is greater than or
-        equal to `n`.
-        
-        #### Parameters
-        - `n` number of row
-        - `inclusive` Optional. Default True. Whether to include the row in which it evaluates to true.
-        
-        ### `cell_value`
-        Evaluate to true if any column in row contains matching `cell_value`. Table terminates the row before.
-        
-        #### Parameters
-        - `cell_value` cell value to match.
-        # Dereferencing
-        There are two types of dereferencing
-        - Spec Creation time dereferencing. The string similar to ``<<A1>>`` will be resolved 
-        to the value at A1 of the template file.
-        - Extraction time dereferencing. This string similar to ``==A1==`` will be resolved
-        to the value at A1 of the extracted file.
-        
-        Here is an example
-        ```
-        {{--
-        key: ==D2==
-        assumptions: # Optional
-            - {key: right_of, name: right_of, label: <<A1>>}
-        parser: int
-        fallback: ==D3== 
-        --}}
-        ```
-        
-        # Handle Identical Sheet with Different Names
-        
-        When an excel file to be extracted has a different sheet name than the one in the template file,
-        use ``sheet_name_checkers`` parameter in ``exco.from_excel()`` to create ``ExcelProcessor`` 
-        with sheet name alias checker.
-        
-        For example, when the sheet name in the template file is 'Test 1/1/2021', 
-        but sheet names can be varied in the extracting files, i.e., 'Test 2/2/2022, 'Test 3/3/2023', etc.
-        ```
-        import exco
-        
-        SheetName = str
-        SheetNameAliasChecker = Callable[[SheetName], bool]
-        test_sheet_checker: SheetNameAliasChecker = lambda sheetname: 'Test' in sheetname
-        checkers: Dict[SheetName, SheetNameAliasChecker] = {'Test 1/1/2021': test_sheet_checker}
-        processor = exco.from_excel(template_excel_path, sheet_name_checkers=checkers)
-        ```
-        
-        # Custom Locator/Parser Etc.
-        
-        See [Advance Features Notebook](notebooks/quickstart/1%20Advance%20Features.ipynb). But, in essence,
-        ```python
-        processor = exco.from_excel('./custom_locator/custom_locator_template.xlsx',
-                                    extra_locators={'diagonal_of': DiagonalOfLocator})
-        ```
-        # Working with .xls files.
-        
-        Exco will not read Excel 97-2003 workbook (.xls) files. Use [XLS2XLSX](https://pypi.org/project/xls2xlsx/) to convert .xls files to the supported .xlsx format.
-Platform: UNKNOWN
 Classifier: 
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+# Exco
+
+[![Build](https://github.com/thegangtechnology/exco/workflows/Build/badge.svg)](https://github.com/thegangtechnology/exco/actions?query=workflow%3ABuild)
+[![Sonarqube](https://github.com/thegangtechnology/exco/workflows/Sonarqube/badge.svg)](https://github.com/thegangtechnology/exco/actions?query=workflow%3ASonarqube)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=thegangtechnology_exco&metric=alert_status)](https://sonarcloud.io/dashboard?id=thegangtechnology_exco)
+[![CodeQL](https://github.com/thegangtechnology/exco/workflows/CodeQL/badge.svg)](https://github.com/thegangtechnology/exco/actions?query=workflow%3ACodeQL)
+[![codecov](https://codecov.io/gh/thegangtechnology/exco/branch/master/graph/badge.svg?token=8BrjxREw2O)](https://codecov.io/gh/thegangtechnology/exco)
+[![PyPI version](https://badge.fury.io/py/exco.svg)](https://badge.fury.io/py/exco)
+
+Excel Comment ORM. Declare ORM Spec descriptively right on the excel file.
+
+# What it does
+
+The package allows you to declare orm mapping right in the excel file in the comments
+ then use it to extract data from other similar files.
+ 
+An example of a template is shown below.
+
+![Template](notebooks/quickstart/template.png)
+
+Dynamic Location, Validation, Assumptions, custom Parser are also supported.
+
+
+# Installation
+
+```
+pip install exco
+```
+
+# Simple Usage
+
+```
+import exco
+processor = exco.from_excel('./quickstart_template.xlsx')
+result = processor.process_excel('./quickstart_data_file.xlsx')
+print(result.to_dict())
+```
+
+See Also [Quick Start Notebook](notebooks/quickstart/0%20Quick%20Start.ipynb)
+
+# Exco Block
+
+Exco relies on yml blocks inside excel comment to build a spec.
+Each comment can contain multiple blocks.
+There are three types of echo block: a cell block, a table block, and a column block.
+
+## Cell Block
+
+A cellblock is a block of yml that is surrounded by `{{--` and `--}}`
+```
+{{--
+key: some_int
+parser: int
+--}}
+```
+
+This means that parse this cell as `int` and put it in the result with key `some_int`.
+
+
+
+Other advance features like, fallback, locator, assumptions, validator are optional.
+The full specification is shown below.
+
+```
+{{--
+key: some_value
+# Optional default at_comment_cell
+locator: {name: at_comment_cell} 
+assumptions: # Optional
+    - {key: right_of, name: right_of, label: marker}
+parser: int
+# Optional
+fallback: 7 
+# Optional. Dict[name, value].
+params: {} 
+validators: # Optional
+    - {key: between, name: between, low: 5, high: 10 }
+metadata: {unit: km}
+--}}
+```
+
+### Processing Flow.
+
+The cell processing flow is
+
+1. Locating the Cell
+2. Check Assumption
+3. Parse
+4. Validation
+
+### Features
+
+#### `key`
+Key where the result will be put. This is required.
+
+#### `fallback`
+
+This is the most useful one where if the cell is failed locating, testing assumption, parsing.
+The fallback value is assumed. If it is not specified, the value None is used. (yml's none is `null`).
+
+#### `locator`
+Locator is a dictionary. The key `name` is the class name to be used to locate the cell. Other parameters
+can be flattened and put in the same dictionary. These parameters will be pass through the constructor
+of such class.
+
+If the locator is left out, it is assumed to be `at_comment_cell` which locate the cell with exactly
+the same coordinate as the commented cell in the template.
+
+#### `assumptions`
+List of dictionaries. The `key` is the name of the check. `name` is the name of the class to be used in
+testing an assumption. Other parameters can be flattened and included in the same dictionary.
+
+#### `parser`
+Required. Name of the parser class.
+
+#### `params`
+Optional. Dictionary of the parameter name to its value. The spread values are passed through the parser
+constructor.
+
+#### `validations`
+Optional. List of Dictionary. Each dictionary must have `key` for the validation key and `name`,
+validator's class name, specified. Other parameters to be passed to the validator constructor can be flattened and specified in this dictionary as well.
+
+### `metadata`
+Optional. Metadata. Dictionary of any object can be put here. The object will be parsed on to the result.
+
+## Table Block
+A table block is for specifying the properties of the table. The table block is surrounded by
+`{{--table` and `--}}`. The simplest table block is
+```
+{{--table
+key: some_table
+--}}
+```
+This is typically what you need. A more complicated example is shown below:
+
+```
+{{--table
+key: some_table
+# optional. default at_comment_cell
+locator: {name: at_comment_cell}
+# optional. default downward
+item_direction: downward
+end_conditions:
+    - {name: all_blank}
+    - {name: max_row, n: 10, inclusive: true}
+--}}
+```
+### Features
+#### `key`
+where the table will be put in the result. The output for the table is a list of dictionaries
+where the key in the dictionaries is the column name specified in column blocks.
+
+#### `locator`
+Optional. Default at_comment_cell. Locator for the table anchor cell. Same as a cell block.
+
+#### `item_direction`
+Optional Direction for items in the table. Default downward. (rightward or downward)
+
+#### `end_conditions`
+A list of dictionary specifying each termination condition. The dictionary contains `name` and flattened
+parameters.
+
+If any of the end condition is met then the parsing for the table terminates. Depending on the end condition's
+class, it may or may not include the matching row.
+
+## Column Block
+
+Column block specifications are very similar to the cell block. The simplest example is shown below.
+```
+{{--col
+table_key: some_table
+key: some_col
+parser: int
+}}
+```
+The column block is very similar to the cell block. It is the cell block with `table_key` and without
+`locator`. The `table_key` tells which table it belongs to. It must match one of the table's `key` defined in the table block.
+
+The position of the column cell when extracting value is computed from the relative position to the table
+ block in the template.
+ 
+ All other features like fallback, assumptions, validations are also supported in the same
+ fashion as the cell block.
+
+# Built-in Functions
+
+## Locator
+### `at_comment_cell`
+Locate the cell right at the comment cell's coordinate in the template.
+
+### `right_of`
+Locate the cell to the right of the cell or merged cell with the given label.
+In the case of a merged cell, right_of will pick the rightmost column and 
+topmost row of the merged cell togo to the right of.
+
+Parameters:
+- `label` label to match.
+- `n` Optional. Default value is 1. Indicates the number of columns to move from label cell to located cell.
+
+### `search_right_of`
+Searches for non-empty cell right of the cell with the given value.
+
+Parameters:
+- `label` label to match.
+- `max_empty_col_search` Indicates the maximum number of columns to search for non-empty cell right of label.
+### `right_of_regex`
+Locate the cell to the right of the cell with a regex match.
+Similarly, in the case of a merged cell, right_of_regex will 
+pick the rightmost column and topmost row of the merged cell 
+togo to the right of.
+
+Parameters:
+- `regex` string for the regular expression.
+- `n` Optional. Default value is 1. Indicates the number of columns to move from regex matched cell to located cell.
+
+### `below_of`
+Locate the cell below of the cell with the given label.
+In the case of a merged cell, below_of will pick the 
+bottommost row and leftmost column of the merged cell togo 
+to the bottom of.
+
+Parameters:
+- `label` label to match.
+- `n` Optional. Default value is 1. Indicates the number of rows to skip from label cell to located cell.
+
+### `search_below_of`
+Searches for non-empty cell below of the cell with the given label.
+
+Parameters:
+- `label` label to match.
+- `max_empty_row_search` Indicates the maximum number of rows to search for non-empty cell below of label.
+
+### `below_of_regex`
+Locate the cell below of the cell with a regex match.
+Similarly, in the case of a merged cell, below_of_regex will 
+pick the bottommost row and leftmost row of the merged cell 
+togo to the bottom of.
+
+Parameters:
+- `regex` string for the regular expression.
+- `n` Optional. Default value is 1. Indicates the number of rows to move from regex matched cell to located cell.
+
+
+### `within`
+Locate the cell between a cell with the given label.
+This function searches to the right of or below of the
+cell with the given label. If it is to the right of, the function
+searches row by row while staying in between the column ranges
+of the cell with the given label. If it is below of, similarly,
+we search row by row while staying in between the row ranges of
+the cell with the given label. On top of this you have the option
+on how to pick your data (to the right of or beneath of) once you have found your desired key within
+the cell range.
+
+Parameters:
+- `label` label of cell you want to search in between
+- `find` the name of the cell you want to find in between the cell with that label's range
+- `direction` direction you want to search for your value, choices are:
+  - `right_of` this will search the right of the cell between the columns row wise
+  - `below_of` this will search the beneath the cell between the rows row wise
+- `perform` the action you want to perform to fetch your data, your options are:
+  - `right_of` fetch the value to the right of the cell labeled in `find`
+  - `below_of` fetch the value to beneath of the cell labeled in `find`
+- `n` pick the value n values away in the specified perform direction (right_of or below_of)
+
+
+## Assumption
+
+### `left_cell_match`
+This is useful in batch processing allowing us to check that we have the correct label to the left.
+
+Parameters:
+
+- `label` string to check that it matches.
+
+## Parser
+### `string`
+parse value as string.
+
+### `int`
+parse the value as an integer. 
+
+### `float`
+parse the value as float
+
+### `date`
+parser the value as a date.
+
+## Validator
+
+### `between`
+valid if the value is between(inclusively) `high` and `low`
+
+#### Parameters
+
+- `high` upper bound value.
+- `low` lower bound value
+
+## TableEndCondition
+
+### `all_blank`
+Evaluate to true if all columns are blank.
+
+### `max_row`
+Evaluate to true if the row number(start from 1) including the parsing row is greater than or
+equal to `n`.
+
+#### Parameters
+- `n` number of row
+- `inclusive` Optional. Default True. Whether to include the row in which it evaluates to true.
+
+### `cell_value`
+Evaluate to true if any column in row contains matching `cell_value`. Table terminates the row before.
+
+#### Parameters
+- `cell_value` cell value to match.
+# Dereferencing
+There are two types of dereferencing
+- Spec Creation time dereferencing. The string similar to ``<<A1>>`` will be resolved 
+to the value at A1 of the template file.
+- Extraction time dereferencing. This string similar to ``==A1==`` will be resolved
+to the value at A1 of the extracted file.
+
+Here is an example
+```
+{{--
+key: ==D2==
+assumptions: # Optional
+    - {key: right_of, name: right_of, label: <<A1>>}
+parser: int
+fallback: ==D3== 
+--}}
+```
+
+# Handle Identical Sheet with Different Names
+
+When an excel file to be extracted has a different sheet name than the one in the template file,
+use ``sheet_name_checkers`` parameter in ``exco.from_excel()`` to create ``ExcelProcessor`` 
+with sheet name alias checker.
+
+For example, when the sheet name in the template file is 'Test 1/1/2021', 
+but sheet names can be varied in the extracting files, i.e., 'Test 2/2/2022, 'Test 3/3/2023', etc.
+```
+import exco
+
+SheetName = str
+SheetNameAliasChecker = Callable[[SheetName], bool]
+test_sheet_checker: SheetNameAliasChecker = lambda sheetname: 'Test' in sheetname
+checkers: Dict[SheetName, SheetNameAliasChecker] = {'Test 1/1/2021': test_sheet_checker}
+processor = exco.from_excel(template_excel_path, sheet_name_checkers=checkers)
+```
+
+In the case where there are hidden sheets that might have information that you dont want to extract,
+make sure to set the accept_only_visible_sheets parameter to True
+
+```
+processor = exco.from_excel(template_excel_path, sheet_name_checkers=checkers, accept_only_visible_sheets=True)
+```
+
+# Custom Locator/Parser Etc.
+
+See [Advance Features Notebook](notebooks/quickstart/1%20Advance%20Features.ipynb). But, in essence,
+```python
+processor = exco.from_excel('./custom_locator/custom_locator_template.xlsx',
+                            extra_locators={'diagonal_of': DiagonalOfLocator})
+```
+# Working with .xls files.
+
+Exco will not read Excel 97-2003 workbook (.xls) files. Use [XLS2XLSX](https://pypi.org/project/xls2xlsx/) to convert .xls files to the supported .xlsx format.
```

### Comparing `exco-0.2.8/README.md` & `exco-0.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -347,14 +347,21 @@
 SheetName = str
 SheetNameAliasChecker = Callable[[SheetName], bool]
 test_sheet_checker: SheetNameAliasChecker = lambda sheetname: 'Test' in sheetname
 checkers: Dict[SheetName, SheetNameAliasChecker] = {'Test 1/1/2021': test_sheet_checker}
 processor = exco.from_excel(template_excel_path, sheet_name_checkers=checkers)
 ```
 
+In the case where there are hidden sheets that might have information that you dont want to extract,
+make sure to set the accept_only_visible_sheets parameter to True
+
+```
+processor = exco.from_excel(template_excel_path, sheet_name_checkers=checkers, accept_only_visible_sheets=True)
+```
+
 # Custom Locator/Parser Etc.
 
 See [Advance Features Notebook](notebooks/quickstart/1%20Advance%20Features.ipynb). But, in essence,
 ```python
 processor = exco.from_excel('./custom_locator/custom_locator_template.xlsx',
                             extra_locators={'diagonal_of': DiagonalOfLocator})
 ```
```

### Comparing `exco-0.2.8/setup.py` & `exco-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/__init__.py` & `exco-0.2.9/src/exco/__init__.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/cell_full_path.py` & `exco-0.2.9/src/exco/cell_full_path.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/cell_location.py` & `exco-0.2.9/src/exco/cell_location.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/dereferator.py` & `exco-0.2.9/src/exco/dereferator.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/exception.py` & `exco-0.2.9/src/exco/exception.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/exco_template/exco_block.py` & `exco-0.2.9/src/exco/exco_template/exco_block.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/exco_template/exco_template.py` & `exco-0.2.9/src/exco/exco_template/exco_template.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/exco_watch/__init__.py` & `exco-0.2.9/src/exco/exco_watch/__init__.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/assumption/assumption_factory.py` & `exco-0.2.9/src/exco/extractor/assumption/assumption_factory.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/assumption/built_in/left_cell_match_assumption.py` & `exco-0.2.9/src/exco/extractor/assumption/built_in/left_cell_match_assumption.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/base_factory.py` & `exco-0.2.9/src/exco/extractor/base_factory.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/cell_extraction_task.py` & `exco-0.2.9/src/exco/extractor/cell_extraction_task.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/excel_processor.py` & `exco-0.2.9/src/exco/extractor/excel_processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import secrets
 from dataclasses import dataclass
 from typing import TypeVar, Dict, Any, List, Optional, Generic, Type
 
 import openpyxl
 from openpyxl import Workbook
 
 from exco.cell_location import CellLocation
@@ -115,39 +116,50 @@
 
 
 @dataclass
 class ExcelProcessor:
     spec: ExcelProcessorSpec  # raw spec
     factory: 'ExcelProcessorFactory'
     sheet_name_checkers: SheetNameAliasCheckers
+    accept_only_visible_sheets: bool
 
     def deref(self, workbook: Optional[Workbook]) -> ExcelDerefedProcessor:
         if workbook is not None:
             derefed_spec = self.spec.spec_to_extractor_deref(workbook)
             return self.factory.create_derefed_processor_from_spec(derefed_spec)
         else:
             return self.factory.create_derefed_processor_from_spec(self.spec)
 
     def process_workbook(self, workbook: Workbook) -> ExcelProcessingResult:
         workbook = self.normalize_workbook_sheet_names(workbook)
         return self.deref(workbook).process_workbook(workbook)
 
+    def deal_with_duplicates(self, workbook: Workbook, template_sheet_names: List[str]) -> Workbook:
+        hidden_sheet_names = [sheet.title for sheet in workbook.worksheets if sheet.sheet_state == "hidden"]
+        for template_sheet_name in template_sheet_names:
+            if template_sheet_name in hidden_sheet_names:
+                workbook[template_sheet_name].title = "duplicate_sheet_name" + str(secrets.randbelow(10000))
+        return workbook
+
     def normalize_workbook_sheet_names(self, workbook: Workbook) -> Workbook:
         if not self.sheet_name_checkers:
             return workbook
-
+        if self.accept_only_visible_sheets:
+            workbook = self.deal_with_duplicates(workbook, list(self.sheet_name_checkers.keys()))
         name_mapping: Dict[SheetName, SheetName] = {}
-        for sheet_name in workbook.sheetnames:
+        for sheet in workbook.worksheets:
+            sheet_name = sheet.title
             for template_sheet_name, checker in self.sheet_name_checkers.items():
+                if self.accept_only_visible_sheets and sheet.sheet_state == "hidden":
+                    continue
                 if checker(sheet_name):
                     name_mapping[sheet_name] = template_sheet_name
                     break
         for sheet_name, template_sheet_name in name_mapping.items():
             workbook[sheet_name].title = template_sheet_name
-
         return workbook
 
     def process_excel(self, fname: str) -> ExcelProcessingResult:
         wb = openpyxl.load_workbook(fname, data_only=True)
         return self.process_workbook(wb)
 
     def __str__(self) -> str:
@@ -228,24 +240,33 @@
             table_tasks[cl] = [
                 self.create_table_extraction_task(spec) for spec in specs]
 
         return ExcelDerefedProcessor(cell_processors=cell_tasks,
                                      table_processors=table_tasks)
 
     def create_from_spec(self, spec: ExcelProcessorSpec,
-                         sheet_name_checkers: Optional[SheetNameAliasCheckers] = None) -> ExcelProcessor:
-        return ExcelProcessor(spec=spec, factory=self, sheet_name_checkers=sheet_name_checkers)
+                         sheet_name_checkers: Optional[SheetNameAliasCheckers] = None,
+                         accept_only_visible_sheets: bool = False) -> ExcelProcessor:
+        return ExcelProcessor(spec=spec, factory=self,
+                              sheet_name_checkers=sheet_name_checkers,
+                              accept_only_visible_sheets=accept_only_visible_sheets)
 
     def create_from_template_excel(self,
                                    fname: str,
-                                   sheet_name_checkers: Optional[SheetNameAliasCheckers] = None
+                                   sheet_name_checkers: Optional[SheetNameAliasCheckers] = None,
+                                   accept_only_visible_sheets: bool = False
                                    ) -> ExcelProcessor:
         workbook = openpyxl.load_workbook(fname, data_only=True)
-        return self.create_from_template_workbook(workbook, sheet_name_checkers=sheet_name_checkers)
+        return self.create_from_template_workbook(workbook,
+                                                  sheet_name_checkers=sheet_name_checkers,
+                                                  accept_only_visible_sheets=accept_only_visible_sheets)
 
     def create_from_template_workbook(
             self,
             workbook: Workbook,
-            sheet_name_checkers: Optional[SheetNameAliasCheckers] = None
+            sheet_name_checkers: Optional[SheetNameAliasCheckers] = None,
+            accept_only_visible_sheets: bool = False
     ) -> ExcelProcessor:
         spec = ExcelProcessorSpec.from_workbook_template(workbook)
-        return self.create_from_spec(spec, sheet_name_checkers=sheet_name_checkers)
+        return self.create_from_spec(spec,
+                                     sheet_name_checkers=sheet_name_checkers,
+                                     accept_only_visible_sheets=accept_only_visible_sheets)
```

### Comparing `exco-0.2.8/src/exco/extractor/locator/built_in/below_of_locator.py` & `exco-0.2.9/src/exco/extractor/locator/built_in/below_of_locator.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/locator/built_in/below_of_regex_locator.py` & `exco-0.2.9/src/exco/extractor/locator/built_in/below_of_regex_locator.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def locate(self, anchor_cell_location: CellLocation,
                workbook: Workbook) -> LocatingResult:
         sheet: Worksheet = workbook[anchor_cell_location.sheet_name]
         compiled_regex = re.compile(self.regex)
         for row in sheet.iter_rows():
             for cell in row:
                 if compiled_regex.fullmatch(str(cell.value)) is not None:
-                    coord = util.get_rightmost_coordinate(sheet=sheet, cell=cell)
+                    coord = util.get_bottommost_coordinate(sheet=sheet, cell=cell)
                     cell_loc = CellLocation(
                         sheet_name=anchor_cell_location.sheet_name,
                         coordinate=util.shift_coord(coord.coordinate, (self.n, 0))
                     )
                     return LocatingResult.good(cell_loc)
         return LocatingResult.bad(
             msg=f"Unable to find cell below of {self.regex}")
```

### Comparing `exco-0.2.8/src/exco/extractor/locator/built_in/right_of_locator.py` & `exco-0.2.9/src/exco/extractor/locator/built_in/right_of_locator.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/locator/built_in/right_of_regex_locator.py` & `exco-0.2.9/src/exco/extractor/locator/built_in/right_of_regex_locator.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/locator/built_in/search_below_of_locator.py` & `exco-0.2.9/src/exco/extractor/locator/built_in/search_below_of_locator.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/locator/built_in/search_right_of_locator.py` & `exco-0.2.9/src/exco/extractor/locator/built_in/search_right_of_locator.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/locator/built_in/within_locator.py` & `exco-0.2.9/src/exco/extractor/locator/built_in/within_locator.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/locator/locating_result.py` & `exco-0.2.9/src/exco/extractor/locator/locating_result.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/locator/locator_factory.py` & `exco-0.2.9/src/exco/extractor/locator/locator_factory.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/parser/built_in/link_parser.py` & `exco-0.2.9/src/exco/extractor/parser/built_in/link_parser.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/parser/built_in/value_parser.py` & `exco-0.2.9/src/exco/extractor/parser/built_in/value_parser.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/parser/parser_factory.py` & `exco-0.2.9/src/exco/extractor/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/parser/parsing_result.py` & `exco-0.2.9/src/exco/extractor/parser/parsing_result.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/table_end_conditions/built_in/all_blank_table_end_condition.py` & `exco-0.2.9/src/exco/extractor/table_end_conditions/built_in/all_blank_table_end_condition.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/table_end_conditions/built_in/cell_value_table_end_condition.py` & `exco-0.2.9/src/exco/extractor/table_end_conditions/built_in/cell_value_table_end_condition.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/table_end_conditions/built_in/max_row_table_end_condition.py` & `exco-0.2.9/src/exco/extractor/table_end_conditions/built_in/max_row_table_end_condition.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/table_end_conditions/table_end_condition.py` & `exco-0.2.9/src/exco/extractor/table_end_conditions/table_end_condition.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/table_end_conditions/table_end_condition_factory.py` & `exco-0.2.9/src/exco/extractor/table_end_conditions/table_end_condition_factory.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/table_end_conditions/table_end_condition_result.py` & `exco-0.2.9/src/exco/extractor/table_end_conditions/table_end_condition_result.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/table_extraction_task.py` & `exco-0.2.9/src/exco/extractor/table_extraction_task.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/validator/built_in/value_validator.py` & `exco-0.2.9/src/exco/extractor/validator/built_in/value_validator.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor/validator/validator_factory.py` & `exco-0.2.9/src/exco/extractor/validator/validator_factory.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor_spec/apv_spec.py` & `exco-0.2.9/src/exco/extractor_spec/apv_spec.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor_spec/assumption_spec.py` & `exco-0.2.9/src/exco/extractor_spec/assumption_spec.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor_spec/cell_extraction_spec.py` & `exco-0.2.9/src/exco/extractor_spec/cell_extraction_spec.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor_spec/excel_processor_spec.py` & `exco-0.2.9/src/exco/extractor_spec/excel_processor_spec.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor_spec/locator_spec.py` & `exco-0.2.9/src/exco/extractor_spec/locator_spec.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor_spec/parser_spec.py` & `exco-0.2.9/src/exco/extractor_spec/parser_spec.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor_spec/table_extraction_spec.py` & `exco-0.2.9/src/exco/extractor_spec/table_extraction_spec.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/extractor_spec/validator_spec.py` & `exco-0.2.9/src/exco/extractor_spec/validator_spec.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/setting.py` & `exco-0.2.9/src/exco/setting.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco/util.py` & `exco-0.2.9/src/exco/util.py`

 * *Files identical despite different names*

### Comparing `exco-0.2.8/src/exco.egg-info/PKG-INFO` & `exco-0.2.9/src/exco.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,376 +1,384 @@
 Metadata-Version: 2.1
 Name: exco
-Version: 0.2.8
+Version: 0.2.9
 Summary: Excel Comment Orm
 Home-page: https://github.com/thegangtechnology/exco
 Author: Piti Ongmongkolkul
 Author-email: piti118@gmail.com
 License: Private
-Description: # Exco
-        
-        [![Build](https://github.com/thegangtechnology/exco/workflows/Build/badge.svg)](https://github.com/thegangtechnology/exco/actions?query=workflow%3ABuild)
-        [![Sonarqube](https://github.com/thegangtechnology/exco/workflows/Sonarqube/badge.svg)](https://github.com/thegangtechnology/exco/actions?query=workflow%3ASonarqube)
-        [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=thegangtechnology_exco&metric=alert_status)](https://sonarcloud.io/dashboard?id=thegangtechnology_exco)
-        [![CodeQL](https://github.com/thegangtechnology/exco/workflows/CodeQL/badge.svg)](https://github.com/thegangtechnology/exco/actions?query=workflow%3ACodeQL)
-        [![codecov](https://codecov.io/gh/thegangtechnology/exco/branch/master/graph/badge.svg?token=8BrjxREw2O)](https://codecov.io/gh/thegangtechnology/exco)
-        [![PyPI version](https://badge.fury.io/py/exco.svg)](https://badge.fury.io/py/exco)
-        
-        Excel Comment ORM. Declare ORM Spec descriptively right on the excel file.
-        
-        # What it does
-        
-        The package allows you to declare orm mapping right in the excel file in the comments
-         then use it to extract data from other similar files.
-         
-        An example of a template is shown below.
-        
-        ![Template](notebooks/quickstart/template.png)
-        
-        Dynamic Location, Validation, Assumptions, custom Parser are also supported.
-        
-        
-        # Installation
-        
-        ```
-        pip install exco
-        ```
-        
-        # Simple Usage
-        
-        ```
-        import exco
-        processor = exco.from_excel('./quickstart_template.xlsx')
-        result = processor.process_excel('./quickstart_data_file.xlsx')
-        print(result.to_dict())
-        ```
-        
-        See Also [Quick Start Notebook](notebooks/quickstart/0%20Quick%20Start.ipynb)
-        
-        # Exco Block
-        
-        Exco relies on yml blocks inside excel comment to build a spec.
-        Each comment can contain multiple blocks.
-        There are three types of echo block: a cell block, a table block, and a column block.
-        
-        ## Cell Block
-        
-        A cellblock is a block of yml that is surrounded by `{{--` and `--}}`
-        ```
-        {{--
-        key: some_int
-        parser: int
-        --}}
-        ```
-        
-        This means that parse this cell as `int` and put it in the result with key `some_int`.
-        
-        
-        
-        Other advance features like, fallback, locator, assumptions, validator are optional.
-        The full specification is shown below.
-        
-        ```
-        {{--
-        key: some_value
-        # Optional default at_comment_cell
-        locator: {name: at_comment_cell} 
-        assumptions: # Optional
-            - {key: right_of, name: right_of, label: marker}
-        parser: int
-        # Optional
-        fallback: 7 
-        # Optional. Dict[name, value].
-        params: {} 
-        validators: # Optional
-            - {key: between, name: between, low: 5, high: 10 }
-        metadata: {unit: km}
-        --}}
-        ```
-        
-        ### Processing Flow.
-        
-        The cell processing flow is
-        
-        1. Locating the Cell
-        2. Check Assumption
-        3. Parse
-        4. Validation
-        
-        ### Features
-        
-        #### `key`
-        Key where the result will be put. This is required.
-        
-        #### `fallback`
-        
-        This is the most useful one where if the cell is failed locating, testing assumption, parsing.
-        The fallback value is assumed. If it is not specified, the value None is used. (yml's none is `null`).
-        
-        #### `locator`
-        Locator is a dictionary. The key `name` is the class name to be used to locate the cell. Other parameters
-        can be flattened and put in the same dictionary. These parameters will be pass through the constructor
-        of such class.
-        
-        If the locator is left out, it is assumed to be `at_comment_cell` which locate the cell with exactly
-        the same coordinate as the commented cell in the template.
-        
-        #### `assumptions`
-        List of dictionaries. The `key` is the name of the check. `name` is the name of the class to be used in
-        testing an assumption. Other parameters can be flattened and included in the same dictionary.
-        
-        #### `parser`
-        Required. Name of the parser class.
-        
-        #### `params`
-        Optional. Dictionary of the parameter name to its value. The spread values are passed through the parser
-        constructor.
-        
-        #### `validations`
-        Optional. List of Dictionary. Each dictionary must have `key` for the validation key and `name`,
-        validator's class name, specified. Other parameters to be passed to the validator constructor can be flattened and specified in this dictionary as well.
-        
-        ### `metadata`
-        Optional. Metadata. Dictionary of any object can be put here. The object will be parsed on to the result.
-        
-        ## Table Block
-        A table block is for specifying the properties of the table. The table block is surrounded by
-        `{{--table` and `--}}`. The simplest table block is
-        ```
-        {{--table
-        key: some_table
-        --}}
-        ```
-        This is typically what you need. A more complicated example is shown below:
-        
-        ```
-        {{--table
-        key: some_table
-        # optional. default at_comment_cell
-        locator: {name: at_comment_cell}
-        # optional. default downward
-        item_direction: downward
-        end_conditions:
-            - {name: all_blank}
-            - {name: max_row, n: 10, inclusive: true}
-        --}}
-        ```
-        ### Features
-        #### `key`
-        where the table will be put in the result. The output for the table is a list of dictionaries
-        where the key in the dictionaries is the column name specified in column blocks.
-        
-        #### `locator`
-        Optional. Default at_comment_cell. Locator for the table anchor cell. Same as a cell block.
-        
-        #### `item_direction`
-        Optional Direction for items in the table. Default downward. (rightward or downward)
-        
-        #### `end_conditions`
-        A list of dictionary specifying each termination condition. The dictionary contains `name` and flattened
-        parameters.
-        
-        If any of the end condition is met then the parsing for the table terminates. Depending on the end condition's
-        class, it may or may not include the matching row.
-        
-        ## Column Block
-        
-        Column block specifications are very similar to the cell block. The simplest example is shown below.
-        ```
-        {{--col
-        table_key: some_table
-        key: some_col
-        parser: int
-        }}
-        ```
-        The column block is very similar to the cell block. It is the cell block with `table_key` and without
-        `locator`. The `table_key` tells which table it belongs to. It must match one of the table's `key` defined in the table block.
-        
-        The position of the column cell when extracting value is computed from the relative position to the table
-         block in the template.
-         
-         All other features like fallback, assumptions, validations are also supported in the same
-         fashion as the cell block.
-        
-        # Built-in Functions
-        
-        ## Locator
-        ### `at_comment_cell`
-        Locate the cell right at the comment cell's coordinate in the template.
-        
-        ### `right_of`
-        Locate the cell to the right of the cell or merged cell with the given label.
-        In the case of a merged cell, right_of will pick the rightmost column and 
-        topmost row of the merged cell togo to the right of.
-        
-        Parameters:
-        - `label` label to match.
-        - `n` Optional. Default value is 1. Indicates the number of columns to move from label cell to located cell.
-        
-        ### `search_right_of`
-        Searches for non-empty cell right of the cell with the given value.
-        
-        Parameters:
-        - `label` label to match.
-        - `max_empty_col_search` Indicates the maximum number of columns to search for non-empty cell right of label.
-        ### `right_of_regex`
-        Locate the cell to the right of the cell with a regex match.
-        Similarly, in the case of a merged cell, right_of_regex will 
-        pick the rightmost column and topmost row of the merged cell 
-        togo to the right of.
-        
-        Parameters:
-        - `regex` string for the regular expression.
-        - `n` Optional. Default value is 1. Indicates the number of columns to move from regex matched cell to located cell.
-        
-        ### `below_of`
-        Locate the cell below of the cell with the given label.
-        In the case of a merged cell, below_of will pick the 
-        bottommost row and leftmost column of the merged cell togo 
-        to the bottom of.
-        
-        Parameters:
-        - `label` label to match.
-        - `n` Optional. Default value is 1. Indicates the number of rows to skip from label cell to located cell.
-        
-        ### `search_below_of`
-        Searches for non-empty cell below of the cell with the given label.
-        
-        Parameters:
-        - `label` label to match.
-        - `max_empty_row_search` Indicates the maximum number of rows to search for non-empty cell below of label.
-        
-        ### `below_of_regex`
-        Locate the cell below of the cell with a regex match.
-        Similarly, in the case of a merged cell, below_of_regex will 
-        pick the bottommost row and leftmost row of the merged cell 
-        togo to the bottom of.
-        
-        Parameters:
-        - `regex` string for the regular expression.
-        - `n` Optional. Default value is 1. Indicates the number of rows to move from regex matched cell to located cell.
-        
-        
-        ### `within`
-        Locate the cell between a cell with the given label.
-        This function searches to the right of or below of the
-        cell with the given label. If it is to the right of, the function
-        searches row by row while staying in between the column ranges
-        of the cell with the given label. If it is below of, similarly,
-        we search row by row while staying in between the row ranges of
-        the cell with the given label. On top of this you have the option
-        on how to pick your data (to the right of or beneath of) once you have found your desired key within
-        the cell range.
-        
-        Parameters:
-        - `label` label of cell you want to search in between
-        - `find` the name of the cell you want to find in between the cell with that label's range
-        - `direction` direction you want to search for your value, choices are:
-          - `right_of` this will search the right of the cell between the columns row wise
-          - `below_of` this will search the beneath the cell between the rows row wise
-        - `perform` the action you want to perform to fetch your data, your options are:
-          - `right_of` fetch the value to the right of the cell labeled in `find`
-          - `below_of` fetch the value to beneath of the cell labeled in `find`
-        - `n` pick the value n values away in the specified perform direction (right_of or below_of)
-        
-        
-        ## Assumption
-        
-        ### `left_cell_match`
-        This is useful in batch processing allowing us to check that we have the correct label to the left.
-        
-        Parameters:
-        
-        - `label` string to check that it matches.
-        
-        ## Parser
-        ### `string`
-        parse value as string.
-        
-        ### `int`
-        parse the value as an integer. 
-        
-        ### `float`
-        parse the value as float
-        
-        ### `date`
-        parser the value as a date.
-        
-        ## Validator
-        
-        ### `between`
-        valid if the value is between(inclusively) `high` and `low`
-        
-        #### Parameters
-        
-        - `high` upper bound value.
-        - `low` lower bound value
-        
-        ## TableEndCondition
-        
-        ### `all_blank`
-        Evaluate to true if all columns are blank.
-        
-        ### `max_row`
-        Evaluate to true if the row number(start from 1) including the parsing row is greater than or
-        equal to `n`.
-        
-        #### Parameters
-        - `n` number of row
-        - `inclusive` Optional. Default True. Whether to include the row in which it evaluates to true.
-        
-        ### `cell_value`
-        Evaluate to true if any column in row contains matching `cell_value`. Table terminates the row before.
-        
-        #### Parameters
-        - `cell_value` cell value to match.
-        # Dereferencing
-        There are two types of dereferencing
-        - Spec Creation time dereferencing. The string similar to ``<<A1>>`` will be resolved 
-        to the value at A1 of the template file.
-        - Extraction time dereferencing. This string similar to ``==A1==`` will be resolved
-        to the value at A1 of the extracted file.
-        
-        Here is an example
-        ```
-        {{--
-        key: ==D2==
-        assumptions: # Optional
-            - {key: right_of, name: right_of, label: <<A1>>}
-        parser: int
-        fallback: ==D3== 
-        --}}
-        ```
-        
-        # Handle Identical Sheet with Different Names
-        
-        When an excel file to be extracted has a different sheet name than the one in the template file,
-        use ``sheet_name_checkers`` parameter in ``exco.from_excel()`` to create ``ExcelProcessor`` 
-        with sheet name alias checker.
-        
-        For example, when the sheet name in the template file is 'Test 1/1/2021', 
-        but sheet names can be varied in the extracting files, i.e., 'Test 2/2/2022, 'Test 3/3/2023', etc.
-        ```
-        import exco
-        
-        SheetName = str
-        SheetNameAliasChecker = Callable[[SheetName], bool]
-        test_sheet_checker: SheetNameAliasChecker = lambda sheetname: 'Test' in sheetname
-        checkers: Dict[SheetName, SheetNameAliasChecker] = {'Test 1/1/2021': test_sheet_checker}
-        processor = exco.from_excel(template_excel_path, sheet_name_checkers=checkers)
-        ```
-        
-        # Custom Locator/Parser Etc.
-        
-        See [Advance Features Notebook](notebooks/quickstart/1%20Advance%20Features.ipynb). But, in essence,
-        ```python
-        processor = exco.from_excel('./custom_locator/custom_locator_template.xlsx',
-                                    extra_locators={'diagonal_of': DiagonalOfLocator})
-        ```
-        # Working with .xls files.
-        
-        Exco will not read Excel 97-2003 workbook (.xls) files. Use [XLS2XLSX](https://pypi.org/project/xls2xlsx/) to convert .xls files to the supported .xlsx format.
-Platform: UNKNOWN
 Classifier: 
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+# Exco
+
+[![Build](https://github.com/thegangtechnology/exco/workflows/Build/badge.svg)](https://github.com/thegangtechnology/exco/actions?query=workflow%3ABuild)
+[![Sonarqube](https://github.com/thegangtechnology/exco/workflows/Sonarqube/badge.svg)](https://github.com/thegangtechnology/exco/actions?query=workflow%3ASonarqube)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=thegangtechnology_exco&metric=alert_status)](https://sonarcloud.io/dashboard?id=thegangtechnology_exco)
+[![CodeQL](https://github.com/thegangtechnology/exco/workflows/CodeQL/badge.svg)](https://github.com/thegangtechnology/exco/actions?query=workflow%3ACodeQL)
+[![codecov](https://codecov.io/gh/thegangtechnology/exco/branch/master/graph/badge.svg?token=8BrjxREw2O)](https://codecov.io/gh/thegangtechnology/exco)
+[![PyPI version](https://badge.fury.io/py/exco.svg)](https://badge.fury.io/py/exco)
+
+Excel Comment ORM. Declare ORM Spec descriptively right on the excel file.
+
+# What it does
+
+The package allows you to declare orm mapping right in the excel file in the comments
+ then use it to extract data from other similar files.
+ 
+An example of a template is shown below.
+
+![Template](notebooks/quickstart/template.png)
+
+Dynamic Location, Validation, Assumptions, custom Parser are also supported.
+
+
+# Installation
+
+```
+pip install exco
+```
+
+# Simple Usage
+
+```
+import exco
+processor = exco.from_excel('./quickstart_template.xlsx')
+result = processor.process_excel('./quickstart_data_file.xlsx')
+print(result.to_dict())
+```
+
+See Also [Quick Start Notebook](notebooks/quickstart/0%20Quick%20Start.ipynb)
+
+# Exco Block
+
+Exco relies on yml blocks inside excel comment to build a spec.
+Each comment can contain multiple blocks.
+There are three types of echo block: a cell block, a table block, and a column block.
+
+## Cell Block
+
+A cellblock is a block of yml that is surrounded by `{{--` and `--}}`
+```
+{{--
+key: some_int
+parser: int
+--}}
+```
+
+This means that parse this cell as `int` and put it in the result with key `some_int`.
+
+
+
+Other advance features like, fallback, locator, assumptions, validator are optional.
+The full specification is shown below.
+
+```
+{{--
+key: some_value
+# Optional default at_comment_cell
+locator: {name: at_comment_cell} 
+assumptions: # Optional
+    - {key: right_of, name: right_of, label: marker}
+parser: int
+# Optional
+fallback: 7 
+# Optional. Dict[name, value].
+params: {} 
+validators: # Optional
+    - {key: between, name: between, low: 5, high: 10 }
+metadata: {unit: km}
+--}}
+```
+
+### Processing Flow.
+
+The cell processing flow is
+
+1. Locating the Cell
+2. Check Assumption
+3. Parse
+4. Validation
+
+### Features
+
+#### `key`
+Key where the result will be put. This is required.
+
+#### `fallback`
+
+This is the most useful one where if the cell is failed locating, testing assumption, parsing.
+The fallback value is assumed. If it is not specified, the value None is used. (yml's none is `null`).
+
+#### `locator`
+Locator is a dictionary. The key `name` is the class name to be used to locate the cell. Other parameters
+can be flattened and put in the same dictionary. These parameters will be pass through the constructor
+of such class.
+
+If the locator is left out, it is assumed to be `at_comment_cell` which locate the cell with exactly
+the same coordinate as the commented cell in the template.
+
+#### `assumptions`
+List of dictionaries. The `key` is the name of the check. `name` is the name of the class to be used in
+testing an assumption. Other parameters can be flattened and included in the same dictionary.
+
+#### `parser`
+Required. Name of the parser class.
+
+#### `params`
+Optional. Dictionary of the parameter name to its value. The spread values are passed through the parser
+constructor.
+
+#### `validations`
+Optional. List of Dictionary. Each dictionary must have `key` for the validation key and `name`,
+validator's class name, specified. Other parameters to be passed to the validator constructor can be flattened and specified in this dictionary as well.
+
+### `metadata`
+Optional. Metadata. Dictionary of any object can be put here. The object will be parsed on to the result.
+
+## Table Block
+A table block is for specifying the properties of the table. The table block is surrounded by
+`{{--table` and `--}}`. The simplest table block is
+```
+{{--table
+key: some_table
+--}}
+```
+This is typically what you need. A more complicated example is shown below:
+
+```
+{{--table
+key: some_table
+# optional. default at_comment_cell
+locator: {name: at_comment_cell}
+# optional. default downward
+item_direction: downward
+end_conditions:
+    - {name: all_blank}
+    - {name: max_row, n: 10, inclusive: true}
+--}}
+```
+### Features
+#### `key`
+where the table will be put in the result. The output for the table is a list of dictionaries
+where the key in the dictionaries is the column name specified in column blocks.
+
+#### `locator`
+Optional. Default at_comment_cell. Locator for the table anchor cell. Same as a cell block.
+
+#### `item_direction`
+Optional Direction for items in the table. Default downward. (rightward or downward)
+
+#### `end_conditions`
+A list of dictionary specifying each termination condition. The dictionary contains `name` and flattened
+parameters.
+
+If any of the end condition is met then the parsing for the table terminates. Depending on the end condition's
+class, it may or may not include the matching row.
+
+## Column Block
+
+Column block specifications are very similar to the cell block. The simplest example is shown below.
+```
+{{--col
+table_key: some_table
+key: some_col
+parser: int
+}}
+```
+The column block is very similar to the cell block. It is the cell block with `table_key` and without
+`locator`. The `table_key` tells which table it belongs to. It must match one of the table's `key` defined in the table block.
+
+The position of the column cell when extracting value is computed from the relative position to the table
+ block in the template.
+ 
+ All other features like fallback, assumptions, validations are also supported in the same
+ fashion as the cell block.
+
+# Built-in Functions
+
+## Locator
+### `at_comment_cell`
+Locate the cell right at the comment cell's coordinate in the template.
+
+### `right_of`
+Locate the cell to the right of the cell or merged cell with the given label.
+In the case of a merged cell, right_of will pick the rightmost column and 
+topmost row of the merged cell togo to the right of.
+
+Parameters:
+- `label` label to match.
+- `n` Optional. Default value is 1. Indicates the number of columns to move from label cell to located cell.
+
+### `search_right_of`
+Searches for non-empty cell right of the cell with the given value.
+
+Parameters:
+- `label` label to match.
+- `max_empty_col_search` Indicates the maximum number of columns to search for non-empty cell right of label.
+### `right_of_regex`
+Locate the cell to the right of the cell with a regex match.
+Similarly, in the case of a merged cell, right_of_regex will 
+pick the rightmost column and topmost row of the merged cell 
+togo to the right of.
+
+Parameters:
+- `regex` string for the regular expression.
+- `n` Optional. Default value is 1. Indicates the number of columns to move from regex matched cell to located cell.
+
+### `below_of`
+Locate the cell below of the cell with the given label.
+In the case of a merged cell, below_of will pick the 
+bottommost row and leftmost column of the merged cell togo 
+to the bottom of.
+
+Parameters:
+- `label` label to match.
+- `n` Optional. Default value is 1. Indicates the number of rows to skip from label cell to located cell.
+
+### `search_below_of`
+Searches for non-empty cell below of the cell with the given label.
+
+Parameters:
+- `label` label to match.
+- `max_empty_row_search` Indicates the maximum number of rows to search for non-empty cell below of label.
+
+### `below_of_regex`
+Locate the cell below of the cell with a regex match.
+Similarly, in the case of a merged cell, below_of_regex will 
+pick the bottommost row and leftmost row of the merged cell 
+togo to the bottom of.
+
+Parameters:
+- `regex` string for the regular expression.
+- `n` Optional. Default value is 1. Indicates the number of rows to move from regex matched cell to located cell.
+
+
+### `within`
+Locate the cell between a cell with the given label.
+This function searches to the right of or below of the
+cell with the given label. If it is to the right of, the function
+searches row by row while staying in between the column ranges
+of the cell with the given label. If it is below of, similarly,
+we search row by row while staying in between the row ranges of
+the cell with the given label. On top of this you have the option
+on how to pick your data (to the right of or beneath of) once you have found your desired key within
+the cell range.
+
+Parameters:
+- `label` label of cell you want to search in between
+- `find` the name of the cell you want to find in between the cell with that label's range
+- `direction` direction you want to search for your value, choices are:
+  - `right_of` this will search the right of the cell between the columns row wise
+  - `below_of` this will search the beneath the cell between the rows row wise
+- `perform` the action you want to perform to fetch your data, your options are:
+  - `right_of` fetch the value to the right of the cell labeled in `find`
+  - `below_of` fetch the value to beneath of the cell labeled in `find`
+- `n` pick the value n values away in the specified perform direction (right_of or below_of)
+
+
+## Assumption
+
+### `left_cell_match`
+This is useful in batch processing allowing us to check that we have the correct label to the left.
+
+Parameters:
+
+- `label` string to check that it matches.
+
+## Parser
+### `string`
+parse value as string.
+
+### `int`
+parse the value as an integer. 
+
+### `float`
+parse the value as float
+
+### `date`
+parser the value as a date.
+
+## Validator
+
+### `between`
+valid if the value is between(inclusively) `high` and `low`
+
+#### Parameters
+
+- `high` upper bound value.
+- `low` lower bound value
+
+## TableEndCondition
+
+### `all_blank`
+Evaluate to true if all columns are blank.
+
+### `max_row`
+Evaluate to true if the row number(start from 1) including the parsing row is greater than or
+equal to `n`.
+
+#### Parameters
+- `n` number of row
+- `inclusive` Optional. Default True. Whether to include the row in which it evaluates to true.
+
+### `cell_value`
+Evaluate to true if any column in row contains matching `cell_value`. Table terminates the row before.
+
+#### Parameters
+- `cell_value` cell value to match.
+# Dereferencing
+There are two types of dereferencing
+- Spec Creation time dereferencing. The string similar to ``<<A1>>`` will be resolved 
+to the value at A1 of the template file.
+- Extraction time dereferencing. This string similar to ``==A1==`` will be resolved
+to the value at A1 of the extracted file.
+
+Here is an example
+```
+{{--
+key: ==D2==
+assumptions: # Optional
+    - {key: right_of, name: right_of, label: <<A1>>}
+parser: int
+fallback: ==D3== 
+--}}
+```
+
+# Handle Identical Sheet with Different Names
+
+When an excel file to be extracted has a different sheet name than the one in the template file,
+use ``sheet_name_checkers`` parameter in ``exco.from_excel()`` to create ``ExcelProcessor`` 
+with sheet name alias checker.
+
+For example, when the sheet name in the template file is 'Test 1/1/2021', 
+but sheet names can be varied in the extracting files, i.e., 'Test 2/2/2022, 'Test 3/3/2023', etc.
+```
+import exco
+
+SheetName = str
+SheetNameAliasChecker = Callable[[SheetName], bool]
+test_sheet_checker: SheetNameAliasChecker = lambda sheetname: 'Test' in sheetname
+checkers: Dict[SheetName, SheetNameAliasChecker] = {'Test 1/1/2021': test_sheet_checker}
+processor = exco.from_excel(template_excel_path, sheet_name_checkers=checkers)
+```
+
+In the case where there are hidden sheets that might have information that you dont want to extract,
+make sure to set the accept_only_visible_sheets parameter to True
+
+```
+processor = exco.from_excel(template_excel_path, sheet_name_checkers=checkers, accept_only_visible_sheets=True)
+```
+
+# Custom Locator/Parser Etc.
+
+See [Advance Features Notebook](notebooks/quickstart/1%20Advance%20Features.ipynb). But, in essence,
+```python
+processor = exco.from_excel('./custom_locator/custom_locator_template.xlsx',
+                            extra_locators={'diagonal_of': DiagonalOfLocator})
+```
+# Working with .xls files.
+
+Exco will not read Excel 97-2003 workbook (.xls) files. Use [XLS2XLSX](https://pypi.org/project/xls2xlsx/) to convert .xls files to the supported .xlsx format.
```

### Comparing `exco-0.2.8/src/exco.egg-info/SOURCES.txt` & `exco-0.2.9/src/exco.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 src/exco/__init__.py
 src/exco/__version__.py
 src/exco/cell_full_path.py
 src/exco/cell_location.py
```

