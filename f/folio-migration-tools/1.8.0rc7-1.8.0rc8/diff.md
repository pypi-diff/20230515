# Comparing `tmp/folio_migration_tools-1.8.0rc7.tar.gz` & `tmp/folio_migration_tools-1.8.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folio_migration_tools-1.8.0rc7.tar", max compression
+gzip compressed data, was "folio_migration_tools-1.8.0rc8.tar", max compression
```

## Comparing `folio_migration_tools-1.8.0rc7.tar` & `folio_migration_tools-1.8.0rc8.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1072 2023-03-06 22:17:01.793515 folio_migration_tools-1.8.0rc7/LICENSE
--rw-r--r--   0        0        0     4193 2023-03-21 14:28:28.887645 folio_migration_tools-1.8.0rc7/README.md
--rw-r--r--   0        0        0     1748 2023-05-03 20:30:40.284410 folio_migration_tools-1.8.0rc7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.810173 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/__init__.py
--rw-r--r--   0        0        0     5322 2023-05-03 19:02:35.338530 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/__main__.py
--rw-r--r--   0        0        0    14007 2023-05-03 19:02:35.494096 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/circulation_helper.py
--rw-r--r--   0        0        0      227 2023-03-06 22:17:01.811146 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/colors.py
--rw-r--r--   0        0        0      648 2023-03-06 22:17:01.811423 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/custom_dict.py
--rw-r--r--   0        0        0     2374 2023-03-06 22:17:01.811751 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/custom_exceptions.py
--rw-r--r--   0        0        0     1678 2023-03-06 22:17:01.812068 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/extradata_writer.py
--rw-r--r--   0        0        0     6573 2023-03-06 22:17:01.812324 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/folder_structure.py
--rw-r--r--   0        0        0     2550 2023-03-06 22:17:01.812602 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/helper.py
--rw-r--r--   0        0        0     7089 2023-03-06 22:17:01.812878 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/holdings_helper.py
--rw-r--r--   0        0        0     2636 2023-04-18 23:46:20.197850 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/library_configuration.py
--rw-r--r--   0        0        0    19528 2023-03-27 22:22:56.113076 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapper_base.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.813766 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/__init__.py
--rw-r--r--   0        0        0     8117 2023-04-19 02:19:29.600062 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py
--rw-r--r--   0        0        0     6423 2023-04-19 02:19:29.616368 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py
--rw-r--r--   0        0        0    10080 2023-05-03 19:02:35.234989 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/item_mapper.py
--rw-r--r--   0        0        0    10431 2023-05-03 19:02:35.235966 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/manual_fee_fines_mapper.py
--rw-r--r--   0        0        0    37072 2023-04-19 02:19:29.621237 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py
--rw-r--r--   0        0        0     3548 2023-03-24 03:05:35.503768 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py
--rw-r--r--   0        0        0    14849 2023-05-03 19:02:35.300564 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/order_mapper.py
--rw-r--r--   0        0        0    14644 2023-05-03 19:02:35.319735 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py
--rw-r--r--   0        0        0     8855 2023-05-03 19:02:35.238368 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py
--rw-r--r--   0        0        0     7683 2023-04-19 02:19:29.634576 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/user_mapper.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.816647 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/__init__.py
--rw-r--r--   0        0        0    34047 2023-04-18 23:46:20.215442 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/conditions.py
--rw-r--r--   0        0        0    11297 2023-03-06 22:17:01.817193 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py
--rw-r--r--   0        0        0     9386 2023-05-03 19:02:35.301485 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py
--rw-r--r--   0        0        0   382912 2023-03-06 22:17:01.818293 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml
--rw-r--r--   0        0        0    10697 2023-05-03 19:02:35.467697 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py
--rw-r--r--   0        0        0     4962 2023-03-06 22:17:01.818809 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py
--rw-r--r--   0        0        0     5850 2023-03-27 22:22:56.116126 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py
--rw-r--r--   0        0        0    34454 2023-04-17 23:01:11.524015 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py
--rw-r--r--   0        0        0    25845 2023-04-17 23:01:11.525499 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py
--rw-r--r--   0        0        0    17417 2023-04-17 23:01:11.530990 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py
--rw-r--r--   0        0        0     4084 2023-03-06 22:17:01.820137 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_report.py
--rw-r--r--   0        0        0      211 2023-03-06 22:17:01.820491 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/__init__.py
--rw-r--r--   0        0        0     4231 2023-04-17 23:01:11.544786 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/authority_transformer.py
--rw-r--r--   0        0        0    28090 2023-05-03 19:02:35.447257 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/batch_poster.py
--rw-r--r--   0        0        0     7360 2023-04-19 02:19:29.638089 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/bibs_transformer.py
--rw-r--r--   0        0        0     5776 2023-03-06 22:17:01.821528 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/courses_migrator.py
--rw-r--r--   0        0        0    19445 2023-05-03 19:02:35.480285 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py
--rw-r--r--   0        0        0     9602 2023-04-19 02:19:29.644858 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py
--rw-r--r--   0        0        0    14990 2023-04-17 23:01:11.562933 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/items_transformer.py
--rw-r--r--   0        0        0    32162 2023-05-03 19:02:35.303753 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/loans_migrator.py
--rw-r--r--   0        0        0     7846 2023-05-03 19:02:35.242340 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/manual_fee_fines_transformer.py
--rw-r--r--   0        0        0    13319 2023-05-03 19:02:35.242626 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/migration_task_base.py
--rw-r--r--   0        0        0    10831 2023-04-30 20:40:23.950774 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/orders_transformer.py
--rw-r--r--   0        0        0    14387 2023-03-06 22:17:01.823616 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/organization_transformer.py
--rw-r--r--   0        0        0    12990 2023-03-06 22:17:01.823855 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/requests_migrator.py
--rw-r--r--   0        0        0     8868 2023-05-03 19:02:35.304239 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/reserves_migrator.py
--rw-r--r--   0        0        0     9305 2023-03-06 22:17:01.824396 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/user_transformer.py
--rw-r--r--   0        0        0    15870 2023-05-03 19:02:35.243912 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/report_blurbs.py
--rw-r--r--   0        0        0      255 2023-03-06 22:17:01.824926 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/task_configuration.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.830348 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/test_infrastructure/__init__.py
--rw-r--r--   0        0        0     8199 2023-05-03 19:02:35.244774 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/test_infrastructure/mocked_classes.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.831318 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/__init__.py
--rw-r--r--   0        0        0     5405 2023-03-06 22:17:01.831654 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/legacy_loan.py
--rw-r--r--   0        0        0     6124 2023-03-06 22:17:01.831928 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/legacy_request.py
--rw-r--r--   0        0        0     1839 2023-03-06 22:17:01.832344 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/legacy_reserve.py
--rw-r--r--   0        0        0      656 2023-03-06 22:17:01.832638 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/transaction_result.py
--rw-r--r--   0        0        0     5623 1970-01-01 00:00:00.000000 folio_migration_tools-1.8.0rc7/setup.py
--rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 folio_migration_tools-1.8.0rc7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-06 22:17:01.793515 folio_migration_tools-1.8.0rc8/LICENSE
+-rw-r--r--   0        0        0     4193 2023-03-21 14:28:28.887645 folio_migration_tools-1.8.0rc8/README.md
+-rw-r--r--   0        0        0     1748 2023-05-15 11:37:25.726916 folio_migration_tools-1.8.0rc8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.810173 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/__init__.py
+-rw-r--r--   0        0        0     5322 2023-05-15 11:23:50.124863 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/__main__.py
+-rw-r--r--   0        0        0    14007 2023-05-15 11:23:50.267365 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/circulation_helper.py
+-rw-r--r--   0        0        0      227 2023-03-06 22:17:01.811146 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/colors.py
+-rw-r--r--   0        0        0      648 2023-03-06 22:17:01.811423 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/custom_dict.py
+-rw-r--r--   0        0        0     2488 2023-05-15 11:23:50.020165 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/custom_exceptions.py
+-rw-r--r--   0        0        0     1678 2023-03-06 22:17:01.812068 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/extradata_writer.py
+-rw-r--r--   0        0        0     6573 2023-03-06 22:17:01.812324 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/folder_structure.py
+-rw-r--r--   0        0        0     2550 2023-03-06 22:17:01.812602 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/helper.py
+-rw-r--r--   0        0        0     7089 2023-03-06 22:17:01.812878 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/holdings_helper.py
+-rw-r--r--   0        0        0     2636 2023-04-18 23:46:20.197850 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/library_configuration.py
+-rw-r--r--   0        0        0    19557 2023-05-15 11:23:50.020857 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapper_base.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.813766 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/__init__.py
+-rw-r--r--   0        0        0     8117 2023-04-19 02:19:29.600062 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py
+-rw-r--r--   0        0        0     6423 2023-04-19 02:19:29.616368 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py
+-rw-r--r--   0        0        0    10080 2023-05-03 19:02:35.234989 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/item_mapper.py
+-rw-r--r--   0        0        0    13432 2023-05-15 11:23:50.021671 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/manual_fee_fines_mapper.py
+-rw-r--r--   0        0        0    37969 2023-05-15 11:23:50.022160 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py
+-rw-r--r--   0        0        0     3456 2023-05-15 11:23:50.022533 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py
+-rw-r--r--   0        0        0    16822 2023-05-15 11:23:50.080287 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/order_mapper.py
+-rw-r--r--   0        0        0    14644 2023-05-15 11:23:50.103757 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py
+-rw-r--r--   0        0        0     8855 2023-05-03 19:02:35.238368 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py
+-rw-r--r--   0        0        0     7683 2023-04-19 02:19:29.634576 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/user_mapper.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.816647 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/__init__.py
+-rw-r--r--   0        0        0    34047 2023-04-18 23:46:20.215442 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/conditions.py
+-rw-r--r--   0        0        0    11297 2023-03-06 22:17:01.817193 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py
+-rw-r--r--   0        0        0     9386 2023-05-15 11:23:50.081780 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py
+-rw-r--r--   0        0        0   382912 2023-03-06 22:17:01.818293 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml
+-rw-r--r--   0        0        0    10697 2023-05-15 11:23:50.218672 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py
+-rw-r--r--   0        0        0     4962 2023-03-06 22:17:01.818809 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py
+-rw-r--r--   0        0        0     5850 2023-03-27 22:22:56.116126 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py
+-rw-r--r--   0        0        0    34454 2023-04-17 23:01:11.524015 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py
+-rw-r--r--   0        0        0    25845 2023-04-17 23:01:11.525499 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py
+-rw-r--r--   0        0        0    17417 2023-04-17 23:01:11.530990 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py
+-rw-r--r--   0        0        0     4084 2023-03-06 22:17:01.820137 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_report.py
+-rw-r--r--   0        0        0      211 2023-03-06 22:17:01.820491 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/__init__.py
+-rw-r--r--   0        0        0     4231 2023-04-17 23:01:11.544786 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/authority_transformer.py
+-rw-r--r--   0        0        0    28090 2023-05-15 11:23:50.202973 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/batch_poster.py
+-rw-r--r--   0        0        0     7360 2023-04-19 02:19:29.638089 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/bibs_transformer.py
+-rw-r--r--   0        0        0     5776 2023-03-06 22:17:01.821528 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/courses_migrator.py
+-rw-r--r--   0        0        0    19445 2023-05-15 11:23:50.252409 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py
+-rw-r--r--   0        0        0     9602 2023-04-19 02:19:29.644858 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py
+-rw-r--r--   0        0        0    14990 2023-04-17 23:01:11.562933 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/items_transformer.py
+-rw-r--r--   0        0        0    32162 2023-05-15 11:23:50.083455 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/loans_migrator.py
+-rw-r--r--   0        0        0     7325 2023-05-15 11:23:50.028181 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/manual_fee_fines_transformer.py
+-rw-r--r--   0        0        0    13448 2023-05-15 11:23:50.029279 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/migration_task_base.py
+-rw-r--r--   0        0        0    11392 2023-05-15 11:23:50.030013 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/orders_transformer.py
+-rw-r--r--   0        0        0    14832 2023-05-15 11:23:50.030305 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/organization_transformer.py
+-rw-r--r--   0        0        0    12990 2023-03-06 22:17:01.823855 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/requests_migrator.py
+-rw-r--r--   0        0        0     8868 2023-05-15 11:23:50.084036 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/reserves_migrator.py
+-rw-r--r--   0        0        0     9919 2023-05-15 11:23:50.032346 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/user_transformer.py
+-rw-r--r--   0        0        0    16086 2023-05-15 11:23:50.033320 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/report_blurbs.py
+-rw-r--r--   0        0        0      255 2023-03-06 22:17:01.824926 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/task_configuration.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.830348 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/test_infrastructure/__init__.py
+-rw-r--r--   0        0        0     9150 2023-05-15 11:23:50.033592 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/test_infrastructure/mocked_classes.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.831318 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/__init__.py
+-rw-r--r--   0        0        0     5405 2023-03-06 22:17:01.831654 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/legacy_loan.py
+-rw-r--r--   0        0        0     6124 2023-03-06 22:17:01.831928 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/legacy_request.py
+-rw-r--r--   0        0        0     1839 2023-03-06 22:17:01.832344 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/legacy_reserve.py
+-rw-r--r--   0        0        0      656 2023-03-06 22:17:01.832638 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/transaction_result.py
+-rw-r--r--   0        0        0     5623 1970-01-01 00:00:00.000000 folio_migration_tools-1.8.0rc8/setup.py
+-rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 folio_migration_tools-1.8.0rc8/PKG-INFO
```

### Comparing `folio_migration_tools-1.8.0rc7/LICENSE` & `folio_migration_tools-1.8.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/README.md` & `folio_migration_tools-1.8.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/pyproject.toml` & `folio_migration_tools-1.8.0rc8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "folio_migration_tools"
-version = "1.8.0rc7"
+version = "1.8.0rc8"
 description =  "A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP"
 authors = ["Theodor Tolstoy <github.teddes@tolstoy.se>", "Lisa Sjögren", "Brooks Travis"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/FOLIO-FSE/folio_migration_tools"
 repository = "https://github.com/FOLIO-FSE/folio_migration_tools"
 keywords = ["FOLIO", "ILS", "LSP", "Library Systems", "MARC21", "Library data"]
```

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/__main__.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/circulation_helper.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/circulation_helper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/custom_dict.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/custom_dict.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/custom_exceptions.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/custom_exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,26 +54,27 @@
             self.index_or_id,
             self.message,
             self.data_value,
         )
 
 
 class TransformationProcessError(TransfomationError):
-    """Raised when the mapping fails due to disconnects in ref data.
-    This error should take the process to a halt"""
+    """Raised when the transformation fails due to incorrect configuraiton,
+    mapping or reference data. This error should take the process to a halt."""
 
     def __init__(
         self,
         index_or_id,
-        message="Critical Process issue. Transformation failed.",
+        message="Critical Process issue. Transformation failed."
+        " Check configuration, mapping files and reference data",
         data_value="",
     ):
         self.index_or_id = index_or_id
         self.message = message
         self.data_value = data_value
         super().__init__(self.message)
 
     def __str__(self):
         return (
-            f"Critical Process issue. Check mapping files and reference data "
+            f"Critical Process issue. Check configuration, mapping files and reference data"
             f"\t{self.index_or_id}\t{self.message}\t{self.data_value}"
         )
```

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/extradata_writer.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/extradata_writer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/folder_structure.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/folder_structure.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/helper.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/helper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/holdings_helper.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/holdings_helper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/library_configuration.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/library_configuration.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapper_base.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapper_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,17 @@
         logging.critical("%s\t%s", idx, error)
         print(f"\n{error.message}: {error.data_value}")
         sys.exit(1)
 
     def handle_transformation_record_failed_error(
         self, records_processed: int, error: TransformationRecordFailedError
     ):
-        self.migration_report.add(Blurbs.GeneralStatistics, "Records failed due to an error")
+        self.migration_report.add(
+            Blurbs.GeneralStatistics, "FAILED Records failed due to an error"
+        )
         error.index_or_id = error.index_or_id or records_processed
         error.log_it()
         self.num_criticalerrors += 1
         if (
             self.num_criticalerrors / (records_processed + 1)
             > (self.library_configuration.failed_percentage_threshold / 100)
             and self.num_criticalerrors > self.library_configuration.failed_records_threshold
```

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/item_mapper.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/item_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/manual_fee_fines_mapper.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/orders_transformer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,276 +1,267 @@
-import uuid
-from typing import Any
-from typing import Dict
-
-from dateutil.parser import parse
-from folio_uuid.folio_uuid import FOLIONamespaces
-from folioclient import FolioClient
+import csv
+import ctypes
+import json
+import logging
+import sys
+import time
+from os.path import isfile
+from typing import List
+from typing import Optional
+
+from deepdiff import DeepDiff
+from folio_uuid.folio_namespaces import FOLIONamespaces
+from pydantic.main import BaseModel
 
-from folio_migration_tools.custom_exceptions import TransformationFieldMappingError
+from folio_migration_tools.custom_exceptions import TransformationProcessError
 from folio_migration_tools.custom_exceptions import TransformationRecordFailedError
+from folio_migration_tools.helper import Helper
+from folio_migration_tools.library_configuration import FileDefinition
 from folio_migration_tools.library_configuration import LibraryConfiguration
 from folio_migration_tools.mapping_file_transformation.mapping_file_mapper_base import (
     MappingFileMapperBase,
 )
-from folio_migration_tools.mapping_file_transformation.ref_data_mapping import (
-    RefDataMapping,
+from folio_migration_tools.mapping_file_transformation.order_mapper import (
+    CompositeOrderMapper,
 )
+from folio_migration_tools.migration_tasks.migration_task_base import MigrationTaskBase
 from folio_migration_tools.report_blurbs import Blurbs
 
+csv.field_size_limit(int(ctypes.c_ulong(-1).value // 2))
+
+
+# Read files and do some work
+class OrdersTransformer(MigrationTaskBase):
+    class TaskConfiguration(BaseModel):
+        name: str
+        migration_task_type: str
+        files: List[FileDefinition]
+        orders_mapping_file_name: str
+        organizations_code_map_file_name: str
+        acquisition_method_map_file_name: str
+        payment_status_map_file_name: Optional[str] = ""
+        receipt_status_map_file_name: Optional[str] = ""
+        workflow_status_map_file_name: Optional[str] = ""
+        location_map_file_name: Optional[str] = ""
+        funds_map_file_name: Optional[str] = ""
+        funds_expense_class_map_file_name: Optional[str] = ""
+
+    @staticmethod
+    def get_object_type() -> FOLIONamespaces:
+        return FOLIONamespaces.orders
 
-class ManualFeeFinesMapper(MappingFileMapperBase):
     def __init__(
         self,
-        folio_client: FolioClient,
-        library_configuration: LibraryConfiguration,
-        task_configuration,
-        feefines_map,
-        feefines_owner_map,
-        feefines_type_map,
-        service_point_map,
-        ignore_legacy_identifier: bool = True,
+        task_config: TaskConfiguration,
+        library_config: LibraryConfiguration,
+        use_logging: bool = True,
     ):
-        self.folio_client: FolioClient = folio_client
-        self.user_cache: dict = {}
-        self.item_cache: dict = {}
-        self.composite_feefine_schema = self.get_composite_feefine_schema()
-
-        self.task_configuration = task_configuration
-
-        super().__init__(
-            folio_client,
-            self.composite_feefine_schema,
-            feefines_map,
-            None,
-            FOLIONamespaces.fees_fines,
-            library_configuration,
-            ignore_legacy_identifier,
-        )
-
-        self.feefines_map = feefines_map
+        csv.register_dialect("tsv", delimiter="\t")
 
-        if feefines_owner_map:
-            self.feefines_owner_map = RefDataMapping(
-                self.folio_client,
-                "/owners",
-                "owners",
-                feefines_owner_map,
-                "owner",
-                Blurbs.FeeFineOnwerMapping,
-            )
-        else:
-            self.feefines_owner_map = None
+        super().__init__(library_config, task_config, use_logging)
+        self.object_type_name = self.get_object_type().name
+        self.task_config = task_config
+        self.files = self.list_source_files()
+        self.total_records = 0
+        self.current_folio_record: dict = {}
+        self.orders_map = self.setup_records_map(
+            self.folder_structure.mapping_files_folder / self.task_config.orders_mapping_file_name
+        )
+        self.results_path = self.folder_structure.created_objects_path
+        self.failed_files: List[str] = []
 
-        if feefines_type_map:
-            self.feefines_type_map = RefDataMapping(
-                self.folio_client,
-                "/feefines",
-                "feefines",
-                feefines_type_map,
-                "feeFineType",
-                Blurbs.FeeFineTypesMapping,
-            )
-        else:
-            self.feefines_type_map = None
+        self.folio_keys = []
+        self.folio_keys = MappingFileMapperBase.get_mapped_folio_properties_from_map(
+            self.orders_map
+        )
+        self.minted_ids: set = set()
 
-        if service_point_map:
-            self.service_point_map = RefDataMapping(
-                self.folio_client,
-                "/service-points",
-                "servicepoints",
-                service_point_map,
-                "name",
-                Blurbs.FeeFineServicePointTypesMapping,
-            )
-        else:
-            self.service_point_map = None
+        self.mapper = CompositeOrderMapper(
+            self.folio_client,
+            self.library_configuration,
+            self.orders_map,
+            self.load_id_map(self.folder_structure.organizations_id_map_path, True),
+            self.load_id_map(self.folder_structure.instance_id_map_path, True),
+            self.load_ref_data_mapping_file(
+                "acquisitionMethod",
+                self.folder_structure.mapping_files_folder
+                / self.task_config.acquisition_method_map_file_name,
+                self.folio_keys,
+            ),
+            self.load_ref_data_mapping_file(  # Not required, on POL
+                "paymentStatus",
+                self.folder_structure.mapping_files_folder
+                / self.task_config.payment_status_map_file_name,
+                self.folio_keys,
+                False,
+            ),
+            self.load_ref_data_mapping_file(  # Not required, on POL
+                "receiptStatus",
+                self.folder_structure.mapping_files_folder
+                / self.task_config.receipt_status_map_file_name,
+                self.folio_keys,
+                False,
+            ),
+            self.load_ref_data_mapping_file(  # Not required
+                "workflowStatus",
+                self.folder_structure.mapping_files_folder
+                / self.task_config.workflow_status_map_file_name,
+                self.folio_keys,
+                False,
+            ),
+            self.load_ref_data_mapping_file(
+                "locationMap",
+                self.folder_structure.mapping_files_folder
+                / self.task_config.location_map_file_name,
+                self.folio_keys,
+                False,
+            ),
+            self.load_ref_data_mapping_file(  # Required if there was is a fund.
+                "fundsMap",
+                self.folder_structure.mapping_files_folder / self.task_config.funds_map_file_name,
+                self.folio_keys,
+                False,
+            ),
+            self.load_ref_data_mapping_file(  # Todo: The property in the schema has no type
+                "fundsExpenseClassMap",
+                self.folder_structure.mapping_files_folder
+                / self.task_config.funds_expense_class_map_file_name,
+                self.folio_keys,
+                False,
+            ),
+        )
 
-    def store_objects(self, composite_feefine):
-        try:
-            self.extradata_writer.write("account", composite_feefine["account"])
-            self.migration_report.add_general_statistics("Stored account")
-            self.extradata_writer.write("feefineaction", composite_feefine["feefineaction"])
-            self.migration_report.add_general_statistics("Stored feefineactions")
-
-        except Exception as ee:
-            raise TransformationRecordFailedError(
-                composite_feefine, "Failed when storing", ee
-            ) from ee
-
-    def get_prop(self, legacy_object, folio_prop_name, index_or_id, schema_default_value):
-        if folio_prop_name == "account.id" or folio_prop_name == "feefineaction.accountId":
-            return index_or_id
-
-        elif folio_prop_name == "account.amount" or folio_prop_name == "account.remaining":
-            return self.parse_sum_as_float(
-                index_or_id,
-                super().get_prop(
-                    legacy_object, folio_prop_name, index_or_id, schema_default_value
-                ),
-                folio_prop_name,
+    def list_source_files(self):
+        files = [
+            self.folder_structure.data_folder / self.object_type_name / f.file_name
+            for f in self.task_config.files
+            if isfile(self.folder_structure.data_folder / self.object_type_name / f.file_name)
+        ]
+        if not any(files):
+            ret_str = ",".join(f.file_name for f in self.task_config.files)
+            raise TransformationProcessError(
+                f"Files {ret_str} not found in"
+                "{self.folder_structure.data_folder} / {self.object_type_name}"
             )
-
-        elif folio_prop_name == "account.ownerId" and self.feefines_owner_map:
-            return self.get_mapped_ref_data_value(
-                self.feefines_owner_map, legacy_object, index_or_id, folio_prop_name, False
+        logging.info("Files to process:")
+        for filename in files:
+            logging.info("\t%s", filename)
+        return files
+
+    def process_single_file(self, filename):
+        with open(filename, encoding="utf-8-sig") as records_file, open(
+            self.folder_structure.created_objects_path, "w+"
+        ) as results_file:
+            self.mapper.migration_report.add_general_statistics("Number of files processed")
+            start = time.time()
+            records_processed = 0
+            for idx, record in enumerate(self.mapper.get_objects(records_file, filename)):
+                records_processed += 1
+
+                try:
+                    # Print first legacy record, then first transformed record
+                    if idx == 0:
+                        logging.info("First legacy record:")
+                        logging.info(json.dumps(record, indent=4))
+
+                    folio_rec, legacy_id = self.mapper.do_map(
+                        record, f"row {idx}", FOLIONamespaces.orders, True
+                    )
+                    self.mapper.perform_additional_mapping(legacy_id, folio_rec)
+
+                    self.mapper.migration_report.add_general_statistics(
+                        "TOTAL Purchase Order Lines created"
+                    )
+                    self.mapper.report_folio_mapping(folio_rec, self.mapper.composite_order_schema)
+                    self.mapper.notes_mapper.map_notes(
+                        record,
+                        legacy_id,
+                        folio_rec["id"],
+                        FOLIONamespaces.orders,
+                    )
+
+                    self.merge_into_orders_with_embedded_pols(folio_rec, results_file)
+
+                except TransformationProcessError as process_error:
+                    self.mapper.handle_transformation_process_error(idx, process_error)
+                except TransformationRecordFailedError as error:
+                    self.mapper.handle_transformation_record_failed_error(idx, error)
+                except Exception as excepion:
+                    self.mapper.handle_generic_exception(idx, excepion)
+
+                # TODO Rewrite to base % value on number of rows in file
+                if idx > 1 and idx % 50 == 0:
+                    elapsed = idx / (time.time() - start)
+                    elapsed_formatted = "{0:.4g}".format(elapsed)
+                    logging.info(  # pylint: disable=logging-fstring-interpolation
+                        f"{idx:,} records processed. Recs/sec: {elapsed_formatted} "
+                    )
+
+            self.total_records = records_processed
+
+            logging.info(  # pylint: disable=logging-fstring-interpolation
+                f"Done processing {filename} containing {self.total_records:,} records. "
+                f"Total records processed: {self.total_records:,}"
             )
-
-        elif folio_prop_name == "account.feeFineId" and self.feefines_type_map:
-            return self.get_mapped_ref_data_value(
-                self.feefines_type_map, legacy_object, index_or_id, folio_prop_name, False
+            logging.info("Storing last record to disk")
+            Helper.write_to_file(results_file, self.current_folio_record)
+            self.mapper.migration_report.add_general_statistics("TOTAL Purchase Orders created")
+
+    def do_work(self):
+        logging.info("Getting started!")
+        for file in self.files:
+            logging.info("Processing %s", file)
+            try:
+                print(file)
+                self.process_single_file(file)
+            except Exception as ee:
+                error_str = (
+                    f"Processing of {file} failed:\n{ee}."
+                    "Check source files for empty lines or missing reference data"
+                )
+                logging.exception(error_str)
+                self.mapper.migration_report.add(Blurbs.FailedFiles, f"{file} - {ee}")
+                sys.exit()
+
+    def wrap_up(self):
+        logging.info("Done. Wrapping up...")
+        with open(self.folder_structure.migration_reports_file, "w") as migration_report_file:
+            logging.info(
+                "Writing migration- and mapping report to %s",
+                self.folder_structure.migration_reports_file,
             )
-
-        elif folio_prop_name == "account.userId" or folio_prop_name == "feefineaction.userId":
-            return self.get_matching_record_from_folio(
-                index_or_id,
-                self.user_cache,
-                "/users",
-                "barcode",
-                super().get_prop(
-                    legacy_object, folio_prop_name, index_or_id, schema_default_value
-                ),
-                "users",
-            )["id"]
-
-        elif folio_prop_name == "feefineaction.id":
-            return str(uuid.uuid4())
-
-        elif folio_prop_name == "feefineaction.createdAt" and self.service_point_map:
-            return self.get_mapped_ref_data_value(
-                self.service_point_map, legacy_object, index_or_id, folio_prop_name, False
+            self.mapper.migration_report.write_migration_report(
+                "Pruchase Orders and Purchase Order Lines Transformation Report",
+                migration_report_file,
+                self.start_datetime,
             )
 
-        elif folio_prop_name == "feefineaction.dateAction":
-            return self.parse_date(
-                folio_prop_name,
-                index_or_id,
-                super().get_prop(
-                    legacy_object, folio_prop_name, index_or_id, schema_default_value
-                ),
-                legacy_object,
+            Helper.print_mapping_report(
+                migration_report_file,
+                self.total_records,
+                self.mapper.mapped_folio_fields,
+                self.mapper.mapped_legacy_fields,
             )
+        logging.info("All done!")
 
-        elif mapped_value := super().get_prop(
-            legacy_object, folio_prop_name, index_or_id, schema_default_value
-        ):
-            return mapped_value
+    def merge_into_orders_with_embedded_pols(self, folio_rec, results_file):
+        # Handle merging and storage
+        if not self.current_folio_record:
+            self.current_folio_record = folio_rec
+        if folio_rec["id"] != self.current_folio_record["id"]:
+            # Writes record to file
+            Helper.write_to_file(results_file, self.current_folio_record)
+            self.mapper.migration_report.add_general_statistics("TOTAL Purchase Orders created")
+            self.current_folio_record = folio_rec
 
         else:
-            return ""
-
-    def get_composite_feefine_schema(self) -> Dict[str, Any]:
-        return {
-            "properties": {
-                "account": FolioClient.get_latest_from_github(
-                    "folio-org", "mod-feesfines", "/ramls/accountdata.json"
-                ),
-                "feefineaction": FolioClient.get_latest_from_github(
-                    "folio-org", "mod-feesfines", "/ramls/feefineactiondata.json"
-                ),
-            }
-        }
-
-    def get_matching_record_from_folio(
-        self,
-        index_or_id,
-        cache: dict,
-        path: str,
-        match_property: str,
-        match_value: str,
-        result_type: str,
-    ):
-        if match_value not in cache:
-            query = f'?query=({match_property}=="{match_value}")'
-            if matching_record := next(
-                self.folio_client.folio_get_all(path, result_type, query), None
-            ):
-                cache[match_value] = matching_record
-                return matching_record
-            else:
-                raise TransformationFieldMappingError(
-                    index_or_id, f"No matching {result_type} for {match_property}", match_value
+            # Merge if possible
+            diff = DeepDiff(self.current_folio_record, folio_rec)
+            if "compositePoLines" in diff.affected_root_keys:
+                self.current_folio_record.get("compositePoLines", []).extend(
+                    folio_rec.get("compositePoLines", [])
                 )
-        else:
-            return cache[match_value]
-
-    def parse_date(self, folio_prop_name: str, index_or_id, mapped_value, legacy_object):
-        try:
-            format_date = parse(mapped_value, fuzzy=True)
-            return format_date.isoformat()
-        except Exception as exception:
-            raise TransformationFieldMappingError(
-                index_or_id, f"Invalid {folio_prop_name} date for {legacy_object} ", mapped_value
-            ) from exception
-
-    def parse_sum_as_float(self, index_or_id, legacy_sum, folio_prop_name):
-        try:
-            return float(legacy_sum)
-        except Exception as ee:
-            raise TransformationRecordFailedError(
-                index_or_id,
-                f"Values mapped to '{folio_prop_name}' may only contain numbers/decimals.",
-                legacy_sum,
-            ) from ee
-
-    def perform_additional_mapping(self, index_or_id, feefine, legacy_object):
-        # Add some name values to ensure nice UI behaviour
-        feefine["account"]["feeFineOwner"] = [
-            owner["owner"]
-            for owner in self.feefines_owner_map.ref_data
-            if owner["id"] == feefine["account"]["ownerId"]
-        ][0]
-
-        type_name = [
-            type["feeFineType"]
-            for type in self.feefines_type_map.ref_data
-            if type["id"] == feefine["account"]["feeFineId"]
-        ][0]
-        feefine["account"]["feeFineType"] = type_name
-        feefine["feefineaction"]["typeAction"] = type_name
-
-        feefine["feefineaction"]["source"] = self.folio_client.username
-        feefine["feefineaction"]["notify"] = False
-        feefine["feefineaction"]["amountAction"] = feefine["account"]["amount"]
-        feefine["feefineaction"]["balance"] = feefine["account"]["remaining"]
-
-        # Add item data from FOLIO if available
-        if folio_item := self.get_matching_record_from_folio(
-            index_or_id,
-            self.item_cache,
-            "/inventory/items",
-            "barcode",
-            super().get_prop(legacy_object, "account.itemId", "", ""),
-            "items",
-        ):
-
-            feefine["account"]["itemId"] = folio_item.get("id", "")
-            feefine["account"]["title"] = folio_item.get("title", "")
-            feefine["account"]["barcode"] = folio_item.get("barcode", "")
-            feefine["account"]["callNumber"] = folio_item.get("callNumber", "")
-            feefine["account"]["materialType"] = folio_item.get("materialType", {}).get("name")
-            feefine["account"]["materialTypeId"] = folio_item.get("materialType", {}).get("id")
-            feefine["account"]["location"] = folio_item.get("effectiveLocation", {}).get("name")
-        else:
-            feefine["account"].pop("itemId")
-
-        # Add the full legacy item dict to the comment field
-        if feefine["feefineaction"].get("comments"):
-            feefine["feefineaction"]["comments"] = (
-                ("STAFF : " + feefine["feefineaction"]["comments"])
-                + " "
-                + self.stringify_legacy_object(legacy_object)
-            )
-
-        else:
-            feefine["feefineaction"]["comments"] = self.stringify_legacy_object(legacy_object)
-
-        return feefine
-
-    def stringify_legacy_object(self, legacy_object):
-        legacy_string = (
-            "MIGRATION NOTE : This fee/fine was migrated to FOLIO from a previous "
-            "library management system. The following is the original data: "
-        )
-        for key, value in legacy_object.items():
-            legacy_string += f"{key.title()}: {value}; "
-        return legacy_string.strip().strip(";")
+                self.mapper.migration_report.add_general_statistics(
+                    "Rows merged to create Purchase Orders"
+                )
+            for key in diff.affected_paths:
+                self.mapper.migration_report.add(Blurbs.DiffsBetweenOrders, key)
```

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,21 @@
         self,
         legacy_object: dict,
         index_or_id,
         object_type: FOLIONamespaces,
         accept_duplicate_ids: bool = False,
     ):
         if self.ignore_legacy_identifier:
-            return ({}, str(uuid.uuid4()))
+            return (
+                {
+                    "id": str(uuid.uuid4()),
+                    "type": "object",
+                },
+                index_or_id,
+            )
 
         if not (
             legacy_id := " ".join(
                 legacy_object.get(li, "") for li in self.legacy_id_property_names
             ).strip()
         ):
             raise TransformationRecordFailedError(
@@ -249,21 +255,29 @@
         )
         if not any(map_entries):
             return ""
         elif len(map_entries) > 1:
             self.migration_report.add(Blurbs.Details, f"{legacy_item_keys} were concatenated")
             return " ".join(
                 MappingFileMapperBase.get_legacy_value(
-                    legacy_object, map_entry, self.migration_report, index_or_id
+                    legacy_object,
+                    map_entry,
+                    self.migration_report,
+                    index_or_id,
+                    self.library_configuration.multi_field_delimiter,
                 )
                 for map_entry in map_entries
             ).strip()
         else:
             legacy_value = MappingFileMapperBase.get_legacy_value(
-                legacy_object, map_entries[0], self.migration_report, index_or_id
+                legacy_object,
+                map_entries[0],
+                self.migration_report,
+                index_or_id,
+                self.library_configuration.multi_field_delimiter,
             )
             if legacy_value or isinstance(legacy_value, bool):
                 return legacy_value
             else:
                 self.migration_report.add(
                     Blurbs.FolioDefaultValuesAdded,
                     f"{schema_default_value} added to {folio_prop_name}",
@@ -344,14 +358,15 @@
 
     @staticmethod
     def get_legacy_value(
         legacy_object: dict,
         mapping_file_entry: dict,
         migration_report: MigrationReport,
         index_or_id: str = "",
+        multi_field_delimiter="",
     ):
         # Mapping from value fields has preceedence and does not get involved in post processing
         if mapping_file_entry.get("value", "") or isinstance(
             mapping_file_entry.get("value", ""), bool
         ):
             value_mapped_value = mapping_file_entry.get("value")
             migration_report.add(
@@ -360,15 +375,24 @@
             )
             return value_mapped_value
 
         # Value mapped from the Legacy field(s)
         value = legacy_object.get(mapping_file_entry["legacy_field"], "")
 
         if value and mapping_file_entry.get("rules", {}).get("replaceValues", {}):
-            if replaced_val := mapping_file_entry["rules"]["replaceValues"].get(value, ""):
+            if multi_field_delimiter and multi_field_delimiter in value:
+                replaced_split_values = [
+                    mapping_file_entry["rules"]["replaceValues"].get(sv, "")
+                    for sv in value.split(multi_field_delimiter)
+                ]
+                replaced_val = multi_field_delimiter.join(replaced_split_values)
+            else:
+                replaced_val = mapping_file_entry["rules"]["replaceValues"].get(value, "")
+
+            if replaced_val or isinstance(replaced_val, bool):
                 migration_report.add(
                     Blurbs.FieldMappingDetails,
                     (
                         f"Replaced {value} in {mapping_file_entry['legacy_field']} "
                         f"with {replaced_val}"
                     ),
                 )
@@ -680,18 +704,20 @@
         return total_rows, empty_rows, dict_reader
 
     def get_objects(self, source_file, file_name: Path):
         total_rows, empty_rows, reader = self._get_delimited_file_reader(source_file, file_name)
         logging.info("Source data file contains %d rows", total_rows)
         logging.info("Source data file contains %d empty rows", empty_rows)
         self.migration_report.set(
-            Blurbs.GeneralStatistics, "Total rows in {}".format(file_name.name), total_rows
+            Blurbs.GeneralStatistics, "Number of rows in {}".format(file_name.name), total_rows
         )
         self.migration_report.set(
-            Blurbs.GeneralStatistics, "Empty rows in {}".format(file_name.name), empty_rows
+            Blurbs.GeneralStatistics,
+            "Number of empty rows in {}".format(file_name.name),
+            empty_rows,
         )
         try:
             yield from reader
         except Exception as exception:
             logging.error("%s at row %s", exception, reader.line_num)
             raise exception from exception
```

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,16 +59,15 @@
                     if "type" in note:
                         del note["type"]
                     self.extradata_writer.write("notes", note)
                     self.migration_report.add_general_statistics("Number of linked notes created")
                     self.migration_report.add(Blurbs.MappedNoteTypes, note["typeId"])
                 else:
                     self.migration_report.add_general_statistics(
-                        "Notes without content that were discarded. Set some default "
-                        "value if you only intend to set the note title"
+                        "Number of discarded notes with no content"
                     )
 
     def get_notes_schema(self):
         notes_schema = self.folio_client.get_from_github(
             "folio-org",
             "mod-notes",
             "src/main/resources/swagger.api/schemas/note.yaml",
```

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/order_mapper.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/order_mapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import uuid
 
 import httpx
 from folio_uuid.folio_uuid import FOLIONamespaces
 from folioclient import FolioClient
 from httpx import HTTPError
 
+from folio_migration_tools.custom_exceptions import TransformationRecordFailedError
 from folio_migration_tools.helper import Helper
 from folio_migration_tools.library_configuration import LibraryConfiguration
 from folio_migration_tools.mapping_file_transformation.mapping_file_mapper_base import (
     MappingFileMapperBase,
 )
 from folio_migration_tools.mapping_file_transformation.notes_mapper import NotesMapper
 from folio_migration_tools.mapping_file_transformation.ref_data_mapping import (
@@ -25,38 +26,42 @@
 
 class CompositeOrderMapper(MappingFileMapperBase):
     def __init__(
         self,
         folio_client: FolioClient,
         library_configuration: LibraryConfiguration,
         composite_order_map: dict,
+        organizations_id_map: dict,
         instance_id_map: dict,
         acquisition_method_map,
         payment_status_map,
         receipt_status_map,
         workflow_status_map,
         location_map,
         funds_map,
         funds_expense_class_map=None,
     ):
         # Get organization schema
-        composite_order_schema = CompositeOrderMapper.get_latest_acq_schemas_from_github(
+        self.composite_order_schema = CompositeOrderMapper.get_latest_acq_schemas_from_github(
             "folio-org", "mod-orders", "mod-orders", "composite_purchase_order"
         )
 
         super().__init__(
             folio_client,
-            composite_order_schema,
+            self.composite_order_schema,
             composite_order_map,
             None,
             FOLIONamespaces.orders,
             library_configuration,
         )
+        logging.info("Loading Instance ID map...")
         self.instance_id_map = instance_id_map
-        self.vendor_code_map = dict(self.setup_vendor_code_map())
+        self.organizations_id_map = organizations_id_map
+        self.folio_organization_cache = {}
+
         self.acquisitions_methods_mapping = RefDataMapping(
             self.folio_client,
             "/orders/acquisition-methods",
             "acquisitionMethods",
             acquisition_method_map,
             "value",
             Blurbs.AcquisitionMethodMapping,
@@ -79,70 +84,42 @@
             FOLIONamespaces.note,
             True,
         )
         self.notes_mapper.migration_report = self.migration_report
 
     def get_prop(self, legacy_order, folio_prop_name: str, index_or_id, schema_default_value):
         if folio_prop_name.endswith(".acquisitionMethod"):
-            mapped_val = self.acquisitions_methods_mapping.get_ref_data_mapping(legacy_order)
-            return mapped_val["folio_id"]
+            return self.get_mapped_ref_data_value(
+                self.acquisitions_methods_mapping,
+                legacy_order,
+                folio_prop_name,
+                index_or_id,
+                False,
+            )
 
         elif re.compile(r"compositePoLines\[(\d+)\]\.id").fullmatch(folio_prop_name):
             return str(uuid.uuid4())
 
         elif re.compile(r"notes\[\d+\]\.").match(folio_prop_name):
             return ""
 
-        mapped_value = super().get_prop(
-            legacy_order, folio_prop_name, index_or_id, schema_default_value
-        )
-
         if folio_prop_name.endswith(".locationId"):
             return self.get_mapped_ref_data_value(
                 self.location_mapping,
                 legacy_order,
                 folio_prop_name,
                 index_or_id,
                 False,
             )
 
-        if folio_prop_name == "vendor":
-            if mapped_value in self.vendor_code_map:
-                self.migration_report.add_general_statistics(
-                    "Successfully matched Vendor against code"
-                )
-                return self.vendor_code_map[mapped_value]
-            else:
-                self.migration_report.add_general_statistics("Orders without assigned vendor")
-                Helper.log_data_issue(
-                    index_or_id, "Vendor code not found among migrated Organizations", mapped_value
-                )
-
-        elif folio_prop_name.endswith(".instanceId"):
-            if mapped_value in self.instance_id_map:
-                self.migration_report.add_general_statistics(
-                    "Instance ID mapped from previously migrated bib records"
-                )
-                return self.instance_id_map.get(mapped_value)[1]
-            else:
-                self.migration_report.add_general_statistics(
-                    "Bib id not found in list over migrated bibs."
-                )
-                Helper.log_data_issue(
-                    index_or_id, "Bib id not found in list over migrated bibs.", mapped_value
-                )
-        return mapped_value
+        mapped_value = super().get_prop(
+            legacy_order, folio_prop_name, index_or_id, schema_default_value
+        )
 
-    def setup_vendor_code_map(self):
-        yield from [
-            (entry["code"], entry["id"])
-            for entry in self.folio_client.get_all(
-                "/organizations-storage/organizations", "organizations"
-            )
-        ]
+        return mapped_value
 
     @staticmethod
     def get_latest_acq_schemas_from_github(owner, repo, module, object):
         """
         Given a repository owner, a repository, a module name and the name
         of a FOLIO acquisition object, returns a schema for that object that
         also includes the schemas of any other referenced acq objects.
@@ -334,15 +311,15 @@
                         actual_path, github_headers, property_level1
                     )
                     p2 = CompositeOrderMapper.build_extended_object(
                         p1, actual_path, github_headers
                     )
                     property_level1["items"] = p2
                 elif property_level1.get("type") == "string" and property_level1.get("$ref"):
-                    logging.info("Fecthing referenced schema for object %s", property_name_level1)
+                    logging.info("Fetching referenced schema for object %s", property_name_level1)
                     actual_path = urllib.parse.urljoin(
                         f"{submodule_path}", object_schema.get("$ref", "")
                     )
                     p1 = CompositeOrderMapper.inject_schema_by_ref(
                         actual_path, github_headers, property_level1
                     )
                     object_schema["properties"][property_name_level1] = p1
@@ -381,7 +358,91 @@
                 schema_url, headers=github_headers, follow_redirects=True, timeout=None
             )
             req.raise_for_status()
             return dict(property["items"], **json.loads(req.text))
         except Exception as ee:
             logging.error(ee)
             return {}
+
+    def perform_additional_mapping(self, index_or_id, composite_order):
+        # Get organization UUID from FOLIO
+        composite_order["vendor"] = self.get_folio_organization_uuid(
+            index_or_id, composite_order.get("vendor")
+        )
+
+        # Replace legacy bib ID with instance UUID from map
+        bib_id = composite_order["compositePoLines"][0].pop("instanceId", "")
+        if matching_instance := self.get_folio_instance_uuid(index_or_id, bib_id):
+            composite_order["compositePoLines"][0]["instanceId"] = matching_instance
+
+        return composite_order
+
+    def get_matching_record_from_folio(
+        self,
+        index_or_id,
+        cache: dict,
+        path: str,
+        match_property: str,
+        match_value: str,
+        result_type: str,
+    ):
+        if match_value in cache:
+            return cache[match_value]
+        else:
+            query = f'?query=({match_property}=="{match_value}")'
+            if matching_record := next(
+                self.folio_client.folio_get_all(path, result_type, query), None
+            ):
+                cache[match_value] = matching_record
+                return matching_record
+
+    def get_folio_organization_uuid(self, index_or_id, org_code):
+        if self.organizations_id_map:
+            self.migration_report.add(
+                Blurbs.PurchaseOrderVendorLinking,
+                "Organizations linked using organizations_id_map",
+            )
+            if matching_org := self.organizations_id_map.get(org_code):
+                return matching_org[1]
+
+        if matching_org := self.get_matching_record_from_folio(
+            index_or_id,
+            self.folio_organization_cache,
+            "/organizations-storage/organizations",
+            "code",
+            org_code,
+            "organizations",
+        ):
+            self.migration_report.add(
+                Blurbs.PurchaseOrderVendorLinking,
+                "Organizations not in ID map, linked using FOLIO lookup",
+            )
+            return matching_org["id"]
+
+        else:
+            self.migration_report.add(
+                Blurbs.PurchaseOrderVendorLinking,
+                "RECORD FAILED Organization identifier not in ID map/FOLIO",
+            )
+            raise TransformationRecordFailedError(
+                index_or_id,
+                "No matching Organization for organization identifier",
+                org_code,
+            )
+
+    def get_folio_instance_uuid(self, index_or_id, bib_id):
+        if matching_instance := self.instance_id_map.get(bib_id):
+            self.migration_report.add(
+                Blurbs.PurchaseOrderInstanceLinking,
+                "Instances linked using instances_id_map",
+            )
+            return matching_instance[1]
+        else:
+            self.migration_report.add(
+                Blurbs.PurchaseOrderInstanceLinking,
+                "Bib identifier not in instances_id_map, no instance linked",
+            )
+            Helper.log_data_issue(
+                index_or_id,
+                "No matching instance for bib identifier",
+                bib_id,
+            )
```

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/user_mapper.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/user_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/conditions.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/conditions.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_report.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_report.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/authority_transformer.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/authority_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/batch_poster.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/batch_poster.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/bibs_transformer.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/bibs_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/courses_migrator.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/courses_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/items_transformer.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/items_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/loans_migrator.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/loans_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/manual_fee_fines_transformer.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/manual_fee_fines_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import csv
 import json
 import logging
 import sys
 import time
 import traceback
-from os.path import isfile
 from typing import List
 from typing import Optional
 
 from folio_uuid.folio_namespaces import FOLIONamespaces
 
+from folio_migration_tools.custom_exceptions import TransformationFieldMappingError
 from folio_migration_tools.custom_exceptions import TransformationProcessError
 from folio_migration_tools.custom_exceptions import TransformationRecordFailedError
 from folio_migration_tools.helper import Helper
 from folio_migration_tools.library_configuration import FileDefinition
 from folio_migration_tools.library_configuration import LibraryConfiguration
 from folio_migration_tools.mapping_file_transformation.manual_fee_fines_mapper import (
     ManualFeeFinesMapper,
@@ -47,21 +47,21 @@
         use_logging: bool = True,
     ):
         csv.register_dialect("tsv", delimiter="\t")
 
         super().__init__(library_config, task_configuration, use_logging)
         self.object_type_name = self.get_object_type().name
         self.task_configuration = task_configuration
-        self.files = self.list_source_files()
+        self.check_source_files(
+            self.folder_structure.legacy_records_folder, self.task_configuration.files
+        )
         self.total_records = 0
-
         self.feefines_map = self.setup_records_map(
             self.folder_structure.mapping_files_folder / self.task_configuration.feefines_map
         )
-
         self.results_path = self.folder_structure.created_objects_path
         self.failed_files: List[str] = []
 
         self.folio_keys = []
         self.folio_keys = MappingFileMapperBase.get_mapped_folio_properties_from_map(
             self.feefines_map
         )
@@ -91,92 +91,73 @@
                 / self.task_configuration.service_point_map,
                 self.folio_keys,
                 False,
             ),
             ignore_legacy_identifier=True,
         )
 
-    def list_source_files(self):
-        files = [
-            self.folder_structure.data_folder / self.object_type_name / f.file_name
-            for f in self.task_configuration.files
-            if isfile(self.folder_structure.data_folder / self.object_type_name / f.file_name)
-        ]
-        if not any(files):
-            ret_str = ",".join(f.file_name for f in self.task_configuration.files)
-            raise TransformationProcessError(
-                f"Files {ret_str} not found in"
-                "{self.folder_structure.data_folder} / {self.object_type_name}"
-            )
-        logging.info("Files to process:")
-        for filename in files:
-            logging.info("\t%s", filename)
-        return files
-
     def do_work(self):
         logging.info("Getting started!")
-        for file in self.files:
+        for file in self.task_configuration.files:
             logging.info("Processing %s", file)
             try:
                 self.process_single_file(file)
             except Exception as ee:
                 error_str = (
                     f"Processing of {file} failed:\n{ee}."
                     "Check source files for empty rows or missing reference data"
                 )
                 logging.exception(error_str)
                 self.mapper.migration_report.add(Blurbs.FailedFiles, f"{file} - {ee}")
                 sys.exit()
 
-    def process_single_file(self, filename):
-        with open(filename, encoding="utf-8-sig") as records_file:
+    def process_single_file(self, file_def: FileDefinition):
+        full_path = self.folder_structure.legacy_records_folder / file_def.file_name
+        with open(full_path, encoding="utf-8-sig") as records_file:
             self.mapper.migration_report.add_general_statistics("Number of files processed")
             start = time.time()
 
-            for idx, record in enumerate(self.mapper.get_objects(records_file, filename)):
+            for idx, record in enumerate(self.mapper.get_objects(records_file, full_path)):
                 try:
                     if idx == 0:
                         logging.info("First legacy record:")
                         logging.info(json.dumps(record, indent=4))
 
                     self.mapper.report_legacy_mapping_no_schema(record)
 
-                    folio_rec, legacy_id = self.mapper.do_map(
-                        record, f"row {idx}", FOLIONamespaces.fees_fines
+                    composite_feefine, legacy_id = self.mapper.do_map(
+                        record, f"Row {idx + 1}", FOLIONamespaces.fees_fines
                     )
 
-                    self.mapper.perform_additional_mapping(f"row {idx}", folio_rec, record)
+                    self.mapper.perform_additional_mapping(legacy_id, composite_feefine, record)
 
                     self.mapper.report_folio_mapping(
-                        folio_rec, self.mapper.composite_feefine_schema
+                        composite_feefine, self.mapper.composite_feefine_schema
                     )
 
-                    self.mapper.store_objects(folio_rec)
+                    self.mapper.store_objects(composite_feefine)
 
                     if idx == 0:
                         logging.info("First FOLIO record:")
-                        logging.info(json.dumps(folio_rec, indent=4))
+                        logging.info(json.dumps(composite_feefine, indent=4))
 
                 except TransformationProcessError as process_error:
                     self.mapper.handle_transformation_process_error(idx, process_error)
                 except TransformationRecordFailedError as data_error:
                     self.mapper.handle_transformation_record_failed_error(idx, data_error)
+                except TransformationFieldMappingError as mapping_error:
+                    self.mapper.handle_transformation_field_mapping_error(idx, mapping_error)
+
                 except AttributeError as attribute_error:
                     traceback.print_exc()
                     logging.fatal(attribute_error)
                     logging.info("Quitting...")
                     sys.exit(1)
-                except Exception as excepion:
-                    self.mapper.handle_generic_exception(idx, excepion)
-
-                self.mapper.migration_report.add(
-                    Blurbs.GeneralStatistics,
-                    "Number of rows in source file",
-                )
-                self.mapper.migration_report.add_general_statistics("Number of records in total")
+                except Exception as exception:
+                    self.mapper.handle_generic_exception(idx, exception)
 
                 self.print_progress(idx, start)
 
     def wrap_up(self):
         logging.info("Done. Transformer wrapping up...")
         self.extradata_writer.flush()
         with open(self.folder_structure.migration_reports_file, "w") as migration_report_file:
```

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/migration_task_base.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/migration_task_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,24 +111,27 @@
             file_defs (list[library_configuration.FileDefinition]): _description_
 
         Raises:
             TransformationProcessError: _description_
 
         """
         files = [source_path / f.file_name for f in file_defs if isfile(source_path / f.file_name)]
-        if len(files) < len(file_defs):
+        ret_str = ", ".join(f.file_name for f in file_defs)
+
+        if files and len(files) < len(file_defs):
             raise TransformationProcessError(
                 "",
-                "Not all files listed in configuration found on disk",
+                f"Some files listed in task configuration not found in {source_path}."
+                f"Listed files: {ret_str}",
             )
         if not any(files):
-            ret_str = ",".join(f.file_name for f in file_defs)
             raise TransformationProcessError(
                 "",
-                f"Files {ret_str} not found in {source_path / 'items'}",
+                f"None of the files listed in task configuration found in {source_path}."
+                f"Listed files: {ret_str}",
             )
         logging.info("Files to process:")
         for filename in files:
             logging.info("\t%s", filename)
 
     @staticmethod
     def load_id_map(map_path, raise_if_empty=False):
```

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/orders_transformer.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/reserves_migrator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,259 +1,216 @@
 import csv
-import ctypes
 import json
 import logging
 import sys
 import time
-from os.path import isfile
-from typing import List
-from typing import Optional
+import traceback
+from typing import Dict
+from urllib.error import HTTPError
 
-from deepdiff import DeepDiff
+import httpx
 from folio_uuid.folio_namespaces import FOLIONamespaces
-from pydantic.main import BaseModel
 
+from folio_migration_tools.custom_dict import InsensitiveDictReader
 from folio_migration_tools.custom_exceptions import TransformationProcessError
-from folio_migration_tools.custom_exceptions import TransformationRecordFailedError
-from folio_migration_tools.helper import Helper
 from folio_migration_tools.library_configuration import FileDefinition
 from folio_migration_tools.library_configuration import LibraryConfiguration
-from folio_migration_tools.mapping_file_transformation.mapping_file_mapper_base import (
-    MappingFileMapperBase,
-)
-from folio_migration_tools.mapping_file_transformation.order_mapper import (
-    CompositeOrderMapper,
-)
+from folio_migration_tools.migration_report import MigrationReport
 from folio_migration_tools.migration_tasks.migration_task_base import MigrationTaskBase
 from folio_migration_tools.report_blurbs import Blurbs
+from folio_migration_tools.task_configuration import AbstractTaskConfiguration
+from folio_migration_tools.transaction_migration.legacy_reserve import LegacyReserve
 
-csv.field_size_limit(int(ctypes.c_ulong(-1).value // 2))
 
-
-# Read files and do some work
-class OrdersTransformer(MigrationTaskBase):
-    class TaskConfiguration(BaseModel):
+class ReservesMigrator(MigrationTaskBase):
+    class TaskConfiguration(AbstractTaskConfiguration):
         name: str
         migration_task_type: str
-        files: List[FileDefinition]
-        orders_mapping_file_name: str
-        organizations_code_map_file_name: str
-        acquisition_method_map_file_name: str
-        payment_status_map_file_name: Optional[str] = ""
-        receipt_status_map_file_name: Optional[str] = ""
-        workflow_status_map_file_name: Optional[str] = ""
-        location_map_file_name: Optional[str] = ""
-        funds_map_file_name: Optional[str] = ""
-        funds_expense_class_map_file_name: Optional[str] = ""
+        course_reserve_file_path: FileDefinition
 
     @staticmethod
     def get_object_type() -> FOLIONamespaces:
-        return FOLIONamespaces.orders
+        return FOLIONamespaces.reserve
 
     def __init__(
         self,
-        task_config: TaskConfiguration,
+        task_configuration: TaskConfiguration,
         library_config: LibraryConfiguration,
-        use_logging: bool = True,
     ):
         csv.register_dialect("tsv", delimiter="\t")
-
-        super().__init__(library_config, task_config, use_logging)
-        self.object_type_name = self.get_object_type().name
-        self.task_config = task_config
-        self.files = self.list_source_files()
-        self.total_records = 0
-        self.current_folio_record: dict = {}
-        self.orders_map = self.setup_records_map(
-            self.folder_structure.mapping_files_folder / self.task_config.orders_mapping_file_name
-        )
-        self.results_path = self.folder_structure.created_objects_path
-        self.failed_files: List[str] = []
-
-        self.folio_keys = []
-        self.folio_keys = MappingFileMapperBase.get_mapped_folio_properties_from_map(
-            self.orders_map
-        )
-        self.minted_ids: set = set()
-
-        self.mapper = CompositeOrderMapper(
-            self.folio_client,
-            self.library_configuration,
-            self.orders_map,
-            self.load_id_map(self.folder_structure.instance_id_map_path, True),
-            self.load_ref_data_mapping_file(
-                "acquisitionMethod",
-                self.folder_structure.mapping_files_folder
-                / self.task_config.acquisition_method_map_file_name,
-                self.folio_keys,
-            ),
-            self.load_ref_data_mapping_file(  # Not required, on POL
-                "paymentStatus",
-                self.folder_structure.mapping_files_folder
-                / self.task_config.payment_status_map_file_name,
-                self.folio_keys,
-                False,
-            ),
-            self.load_ref_data_mapping_file(  # Not required, on POL
-                "receiptStatus",
-                self.folder_structure.mapping_files_folder
-                / self.task_config.receipt_status_map_file_name,
-                self.folio_keys,
-                False,
-            ),
-            self.load_ref_data_mapping_file(  # Not required
-                "workflowStatus",
-                self.folder_structure.mapping_files_folder
-                / self.task_config.workflow_status_map_file_name,
-                self.folio_keys,
-                False,
-            ),
-            self.load_ref_data_mapping_file(
-                "locationMap",
-                self.folder_structure.mapping_files_folder
-                / self.task_config.location_map_file_name,
-                self.folio_keys,
-                False,
-            ),
-            self.load_ref_data_mapping_file(  # Required if there was is a fund.
-                "fundsMap",
-                self.folder_structure.mapping_files_folder / self.task_config.funds_map_file_name,
-                self.folio_keys,
-                False,
-            ),
-            self.load_ref_data_mapping_file(  # Todo: The property in the schema has no type
-                "fundsExpenseClassMap",
-                self.folder_structure.mapping_files_folder
-                / self.task_config.funds_expense_class_map_file_name,
-                self.folio_keys,
-                False,
-            ),
-        )
-
-    def list_source_files(self):
-        files = [
-            self.folder_structure.data_folder / self.object_type_name / f.file_name
-            for f in self.task_config.files
-            if isfile(self.folder_structure.data_folder / self.object_type_name / f.file_name)
-        ]
-        if not any(files):
-            ret_str = ",".join(f.file_name for f in self.task_config.files)
-            raise TransformationProcessError(
-                f"Files {ret_str} not found in"
-                "{self.folder_structure.data_folder} / {self.object_type_name}"
+        self.migration_report = MigrationReport()
+        self.valid_reserves = []
+        super().__init__(library_config, task_configuration)
+        with open(
+            self.folder_structure.legacy_records_folder
+            / task_configuration.course_reserve_file_path.file_name,
+            "r",
+            encoding="utf-8",
+        ) as reserves_file:
+            self.semi_valid_reserves = list(
+                self.load_and_validate_legacy_reserves(
+                    InsensitiveDictReader(reserves_file, dialect="tsv")
+                )
             )
-        logging.info("Files to process:")
-        for filename in files:
-            logging.info("\t%s", filename)
-        return files
-
-    def process_single_file(self, filename):
-        with open(filename, encoding="utf-8-sig") as records_file, open(
-            self.folder_structure.created_objects_path, "w+"
-        ) as results_file:
-            self.mapper.migration_report.add_general_statistics("Number of files processed")
-            start = time.time()
-            records_processed = 0
-            for idx, record in enumerate(self.mapper.get_objects(records_file, filename)):
-                records_processed += 1
-
-                try:
-                    # Print first legacy record, then first transformed record
-                    if idx == 0:
-                        logging.info("First legacy record:")
-                        logging.info(json.dumps(record, indent=4))
-
-                    folio_rec, legacy_id = self.mapper.do_map(
-                        record, f"row {idx}", FOLIONamespaces.orders, True
-                    )
-
-                    # Add notes
-                    self.mapper.notes_mapper.map_notes(
-                        record,
-                        legacy_id,
-                        folio_rec["id"],
-                        FOLIONamespaces.orders,
-                    )
-
-                    self.merge_into_orders_with_embedded_pols(folio_rec, results_file)
-
-                except TransformationProcessError as process_error:
-                    self.mapper.handle_transformation_process_error(idx, process_error)
-                except TransformationRecordFailedError as error:
-                    self.mapper.handle_transformation_record_failed_error(idx, error)
-                except Exception as excepion:
-                    self.mapper.handle_generic_exception(idx, excepion)
-
-                # TODO Rewrite to base % value on number of rows in file
-                if idx > 1 and idx % 50 == 0:
-                    elapsed = idx / (time.time() - start)
-                    elapsed_formatted = "{0:.4g}".format(elapsed)
-                    logging.info(  # pylint: disable=logging-fstring-interpolation
-                        f"{idx:,} records processed. Recs/sec: {elapsed_formatted} "
-                    )
-
-            self.total_records = records_processed
-
-            logging.info(  # pylint: disable=logging-fstring-interpolation
-                f"Done processing {filename} containing {self.total_records:,} records. "
-                f"Total records processed: {self.total_records:,}"
+            logging.info(
+                "Loaded and validated %s reserves in file",
+                len(self.semi_valid_reserves),
             )
-            logging.info("Storing last record to disk")
-            Helper.write_to_file(results_file, self.current_folio_record)
+
+            self.valid_reserves = self.semi_valid_reserves
+        self.t0 = time.time()
+        self.failed: Dict = {}
+        logging.info("Init completed")
 
     def do_work(self):
-        logging.info("Getting started!")
-        for file in self.files:
-            logging.info("Processing %s", file)
+        logging.info("Starting")
+        for num_reserves, legacy_reserve in enumerate(self.valid_reserves, start=1):
+            t0_migration = time.time()
+            self.migration_report.add_general_statistics("Processed reserves")
             try:
-                print(file)
-                self.process_single_file(file)
+                self.post_single_reserve(legacy_reserve)
             except Exception as ee:
-                error_str = (
-                    f"Processing of {file} failed:\n{ee}."
-                    "Check source files for empty lines or missing reference data"
+                logging.exception(
+                    f"Error in row {num_reserves}  Reserve: {json.dumps(legacy_reserve)} {ee}"
                 )
-                logging.exception(error_str)
-                self.mapper.migration_report.add(Blurbs.FailedFiles, f"{file} - {ee}")
-                sys.exit()
+            if num_reserves % 50 == 0:
+                logging.info(f"{timings(self.t0, t0_migration, num_reserves)} {num_reserves}")
+
+    def post_single_reserve(self, legacy_reserve: LegacyReserve):
+        try:
+            path = f"/coursereserves/courselistings/{legacy_reserve.course_listing_id}/reserves"
+            if self.folio_put_post(path, legacy_reserve.to_dict(), "POST", "Posted reserves"):
+                self.migration_report.add_general_statistics("Successfully posted reserves")
+            else:
+                self.migration_report.add_general_statistics("Failure to post reserve")
+        except Exception as ee:
+            logging.error(ee)
 
     def wrap_up(self):
-        logging.info("Done. Wrapping up...")
-        with open(self.folder_structure.migration_reports_file, "w") as migration_report_file:
-            logging.info(
-                "Writing migration- and mapping report to %s",
-                self.folder_structure.migration_reports_file,
-            )
-            self.mapper.migration_report.write_migration_report(
-                "Orders and Orderlines Transformation Report",
-                migration_report_file,
-                self.start_datetime,
+        self.extradata_writer.flush()
+        for k, v in self.failed.items():
+            self.failed_and_not_dupe[k] = [v.to_dict()]
+        self.migration_report.set(Blurbs.GeneralStatistics, "Failed loans", len(self.failed))
+        self.write_failed_reserves_to_file()
+
+        with open(self.folder_structure.migration_reports_file, "w+") as report_file:
+            self.migration_report.write_migration_report(
+                "Reserves migration report", report_file, self.start_datetime
             )
+        self.clean_out_empty_logs()
 
-            Helper.print_mapping_report(
-                migration_report_file,
-                self.total_records,
-                self.mapper.mapped_folio_fields,
-                self.mapper.mapped_legacy_fields,
-            )
-        logging.info("All done!")
+    def write_failed_reserves_to_file(self):
+        # POST /coursereserves/courselistings/40a085bd-b44b-42b3-b92f-61894a75e3ce/reserves
+        # Match on legacy course number ()
+
+        csv_columns = ["legacy_identifier", "barcode"]
+        with open(self.folder_structure.failed_recs_path, "w+") as failed_reserves_file:
+            writer = csv.DictWriter(failed_reserves_file, fieldnames=csv_columns, dialect="tsv")
+            writer.writeheader()
+            for _k, failed_reserve in self.failed.items():
+                writer.writerow(failed_reserve[0])
+
+    def check_barcodes(self):
+        """Stub for extension.
+
+        Yields:
+            _type_: _description_
+        """
+        item_barcodes = set()
+        self.circulation_helper.load_migrated_item_barcodes(
+            item_barcodes, self.task_configuration.item_files, self.folder_structure
+        )
+        for loan in self.semi_valid_legacy_loans:
+            has_item_barcode = loan.item_barcode in item_barcodes or not any(item_barcodes)
+            if has_item_barcode:
+                self.migration_report.add_general_statistics(
+                    "Reserve verified against migrated item"
+                )
+                yield loan
+            else:
+                self.migration_report.add(
+                    Blurbs.DiscardedLoans, "Reserve discarded. Could not find migrated barcode"
+                )
 
-    def merge_into_orders_with_embedded_pols(self, folio_rec, results_file):
-        # Handle merging and storage
-        if not self.current_folio_record:
-            self.current_folio_record = folio_rec
-        if folio_rec["id"] != self.current_folio_record["id"]:
-            # Writes record to file
-            Helper.write_to_file(results_file, self.current_folio_record)
-            self.mapper.migration_report.add_general_statistics("Orders written to disk")
-            self.current_folio_record = folio_rec
-
-        else:
-            # Merge if possible
-            diff = DeepDiff(self.current_folio_record, folio_rec)
-            if "compositePoLines" in diff.affected_root_keys:
-                self.current_folio_record.get("compositePoLines", []).extend(
-                    folio_rec.get("compositePoLines", [])
+    def load_and_validate_legacy_reserves(self, reserves_reader):
+        num_bad = 0
+        logging.info("Validating legacy loans in file...")
+        for legacy_reserve_count, legacy_reserve_dict in enumerate(reserves_reader):
+            try:
+                legacy_reserve = LegacyReserve(
+                    legacy_reserve_dict,
+                    self.folio_client,
+                    legacy_reserve_count,
+                )
+                if any(legacy_reserve.errors):
+                    num_bad += 1
+                    self.migration_report.add_general_statistics("Discarded reserves")
+                    for error in legacy_reserve.errors:
+                        self.migration_report.add(
+                            Blurbs.DiscardedReserves, f"{error[0]} - {error[1]}"
+                        )
+                else:
+                    yield legacy_reserve
+            except ValueError as ve:
+                logging.exception(ve)
+        logging.info(
+            f"Done validating {legacy_reserve_count} legacy reserves with {num_bad} rotten apples"
+        )
+        if num_bad / legacy_reserve_count > 0.5:
+            q = num_bad / legacy_reserve_count
+            logging.error("%s percent of reserves failed to validate.", (q * 100))
+            self.migration_report.log_me()
+            logging.critical("Halting...")
+            sys.exit(1)
+
+    def folio_put_post(self, url, data_dict, verb, action_description=""):
+        full_url = f"{self.folio_client.okapi_url}{url}"
+        try:
+            if verb == "PUT":
+                resp = httpx.put(
+                    full_url,
+                    headers=self.folio_client.okapi_headers,
+                    json=data_dict,
+                )
+            elif verb == "POST":
+                resp = httpx.post(
+                    full_url,
+                    headers=self.folio_client.okapi_headers,
+                    json=data_dict,
+                )
+            else:
+                raise TransformationProcessError("Bad verb supplied. This is a code issue.")
+            if resp.status_code == 422:
+                error_message = json.loads(resp.text)["errors"][0]["message"]
+                logging.error(error_message)
+                self.migration_report.add(
+                    Blurbs.Details, f"{action_description} error: {error_message}"
+                )
+                resp.raise_for_status()
+            elif resp.status_code in [201, 204]:
+                self.migration_report.add(
+                    Blurbs.Details,
+                    f"Successfully {action_description} ({resp.status_code})",
+                )
+            else:
+                self.migration_report.add(
+                    Blurbs.Details,
+                    f"{action_description} error. http status: {resp.status_code}",
                 )
-                self.mapper.migration_report.add_general_statistics("PO-lines merged into one PO")
-            for key in diff.affected_paths:
-                self.mapper.migration_report.add(Blurbs.DiffsBetweenOrders, key)
+                logging.error(json.dumps(data_dict))
+                resp.raise_for_status()
+            return True
+        except HTTPError as exception:
+            logging.error(f"{resp.status_code}. {verb} FAILED for {url}")
+            traceback.print_exc()
+            logging.info(exception)
+            return False
+
+
+def timings(t0, t0func, num_objects):
+    avg = num_objects / (time.time() - t0)
+    elapsed = time.time() - t0
+    elapsed_func = time.time() - t0func
+    return (
+        f"Total objects: {num_objects}\tTotal elapsed: {elapsed:.2f}\t"
+        f"Average per object: {avg:.2f}\tElapsed this time: {elapsed_func:.2f}"
+    )
```

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/organization_transformer.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/organization_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,17 @@
         self.organization_map = self.setup_records_map(
             self.folder_structure.mapping_files_folder
             / self.task_configuration.organization_map_path
         )
 
         self.results_path = self.folder_structure.created_objects_path
         self.failed_files: List[str] = []
+        self.organizations_id_map = self.load_id_map(
+            self.folder_structure.organizations_id_map_path
+        )
 
         self.folio_keys = []
         self.folio_keys = MappingFileMapperBase.get_mapped_folio_properties_from_map(
             self.organization_map
         )
 
         self.mapper = OrganizationMapper(
@@ -151,14 +154,17 @@
                     self.mapper.notes_mapper.map_notes(
                         record,
                         legacy_id,
                         folio_rec["id"],
                         FOLIONamespaces.organizations,
                     )
                     folio_rec = self.clean_org(folio_rec)
+                    self.organizations_id_map[legacy_id] = self.mapper.get_id_map_tuple(
+                        legacy_id, folio_rec, self.object_type
+                    )
 
                     Helper.write_to_file(results_file, folio_rec)
 
                     if idx == 0:
                         logging.info("First FOLIO record:")
                         logging.info(json.dumps(folio_rec, indent=4))
 
@@ -221,14 +227,17 @@
             Helper.print_mapping_report(
                 migration_report_file,
                 self.total_records,
                 self.mapper.mapped_folio_fields,
                 self.mapper.mapped_legacy_fields,
             )
 
+            self.mapper.save_id_map_file(
+                self.folder_structure.organizations_id_map_path, self.organizations_id_map
+            )
         self.clean_out_empty_logs()
 
         logging.info("All done!")
 
     def clean_org(self, record):
         if record.get("addresses"):
             self.clean_addresses(record)
```

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/requests_migrator.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/requests_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/user_transformer.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/user_transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -177,26 +177,43 @@
                 self.mapper.mapped_legacy_fields,
             )
         logging.info("All done!")
         self.clean_out_empty_logs()
 
     @staticmethod
     def clean_user(folio_user, index_or_id):
-        if addresses := folio_user.get("personal", {}).get("addresses", []):
-            # More than one primary address
-            if primaries := [a for a in addresses if a["primaryAddress"] is True]:
-                for primary in primaries[1:]:
-                    primary["primaryAddress"] = False
-            else:
-                # No primary address
-                addresses[0]["primaryAddress"] = True
         # TODO: Consider removing the object metadata construct globally in MappingFileMapperBase
         if folio_user.get("metadata", {}):
             del folio_user["metadata"]
 
+        # Make sure the user has exactly one primary address
+        if addresses := folio_user.get("personal", {}).get("addresses", []):
+            primary_true = []
+            for address in addresses:
+                if "primaryAddress" not in address:
+                    address["primaryAddress"] = False
+                elif (
+                    isinstance(address["primaryAddress"], bool)
+                    and address["primaryAddress"] is True
+                ):
+                    primary_true.append(address)
+
+            if len(primary_true) < 1:
+                addresses[0]["primaryAddress"] = True
+            elif len(primary_true) > 1:
+                logging.log(
+                    26,
+                    "DATA ISSUE\t%s\t%s\t%s",
+                    index_or_id,
+                    "Too many addresses mapped as primary. Setting first one to primary.",
+                    primary_true,
+                )
+                for pt in primary_true[1:]:
+                    pt["primaryAddress"] = False
+
 
 def print_email_warning():
     s = (
         "  ______   __  __              _____   _         _____     ___  \n"  # noqa: E501, W605
         " |  ____| |  \/  |     /\     |_   _| | |       / ____|   |__ \ \n"  # noqa: E501, W605
         " | |__    | \  / |    /  \      | |   | |      | (___        ) |\n"  # noqa: E501, W605
         " |  __|   | |\/| |   / /\ \     | |   | |       \___ \      / / \n"  # noqa: E501, W605
```

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/report_blurbs.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/report_blurbs.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         "Sub-property removed due to missing required fields",
         "Add the missing required information to the record in your current ILS to ensure that it can be migrated over.",
     )
     POLCreation = (
         "PO-Line creation",
         "Report on how PO-Line creation went, what merge criterias were used, etc",
     )
-    AcquisitionMethodMapping = ("Acquisition Method Mapping", "")
+    AcquisitionMethodMapping = ("POL Acquisition Method Mapping", "")
     MalformedInterfaceUri = (
         "Malformed interface URIs",
         "Interfaces with malformed URIs will not be migrated. See data issues log.\nFOLIO Interface URIs must start with one of the following: 'ftp://', 'sftp://', 'http://', 'https://'.",
     )
     FieldMappingDetails = ("Mapping details", "")
     CatalogingAgency = ("Cataloging sources", "")
     Trivia = ("Trivia", "")
@@ -244,16 +244,24 @@
     )
     FailedFiles = ("Failed files", "")
     BoundWithMappings = ("Bound-with mapping", "")
     TemporaryLocationMapping = ("Temporary location mapping", "")
     TemporaryLoanTypeMapping = ("Temporary Loan type mapping", "")
     PermanentLoanTypeMapping = ("Permanent Loan type mapping", "")
     OrderLineLocationMapping = (
-        "Order line location mapping",
-        "This is the holdings location for for the order line (used to create holdings records if settings are configured to do so)",
+        "POL location mapping",
+        "This is the location for for the purchase order line.",
+    )
+    PurchaseOrderVendorLinking = (
+        "Linked Organizations",
+        "All purchase orders MUST be linked to an organization.",
+    )
+    PurchaseOrderInstanceLinking = (
+        "Linked Instances",
+        "Purchase Order Lines can but do not have to be linked to instances",
     )
     StatisticalCodeMapping = ("Statistical code mapping", "")
     HoldingsRecordIdMapping = ("Holdings IDs mapped", "")
     UnmappedProperties = ("Unmapped properties", "")
     StatusMapping = ("Status mapping", "")
     ReferenceDataMapping = ("Reference Data Mapping", "")
     FieldMappingErrors = ("Field mapping errors", "")
```

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/test_infrastructure/mocked_classes.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/test_infrastructure/mocked_classes.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,24 +68,37 @@
         ]
 
     elif ref_data_path == "/organizations-storage/organization-types":
         yield from [
             {"id": "837d04b6-d81c-4c49-9efd-2f62515999b3", "name": "Consortium"},
             {"id": "fc54327d-fd60-4f6a-ba37-a4375511b91b", "name": "Unspecified"},
         ]
+    elif (
+        ref_data_path == "/organizations-storage/organizations"
+        and query == '?query=(code=="EBSCO")'
+    ):
+        yield from [{"id": "some id", "code": "some code", "name": "EBSCO Information Services"}]
+
+    elif (
+        ref_data_path == "/organizations-storage/organizations"
+        and query == '?query=(code=="LisasAwesomeStartup")'
+    ):
+        yield from []
+
     elif ref_data_path == "/organizations-storage/organizations":
         yield from [
             {"id": "837d04b6-d81c-4c49-9efd-2f62515999b3", "code": "GOBI"},
             {"id": "fc54327d-fd60-4f6a-ba37-a4375511b91b", "code": "EBSCO"},
         ]
 
     elif ref_data_path == "/orders/acquisition-methods":
         yield from [
             {"id": "837d04b6-d81c-4c49-9efd-2f62515999b3", "value": "Purchase"},
             {"id": "fc54327d-fd60-4f6a-ba37-a4375511b91b", "value": "Theft"},
+            {"id": "fc54327d-fd60-4f6a-ba37-a437551sarfs91b", "value": "Other"},
         ]
 
     elif ref_data_path == "/groups":
         yield from [
             {
                 "group": "FOLIO fallback group name",
                 "desc": "Mocked response",
@@ -168,17 +181,18 @@
                 "name": "Library Main Desk",
                 "code": "lmd",
             },
         ]
 
     elif ref_data_path == "/users" and query == '?query=(externalSystemId=="Some external id")':
         yield from [{"id": "some id", "barcode": "some barcode", "patronGroup": "some group"}]
-
-    elif ref_data_path == "/users" and query == '?query=(barcode=="some barcode")':
-        yield from [{"id": "a FOLIO user uuid"}]
+    elif ref_data_path == "/users" and query == '?query=(barcode=="u123")':
+        yield from [{"id": "user123", "barcode": "u123", "patronGroup": "some group"}]
+    elif ref_data_path == "/users" and query == '?query=(barcode=="u456")':
+        yield from [{"id": "user456", "barcode": "u456", "patronGroup": "some group"}]
 
     elif ref_data_path == "/inventory/items" and query == '?query=(barcode=="some barcode")':
         yield from [
             {
                 "id": "a FOLIO item uuid",
                 "title": "Döda fallen i Avesta.",
                 "barcode": "some barcode",
@@ -206,13 +220,25 @@
     if args[0] == "/hrid-settings-storage/hrid-settings":
         return {
             "instances": {"prefix": "pref", "startNumber": 1},
             "holdings": {"prefix": "pref", "startNumber": 1},
             "items": {"prefix": "pref", "startNumber": 1},
             "commonRetainLeadingZeroes": True,
         }
+
+    elif (
+        args[0] == "/configurations/entries?query=(module==ORG%20and%20configName==localeSettings)"
+    ):
+        return {
+            "configs": [
+                {
+                    "value": '{"timezone":"America/New_York"}',
+                }
+            ]
+        }
+
     elif args[0] in super_schema:
         return super_schema.get(args[0])
 
 
 def folio_get_from_github(owner, repo, file_path):
     return FolioClient.get_latest_from_github(owner, repo, file_path, "")
```

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/legacy_loan.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/legacy_loan.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/legacy_request.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/legacy_request.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/legacy_reserve.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/legacy_reserve.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/transaction_result.py` & `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/transaction_result.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc7/setup.py` & `folio_migration_tools-1.8.0rc8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
  'pydantic>=1.10.2,<2.0.0',
  'pyhumps>=3.7.3,<4.0.0',
  'pymarc>=4.2.1,<5.0.0',
  'python-dateutil>=2.8.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'folio-migration-tools',
-    'version': '1.8.0rc7',
+    'version': '1.8.0rc8',
     'description': 'A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP',
     'long_description': '# FOLIO Migration Tools\n![example workflow](https://github.com/FOLIO-FSE/MARC21-To-FOLIO/actions/workflows/python-app.yml/badge.svg)[![codecov](https://codecov.io/gh/FOLIO-FSE/folio_migration_tools/branch/main/graph/badge.svg?token=ZQL5ILWWGT)](https://codecov.io/gh/FOLIO-FSE/folio_migration_tools)   [![readthedocs](https://readthedocs.org/projects/docs/badge/?version=latest)](https://folio-migration-tools.readthedocs.io/)\n\nA toolkit that enables you to migrate data over from a legacy ILS system into [FOLIO LSP](https://www.folio.org/)\n\n# What is it good for?\nFOLIO Migration tools enables you to migrate libraries with the most common ILS:s over to FOLIO without data losses or any major data transformation tasks. \nThe tools transforms and loads the data providing you and the library with good actionable logs and data cleaning task lists together with the migrated data.\n\n## What data does it cover?\nFOLIO Migration Tools currently covers the following data sets:\n* Catalog (Inventory and SRS in FOLIO terminology)\n* Circulation transactions (Open loans and requests)\n* Users/Patrons (In FOLIO, these share the same app/database)\n* Courses and Reserves (Course reserves)\n* Organizations (Vendor records)\n* Orders (limited support)\n\n### What additional functionality is on the roadmap?\nThis is the loose roadmap, in order of most likely implementations first\n* ERM-related objects\n* Financial records\n\n### Can I use the tools for ongoing imports and integrations?\nThe tools are primarliy maintained for performing initial data migrations. We recommend that you use native FOLIO functionality for ongoing loads where possible. \nIn theory, these tools can be used for ongoing patron loads from systems like Banner, Workday, or PeopleSoft. But we recommend you to weigh your options carefully before going down this path. \n\n# Contributing\nWant to contribute? Read the [CONTRIBUTING.MD](https://github.com/FOLIO-FSE/folio_migration_tools/blob/main/CONTRIBUTING.md)\n\n# Found an issue?\nReport it on the [Github Issue tracker](https://github.com/FOLIO-FSE/folio_migration_tools/issues)\n\nThe scripts requires a FOLIO tenant with reference data properly set up. The script will throw messages telling what reference data is missing.\n# Installing\nMake sure you are running Python 3.9 or above. \n## 1. Using pip and venv\n### 2.1. Create and activate a [virtual environment](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment)   \n```   \npython -m venv ./.venv     # Creates a virtual env in the current folder\nsource .venv/bin/activate  # Activates the venv    \n```\n### 2. Install using pip: \n```\npython -m pip install folio_migration_tools\n```\n### 3. Test the installation by showing the help pages \n```   \npython -m folio_migration_tools -h\n```    \n\n## 2. Using pipenv\n### 1. Run\n```   \npipenv install folio-migration-tools\n```   \n### 2. Test the installation by showing the help pages\n```  \npipenv run python3 -m folio_migration_tools -h\n```  \n\n# FOLIO migration process\nThis repo plays the main part in a process using a collection of tools. The process itself is documented in more detail, including example configuration files, at [this template repository](https://github.com/FOLIO-FSE/migration_repo_template)\nIn order to perform migrations according to this process, you need the following:\n* An Installation of [FOLIO Migration Tools](https://pypi.org/project/folio-migration-tools/). Installation instructions above.\n* A clone, or a separate repo created from [migration_repo_template](https://github.com/FOLIO-FSE/migration_repo_template)\n* Access to the [Data mapping file creator](https://data-mapping-file-creator.folio.ebsco.com/data_mapping_creation) web tool\n* A FOLIO tenant running the latest or the second latest version of FOLIO\n\n\n\n# Running the scripts\nFor information on syntax, what files are needed and produced by the toolkit, refer to the documentation and example files in the [template repository](https://github.com/FOLIO-FSE/migration_repo_template). We are building out the docs section in this repository as well:[Documentation](https://folio-migration-tools.readthedocs.io/en/latest/)\n¨\n',
     'author': 'Theodor Tolstoy',
     'author_email': 'github.teddes@tolstoy.se',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/FOLIO-FSE/folio_migration_tools',
```

### Comparing `folio_migration_tools-1.8.0rc7/PKG-INFO` & `folio_migration_tools-1.8.0rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folio-migration-tools
-Version: 1.8.0rc7
+Version: 1.8.0rc8
 Summary: A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP
 Home-page: https://github.com/FOLIO-FSE/folio_migration_tools
 License: MIT
 Keywords: FOLIO,ILS,LSP,Library Systems,MARC21,Library data
 Author: Theodor Tolstoy
 Author-email: github.teddes@tolstoy.se
 Requires-Python: >=3.9,<4.0
```

