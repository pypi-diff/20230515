# Comparing `tmp/usdm-0.25.0.tar.gz` & `tmp/usdm-0.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usdm-0.25.0.tar", last modified: Fri Apr 14 13:51:32 2023, max compression
+gzip compressed data, was "usdm-0.26.0.tar", last modified: Mon May 15 06:15:29 2023, max compression
```

## Comparing `usdm-0.25.0.tar` & `usdm-0.26.0.tar`

### file list

```diff
@@ -1,134 +1,140 @@
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.374523 usdm-0.25.0/
--rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.25.0/LICENSE
--rw-r--r--   0 daveih     (501) staff       (20)    19581 2023-04-14 13:51:32.374247 usdm-0.25.0/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)    19131 2023-04-14 12:14:15.000000 usdm-0.25.0/README.md
--rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.25.0/pyproject.toml
--rw-r--r--   0 daveih     (501) staff       (20)       38 2023-04-14 13:51:32.374586 usdm-0.25.0/setup.cfg
--rw-r--r--   0 daveih     (501) staff       (20)      932 2023-04-12 12:31:13.000000 usdm-0.25.0/setup.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.329578 usdm-0.25.0/src/
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.332738 usdm-0.25.0/src/usdm.egg-info/
--rw-r--r--   0 daveih     (501) staff       (20)    19581 2023-04-14 13:51:32.000000 usdm-0.25.0/src/usdm.egg-info/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)     4238 2023-04-14 13:51:32.000000 usdm-0.25.0/src/usdm.egg-info/SOURCES.txt
--rw-r--r--   0 daveih     (501) staff       (20)        1 2023-04-14 13:51:32.000000 usdm-0.25.0/src/usdm.egg-info/dependency_links.txt
--rw-r--r--   0 daveih     (501) staff       (20)       45 2023-04-14 13:51:32.000000 usdm-0.25.0/src/usdm.egg-info/requires.txt
--rw-r--r--   0 daveih     (501) staff       (20)       32 2023-04-14 13:51:32.000000 usdm-0.25.0/src/usdm.egg-info/top_level.txt
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.340448 usdm-0.25.0/src/usdm_excel/
--rw-r--r--   0 daveih     (501) staff       (20)     1122 2023-04-13 04:26:45.000000 usdm-0.25.0/src/usdm_excel/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      269 2023-03-31 14:50:16.000000 usdm-0.25.0/src/usdm_excel/alias.py
--rw-r--r--   0 daveih     (501) staff       (20)     8005 2023-04-13 04:26:45.000000 usdm-0.25.0/src/usdm_excel/base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     3766 2023-04-05 14:21:45.000000 usdm-0.25.0/src/usdm_excel/cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      787 2023-03-31 14:50:16.000000 usdm-0.25.0/src/usdm_excel/cdisc_ct.py
--rw-r--r--   0 daveih     (501) staff       (20)     4349 2023-04-11 15:59:49.000000 usdm-0.25.0/src/usdm_excel/cdisc_ct_library.py
--rw-r--r--   0 daveih     (501) staff       (20)     1366 2023-04-13 04:26:45.000000 usdm-0.25.0/src/usdm_excel/configuration_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      400 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/cross_ref.py
--rw-r--r--   0 daveih     (501) staff       (20)      337 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/ct_version_manager.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.341652 usdm-0.25.0/src/usdm_excel/data/
--rw-r--r--   0 daveih     (501) staff       (20)      963 2023-04-14 12:14:15.000000 usdm-0.25.0/src/usdm_excel/data/cdisc_ct_config.yaml
--rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/data/iso_3166.json
--rw-r--r--   0 daveih     (501) staff       (20)     3453 2023-04-11 15:59:49.000000 usdm-0.25.0/src/usdm_excel/data/missing_ct.yaml
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.342552 usdm-0.25.0/src/usdm_excel/errors/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-06 07:20:00.000000 usdm-0.25.0/src/usdm_excel/errors/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      627 2023-04-11 13:28:10.000000 usdm-0.25.0/src/usdm_excel/errors/error.py
--rw-r--r--   0 daveih     (501) staff       (20)      650 2023-04-11 13:28:10.000000 usdm-0.25.0/src/usdm_excel/errors/errors.py
--rw-r--r--   0 daveih     (501) staff       (20)     1189 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/id_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)      744 2023-04-13 09:34:38.000000 usdm-0.25.0/src/usdm_excel/iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      111 2023-04-03 10:43:35.000000 usdm-0.25.0/src/usdm_excel/logger.py
--rw-r--r--   0 daveih     (501) staff       (20)      309 2023-03-31 14:50:16.000000 usdm-0.25.0/src/usdm_excel/ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)     3730 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/nodes_and_edges.py
--rw-r--r--   0 daveih     (501) staff       (20)      512 2023-04-13 04:26:45.000000 usdm-0.25.0/src/usdm_excel/option_manager.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.343116 usdm-0.25.0/src/usdm_excel/study_design_arm_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.25.0/src/usdm_excel/study_design_arm_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1443 2023-04-14 12:14:15.000000 usdm-0.25.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.343880 usdm-0.25.0/src/usdm_excel/study_design_element_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_element_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1834 2023-04-11 13:28:10.000000 usdm-0.25.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.344639 usdm-0.25.0/src/usdm_excel/study_design_encounter_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2429 2023-04-11 13:28:10.000000 usdm-0.25.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.345310 usdm-0.25.0/src/usdm_excel/study_design_epoch_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.25.0/src/usdm_excel/study_design_epoch_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1124 2023-04-14 12:14:15.000000 usdm-0.25.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.346023 usdm-0.25.0/src/usdm_excel/study_design_estimands_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2259 2023-04-11 13:28:10.000000 usdm-0.25.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.346711 usdm-0.25.0/src/usdm_excel/study_design_ii_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_ii_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1655 2023-04-11 13:28:10.000000 usdm-0.25.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.347421 usdm-0.25.0/src/usdm_excel/study_design_objective_endpoint_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2025 2023-04-14 13:39:15.000000 usdm-0.25.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.348146 usdm-0.25.0/src/usdm_excel/study_design_population_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_population_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1631 2023-04-11 13:28:10.000000 usdm-0.25.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.348732 usdm-0.25.0/src/usdm_excel/study_design_procedure_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1590 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.349391 usdm-0.25.0/src/usdm_excel/study_design_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     5094 2023-04-14 12:14:15.000000 usdm-0.25.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.350053 usdm-0.25.0/src/usdm_excel/study_identifiers_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_identifiers_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2559 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.350699 usdm-0.25.0/src/usdm_excel/study_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     7444 2023-04-14 12:14:15.000000 usdm-0.25.0/src/usdm_excel/study_sheet/study_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.356163 usdm-0.25.0/src/usdm_excel/study_soa_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      637 2023-04-03 10:43:35.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/activities.py
--rw-r--r--   0 daveih     (501) staff       (20)     2899 2023-04-05 14:06:46.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      888 2023-04-05 14:06:46.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/cycle.py
--rw-r--r--   0 daveih     (501) staff       (20)     1864 2023-04-05 14:06:46.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/cycles.py
--rw-r--r--   0 daveih     (501) staff       (20)      993 2023-04-05 14:06:46.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/encounters.py
--rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/soa_column_rows.py
--rw-r--r--   0 daveih     (501) staff       (20)     4645 2023-04-13 09:55:50.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     5048 2023-04-13 04:26:45.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/timepoint.py
--rw-r--r--   0 daveih     (501) staff       (20)     2748 2023-04-13 04:26:45.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/timepoints.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.356556 usdm-0.25.0/src/usdm_info/
--rw-r--r--   0 daveih     (501) staff       (20)       59 2023-04-13 09:55:50.000000 usdm-0.25.0/src/usdm_info/__init__.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.369329 usdm-0.25.0/src/usdm_model/
--rw-r--r--   0 daveih     (501) staff       (20)     1685 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      545 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      210 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/address.py
--rw-r--r--   0 daveih     (501) staff       (20)      229 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/aliasCode.py
--rw-r--r--   0 daveih     (501) staff       (20)      229 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/alias_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      139 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/analysis_population.py
--rw-r--r--   0 daveih     (501) staff       (20)      844 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/api_base_model.py
--rw-r--r--   0 daveih     (501) staff       (20)      375 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      315 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/biomedical_concept_category.py
--rw-r--r--   0 daveih     (501) staff       (20)      394 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/biomedical_concept_property.py
--rw-r--r--   0 daveih     (501) staff       (20)      216 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/biomedical_concept_surrogate.py
--rw-r--r--   0 daveih     (501) staff       (20)      152 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/code.py
--rw-r--r--   0 daveih     (501) staff       (20)      642 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/encounter.py
--rw-r--r--   0 daveih     (501) staff       (20)      262 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/endpoint.py
--rw-r--r--   0 daveih     (501) staff       (20)      543 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/estimand.py
--rw-r--r--   0 daveih     (501) staff       (20)      224 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/indication.py
--rw-r--r--   0 daveih     (501) staff       (20)      206 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/intercurrent_event.py
--rw-r--r--   0 daveih     (501) staff       (20)      260 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/investigational_intervention.py
--rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/objective.py
--rw-r--r--   0 daveih     (501) staff       (20)      347 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/organisation.py
--rw-r--r--   0 daveih     (501) staff       (20)      274 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/procedure.py
--rw-r--r--   0 daveih     (501) staff       (20)      186 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/response_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      509 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/schedule_timeline.py
--rw-r--r--   0 daveih     (501) staff       (20)      114 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/schedule_timeline_exit.py
--rw-r--r--   0 daveih     (501) staff       (20)      691 2023-04-13 04:26:45.000000 usdm-0.25.0/src/usdm_model/scheduled_instance.py
--rw-r--r--   0 daveih     (501) staff       (20)      677 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/study.py
--rw-r--r--   0 daveih     (501) staff       (20)      296 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/study_arm.py
--rw-r--r--   0 daveih     (501) staff       (20)      380 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/study_cell.py
--rw-r--r--   0 daveih     (501) staff       (20)     1583 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/study_design.py
--rw-r--r--   0 daveih     (501) staff       (20)      351 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/study_design_population.py
--rw-r--r--   0 daveih     (501) staff       (20)      359 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/study_element.py
--rw-r--r--   0 daveih     (501) staff       (20)      401 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/study_epoch.py
--rw-r--r--   0 daveih     (501) staff       (20)      583 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/study_identifier.py
--rw-r--r--   0 daveih     (501) staff       (20)      412 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/study_protocol_version.py
--rw-r--r--   0 daveih     (501) staff       (20)      336 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/timing.py
--rw-r--r--   0 daveih     (501) staff       (20)      134 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/transition_rule.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.373707 usdm-0.25.0/tests/
--rw-r--r--   0 daveih     (501) staff       (20)    12726 2023-04-11 13:28:11.000000 usdm-0.25.0/tests/test_base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     2129 2023-04-05 14:43:30.000000 usdm-0.25.0/tests/test_cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      679 2023-04-11 13:28:11.000000 usdm-0.25.0/tests/test_error.py
--rw-r--r--   0 daveih     (501) staff       (20)     1126 2023-04-11 13:28:11.000000 usdm-0.25.0/tests/test_errors.py
--rw-r--r--   0 daveih     (501) staff       (20)      971 2023-04-13 09:35:41.000000 usdm-0.25.0/tests/test_iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      412 2023-04-05 14:06:46.000000 usdm-0.25.0/tests/test_ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)      969 2023-04-13 04:26:45.000000 usdm-0.25.0/tests/test_option_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)     3320 2023-04-14 12:14:15.000000 usdm-0.25.0/tests/test_study_design_arm_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     2716 2023-04-14 12:14:15.000000 usdm-0.25.0/tests/test_study_design_epoch_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.536518 usdm-0.26.0/
+-rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.26.0/LICENSE
+-rw-r--r--   0 daveih     (501) staff       (20)    21059 2023-05-15 06:15:29.536306 usdm-0.26.0/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)    20609 2023-05-08 14:51:48.000000 usdm-0.26.0/README.md
+-rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.26.0/pyproject.toml
+-rw-r--r--   0 daveih     (501) staff       (20)       38 2023-05-15 06:15:29.536562 usdm-0.26.0/setup.cfg
+-rw-r--r--   0 daveih     (501) staff       (20)      932 2023-04-12 12:31:13.000000 usdm-0.26.0/setup.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.479967 usdm-0.26.0/src/
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.484608 usdm-0.26.0/src/usdm.egg-info/
+-rw-r--r--   0 daveih     (501) staff       (20)    21059 2023-05-15 06:15:29.000000 usdm-0.26.0/src/usdm.egg-info/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)     4469 2023-05-15 06:15:29.000000 usdm-0.26.0/src/usdm.egg-info/SOURCES.txt
+-rw-r--r--   0 daveih     (501) staff       (20)        1 2023-05-15 06:15:29.000000 usdm-0.26.0/src/usdm.egg-info/dependency_links.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       45 2023-05-15 06:15:29.000000 usdm-0.26.0/src/usdm.egg-info/requires.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       32 2023-05-15 06:15:29.000000 usdm-0.26.0/src/usdm.egg-info/top_level.txt
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.492327 usdm-0.26.0/src/usdm_excel/
+-rw-r--r--   0 daveih     (501) staff       (20)     1330 2023-05-15 06:05:22.000000 usdm-0.26.0/src/usdm_excel/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      269 2023-03-31 14:50:16.000000 usdm-0.26.0/src/usdm_excel/alias.py
+-rw-r--r--   0 daveih     (501) staff       (20)     8852 2023-05-09 10:09:13.000000 usdm-0.26.0/src/usdm_excel/base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4667 2023-05-01 12:04:14.000000 usdm-0.26.0/src/usdm_excel/cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      787 2023-03-31 14:50:16.000000 usdm-0.26.0/src/usdm_excel/cdisc_ct.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4349 2023-04-11 15:59:49.000000 usdm-0.26.0/src/usdm_excel/cdisc_ct_library.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1564 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      400 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/cross_ref.py
+-rw-r--r--   0 daveih     (501) staff       (20)      337 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/ct_version_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.493768 usdm-0.26.0/src/usdm_excel/data/
+-rw-r--r--   0 daveih     (501) staff       (20)      963 2023-04-14 12:14:15.000000 usdm-0.26.0/src/usdm_excel/data/cdisc_ct_config.yaml
+-rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/data/iso_3166.json
+-rw-r--r--   0 daveih     (501) staff       (20)     3453 2023-04-11 15:59:49.000000 usdm-0.26.0/src/usdm_excel/data/missing_ct.yaml
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.494952 usdm-0.26.0/src/usdm_excel/errors/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-06 07:20:00.000000 usdm-0.26.0/src/usdm_excel/errors/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      715 2023-05-09 05:56:05.000000 usdm-0.26.0/src/usdm_excel/errors/error.py
+-rw-r--r--   0 daveih     (501) staff       (20)      672 2023-05-09 05:53:57.000000 usdm-0.26.0/src/usdm_excel/errors/errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1189 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/id_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)      744 2023-04-13 09:34:38.000000 usdm-0.26.0/src/usdm_excel/iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)      111 2023-04-03 10:43:35.000000 usdm-0.26.0/src/usdm_excel/logger.py
+-rw-r--r--   0 daveih     (501) staff       (20)      309 2023-03-31 14:50:16.000000 usdm-0.26.0/src/usdm_excel/ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5161 2023-05-15 06:05:22.000000 usdm-0.26.0/src/usdm_excel/nodes_and_edges.py
+-rw-r--r--   0 daveih     (501) staff       (20)      824 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/option_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.495696 usdm-0.26.0/src/usdm_excel/study_design_activity_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-05-03 10:02:41.000000 usdm-0.26.0/src/usdm_excel/study_design_activity_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1404 2023-05-08 14:51:48.000000 usdm-0.26.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.496435 usdm-0.26.0/src/usdm_excel/study_design_arm_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.26.0/src/usdm_excel/study_design_arm_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1457 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.497172 usdm-0.26.0/src/usdm_excel/study_design_element_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_element_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1841 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.497925 usdm-0.26.0/src/usdm_excel/study_design_encounter_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2338 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.498537 usdm-0.26.0/src/usdm_excel/study_design_epoch_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.26.0/src/usdm_excel/study_design_epoch_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1131 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.499513 usdm-0.26.0/src/usdm_excel/study_design_estimands_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2273 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.501243 usdm-0.26.0/src/usdm_excel/study_design_ii_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_ii_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1662 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.502396 usdm-0.26.0/src/usdm_excel/study_design_objective_endpoint_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2024 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.503691 usdm-0.26.0/src/usdm_excel/study_design_population_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_population_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1638 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.504454 usdm-0.26.0/src/usdm_excel/study_design_procedure_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1499 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.505451 usdm-0.26.0/src/usdm_excel/study_design_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5094 2023-04-14 12:14:15.000000 usdm-0.26.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.506870 usdm-0.26.0/src/usdm_excel/study_identifiers_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_identifiers_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2559 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.507731 usdm-0.26.0/src/usdm_excel/study_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     7614 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_sheet/study_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.512223 usdm-0.26.0/src/usdm_excel/study_soa_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      637 2023-04-03 10:43:35.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/activities.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3498 2023-05-09 06:07:57.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      888 2023-04-05 14:06:46.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/cycle.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1864 2023-04-05 14:06:46.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/cycles.py
+-rw-r--r--   0 daveih     (501) staff       (20)      993 2023-04-05 14:06:46.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/encounters.py
+-rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/soa_column_rows.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4645 2023-04-13 09:55:50.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5048 2023-04-13 04:26:45.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/timepoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2748 2023-04-13 04:26:45.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/timepoints.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.512615 usdm-0.26.0/src/usdm_info/
+-rw-r--r--   0 daveih     (501) staff       (20)       59 2023-05-01 12:04:14.000000 usdm-0.26.0/src/usdm_info/__init__.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.529281 usdm-0.26.0/src/usdm_model/
+-rw-r--r--   0 daveih     (501) staff       (20)     1685 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      545 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      210 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/address.py
+-rw-r--r--   0 daveih     (501) staff       (20)      229 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/aliasCode.py
+-rw-r--r--   0 daveih     (501) staff       (20)      229 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/alias_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      139 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/analysis_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)      844 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/api_base_model.py
+-rw-r--r--   0 daveih     (501) staff       (20)      375 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      315 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/biomedical_concept_category.py
+-rw-r--r--   0 daveih     (501) staff       (20)      394 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/biomedical_concept_property.py
+-rw-r--r--   0 daveih     (501) staff       (20)      216 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/biomedical_concept_surrogate.py
+-rw-r--r--   0 daveih     (501) staff       (20)      152 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      642 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/encounter.py
+-rw-r--r--   0 daveih     (501) staff       (20)      262 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/endpoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)      543 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/estimand.py
+-rw-r--r--   0 daveih     (501) staff       (20)      224 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/indication.py
+-rw-r--r--   0 daveih     (501) staff       (20)      206 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/intercurrent_event.py
+-rw-r--r--   0 daveih     (501) staff       (20)      260 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/investigational_intervention.py
+-rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/objective.py
+-rw-r--r--   0 daveih     (501) staff       (20)      347 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/organisation.py
+-rw-r--r--   0 daveih     (501) staff       (20)      274 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/procedure.py
+-rw-r--r--   0 daveih     (501) staff       (20)      186 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/response_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      509 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/schedule_timeline.py
+-rw-r--r--   0 daveih     (501) staff       (20)      114 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/schedule_timeline_exit.py
+-rw-r--r--   0 daveih     (501) staff       (20)      691 2023-04-13 04:26:45.000000 usdm-0.26.0/src/usdm_model/scheduled_instance.py
+-rw-r--r--   0 daveih     (501) staff       (20)      677 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/study.py
+-rw-r--r--   0 daveih     (501) staff       (20)      296 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/study_arm.py
+-rw-r--r--   0 daveih     (501) staff       (20)      380 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/study_cell.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1583 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/study_design.py
+-rw-r--r--   0 daveih     (501) staff       (20)      351 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/study_design_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)      359 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/study_element.py
+-rw-r--r--   0 daveih     (501) staff       (20)      401 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/study_epoch.py
+-rw-r--r--   0 daveih     (501) staff       (20)      583 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/study_identifier.py
+-rw-r--r--   0 daveih     (501) staff       (20)      412 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/study_protocol_version.py
+-rw-r--r--   0 daveih     (501) staff       (20)      336 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/timing.py
+-rw-r--r--   0 daveih     (501) staff       (20)      134 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/transition_rule.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.535679 usdm-0.26.0/tests/
+-rw-r--r--   0 daveih     (501) staff       (20)    13402 2023-05-08 13:47:22.000000 usdm-0.26.0/tests/test_base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2129 2023-04-05 14:43:30.000000 usdm-0.26.0/tests/test_cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1517 2023-05-08 13:47:22.000000 usdm-0.26.0/tests/test_configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      679 2023-04-11 13:28:11.000000 usdm-0.26.0/tests/test_error.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1126 2023-04-11 13:28:11.000000 usdm-0.26.0/tests/test_errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)      762 2023-05-09 10:48:00.000000 usdm-0.26.0/tests/test_integration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      971 2023-04-13 09:35:41.000000 usdm-0.26.0/tests/test_iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)      412 2023-04-05 14:06:46.000000 usdm-0.26.0/tests/test_ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1098 2023-05-08 13:47:22.000000 usdm-0.26.0/tests/test_option_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3199 2023-05-08 14:51:48.000000 usdm-0.26.0/tests/test_study_design_activity_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3320 2023-04-14 12:14:15.000000 usdm-0.26.0/tests/test_study_design_arm_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2716 2023-04-14 12:14:15.000000 usdm-0.26.0/tests/test_study_design_epoch_sheet.py
```

### Comparing `usdm-0.25.0/LICENSE` & `usdm-0.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/PKG-INFO` & `usdm-0.26.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usdm
-Version: 0.25.0
+Version: 0.26.0
 Summary: A python package for using the CDISC TransCelerate USDM
 Author: D Iberson-Hurst
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -53,47 +53,52 @@
 excel = USDMExcel("source_data/simple_1.xlsx")
 with open('source_data/simple_1.json', 'w', encoding='utf-8') as f:
   f.write(json.dumps(json.loads(excel.to_json()), indent=2))
 ```
 
 ## Format of Workbook
 
-### General
+### Sheets
 
-#### Sheets
-
-The workbook consists of several sheets each with a dedicated purpose. All sheets must be present.
+The workbook consists of several sheets each with a dedicated purpose. All sheets must be present except for those marked optional.
 
 - Study sheet
 - Study Identifiers sheet
 - Study Design sheet
 - one or more Timeline sheets
+- Study Design Activities sheet (optional)
 - Study Design Indications and Interventions sheet
 - Study Design Populations sheet
 - Study Design Objectives and Endpoints sheet
 - Study Design Estimands sheet
 - Study Design Procedures sheet
 - Study Design Encounters sheet
 - Study Design Elements sheet
 - Configuration sheet
 
 The content of each sheet is described below. Example workbooks can be found in the [CDISC Reference Architecture repo](https://github.com/cdisc-org/DDF-RA/tree/sprint-11/Deliverables/IG/examples). *Note: the link above points to the sprint 11 branch. This will be merged into the main branch prior to public review.*
 
-#### CDISC Terminology
+### CDISC Terminology
 
 For those cells where CDISC codes are used the user can enter either the CDISC C Code, for example `C15602`, the CDISC submission value, for example `PHASE III TRIAL`, or the preferred term, for example `Phase III Trial`
 
-#### External Terminology
+### External Terminology
 
 For those cells where external CT is referenced the user can enter code in the form `<code system>: <code> = <decode>`. For example `SPONSOR: A = decode 1, SPONSOR: B = decode 2`.
 
+### Boolean Values
+
+For boolean fields the following can be used to indicate a `true` value `'Y', 'YES', 'T', 'TRUE', '1'` or the lower case equivalents.
+
 ### Identifiers and Cross References
 
 Some content defined within the sheets contain unique identifiers such that the content can be cross referenced in other sheets. This is done so as to link content or expand definitions. Identifiers are simple strings that need to be unique within the workbook. There is a single definition and one or more cross references.
 
+See the [infographic](https://github.com/data4knowledge/usdm/blob/main/docs/sheets.png) for further information.
+
 ### Study Sheet
 
 #### Sheet Name
 
 `study`
 
 #### Sheet Contents
@@ -138,15 +143,17 @@
 | Column | Column Name | Description | Format and Values |
 | :--- | :--- | :--- | :--- |
 | A | organisationIdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
 | B | organisationIdentifier | Organisation identifier | Text string |
 | C | organisationName | Organisation name | Text string |
 | D | organisationType | Organisation type | CDISC code reference |
 | E | studyIdentifier | The identifier for the study | Text string |
-| F | organisationAddress | The organisation address | Formated using a pipe delimited form `line|city|district|state|postal_code|<country code>`. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code. |
+| F | organisationAddress | The organisation address | Formated using a pipe delimited form, see below |
+
+The organisation address is of the form: ```line|city|district|state|postal_code|<country code>```. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code.
 
 ### Study Design sheet
 
 #### Sheet Name
 
 `studyDesign`
 
@@ -287,14 +294,35 @@
 
 `BC: Age, BC: Sec, PR:Informed Consent Form, TL:Exercise` indicates the activity consists of the bcs Age and Sex, a procedure for the informed consent and a timeline specified in the Exercise sheet.
 
 ##### Link
 
 The link section consists of a set of cells into which an upper case 'X' can be placed to link a timepoint with an activity. Otherwise the cell will be ignored. A '-' can be used to fill in cells but "empty".
 
+### Study Design Activities sheet
+
+#### Sheet Name
+
+`studyDesignActivities`
+
+#### Sheet Contents
+
+A header row in row 1 followed by repeating rows from row 2, containing encounter definitions.
+
+| Column | Column Name | Description | Format and Values |
+| :--- | :--- | :--- | :--- |
+| A | activityName	| Name | Text string |
+| B | activityDescription	| Description | Text string |
+| C | activityIsConditional | Conditional flag | Boolean |
+| D | activityIsConditionalReason | Reason | Text string |
+
+Note that this sheet is optional. If the sheet is not provided the activities will be created from those defined in the timeline sheets. These activities will have the name and description set to the name used in the timeline sheet and no condition will be set.
+
+If the sheet is provided but there is no definition in the sheet for an activity referenced in a timeline sheet then the name and description will be set to the name used in the timeline sheet and no condition will be set.
+
 ### Study Design Indications and Interventions Sheet
 	
 #### Sheet Name
 
 `studyDesignII`
 
 #### Sheet Contents
@@ -437,17 +465,12 @@
 A set of rows consisting of configuration parameters. The first column is the type of configuration parameter while the second is the value. The values for specific parameters may vary in their format
 
 | Parameter | Description | Format and Values |
 | :--- | :--- | :--- |
 | CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form CT name = Version value, For example `SNOMED = 21st June 2012`|
 | SDR Prev Next | Allows for next and previous ids to be set to '' rather than null values so as to accomodate the SDR validation checks | Set to 'SDR' to use '' or leave empty to set null values |
 | SDR Root | Allows for the API specification complant JSON output to be wrpaped in a root "clinicalStudy" element so as to accomodate the SDR validation checks | Set to 'SDR' to use wrapper or leave empty to just generate the API compliant JSON |
+| SDR Description | Allows for the description fields within the JSON to be fillled with a string value rather than being set to an empty string if they are left blank in the excel sheets. Currently only applies to description fields | A non-empty string such as `'-', 'not set'` etc |
 
-### Content Not Suported As Yet
-
-It is intended to support all of the content in the USDM. The following features are not yet supported:
-
-- Full Arm definitions
-- Full Epoch definitions
-- BC categories
+### Issues
 
 See the [github issues](https://github.com/data4knowledge/usdm/issues)
```

### Comparing `usdm-0.25.0/README.md` & `usdm-0.26.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,47 +39,52 @@
 excel = USDMExcel("source_data/simple_1.xlsx")
 with open('source_data/simple_1.json', 'w', encoding='utf-8') as f:
   f.write(json.dumps(json.loads(excel.to_json()), indent=2))
 ```
 
 ## Format of Workbook
 
-### General
+### Sheets
 
-#### Sheets
-
-The workbook consists of several sheets each with a dedicated purpose. All sheets must be present.
+The workbook consists of several sheets each with a dedicated purpose. All sheets must be present except for those marked optional.
 
 - Study sheet
 - Study Identifiers sheet
 - Study Design sheet
 - one or more Timeline sheets
+- Study Design Activities sheet (optional)
 - Study Design Indications and Interventions sheet
 - Study Design Populations sheet
 - Study Design Objectives and Endpoints sheet
 - Study Design Estimands sheet
 - Study Design Procedures sheet
 - Study Design Encounters sheet
 - Study Design Elements sheet
 - Configuration sheet
 
 The content of each sheet is described below. Example workbooks can be found in the [CDISC Reference Architecture repo](https://github.com/cdisc-org/DDF-RA/tree/sprint-11/Deliverables/IG/examples). *Note: the link above points to the sprint 11 branch. This will be merged into the main branch prior to public review.*
 
-#### CDISC Terminology
+### CDISC Terminology
 
 For those cells where CDISC codes are used the user can enter either the CDISC C Code, for example `C15602`, the CDISC submission value, for example `PHASE III TRIAL`, or the preferred term, for example `Phase III Trial`
 
-#### External Terminology
+### External Terminology
 
 For those cells where external CT is referenced the user can enter code in the form `<code system>: <code> = <decode>`. For example `SPONSOR: A = decode 1, SPONSOR: B = decode 2`.
 
+### Boolean Values
+
+For boolean fields the following can be used to indicate a `true` value `'Y', 'YES', 'T', 'TRUE', '1'` or the lower case equivalents.
+
 ### Identifiers and Cross References
 
 Some content defined within the sheets contain unique identifiers such that the content can be cross referenced in other sheets. This is done so as to link content or expand definitions. Identifiers are simple strings that need to be unique within the workbook. There is a single definition and one or more cross references.
 
+See the [infographic](https://github.com/data4knowledge/usdm/blob/main/docs/sheets.png) for further information.
+
 ### Study Sheet
 
 #### Sheet Name
 
 `study`
 
 #### Sheet Contents
@@ -124,15 +129,17 @@
 | Column | Column Name | Description | Format and Values |
 | :--- | :--- | :--- | :--- |
 | A | organisationIdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
 | B | organisationIdentifier | Organisation identifier | Text string |
 | C | organisationName | Organisation name | Text string |
 | D | organisationType | Organisation type | CDISC code reference |
 | E | studyIdentifier | The identifier for the study | Text string |
-| F | organisationAddress | The organisation address | Formated using a pipe delimited form `line|city|district|state|postal_code|<country code>`. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code. |
+| F | organisationAddress | The organisation address | Formated using a pipe delimited form, see below |
+
+The organisation address is of the form: ```line|city|district|state|postal_code|<country code>```. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code.
 
 ### Study Design sheet
 
 #### Sheet Name
 
 `studyDesign`
 
@@ -273,14 +280,35 @@
 
 `BC: Age, BC: Sec, PR:Informed Consent Form, TL:Exercise` indicates the activity consists of the bcs Age and Sex, a procedure for the informed consent and a timeline specified in the Exercise sheet.
 
 ##### Link
 
 The link section consists of a set of cells into which an upper case 'X' can be placed to link a timepoint with an activity. Otherwise the cell will be ignored. A '-' can be used to fill in cells but "empty".
 
+### Study Design Activities sheet
+
+#### Sheet Name
+
+`studyDesignActivities`
+
+#### Sheet Contents
+
+A header row in row 1 followed by repeating rows from row 2, containing encounter definitions.
+
+| Column | Column Name | Description | Format and Values |
+| :--- | :--- | :--- | :--- |
+| A | activityName	| Name | Text string |
+| B | activityDescription	| Description | Text string |
+| C | activityIsConditional | Conditional flag | Boolean |
+| D | activityIsConditionalReason | Reason | Text string |
+
+Note that this sheet is optional. If the sheet is not provided the activities will be created from those defined in the timeline sheets. These activities will have the name and description set to the name used in the timeline sheet and no condition will be set.
+
+If the sheet is provided but there is no definition in the sheet for an activity referenced in a timeline sheet then the name and description will be set to the name used in the timeline sheet and no condition will be set.
+
 ### Study Design Indications and Interventions Sheet
 	
 #### Sheet Name
 
 `studyDesignII`
 
 #### Sheet Contents
@@ -423,17 +451,12 @@
 A set of rows consisting of configuration parameters. The first column is the type of configuration parameter while the second is the value. The values for specific parameters may vary in their format
 
 | Parameter | Description | Format and Values |
 | :--- | :--- | :--- |
 | CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form CT name = Version value, For example `SNOMED = 21st June 2012`|
 | SDR Prev Next | Allows for next and previous ids to be set to '' rather than null values so as to accomodate the SDR validation checks | Set to 'SDR' to use '' or leave empty to set null values |
 | SDR Root | Allows for the API specification complant JSON output to be wrpaped in a root "clinicalStudy" element so as to accomodate the SDR validation checks | Set to 'SDR' to use wrapper or leave empty to just generate the API compliant JSON |
+| SDR Description | Allows for the description fields within the JSON to be fillled with a string value rather than being set to an empty string if they are left blank in the excel sheets. Currently only applies to description fields | A non-empty string such as `'-', 'not set'` etc |
 
-### Content Not Suported As Yet
-
-It is intended to support all of the content in the USDM. The following features are not yet supported:
-
-- Full Arm definitions
-- Full Epoch definitions
-- BC categories
+### Issues
 
 See the [github issues](https://github.com/data4knowledge/usdm/issues)
```

### Comparing `usdm-0.25.0/setup.py` & `usdm-0.26.0/setup.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm.egg-info/PKG-INFO` & `usdm-0.26.0/src/usdm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usdm
-Version: 0.25.0
+Version: 0.26.0
 Summary: A python package for using the CDISC TransCelerate USDM
 Author: D Iberson-Hurst
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -53,47 +53,52 @@
 excel = USDMExcel("source_data/simple_1.xlsx")
 with open('source_data/simple_1.json', 'w', encoding='utf-8') as f:
   f.write(json.dumps(json.loads(excel.to_json()), indent=2))
 ```
 
 ## Format of Workbook
 
-### General
+### Sheets
 
-#### Sheets
-
-The workbook consists of several sheets each with a dedicated purpose. All sheets must be present.
+The workbook consists of several sheets each with a dedicated purpose. All sheets must be present except for those marked optional.
 
 - Study sheet
 - Study Identifiers sheet
 - Study Design sheet
 - one or more Timeline sheets
+- Study Design Activities sheet (optional)
 - Study Design Indications and Interventions sheet
 - Study Design Populations sheet
 - Study Design Objectives and Endpoints sheet
 - Study Design Estimands sheet
 - Study Design Procedures sheet
 - Study Design Encounters sheet
 - Study Design Elements sheet
 - Configuration sheet
 
 The content of each sheet is described below. Example workbooks can be found in the [CDISC Reference Architecture repo](https://github.com/cdisc-org/DDF-RA/tree/sprint-11/Deliverables/IG/examples). *Note: the link above points to the sprint 11 branch. This will be merged into the main branch prior to public review.*
 
-#### CDISC Terminology
+### CDISC Terminology
 
 For those cells where CDISC codes are used the user can enter either the CDISC C Code, for example `C15602`, the CDISC submission value, for example `PHASE III TRIAL`, or the preferred term, for example `Phase III Trial`
 
-#### External Terminology
+### External Terminology
 
 For those cells where external CT is referenced the user can enter code in the form `<code system>: <code> = <decode>`. For example `SPONSOR: A = decode 1, SPONSOR: B = decode 2`.
 
+### Boolean Values
+
+For boolean fields the following can be used to indicate a `true` value `'Y', 'YES', 'T', 'TRUE', '1'` or the lower case equivalents.
+
 ### Identifiers and Cross References
 
 Some content defined within the sheets contain unique identifiers such that the content can be cross referenced in other sheets. This is done so as to link content or expand definitions. Identifiers are simple strings that need to be unique within the workbook. There is a single definition and one or more cross references.
 
+See the [infographic](https://github.com/data4knowledge/usdm/blob/main/docs/sheets.png) for further information.
+
 ### Study Sheet
 
 #### Sheet Name
 
 `study`
 
 #### Sheet Contents
@@ -138,15 +143,17 @@
 | Column | Column Name | Description | Format and Values |
 | :--- | :--- | :--- | :--- |
 | A | organisationIdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
 | B | organisationIdentifier | Organisation identifier | Text string |
 | C | organisationName | Organisation name | Text string |
 | D | organisationType | Organisation type | CDISC code reference |
 | E | studyIdentifier | The identifier for the study | Text string |
-| F | organisationAddress | The organisation address | Formated using a pipe delimited form `line|city|district|state|postal_code|<country code>`. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code. |
+| F | organisationAddress | The organisation address | Formated using a pipe delimited form, see below |
+
+The organisation address is of the form: ```line|city|district|state|postal_code|<country code>```. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code.
 
 ### Study Design sheet
 
 #### Sheet Name
 
 `studyDesign`
 
@@ -287,14 +294,35 @@
 
 `BC: Age, BC: Sec, PR:Informed Consent Form, TL:Exercise` indicates the activity consists of the bcs Age and Sex, a procedure for the informed consent and a timeline specified in the Exercise sheet.
 
 ##### Link
 
 The link section consists of a set of cells into which an upper case 'X' can be placed to link a timepoint with an activity. Otherwise the cell will be ignored. A '-' can be used to fill in cells but "empty".
 
+### Study Design Activities sheet
+
+#### Sheet Name
+
+`studyDesignActivities`
+
+#### Sheet Contents
+
+A header row in row 1 followed by repeating rows from row 2, containing encounter definitions.
+
+| Column | Column Name | Description | Format and Values |
+| :--- | :--- | :--- | :--- |
+| A | activityName	| Name | Text string |
+| B | activityDescription	| Description | Text string |
+| C | activityIsConditional | Conditional flag | Boolean |
+| D | activityIsConditionalReason | Reason | Text string |
+
+Note that this sheet is optional. If the sheet is not provided the activities will be created from those defined in the timeline sheets. These activities will have the name and description set to the name used in the timeline sheet and no condition will be set.
+
+If the sheet is provided but there is no definition in the sheet for an activity referenced in a timeline sheet then the name and description will be set to the name used in the timeline sheet and no condition will be set.
+
 ### Study Design Indications and Interventions Sheet
 	
 #### Sheet Name
 
 `studyDesignII`
 
 #### Sheet Contents
@@ -437,17 +465,12 @@
 A set of rows consisting of configuration parameters. The first column is the type of configuration parameter while the second is the value. The values for specific parameters may vary in their format
 
 | Parameter | Description | Format and Values |
 | :--- | :--- | :--- |
 | CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form CT name = Version value, For example `SNOMED = 21st June 2012`|
 | SDR Prev Next | Allows for next and previous ids to be set to '' rather than null values so as to accomodate the SDR validation checks | Set to 'SDR' to use '' or leave empty to set null values |
 | SDR Root | Allows for the API specification complant JSON output to be wrpaped in a root "clinicalStudy" element so as to accomodate the SDR validation checks | Set to 'SDR' to use wrapper or leave empty to just generate the API compliant JSON |
+| SDR Description | Allows for the description fields within the JSON to be fillled with a string value rather than being set to an empty string if they are left blank in the excel sheets. Currently only applies to description fields | A non-empty string such as `'-', 'not set'` etc |
 
-### Content Not Suported As Yet
-
-It is intended to support all of the content in the USDM. The following features are not yet supported:
-
-- Full Arm definitions
-- Full Epoch definitions
-- BC categories
+### Issues
 
 See the [github issues](https://github.com/data4knowledge/usdm/issues)
```

### Comparing `usdm-0.25.0/src/usdm.egg-info/SOURCES.txt` & `usdm-0.26.0/src/usdm.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 src/usdm_excel/option_manager.py
 src/usdm_excel/data/cdisc_ct_config.yaml
 src/usdm_excel/data/iso_3166.json
 src/usdm_excel/data/missing_ct.yaml
 src/usdm_excel/errors/__init__.py
 src/usdm_excel/errors/error.py
 src/usdm_excel/errors/errors.py
+src/usdm_excel/study_design_activity_sheet/__init__.py
+src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py
 src/usdm_excel/study_design_arm_sheet/__init__.py
 src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
 src/usdm_excel/study_design_element_sheet/__init__.py
 src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
 src/usdm_excel/study_design_encounter_sheet/__init__.py
 src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
 src/usdm_excel/study_design_epoch_sheet/__init__.py
@@ -97,14 +99,17 @@
 src/usdm_model/study_epoch.py
 src/usdm_model/study_identifier.py
 src/usdm_model/study_protocol_version.py
 src/usdm_model/timing.py
 src/usdm_model/transition_rule.py
 tests/test_base_sheet.py
 tests/test_cdisc_biomedical_concept.py
+tests/test_configuration_sheet.py
 tests/test_error.py
 tests/test_errors.py
+tests/test_integration.py
 tests/test_iso_3166.py
 tests/test_ncit.py
 tests/test_option_manager.py
+tests/test_study_design_activity_sheet.py
 tests/test_study_design_arm_sheet.py
 tests/test_study_design_epoch_sheet.py
```

### Comparing `usdm-0.25.0/src/usdm_excel/base_sheet.py` & `usdm-0.26.0/src/usdm_excel/base_sheet.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import pandas as pd
+from openpyxl import load_workbook
 from usdm_excel.id_manager import id_manager
 from usdm_excel.cdisc_ct import CDISCCT
 from usdm_model.code import Code
 from usdm_excel.ct_version_manager import ct_version_manager
 from usdm_excel.errors.errors import error_manager
 from usdm_excel.logger import package_logger
 from usdm_excel.option_manager import *
 
 class BaseSheet():
 
-  def __init__(self, file_path, sheet_name, header=0):
+  def __init__(self, file_path, sheet_name, header=0, optional=False):
     self.file_path = file_path
     self.sheet_name = sheet_name
-    self.sheet = pd.read_excel(open(file_path, 'rb'), sheet_name=sheet_name, header=header)
+    if optional and not self._sheet_present(file_path, sheet_name):
+      self.sheet = None
+    else:
+      self.sheet = pd.read_excel(open(file_path, 'rb'), sheet_name=sheet_name, header=header)
     self._general_info("Processed sheet %s" % (sheet_name))
 
   def cell_empty(self, row_index, col_index):
     return pd.isnull(self.sheet.iloc[row_index, col_index])  
 
   def read_cell_by_name(self, row_index, field_name):
     try:
@@ -73,18 +77,25 @@
       return ""
     except Exception as e:
       self._error(row_index, col_index, "Error (%s) reading cell row '%s', field '%s'" % (e, row_index, col_index))
       return ""
 
   def read_boolean_cell_by_name(self, row_index, field_name):
     value = self.read_cell_by_name(row_index, field_name)
-    if value.strip().upper() in ['Y', 'YES', 'TRUE', '1']:
+    if value.strip().upper() in ['Y', 'YES', 'T', 'TRUE', '1']:
       return True
     return False
 
+  def read_description_by_name(self, row_index, field_name):
+    value = self.read_cell_by_name(row_index, field_name)
+    empty_value = option_manager.get(Options.DESCRIPTION)
+    if value == "" and not empty_value == "":
+      return empty_value
+    return value
+
   # Want to kill this method
   def set_cdisc_code(self, value):
     if value.strip() == "":
       return None
     parts = value.split("=")
     try:
       return CDISCCT().code(code=parts[0].strip(), decode=parts[1].strip())
@@ -151,23 +162,23 @@
       else:
         self._error(row_index, col_index, f"CDISC CT not found for value '{item.strip()}'.")
     return result
 
   def double_link(self, items, id, prev, next):
     for idx, item in enumerate(items):
       if idx == 0:
-        if option_manager.get(Options.PREVIOUS_NEXT) == PrevNextOption.NULL_STRING:
+        if option_manager.get(Options.PREVIOUS_NEXT) == PrevNextOption.NULL_STRING.value:
           setattr(item, prev, "")
         else:
           setattr(item, prev, None)
       else:
         the_id = getattr(items[idx-1], id)
         setattr(item, prev, the_id)
       if idx == len(items)-1:  
-        if option_manager.get(Options.PREVIOUS_NEXT) == PrevNextOption.NULL_STRING:
+        if option_manager.get(Options.PREVIOUS_NEXT) == PrevNextOption.NULL_STRING.value:
           setattr(item, next, "")
         else:
           setattr(item, next, None)
       else:
         the_id = getattr(items[idx+1], id)
         setattr(item, next, the_id)
 
@@ -198,17 +209,29 @@
 
   def _general_error(self, message):
     error_manager.add(self.sheet_name, None, None, message)
 
   def _warning(self, row, column, message):
     error_manager.add(self.sheet_name, row + 1, column + 1, message, error_manager.WARNING)
 
+  def _debug(self, row, column, message):
+    error_manager.add(self.sheet_name, row + 1, column + 1, message, error_manager.DEBUG)
+
   def _traceback(self, message):
     package_logger.debug(message)
 
   def _format(self, row, column, message):
     if self.sheet_name == None:
       return f"{self.message}"
     elif row == None:
       return f"In sheet {self.sheet_name}: {message}"
     else:
       return f"In sheet {self.sheet_name} at [{row},{column}]: {message}"
+
+  def _get_sheet_names(self, file_path):
+    wb = load_workbook(file_path, read_only=True, keep_links=False)
+    return wb.sheetnames
+
+  def _sheet_present(self, file_path, sheet_name):
+    sheet_names = self._get_sheet_names(file_path)
+    return sheet_name in sheet_names
+
```

### Comparing `usdm-0.25.0/src/usdm_excel/cdisc_ct.py` & `usdm-0.26.0/src/usdm_excel/cdisc_ct.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/cdisc_ct_library.py` & `usdm-0.26.0/src/usdm_excel/cdisc_ct_library.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/configuration_sheet.py` & `usdm-0.26.0/src/usdm_excel/configuration_sheet.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,29 +8,34 @@
 
   PARAMS_NAME_COL = 0
   PARAMS_VALUE_COL = 1
 
   def __init__(self, file_path):
     try:
       super().__init__(file_path=file_path, sheet_name='configuration', header=None)
-      option_manager.set('previous_next', PrevNextOption.NONE)
-      option_manager.set('root', RootOption.API_COMPLIANT)
+      option_manager.set(Options.PREVIOUS_NEXT, PrevNextOption.NONE)
+      option_manager.set(Options.ROOT, RootOption.API_COMPLIANT)
+      option_manager.set(Options.DESCRIPTION, "")
       self._process_sheet()
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet.")
       self._traceback(f"{traceback.format_exc()}")
 
+  def om(self):
+    return option_manager
+  
   def _process_sheet(self):
     for rindex, row in self.sheet.iterrows():
       name = self.read_cell(rindex, self.PARAMS_NAME_COL).strip().upper()
       value = self.read_cell(rindex, self.PARAMS_VALUE_COL)
       if name == 'CT VERSION':
         parts = value.split('=')
         if len(parts) == 2:
           ct_version_manager.add(parts[0].strip(), parts[1].strip())
       elif name == 'SDR PREV NEXT':
         if value.strip().upper() == 'SDR':
           option_manager.set(Options.PREVIOUS_NEXT, PrevNextOption.NULL_STRING)
       elif name == 'SDR ROOT':
         if value.strip().upper() == 'SDR':
           option_manager.set(Options.ROOT, RootOption.SDR_COMPATABLE)
-  
+      elif name == 'SDR DESCRIPTION':
+        option_manager.set(Options.DESCRIPTION, value)
```

### Comparing `usdm-0.25.0/src/usdm_excel/data/cdisc_ct_config.yaml` & `usdm-0.26.0/src/usdm_excel/data/cdisc_ct_config.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/data/iso_3166.json` & `usdm-0.26.0/src/usdm_excel/data/iso_3166.json`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/data/missing_ct.yaml` & `usdm-0.26.0/src/usdm_excel/data/missing_ct.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/errors/error.py` & `usdm-0.26.0/src/usdm_excel/errors/error.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-class Error():
+import logging
 
-  ERROR = 40
-  WARNING = 30
+class Error():
 
-  LABEL = { 40: "error", 30: "warning"}
+  ERROR = logging.ERROR
+  WARNING = logging.WARNING
+  DEBUG = logging.DEBUG
+  LABEL = { ERROR: "error", WARNING: "warning", DEBUG: "debug" }
 
   def __init__(self, sheet: str, row: int, column: int, message: str, level: int=ERROR):
     self.sheet = sheet
     self.row = row
     self.column = column
     self.message = message
     self.level = level
```

### Comparing `usdm-0.25.0/src/usdm_excel/errors/errors.py` & `usdm-0.26.0/src/usdm_excel/errors/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .error import Error
 from usdm_excel.logger import package_logger
 
 class Errors():
 
   WARNING = Error.WARNING
   ERROR = Error.ERROR
+  DEBUG = Error.DEBUG
 
   def __init__(self):
     self.items = []
 
   def clear(self):
     self.items = []
```

### Comparing `usdm-0.25.0/src/usdm_excel/id_manager.py` & `usdm-0.26.0/src/usdm_excel/id_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/iso_3166.py` & `usdm-0.26.0/src/usdm_excel/iso_3166.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/nodes_and_edges.py` & `usdm-0.26.0/src/usdm_excel/nodes_and_edges.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import stringcase
 import json
 
 class NodesAndEdges():
 
-  def __init__(self, study):
+  FULL = "full"
+  TIMELINE = "timeline"
+
+  def __init__(self, study, view=FULL):
     self.study = study
     self.nodes = []
     self.edges = []
     self.add_edges = []
     self.node_index = 1
     self.edge_index = 1
     self.id_node_index_map = {}
@@ -31,15 +34,30 @@
     ]
     self.fix_id_name = {
       'scheduledActivityInstanceId': 'scheduledInstanceId',
       'scheduledDecisionInstanceId': 'scheduledInstanceId',
       'biomedicalConceptSurrogateId': 'bcSurrogateId',
       'biomedicalConceptPropertyId': 'bcPropertyId'
     }
-  
+    self.order_attributes = []
+    self.ignore_klass = []
+    self.collapse_klass = []
+    if view == self.__class__.TIMELINE:
+      self.ignore_klass = [
+        'StudyProtocolVersion', 'StudyIdentifier', 'Indication', 
+        'InvestigationalIntervention', 'Objective', 'StudyDesignPopulation', 
+        'Estimand', 'StudyCell', 'TransitionRule',
+        'BiomedicalConcept', 'BiomedicalConceptCategory', 'BiomedicalConceptSurrogate', 'Procedure', 'AliasCode'
+      ]
+      self.collapse_klass = ['Code']
+      self.order_attributes = [
+        'scheduleSequenceNumber'
+      ]
+    self.sequence_number_map = {}
+      
   def nodes_and_edges(self):
     node = json.loads(self.study.to_json_with_type())
     self._process_node(node)
     for edge in self.add_edges:
       if edge['end'] in self.id_node_index_map:
         edge['id'] = self.edge_index
         edge['end'] = self.id_node_index_map[edge['end']]
@@ -50,42 +68,58 @@
     return self.nodes, self.edges
   
   def _process_node(self, node):
     if type(node) == list:
       result = []
       for item in node:
         indexes = self._process_node(item)
+        if indexes is None:
+          return None
         result = result + indexes
       return result
     elif type(node) == dict:
       if node == {}:
         return []
       properties = {}
       id_field, klass = self._get_id_field_and_klass(node)
+      if klass in self.ignore_klass:
+        return None
       if node[id_field] in self.id_node_index_map:
         return [self.id_node_index_map[node[id_field]]]
       this_node_index = self.node_index
       self.node_index += 1
+      if klass in self.collapse_klass:
+        return []
       for key, value in node.items():
+        # Special case, get the ids for the sequence numbers but within scope of each timeline
+        if key == "scheduleTimelineInstances":
+          self.sequence_number_map = {}
+          for item in value:
+            self.sequence_number_map[item['scheduleSequenceNumber']] = item['scheduledInstanceId']
+        # Link the sequence numbers
+        if key in self.order_attributes:
+          seq = value + 1
+          if seq in self.sequence_number_map:
+            self.add_edges.append( { 'start': this_node_index, 'end': self.sequence_number_map[seq], 'properties': { 'label': key, 'type': 'Order' }})
         if key in self.edge_attributes:
           if key == "conditionAssignments":
             # Special case, array of arrays of condition and link id
             for item in value:
               self.add_edges.append( { 'start': this_node_index, 'end': item[1], 'properties': { 'label': key, 'type': 'Condition' }})
           elif type(value) == list:
             for item in value:
               self.add_edges.append( { 'start': this_node_index, 'end': item, 'properties': { 'label': key, 'type': 'List' }})
           else:
             if not value == "":
               self.add_edges.append( { 'start': this_node_index, 'end': value, 'properties': { 'label': key, 'type': 'Other' }})
-            # else:
-            #   print("Key %s, value >%s<" % (key, value))
         else:
           indexes = self._process_node(value)
-          if indexes == []:
+          if indexes == None:
+            properties[key] = {}
+          elif indexes == []:
             properties[key] = value
           else:
             for index in indexes:
               self.edges.append( {'id': self.edge_index, 'start': this_node_index, 'end': index, 'properties': {'label': key}})
               self.edge_index += 1
       if klass == "Study":
         node[id_field] = "Study"
```

### Comparing `usdm-0.25.0/src/usdm_excel/option_manager.py` & `usdm-0.26.0/src/usdm_excel/option_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 from enum import Enum
 
 class Options(Enum):
-  PREVIOUS_NEXT = 1
-  ROOT = 2
+  PREVIOUS_NEXT = 'previous'
+  ROOT = 'root'
+  DESCRIPTION = 'description'
 
 class PrevNextOption(Enum):
-  NULL_STRING = 1
-  NONE = 2
+  NULL_STRING = 'null_string'
+  NONE = 'none'
 
 class RootOption(Enum):
-  SDR_COMPATABLE = 1
-  API_COMPLIANT = 2
+  SDR_COMPATABLE = 'sdr_compatable'
+  API_COMPLIANT = 'api_compliant'
 
 class OptionManager():
 
   def __init__(self):
     self.items = {}
 
   def clear(self):
     self.items = {}
 
   def set(self, name, value):
+    name = self._to_string(name)
+    value = self._to_string(value)
     self.items[name] = value
 
   def get(self, name):
+    name = self._to_string(name)
     if name in self.items:
       return self.items[name]
     else:
       return ""
+  
+  def _to_string(self, item):
+    if isinstance(item, Enum):
+      return item.value
+    else:
+      return str(item)
     
 option_manager = OptionManager()
```

### Comparing `usdm-0.25.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py` & `usdm-0.26.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
   def __init__(self, file_path):
     try:
       super().__init__(file_path=file_path, sheet_name='studyDesignArms')
       self.items = []
       for index, row in self.sheet.iterrows():
         name = self.read_cell_by_name(index, 'studyArmName')
-        description = self.read_cell_by_name(index, 'studyArmDescription')
+        description = self.read_description_by_name(index, 'studyArmDescription')
         arm_type = self.read_cdisc_klass_attribute_cell_by_name('StudyArm', 'studyArmType', index, 'studyArmType')
-        arm_origin_description = self.read_cell_by_name(index, 'studyArmDataOriginDescription')
+        arm_origin_description = self.read_description_by_name(index, 'studyArmDataOriginDescription')
         arm_origin_type = self.read_cdisc_klass_attribute_cell_by_name('StudyArm', 'studyArmDataOriginType', index, 'studyArmDataOriginType')
         item = StudyArm(
           studyArmId=id_manager.build_id(StudyArm), 
           studyArmName=name,
           studyArmDescription=description,
           studyArmType=arm_type,
           studyArmDataOriginDescription=arm_origin_description,
```

### Comparing `usdm-0.25.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py` & `usdm-0.26.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       super().__init__(file_path=file_path, sheet_name='studyDesignElements')
       self.items = []
       for index, row in self.sheet.iterrows():
         start_rule = None
         end_rule = None
         xref = self.read_cell_by_name(index, 'xref')
         name = self.read_cell_by_name(index, 'studyElementName')
-        description = self.read_cell_by_name(index, 'studyElementDescription')
+        description = self.read_description_by_name(index, 'studyElementDescription')
         start_rule_text = self.read_cell_by_name(index, 'transitionStartRule')
         end_rule_text = self.read_cell_by_name(index, 'transitionEndRule')
         if not start_rule_text == "":
           start_rule = TransitionRule(transitionRuleId=id_manager.build_id(TransitionRule), transitionRuleDescription=start_rule_text)
         if not end_rule_text == "":
           end_rule = TransitionRule(transitionRuleId=id_manager.build_id(TransitionRule), transitionRuleDescription=end_rule_text)
         item = StudyElement(
```

### Comparing `usdm-0.25.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py` & `usdm-0.26.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 from usdm_model.encounter import Encounter
 from usdm_model.transition_rule import TransitionRule
 
 class StudyDesignEncounterSheet(BaseSheet):
 
   def __init__(self, file_path):
     try:
-      #super().__init__(pd.read_excel(open(file_path, 'rb'), sheet_name='studyDesignEncounters'))
       super().__init__(file_path=file_path, sheet_name='studyDesignEncounters')
       self.items = []
       for index, row in self.sheet.iterrows():
         start_rule = None
         end_rule = None
         xref = self.read_cell_by_name(index, 'xref')
         name = self.read_cell_by_name(index, 'encounterName')
-        description = self.read_cell_by_name(index, 'encounterDescription')
+        description = self.read_description_by_name(index, 'encounterDescription')
         type = self.read_cdisc_klass_attribute_cell_by_name('Encounter', 'encounterType', index, 'encounterType')
         setting = self.read_cdisc_klass_attribute_cell_by_name('Encounter', 'encounterEnvironmentalSetting', index, 'encounterEnvironmentalSetting')
         modes = self.read_cdisc_klass_attribute_cell_multiple_by_name('Encounter', 'encounterContactModes', index, 'encounterContactModes')
         start_rule_text = self.read_cell_by_name(index, 'transitionStartRule')
         end_rule_text = self.read_cell_by_name(index, 'transitionEndRule')
         if not start_rule_text == "":
           start_rule = TransitionRule(transitionRuleId=id_manager.build_id(TransitionRule), transitionRuleDescription=start_rule_text)
```

### Comparing `usdm-0.25.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py` & `usdm-0.26.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
   def __init__(self, file_path):
     try:
       super().__init__(file_path=file_path, sheet_name='studyDesignEpochs')
       self.items = []
       for index, row in self.sheet.iterrows():
         name = self.read_cell_by_name(index, 'studyEpochName')
-        description = self.read_cell_by_name(index, 'studyEpochDescription')
+        description = self.read_description_by_name(index, 'studyEpochDescription')
         epoch_type = self.read_cdisc_klass_attribute_cell_by_name('StudyEpoch', 'studyEpochType', index, 'studyEpochType')
         item = StudyEpoch(
           studyEpochId=id_manager.build_id(StudyEpoch), 
           studyEpochName=name, 
           studyEpochDescription=description,
           studyEpochType=epoch_type
         )
```

### Comparing `usdm-0.25.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py` & `usdm-0.26.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     try:
       #super().__init__(pd.read_excel(open(file_path, 'rb'), sheet_name='studyDesignEstimands'))
       super().__init__(file_path=file_path, sheet_name='studyDesignEstimands')
       self.estimands = []
       current = None
       for index, row in self.sheet.iterrows():
         e_summary = self.read_cell_by_name(index, "summaryMeasure")
-        ap_description = self.read_cell_by_name(index, "populationDescription")
+        ap_description = self.read_description_by_name(index, 'populationDescription')
         ice_name = self.read_cell_by_name(index, "intercurrentEventName")
-        ice_description = self.read_cell_by_name(index, "intercurrentEventDescription")
+        ice_description = self.read_description_by_name(index, 'intercurrentEventDescription')
         ice_strategy = self.read_cell_by_name(index, "intercurrentEventStrategy")
         treatment_xref = self.read_cell_by_name(index, "treatmentXref")
         treatment_id = cross_references.get(treatment_xref)
         endpoint_xref = self.read_cell_by_name(index, "endpointXref")
         endpoint_id = cross_references.get(endpoint_xref)
         if not e_summary == "":
           ap = AnalysisPopulation(analysisPopulationId=id_manager.build_id(AnalysisPopulation), populationDescription=ap_description)
```

### Comparing `usdm-0.25.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py` & `usdm-0.26.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       #super().__init__(pd.read_excel(open(file_path, 'rb'), sheet_name='studyDesignII'))
       super().__init__(file_path=file_path, sheet_name='studyDesignII')
       self.indications = []
       self.interventions = []
       for index, row in self.sheet.iterrows():
         xref = self.read_cell_by_name(index, "xref")
         type = self.read_cell_by_name(index, "type")
-        description = self.read_cell_by_name(index, "description")
+        description = self.read_description_by_name(index, "description")
         #codes = self._build_codes(row, index)
         codes = self.read_other_code_cell_multiple_by_name(index, "codes")
         if type.upper() == "IND":
           item = Indication(indicationId=id_manager.build_id(Indication), indicationDescription=description, codes=codes)
           self.indications.append(item)
           cross_references.add(xref, item.indicationId)
         else:
```

### Comparing `usdm-0.25.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py` & `usdm-0.26.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
   def __init__(self, file_path):
     try:
       #super().__init__(pd.read_excel(open(file_path, 'rb'), sheet_name='studyDesignPopulations'))
       super().__init__(file_path=file_path,  sheet_name='studyDesignPopulations')
       self.populations = []
       for index, row in self.sheet.iterrows():
-        description = self.read_cell_by_name(index, "populationDescription")
+        description = self.read_description_by_name(index, 'populationDescription')
         number = self.read_cell_by_name(index, "plannedNumberOfParticipants")
         min = self.read_cell_by_name(index, "plannedMinimumAgeOfParticipants")
         max = self.read_cell_by_name(index, "plannedMaximumAgeOfParticipants")
         codes = self._build_codes(row, index)
         self.populations.append(
           StudyDesignPopulation(studyDesignPopulationId=id_manager.build_id(StudyDesignPopulation), 
             populationDescription=description,
```

### Comparing `usdm-0.25.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py` & `usdm-0.26.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 import pandas as pd
 from usdm_model.procedure import Procedure
 
 class StudyDesignProcedureSheet(BaseSheet):
 
   def __init__(self, file_path):
     try:
-      #super().__init__(pd.read_excel(open(file_path, 'rb'), sheet_name='studyDesignProcedures'))
       super().__init__(file_path=file_path, sheet_name='studyDesignProcedures')
       self.procedures = []
       for index, row in self.sheet.iterrows():
         xref = self.read_cell_by_name(index, "xref")
         name = self.read_cell_by_name(index, "procedureName")
-        description = self.read_cell_by_name(index, "procedureDescription")
+        description = self.read_description_by_name(index, 'procedureDescription')
         type = self.read_cell_by_name(index, "procedureType")
         code = self.read_other_code_cell_by_name(index, 'procedureCode')
         conditional = self.read_boolean_cell_by_name(index, 'procedureIsConditional')
         reason = self.read_cell_by_name(index, 'procedureIsConditionalReason')
         item = Procedure(procedureId=id_manager.build_id(Procedure),
           procedureName=name,
           procedureDescription=description,
```

### Comparing `usdm-0.25.0/src/usdm_excel/study_design_sheet/study_design_sheet.py` & `usdm-0.26.0/src/usdm_excel/study_design_sheet/study_design_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py` & `usdm-0.26.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/study_sheet/study_sheet.py` & `usdm-0.26.0/src/usdm_excel/study_sheet/study_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from usdm_excel.study_design_objective_endpoint_sheet.study_design_objective_endpoint_sheet import StudyDesignObjectiveEndpointSheet
 from usdm_excel.study_design_estimands_sheet.study_design_estimands_sheet import StudyDesignEstimandsSheet
 from usdm_excel.study_design_procedure_sheet.study_design_procedure_sheet import StudyDesignProcedureSheet
 from usdm_excel.study_design_encounter_sheet.study_design_encounter_sheet import StudyDesignEncounterSheet
 from usdm_excel.study_design_element_sheet.study_design_element_sheet import StudyDesignElementSheet
 from usdm_excel.study_design_arm_sheet.study_design_arm_sheet import StudyDesignArmSheet
 from usdm_excel.study_design_epoch_sheet.study_design_epoch_sheet import StudyDesignEpochSheet
+from usdm_excel.study_design_activity_sheet.study_design_activity_sheet import StudyDesignActivitySheet
 from usdm_excel.alias import Alias
 from usdm_excel.id_manager import id_manager
 from usdm_excel.cross_ref import cross_references
 from usdm_excel.option_manager import *
 from usdm_model.api_base_model import ApiBaseModel
 from usdm_model.study import Study
 from usdm_model.study_protocol_version import StudyProtocolVersion
@@ -57,14 +58,15 @@
       self._process_sheet()
       self.study_identifiers = StudyIdentifiersSheet(file_path)
       self.procedures = StudyDesignProcedureSheet(file_path)
       self.encounters = StudyDesignEncounterSheet(file_path)
       self.elements = StudyDesignElementSheet(file_path)
       self.arms = StudyDesignArmSheet(file_path)
       self.epochs = StudyDesignEpochSheet(file_path)
+      self.activities = StudyDesignActivitySheet(file_path)
       self.study_design = StudyDesignSheet(file_path)
       for timeline in self.study_design.other_timelines:
         tl = StudySoASheet(file_path, timeline)
         self.timelines[timeline] = tl
         cross_references.add(timeline, tl.timeline.scheduleTimelineId)
       self.soa = StudySoASheet(file_path, self.study_design.main_timeline)
       self.ii = StudyDesignIISheet(file_path)
@@ -115,15 +117,15 @@
   def study_regulatory(self):
     return self.cdisc_code(code="C93453", decode="Study Registry")
 
   def the_study(self):
     return self.study
   
   def api_root(self):
-    if option_manager.get(Options.ROOT) == RootOption.SDR_COMPATABLE:
+    if option_manager.get(Options.ROOT) == RootOption.SDR_COMPATABLE.value:
       root = SDRRoot(clinicalStudy=self.study)
     else:
       root = self.study
     return root
 
   def _process_sheet(self):
     fields = [ 'briefTitle', 'officialTitle', 'publicTitle', 'scientificTitle', 'protocolVersion', 'protocolAmendment', 'protocolEffectiveDate', 'protocolStatus' ]
```

### Comparing `usdm-0.25.0/src/usdm_excel/study_soa_sheet/activities.py` & `usdm-0.26.0/src/usdm_excel/study_soa_sheet/activities.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/study_soa_sheet/activity.py` & `usdm-0.26.0/src/usdm_excel/study_soa_sheet/activity.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,54 +6,65 @@
 from usdm_model.biomedical_concept_surrogate import BiomedicalConceptSurrogate
 from usdm_excel.cdisc_biomedical_concept import cdisc_bc_library
 import pandas as pd
 
 class Activity():
   
   def __init__(self, parent, row_index):
-    #super().__init__(sheet)
-    #self._row_index = row_index
     self.parent = parent
+    self.row_index = row_index
     self.usdm_biomedical_concept_surrogates = []
     self.usdm_biomedical_concepts = []
     self.name = parent.read_cell(row_index, SoAColumnRows.CHILD_ACTIVITY_COL)
     self._bcs, self._prs, self._tls = self._get_observation_cell(row_index, SoAColumnRows.BC_COL)
+    self.parent._debug(row_index, SoAColumnRows.BC_COL, f"Activity {self.name} read. BC: {self._bcs}, PR: {self._prs}, TL: {self._tls}")
     self.usdm_activity = self._as_usdm()
     
   def _as_usdm(self):
     surrogate_bc_items = []
     full_bc_items = []
     procedures = []
-    #cdisc_bcs = CDISCBiomedicalConcepts()
     for bc in self._bcs:
       if cdisc_bc_library.exists(bc):
         full_bc = cdisc_bc_library.usdm(bc)
         full_bc_items.append(full_bc.biomedicalConceptId)
         self.usdm_biomedical_concepts.append(full_bc)
       else:
         surrogate = self._to_bc_surrogates(bc)
         surrogate_bc_items.append(surrogate.bcSurrogateId)
         self.usdm_biomedical_concept_surrogates.append(surrogate)
     timelineId = ""
     if len(self._tls) > 0:
       timelineId = cross_references.get(self._tls[0])
     for procedure in self._prs:
-      procedures.append(cross_references.get(procedure))
-    return USDMActivity(
-      activityId=id_manager.build_id(Activity),
-      activityName=self.name,
-      activityDescription=self.name,
-      definedProcedures=procedures,
-      activityIsConditional=False,
-      activityIsConditionalReason="",
-      biomedicalConceptIds=full_bc_items,
-      bcCategoryIds=[],
-      bcSurrogateIds=surrogate_bc_items,
-      activityTimelineId=timelineId
-    )
+      ref = cross_references.get(procedure)
+      if ref is not None:
+        procedures.append(cross_references.get(procedure))
+      else:
+        self.parent._warning(self.row_index, SoAColumnRows.BC_COL, f"Cross reference error for procedure {procedure}, not found")
+    activity = cross_references.get(self.name)
+    if activity is None:
+      return USDMActivity(
+        activityId=id_manager.build_id(Activity),
+        activityName=self.name,
+        activityDescription=self.name,
+        definedProcedures=procedures,
+        activityIsConditional=False,
+        activityIsConditionalReason="",
+        biomedicalConceptIds=full_bc_items,
+        bcCategoryIds=[],
+        bcSurrogateIds=surrogate_bc_items,
+        activityTimelineId=timelineId
+      )
+    else:
+      activity.definedProcedures = procedures
+      activity.biomedicalConceptIds = full_bc_items
+      activity.bcSurrogateIds = surrogate_bc_items
+      activity.activityTimelineId = timelineId
+    return activity
   
   def _to_bc_surrogates(self, name):
     return BiomedicalConceptSurrogate(
       bcSurrogateId=id_manager.build_id(BiomedicalConceptSurrogate),
       bcSurrogateName=name,
       bcSurrogateDescription=name,
       bcSurrogateReference=''
```

### Comparing `usdm-0.25.0/src/usdm_excel/study_soa_sheet/cycle.py` & `usdm-0.26.0/src/usdm_excel/study_soa_sheet/cycle.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/study_soa_sheet/cycles.py` & `usdm-0.26.0/src/usdm_excel/study_soa_sheet/cycles.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/study_soa_sheet/encounters.py` & `usdm-0.26.0/src/usdm_excel/study_soa_sheet/encounters.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py` & `usdm-0.26.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/study_soa_sheet/timepoint.py` & `usdm-0.26.0/src/usdm_excel/study_soa_sheet/timepoint.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_excel/study_soa_sheet/timepoints.py` & `usdm-0.26.0/src/usdm_excel/study_soa_sheet/timepoints.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_model/__init__.py` & `usdm-0.26.0/src/usdm_model/__init__.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_model/activity.py` & `usdm-0.26.0/src/usdm_model/activity.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_model/api_base_model.py` & `usdm-0.26.0/src/usdm_model/api_base_model.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_model/encounter.py` & `usdm-0.26.0/src/usdm_model/encounter.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_model/estimand.py` & `usdm-0.26.0/src/usdm_model/estimand.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_model/scheduled_instance.py` & `usdm-0.26.0/src/usdm_model/scheduled_instance.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_model/study.py` & `usdm-0.26.0/src/usdm_model/study.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_model/study_design.py` & `usdm-0.26.0/src/usdm_model/study_design.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/src/usdm_model/study_identifier.py` & `usdm-0.26.0/src/usdm_model/study_identifier.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/tests/test_base_sheet.py` & `usdm-0.26.0/tests/test_base_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,32 +138,50 @@
 
 # read_cell_with_previous
 
 def test_read_boolean_cell_by_name(mocker):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   #data = [[0, 1, 2, 3, 4, 5, 6, 7, 8], ['a', 'y', 'Y', 'true', 'True', 'yes', 1, '1', '']]
-  data = [[0, 'a'], [1, 'y'], [2, 'Y'], [3, 'true'], [4, 'True'], [5, 'yes'], [6, 1,], [7, '1'], [8, '']]
+  data = [[0, 'a'], [1, 'y'], [2, 'Y'], [3, 'true'], [4, 'True'], [5, 'yes'], [6, 1,], [7, '1'], [8, ''], [9, 'T']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['Name', 'Children'])
   base = BaseSheet("", "sheet")
   test_data = [
     (0,'Children',False),
     (1,'Children',True),
     (2,'Children',True),
     (3,'Children',True),
     (4,'Children',True),
     (5,'Children',True),
     (6,'Children',True),
     (7,'Children',True),
     (8,'Children',False),
+    (9,'Children',True),
   ]
   for test in test_data:
     assert(base.read_boolean_cell_by_name(test[0],test[1])) == test[2]
 
+def test_read_description_by_name(mocker):
+  mock_option = mocker.patch("usdm_excel.om.get")
+  mock_option.side_effect=['xxx', 'xxx', 'xxx']
+  mocked_open = mocker.mock_open(read_data="File")
+  mocker.patch("builtins.open", mocked_open)
+  data = [[0, ''], [1, 'something'], [2, '  ']]
+  mock_read = mocker.patch("pandas.read_excel")
+  mock_read.return_value = pd.DataFrame(data, columns=['Name', 'Children'])
+  base = BaseSheet("", "sheet")
+  test_data = [
+    (0,'Children','xxx'),
+    (1,'Children','something'),
+    (2,'Children','xxx'),
+  ]
+  for test in test_data:
+    assert(base.read_description_by_name(test[0],test[1])) == test[2]
+
 @xfail
 def test_read_cell_with_previous():
   assert 0
 
 @xfail
 def test_read_other_code_cell_by_name():
   assert 0
```

### Comparing `usdm-0.25.0/tests/test_cdisc_biomedical_concept.py` & `usdm-0.26.0/tests/test_cdisc_biomedical_concept.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/tests/test_error.py` & `usdm-0.26.0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/tests/test_errors.py` & `usdm-0.26.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/tests/test_iso_3166.py` & `usdm-0.26.0/tests/test_iso_3166.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/tests/test_study_design_arm_sheet.py` & `usdm-0.26.0/tests/test_study_design_arm_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.25.0/tests/test_study_design_epoch_sheet.py` & `usdm-0.26.0/tests/test_study_design_epoch_sheet.py`

 * *Files identical despite different names*

