# Comparing `tmp/aiida_sssp_workflow-3.0.2.tar.gz` & `tmp/aiida_sssp_workflow-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_sssp_workflow-3.0.2.tar", last modified: Fri Apr 14 09:00:31 2023, max compression
+gzip compressed data, was "aiida_sssp_workflow-3.0.3.tar", last modified: Mon May 15 15:36:58 2023, max compression
```

## Comparing `aiida_sssp_workflow-3.0.2.tar` & `aiida_sssp_workflow-3.0.3.tar`

### file list

```diff
@@ -1,1136 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.715153 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/birch_murnaghan_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/calculate_bands_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/calculate_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/wien2k_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/tools/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/tools/relabel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/efermi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/bands.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/control.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/criteria.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/delta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/
--rw-r--r--   0 runner    (1001) docker     (123)   113612 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/AE-average-oxides.json
--rw-r--r--   0 runner    (1001) docker     (123)    81057 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/AE-average-unaries.json
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_LANN.json
--rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_TYPICAL.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/mapping.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.787159 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.799159 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ag.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Al.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ar.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/As.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Au.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/B.cif
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ba.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Be.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Bi.cif
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Br.cif
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/C.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ca.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cd.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/CeN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cl.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Co.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cr.cif
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cs.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cu.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/DyN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/ErN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/EuN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/F.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Fe.cif
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ga.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/GdN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ge.cif
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/H.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/He.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Hf.cif
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Hg.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/HoN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/I.cif
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/In.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ir.cif
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/K.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Kr.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/LaN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Li.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Lu.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/LuN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Mg.cif
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Mn.cif
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Mo.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/N.cif
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Na.cif
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Nb.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/NdN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ne.cif
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ni.cif
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/O.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Os.cif
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/P.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Pb.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Pd.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/PmN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Po.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/PrN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Pt.cif
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Rb.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Re.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Rh.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Rn.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ru.cif
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/S.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Sb.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Sc.cif
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Se.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Si.cif
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/SiF4.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/SmN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Sn.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Sr.cif
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ta.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/TbN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Tc.cif
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Te.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ti.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Tl.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/TmN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/V.cif
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/W.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Xe.cif
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Y.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/YbN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Zn.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Zr.cif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.871165 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ac_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ac_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ac_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ac_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ag_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ag_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ag_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ag_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Al_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Al_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Al_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Al_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Am_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Am_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Am_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Am_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ar_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ar_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ar_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ar_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/As_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/As_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/As_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/As_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/At_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/At_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/At_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/At_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Au_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Au_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Au_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Au_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/B_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/B_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/B_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/B_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ba_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ba_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ba_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ba_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Be_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Be_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Be_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Be_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Bi_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Bi_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Bi_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Bi_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Br_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Br_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Br_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Br_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/C_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/C_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/C_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/C_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ca_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ca_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ca_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ca_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cd_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cd_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cd_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cd_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ce_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ce_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ce_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ce_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cl_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cl_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cl_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cl_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cm_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cm_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cm_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cm_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Co_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Co_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Co_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Co_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cr_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cr_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cr_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cr_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cs_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cs_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cs_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cs_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cu_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cu_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cu_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cu_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Dy_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Dy_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Dy_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Dy_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Er_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Er_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Er_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Er_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Eu_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Eu_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Eu_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Eu_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/F_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/F_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/F_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/F_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fe_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fe_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fe_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fe_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fr_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fr_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fr_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fr_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ga_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ga_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ga_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ga_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Gd_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Gd_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Gd_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Gd_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ge_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ge_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ge_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ge_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/H_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/H_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/H_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/H_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/He_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/He_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/He_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/He_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hf_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hf_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hf_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hf_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hg_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hg_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hg_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hg_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ho_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ho_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ho_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ho_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/I_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/I_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/I_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/I_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/In_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/In_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/In_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/In_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ir_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ir_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ir_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ir_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/K_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/K_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/K_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/K_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Kr_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Kr_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Kr_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Kr_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/La_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/La_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/La_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/La_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Li_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Li_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Li_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Li_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Lu_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Lu_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Lu_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Lu_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mg_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mg_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mg_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mg_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mn_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mn_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mn_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mn_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mo_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mo_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mo_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mo_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/N_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/N_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/N_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/N_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Na_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Na_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Na_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Na_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nb_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nb_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nb_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nb_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nd_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nd_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nd_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nd_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ne_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ne_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ne_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ne_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ni_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ni_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ni_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ni_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Np_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Np_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Np_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Np_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/O_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/O_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/O_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/O_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Os_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Os_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Os_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Os_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/P_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/P_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/P_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/P_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pa_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pa_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pa_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pa_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pb_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pb_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pb_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pb_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pd_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pd_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pd_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pd_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pm_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pm_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pm_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pm_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Po_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Po_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Po_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Po_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pr_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pr_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pr_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pr_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pt_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pt_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pt_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pt_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pu_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pu_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pu_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pu_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ra_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ra_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ra_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ra_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rb_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rb_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rb_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rb_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Re_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Re_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Re_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Re_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rh_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rh_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rh_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rh_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rn_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rn_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rn_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rn_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ru_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ru_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ru_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ru_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/S_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/S_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/S_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/S_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sb_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sb_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sb_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sb_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sc_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sc_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sc_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sc_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Se_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Se_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Se_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Se_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Si_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Si_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Si_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Si_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sm_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sm_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sm_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sm_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sn_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sn_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sn_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sn_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sr_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sr_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sr_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sr_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ta_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ta_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ta_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ta_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tb_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tb_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tb_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tb_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tc_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tc_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tc_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tc_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Te_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Te_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Te_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Te_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Th_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Th_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Th_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Th_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ti_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ti_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ti_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ti_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tl_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tl_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tl_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tl_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tm_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tm_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tm_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tm_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/U_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/U_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/U_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/U_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/V_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/V_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/V_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/V_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/W_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/W_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/W_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/W_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Xe_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Xe_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Xe_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Xe_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Y_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Y_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Y_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Y_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Yb_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Yb_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Yb_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Yb_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zn_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zn_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zn_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zn_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zr_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zr_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zr_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zr_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.871165 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/upf/
--rw-r--r--   0 runner    (1001) docker     (123)   632448 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/upf/N.us.z_5.ld1.theose.v0.upf
--rw-r--r--   0 runner    (1001) docker     (123)   880280 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/upf/O.paw.z_6.ld1.psl.v0.1.upf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/upf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.871165 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/bands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/cohesive_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/phonon_frequencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/pressure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_bands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_cohesive_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_eos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_phonon_frequencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_pressure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/measure/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/measure/bands.py
--rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/measure/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)    14256 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/verifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-04-14 09:00:31.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    55501 2023-04-14 09:00:31.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:00:31.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-14 09:00:31.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-14 09:00:31.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 09:00:31.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/efermi/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/efermi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/pseudo_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/pseudo_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/pseudo_parser/upf_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/pseudo_parser/upf_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/tests/test_nightly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.445793 aiida_sssp_workflow-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-05-15 15:36:58.445793 aiida_sssp_workflow-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.433792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.433792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/calculations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/calculations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/calculations/birch_murnaghan_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/calculations/calculate_bands_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/calculations/calculate_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/calculations/wien2k_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.433792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/cli/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.433792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/cli/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/cli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/cli/tools/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/cli/tools/relabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/efermi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.437792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/protocol/bands.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/protocol/control.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/protocol/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/protocol/criteria.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/protocol/delta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.437792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.437792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/AE_EOS/
+-rw-r--r--   0 runner    (1001) docker     (123)   113612 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/AE_EOS/AE-average-oxides.json
+-rw-r--r--   0 runner    (1001) docker     (123)    81057 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/AE_EOS/AE-average-unaries.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_LANN.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_TYPICAL.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/AE_EOS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.437792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/structures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.437792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/structures/oxides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/structures/oxides/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.437792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/structures/typical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/structures/typical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.437792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/structures/unaries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/structures/unaries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.437792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/upf/
+-rw-r--r--   0 runner    (1001) docker     (123)   632448 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/upf/N.us.z_5.ld1.theose.v0.upf
+-rw-r--r--   0 runner    (1001) docker     (123)   880280 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/upf/O.paw.z_6.ld1.psl.v0.1.upf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/upf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.441792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.441792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24134 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/cohesive_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/phonon_frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/pressure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.441792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/_bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/_cohesive_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/_eos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/_phonon_frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/_pressure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.445793 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/measure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/measure/bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/measure/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14258 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/verifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.433792 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-05-15 15:36:58.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-15 15:36:58.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:36:58.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-15 15:36:58.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-15 15:36:58.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 15:36:58.000000 aiida_sssp_workflow-3.0.3/aiida_sssp_workflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.445793 aiida_sssp_workflow-3.0.3/efermi/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/efermi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.445793 aiida_sssp_workflow-3.0.3/pseudo_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/pseudo_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.445793 aiida_sssp_workflow-3.0.3/pseudo_parser/upf_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/pseudo_parser/upf_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-15 15:36:58.445793 aiida_sssp_workflow-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:36:58.445793 aiida_sssp_workflow-3.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-15 15:36:49.000000 aiida_sssp_workflow-3.0.3/tests/test_nightly.py
```

### Comparing `aiida_sssp_workflow-3.0.2/LICENSE` & `aiida_sssp_workflow-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/PKG-INFO` & `aiida_sssp_workflow-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida_sssp_workflow
-Version: 3.0.2
+Version: 3.0.3
 Summary: Package for the AiiDA SSSP workflow
 Home-page: https://github.com/aiidateam/aiida-sssp-workflow
 Author: Jusong Yu
 Author-email: jusong.yu@epfl.ch
 License: MIT
 Project-URL: Bug Tracker, https://github.com/aiidateam/aiida-sssp-workflow/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aiida_sssp_workflow-3.0.2/README.md` & `aiida_sssp_workflow-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/birch_murnaghan_fit.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/calculations/birch_murnaghan_fit.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/calculate_bands_distance.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/calculations/calculate_bands_distance.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/calculate_delta.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/calculations/calculate_delta.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/wien2k_ref.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/calculations/wien2k_ref.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/__init__.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/extract.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/cli/extract.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/run.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/cli/run.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 
 from aiida_sssp_workflow.cli import cmd_root
 from aiida_sssp_workflow.workflows.verifications import DEFAULT_PROPERTIES_LIST
 
 UpfData = DataFactory("pseudo.upf")
 VerificationWorkChain = WorkflowFactory("sssp_workflow.verification")
 
-SSSP_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "_sssp")
-
 # Trigger the launch by running:
 # aiida-sssp-workflow launch --property accuracy.delta --pw-code pw-7.0@localhost --ph-code ph-7.0@localhost --protocol test --cutoff-control test --criteria efficiency --withmpi True -- examples/_static/Si_ONCV_PBE-1.2.upf
 
 
 @cmd_root.command("launch")
 @options.OverridableOption(
     "--pw-code", "pw_code", type=types.CodeParamType(entry_point="quantumespresso.pw")
@@ -48,14 +46,19 @@
     "--cutoff-control",
     default="standard",
     help="Control of convergence.",
 )
 @click.option(
     "criteria", "--criteria", default="efficiency", help="Criteria of convergence."
 )
+@click.option(
+    "configuration",
+    "--configuration",
+    help="(convergence only) Configuration of structure, can be: SC, FCC, BCC, Diamond, XO, XO2, XO3, X2O, X2O3, X2O5, TYPICAL.",
+)
 @click.option("withmpi", "--withmpi", default=True, help="Run with mpi.")
 @click.option("npool", "--npool", default=1, help="Number of pool.")
 @click.option("walltime", "--walltime", default=3600, help="Walltime.")
 @click.option("num_mpiprocs", "--num-mpiprocs", default=1, help="Number of mpiprocs.")
 @click.option(
     "--clean-workchain/--no-clean-workchain",
     default=True,
@@ -70,14 +73,15 @@
 def launch(
     pw_code,
     ph_code,
     property,
     protocol,
     cutoff_control,
     criteria,
+    configuration,
     withmpi,
     npool,
     walltime,
     num_mpiprocs,
     pseudo,
     clean_workchain,
     daemon,
@@ -102,102 +106,52 @@
     computer = pw_code.computer.label
     label, _ = os.path.splitext(basename)
     label = orm.Str(f"({protocol}-{criteria}-{cutoff_control} at {computer}) {label}")
 
     with open(pseudo, "rb") as stream:
         pseudo = UpfData(stream)
 
-    _basic_inputs = {
+    inputs = {
+        "accuracy": {
+            "protocol": orm.Str(protocol),
+            "cutoff_control": orm.Str(cutoff_control),
+        },
+        "convergence": {
+            "protocol": orm.Str(protocol),
+            "cutoff_control": orm.Str(cutoff_control),
+            "criteria": orm.Str(criteria),
+        },
         "pw_code": pw_code,
         "ph_code": ph_code,
-        "protocol": orm.Str(protocol),
-        "cutoff_control": orm.Str(cutoff_control),
-        "criteria": orm.Str(criteria),
+        "pseudo": pseudo,
+        "label": label,
+        "properties_list": orm.List(properties_list),
         "options": orm.Dict(
             dict={
                 "resources": {
                     "num_machines": 1,
                     "num_mpiprocs_per_machine": num_mpiprocs,
                 },
                 "max_wallclock_seconds": walltime,
                 "withmpi": withmpi,
             }
         ),
-        "parallization": orm.Dict(dict={"npool": npool}),
-        "properties_list": orm.List(list=properties_list),
-    }
-
-    _pseudo_inputs = {
-        "pseudo": pseudo,
-        "label": label,
-        "extra_desc": extra_desc,
-    }
-
-    node = run_verification(
-        **_basic_inputs,
-        **_pseudo_inputs,
-        clean_workchain=clean_workchain,
-        on_daemon=daemon,
-    )
-
-    click.echo(node)
-    click.echo(f"calculated on property: {'/'.join(properties_list)}")
-
-
-def run_verification(
-    pseudo,
-    pw_code,
-    ph_code,
-    protocol,
-    cutoff_control,
-    criteria,
-    options,
-    parallization,
-    properties_list,
-    label,
-    extra_desc,
-    clean_workchain,
-    on_daemon,
-):
-    """
-    pw_code: code for pw.x calculation
-    ph_code: code for ph.x calculation
-    upf: upf file to verify
-    properties_list: propertios to verified
-    label: if None, label will parsed from filename
-    mode:
-        test to run on localhost with test protocol
-        precheck: precheck control protocol on convergence verification
-        standard: running a production on eiger
-    """
-    inputs = {
-        "accuracy": {
-            "protocol": protocol,
-            "cutoff_control": cutoff_control,
-        },
-        "convergence": {
-            "protocol": protocol,
-            "cutoff_control": cutoff_control,
-            "criteria": criteria,
-        },
-        "pw_code": pw_code,
-        "ph_code": ph_code,
-        "pseudo": pseudo,
-        "label": label,
-        "properties_list": properties_list,
-        "options": options,
-        "parallelization": parallization,
+        "parallelization": orm.Dict(dict={"npool": npool}),
         "clean_workchain": orm.Bool(clean_workchain),
     }
 
-    if on_daemon:
+    if configuration is not None:
+        inputs["convergence"]["configuration"] = orm.Str(configuration)
+
+    if daemon:
         node = submit(VerificationWorkChain, **inputs)
     else:
         _, node = run_get_node(VerificationWorkChain, **inputs)
 
     node.description = f"{label.value} ({extra_desc})"
 
-    return node
+    click.echo(node)
+    click.echo(f"calculated on property: {'/'.join(properties_list)}")
 
 
 if __name__ == "__main__":
     launch()
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/tools/dump.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/cli/tools/dump.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/tools/relabel.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/cli/tools/relabel.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/efermi.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/efermi.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/bands.yml` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/protocol/bands.yml`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/control.yml` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/protocol/control.yml`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/converge.yml` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/protocol/converge.yml`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/criteria.yml` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/protocol/criteria.yml`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/delta.yml` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/protocol/delta.yml`

 * *Files 0% similar despite different names*

```diff
@@ -19,31 +19,31 @@
     degauss: 0.0045
     smearing: fd
     electron_conv_thr: 1.0e-6
     kpoints_distance: 0.5
     scale_count: 5
     scale_increment: 0.02
     configurations:
-        - XO
+        - XO2
         - BCC
 
 opsp:
     name: opsp
     description: For OPSP verifications
 
     occupations: smearing
     degauss: 0.0045
     smearing: fd
     electron_conv_thr: 1.0e-8
     kpoints_distance: 0.2
     scale_count: 7
     scale_increment: 0.02
     configurations:
-        - XO2
-        - SC
+        - XO
+        - BCC
 
 opsp-full:
     name: opsp-full
     description: For OPSP verifications with all configurations
 
     occupations: smearing
     degauss: 0.0045
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/AE-average-oxides.json` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/AE_EOS/AE-average-oxides.json`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/AE-average-unaries.json` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/AE_EOS/AE-average-unaries.json`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_LANN.json` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_LANN.json`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_TYPICAL.json` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_TYPICAL.json`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/upf/N.us.z_5.ld1.theose.v0.upf` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/upf/N.us.z_5.ld1.theose.v0.upf`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/upf/O.paw.z_6.ld1.psl.v0.1.upf` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/statics/upf/O.paw.z_6.ld1.psl.v0.1.upf`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/utils.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,81 +118,107 @@
 ) -> orm.StructureData:
     """
     get cif abspath from element for bands measure and convergence
     property can be `delta`, `bands` or `convergence`
 
     The principles are for bands measure, using the configurations from Cottiner's paper since they are the groud state structures exist in real wolrd.
     And for lanthanides using the Nitrides from Wenzowech paper.
-    Using the uniaries/diamond configurations for convergence verification.
+    For elements that don't have configuration from Cottiner's paper, using the uniaries/diamond configurations for convergence verification.
 
     The structure is convert to primitive cell except for those magnetic elements
     configurations (typical ones of Cottiner's paper) for bands measure, since we need to
     set the starting magnetizations for sites.
 
     If prop is delta must provide specific configuration name.
 
     Args:
         element (str): element
         configuration (str): BCC, FCC, SC, Diamond, XO, XO2, XO3, X2O, X2O3, X2O5, RE
 
     Returns:
         orm.StructureData: return a orm.StructureData
     """
+    from pathlib import Path
+
+    from aiida.tools.data.array.kpoints import get_kpoints_path
+    from ase import io
+
     # If for delta measure workflow
-    base_cif_module = "aiida_sssp_workflow.statics.cif"
-    if prop == "delta":
-        if configuration == "RE":
-            assert element in RARE_EARTH_ELEMENTS
+    base_structure_module = "aiida_sssp_workflow.statics.structures"
 
-            # use RE-nitrides of Wenzovich paper
-            # from typical cif folder
-            res_path = importlib.resources.path(
-                f"{base_cif_module}.typical", f"{element}N.cif"
-            )
-
-        if configuration == "TYPICAL":
-            res_path = importlib.resources.path(
-                f"{base_cif_module}.typical", f"{element}.cif"
-            )
-
-        if configuration in OXIDE_CONFIGURATIONS:
-            res_path = importlib.resources.path(
-                f"{base_cif_module}.oxides", f"{element}_{configuration}.cif"
-            )
-
-        if configuration in UNARIE_CONFIGURATIONS:
-            res_path = importlib.resources.path(
-                f"{base_cif_module}.unaries", f"{element}_{configuration}.cif"
-            )
+    if configuration == "RE":
+        assert element in RARE_EARTH_ELEMENTS
 
-    else:
-        # If for bands measure or convergence workflow
+        # use RE-nitrides of Wenzovich paper
+        # from typical cif folder
+        res_path = importlib.resources.path(
+            f"{base_structure_module}.typical", f"{element}N.cif"
+        )
+
+    if configuration == "TYPICAL":
+        res_path = importlib.resources.path(
+            f"{base_structure_module}.typical", f"{element}.cif"
+        )
+
+    # For elements that are verified in ACWF paper, use the XSF files.
+    # https://github.com/aiidateam/acwf-verification-scripts/tree/main/0-preliminary-do-not-run
+    if configuration in OXIDE_CONFIGURATIONS:
+        res_path = importlib.resources.path(
+            f"{base_structure_module}.oxides", f"{element}-{configuration}.xsf"
+        )
+
+    if configuration in UNARIE_CONFIGURATIONS:
+        res_path = importlib.resources.path(
+            f"{base_structure_module}.unaries", f"{element}-{configuration}.xsf"
+        )
+
+    if configuration is None:
+        # If configuration is not specified, use the one from mapping.json as default
         # after some back-forward, most elements only use typical structure
         # for bands and for convergence. But with the primitived structure.
         # But for future maintainance, I keep the mapping.json for configuration
-        # mapping. Only At using unaries since it is not in typical.
+        # mapping. Only At, Fr, Ra and actinides using unaries FCC since it is not in typical.
         import_path = importlib.resources.path(
-            "aiida_sssp_workflow.statics.cif", f"mapping.json"
+            "aiida_sssp_workflow.statics.structures", f"mapping.json"
         )
 
         with import_path as path, open(path, "r") as handle:
             mapping = json.load(handle)
 
         dir, fn = mapping[element][prop].split("/")
-        res_path = importlib.resources.path(f"{base_cif_module}.{dir}", fn)
+        res_path = importlib.resources.path(f"{base_structure_module}.{dir}", fn)
 
+    # For magnetic elements, use the conventional cell
     if element in MAGNETIC_ELEMENTS:
         primitive_cell = False
     else:
         primitive_cell = True
 
+    if prop == "delta":
+        primitive_cell = False
+    else:
+        # bands and convergence test.
+        # Since we want the convergence test run fast, use primitive cell.
+        primitive_cell = True
+
     with res_path as path:
-        structure = orm.CifData.get_or_create(str(path), use_first=True)[
-            0
-        ].get_structure(primitive_cell=primitive_cell)
+        if Path(path).suffix == ".cif":
+            structure = orm.CifData.get_or_create(str(path), use_first=True)[
+                0
+            ].get_structure(primitive_cell=primitive_cell)
+        elif Path(path).suffix == ".xsf":
+            ase_structure = io.read(str(path))
+            structure = orm.StructureData(ase=ase_structure)
+            # No functionality for primitive cell in ase
+        else:
+            raise ValueError(f"Unknown file type {Path(path).suffix}")
+
+    # To make the structure consistent with the structure from acwf
+    res = get_kpoints_path(structure, method="seekpath")
+    structure = res["primitive_structure"]
 
     return structure
 
 
 def parse_upf(upf_content: str) -> dict:
     """
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/__init__.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,19 +34,23 @@
         if self.inputs.clean_workchain.value is False:
             self.report(f"{type(self)}: remote folders will not be cleaned")
             return
 
         cleaned_calcs = operate_calcjobs(
             self.node, operator=clean_workdir, all_same_nodes=False
         )
-        cache_invalid_calcs = operate_calcjobs(
-            self.node, operator=invalid_cache, all_same_nodes=False
-        )
 
         if cleaned_calcs:
             self.report(
                 f"cleaned remote folders of calculations: {' '.join(map(str, cleaned_calcs))}"
             )
-        if cache_invalid_calcs:
-            self.report(
-                f"Invalid cache of cached calculations: {' '.join(map(str, cache_invalid_calcs))}"
-            )
+
+        # This is not turned on since it will make all finished workflow not cacheable.
+        # I need to find a way to properly work around the parent_folder empty issue.
+        # cache_invalid_calcs = operate_calcjobs(
+        #     self.node, operator=invalid_cache, all_same_nodes=False
+        # )
+
+        # if cache_invalid_calcs:
+        #     self.report(
+        #         f"Invalid cache of cached calculations: {' '.join(map(str, cache_invalid_calcs))}"
+        #     )
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/common.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/common.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/_base.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     update_dict,
 )
 from aiida_sssp_workflow.workflows import SelfCleanWorkChain
 from aiida_sssp_workflow.workflows.common import (
     get_extra_parameters_for_lanthanides,
     get_pseudo_element_and_type,
     get_pseudo_N,
+    get_pseudo_O,
 )
 
 UpfData = DataFactory('pseudo.upf')
 
 
 class abstract_attribute(object):
     """lazy variable check: https://stackoverflow.com/a/32536493"""
@@ -69,14 +70,15 @@
                     help='Pseudopotential to be verified')
         spec.input('protocol', valid_type=orm.Str, required=True,
                     help='The calculation protocol to use for the workchain.')
         spec.input('cutoff_control', valid_type=orm.Str, required=True,
                     help='The cutoff control list to use for the workchain.')
         spec.input('criteria', valid_type=orm.Str, required=True,
                     help='Criteria for convergence measurement to give recommend cutoff pair.')
+        spec.input('configuration', valid_type=orm.Str, required=False)
         spec.input('preset_ecutwfc', valid_type=orm.Int, required=False,
                     help='Preset wavefunction cutoff will be used and skip wavefunction test.')
         spec.input('options', valid_type=orm.Dict, required=False,
                     help='Optional `options`.')
         spec.input('parallelization', valid_type=orm.Dict, required=False,
                     help='Parallelization options')
 
@@ -225,15 +227,24 @@
                 # charge density cutoff.
                 self.ctx.dual_scan_list = cutoff_control['nonnc_dual_scan']
 
         self.ctx.pseudos = {self.ctx.element: self.inputs.pseudo}
 
         # Please check README for what and why we use configuration set 'convergence'
         # for convergence verification.
-        self.ctx.structure = get_standard_structure(self.ctx.element, prop='convergence')
+        if "configuration" in self.inputs:
+            configuration = self.inputs.configuration.value
+        else:
+            # will use the default configuration set in the protocol (mapping.json)
+            configuration = None
+        self.ctx.structure = get_standard_structure(self.ctx.element, prop='convergence', configuration=configuration)
+
+        # For configuration that contains O, which is the configuration from ACWF set, we need to add O pseudo
+        if "O" in self.ctx.structure.get_kind_names():
+            self.ctx.pseudos["O"] = get_pseudo_O()
 
     def is_magnetic_element(self):
         """Check if the element is magnetic"""
         return self.ctx.element in MAGNETIC_ELEMENTS
 
     def extra_setup_for_magnetic_element(self):
         """
@@ -285,15 +296,15 @@
                 'occupations': occupations,
                 'smearing': smearing,
             },
             'ELECTRONS': {
                 'conv_thr': conv_thr,
             },
             'CONTROL': {
-                # 'calculation': 'scf', NOT EXPLICITLY SET. `scf` is default if not override.
+                'calculation': 'scf',
                 'tstress': True,    # for pressue to use _caching node directly.
             },
         }
 
         # update with extra pw params, for magnetic and lanthenides
         if self.ctx.extra_pw_parameters:
             parameters = update_dict(parameters, self.ctx.extra_pw_parameters)
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/bands.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/bands.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
         }
 
         parameters = update_dict(parameters, self.ctx.pw_parameters)
 
         parameters_bands = update_dict(parameters, {})
         parameters_bands["SYSTEM"].pop("nbnd", None)
         parameters_bands["CONTROL"].pop("tstress", None)
+        parameters_bands["CONTROL"]["calculation"] = "bands"
 
         inputs = {
             "structure": self.ctx.structure,
             "scf": {
                 "pw": {
                     "code": self.inputs.code,
                     "pseudos": self.ctx.pseudos,
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/caching.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/caching.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,22 @@
         spec.input(
             "clean_workchain",
             valid_type=orm.Bool,
             default=lambda: orm.Bool(False),
             help="If `True`, work directories of all called calculation will be cleaned at the end of execution.",
         )
 
+    def init_setup(self):
+        super().init_setup()
+        self.ctx.extra_pw_parameters = {
+            "CONTROL": {
+                "disk_io": "nowf",  # no wavefunction file
+            },
+        }
+
     def inspect_wfc_convergence_test(self):
         """Override this step to do nothing to parse wavefunction
         cutoff test results but only run it."""
         return None
 
     def setup_criteria_parameters_from_protocol(self):
         """Override this step to do nothing, since it is not
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/cohesive_energy.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/cohesive_energy.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,40 +44,49 @@
 
     _PROPERTY_NAME = "cohesive_energy"
     _EVALUATE_WORKCHAIN = CohesiveEnergyWorkChain
     _MEASURE_OUT_PROPERTY = "absolute_diff"
 
     def init_setup(self):
         super().init_setup()
-        self.ctx.extra_pw_parameters = {}
-        self.ctx.extra_pw_parameters_for_atom = {}
+        self.ctx.extra_pw_parameters = {
+            "CONTROL": {
+                "disk_io": "nowf",  # no wavefunction file
+            },
+        }
+        self.ctx.extra_pw_parameters_for_atom = {
+            "CONTROL": {
+                "disk_io": "nowf",  # no wavefunction file
+            },
+        }
 
     def extra_setup_for_magnetic_element(self):
         """Extra setup for magnetic element, for atom especially"""
         super().extra_setup_for_magnetic_element()
-        self.ctx.extra_pw_parameters_for_atom = {
+        extra_pw_parameters_for_atom_magnetic_element = {
             self.ctx.element: {
                 "SYSTEM": {
                     "nspin": 2,
                     "starting_magnetization": {
                         self.ctx.element: 0.5,
                     },
                 },
                 "ELECTRONS": {
                     "diagonalization": "cg",
                     "mixing_beta": 0.5,
                     "electron_maxstep": 200,
                 },
             }
         }
+        self.ctx.extra_pw_parameters_for_atom = update_dict(extra_pw_parameters_for_atom_magnetic_element, self.ctx.extra_pw_parameters_for_atom)
 
     def extra_setup_for_rare_earth_element(self):
         """Extra setup for rare earth element, for atom especially"""
         super().extra_setup_for_rare_earth_element()
-        self.ctx.extra_pw_parameters_for_atom = {
+        extra_pw_parameters_for_atom_rare_earth_element = {
             self.ctx.element: {
                 "SYSTEM": {
                     "nspin": 2,
                     "starting_magnetization": {
                         self.ctx.element: 0.5,
                     },
                     # Need high number of bands to make atom calculation of lanthanoids
@@ -87,14 +96,15 @@
                 "ELECTRONS": {
                     "diagonalization": "cg",
                     "mixing_beta": 0.3,  # even small mixing_beta value
                     "electron_maxstep": 200,
                 },
             },
         }
+        self.ctx.extra_pw_parameters_for_atom = update_dict(extra_pw_parameters_for_atom_rare_earth_element, self.ctx.extra_pw_parameters_for_atom)
 
     def setup_code_parameters_from_protocol(self):
         """Input validation"""
         # pylint: disable=invalid-name, attribute-defined-outside-init
 
         # Read from protocol if parameters not set from inputs
         super().setup_code_parameters_from_protocol()
@@ -118,14 +128,17 @@
                 "degauss": self._DEGAUSS,
                 "occupations": self._OCCUPATIONS,
                 "smearing": self._ATOM_SMEARING,
             },
             "ELECTRONS": {
                 "conv_thr": self._CONV_THR,
             },
+            "CONTROL": {
+                "calculation": "scf",
+            },
         }
 
         self.ctx.atom_parameters = {}
         for element in self.ctx.structure.get_symbols_set():
             self.ctx.atom_parameters[element] = base_atom_pw_parameters
 
         self.ctx.atom_parameters = update_dict(
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/delta.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/delta.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # -*- coding: utf-8 -*-
 """
 Convergence test on cohesive energy of a given pseudopotential
 """
+import importlib
+import json
 
 from aiida import orm
 from aiida.engine import calcfunction
 from aiida.plugins import DataFactory
 
-from aiida_sssp_workflow.utils import (
-    ACTINIDE_ELEMENTS,
-    RARE_EARTH_ELEMENTS,
-    update_dict,
-)
+from aiida_sssp_workflow.utils import RARE_EARTH_ELEMENTS, update_dict
 from aiida_sssp_workflow.workflows.convergence._base import _BaseConvergenceWorkChain
 from aiida_sssp_workflow.workflows.evaluate._delta import DeltaWorkChain
 
 UpfData = DataFactory("pseudo.upf")
 
 
 @calcfunction
@@ -46,15 +44,19 @@
 
     _PROPERTY_NAME = "delta"
     _EVALUATE_WORKCHAIN = DeltaWorkChain
     _MEASURE_OUT_PROPERTY = "absolute_diff"
 
     def init_setup(self):
         super().init_setup()
-        self.ctx.extra_pw_parameters = {}
+        self.ctx.extra_pw_parameters = {
+            "CONTROL": {
+                "disk_io": "nowf",  # no wavefunction file
+            },
+        }
 
     def extra_setup_for_rare_earth_element(self):
         super().extra_setup_for_rare_earth_element()
 
     def setup_code_parameters_from_protocol(self):
         """Input validation"""
         # pylint: disable=invalid-name, attribute-defined-outside-init
@@ -69,21 +71,37 @@
         self._SMEARING = protocol["smearing"]
         self._CONV_THR = protocol["electron_conv_thr"]
         self._KDISTANCE = protocol["kpoints_distance"]
 
         self.ctx.scale_count = self._SCALE_COUNT = protocol["scale_count"]
         self.ctx.scale_increment = self._SCALE_INCREMENT = protocol["scale_increment"]
 
-        # configuration for delta convergence
-        if self.ctx.element in RARE_EARTH_ELEMENTS:
-            self.ctx.configuration = "RE"
-        if self.ctx.element in ACTINIDE_ELEMENTS:
-            self.ctx.configuration = "FCC"
-        else:
+        # configuration for delta convergence read from mapping.json of static
+        # Instead of hard code the configuration, the configuration is read from mapping.json
+        import_path = importlib.resources.path(
+            "aiida_sssp_workflow.statics.structures", f"mapping.json"
+        )
+        with import_path as path, open(path, "r") as handle:
+            mapping = json.load(handle)
+
+        dir, fn = mapping[self.ctx.element]["convergence"].split("/")
+
+        if str.upper(dir) == "TYPICAL":
+            self.report(f"Use typical configuration for {self.ctx.element}")
+            element = fn.split(".")[0]
+            assert element == self.ctx.element
             self.ctx.configuration = "TYPICAL"
+        else:
+            # the convergence configuration is read from ACWF set
+            element, configuration = fn.replace("-", ".").split(".")[:-1]
+            self.report(
+                f"Use ACWF configuration {configuration} for {self.ctx.element}"
+            )
+            assert element == self.ctx.element
+            self.ctx.configuration = configuration
 
         # Set context parameters
         self.ctx.kpoints_distance = self._KDISTANCE
         self.ctx.pw_parameters = super()._get_pw_base_parameters(
             self._DEGAUSS, self._OCCUPATIONS, self._SMEARING, self._CONV_THR
         )
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/phonon_frequencies.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/phonon_frequencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     because the frequencies are negative and/or with strong oscillations as
     function of the cutoff for all the considered pseudos).
     We have neglected the first 4 frequencies for H and I, 12 for N and Cl,
     6 for O and ??SiF4 (which replaces F)??.
     """
     import numpy as np
 
-    input_frequencies = input_parameters["dynamical_matrix_0"]["frequencies"]
-    ref_frequencies = ref_parameters["dynamical_matrix_0"]["frequencies"]
+    input_frequencies = input_parameters["dynamical_matrix_1"]["frequencies"]
+    ref_frequencies = ref_parameters["dynamical_matrix_1"]["frequencies"]
 
     # set strat_idx the idx of frequencies start to count
     element = element.value
     if element == 'N' or element == 'Cl':
         start_idx = 12
     elif element == 'H' or element == 'I':
         start_idx = 4
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/pressure.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/convergence/pressure.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,19 @@
     _PROPERTY_NAME = "pressure"
     _EVALUATE_WORKCHAIN = PressureWorkChain
     _MEASURE_OUT_PROPERTY = "relative_diff"
 
     def init_setup(self):
         super().init_setup()
         self.ctx.pw_parameters = {}
+        self.ctx.extra_pw_parameters = {
+            "CONTROL": {
+                "disk_io": "nowf",  # no wavefunction file
+            },
+        }
 
     def setup_code_parameters_from_protocol(self):
         """Input validation"""
         # pylint: disable=invalid-name, attribute-defined-outside-init
 
         # Read from protocol if parameters not set from inputs
         super().setup_code_parameters_from_protocol()
@@ -196,14 +201,15 @@
                 "pseudos": self.ctx.pseudos,
                 "parameters": orm.Dict(dict=parameters),
                 "metadata": {
                     "options": self.ctx.options
                 },
                 "parallelization": orm.Dict(dict=self.ctx.parallelization),
             },
+            "clean_workchain": self.inputs.clean_workchain,
         }
 
         running = self.submit(_EquationOfStateWorkChain, **inputs)
         self.report(f"launching _EquationOfStateWorkChain<{running.pk}>")
 
         self.to_context(extra_reference=running)
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/__init__.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_bands.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/_bands.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_cohesive_energy.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/_cohesive_energy.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_delta.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/_delta.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_eos.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/_eos.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_phonon_frequencies.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/_phonon_frequencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,27 +72,37 @@
             self.ctx.not_ready_for_ph = False
 
             return self.exit_codes.ERROR_SUB_PROCESS_FAILED_SCF
 
         try:
             remote_folder = self.ctx.scf_remote_folder = workchain.outputs.remote_folder
 
-            if not remote_folder.is_empty:
-                # when the remote_folder is not empty we regard it is ready for ph
-                # even if the subsequent ph is successful
-                self.ctx.not_ready_for_ph = False
-            else:
-                # set all same node to caching off and rerun
+            if remote_folder.is_empty:
+                # set all same node to caching off and re-run scf calculation
                 pw_node = [
                     c for c in workchain.called if isinstance(c, orm.CalcJobNode)
                 ][0]
-                all_same_nodes = pw_node.get_all_same_nodes()
+                all_same_nodes = pw_node.base.caching.get_all_same_nodes()
                 for node in all_same_nodes:
                     node.is_valid_cache = False
 
+                # also set valid_cache=False for the source node
+                # It should be included in all_same_nodes, but because of the bug in aiida-core
+                # that the hash is not stable see: https://github.com/aiidateam/aiida-core/issues/5997
+                src_node = orm.load_node(pw_node.base.caching.get_cache_source())
+                src_node.is_valid_cache = False
+                all_same_nodes = src_node.base.caching.get_all_same_nodes()
+                for node in all_same_nodes:
+                    node.is_valid_cache = False
+            else:
+                # when the remote_folder is not empty we regard it is ready for ph
+                # This has a potential problem that even the subsequent ph calculation is
+                # finished, it will be re-run since the remote_folder is changed.
+                self.ctx.not_ready_for_ph = False
+
         except NotExistentAttributeError:
             # set condition to False to break loop
             self.ctx.not_ready_for_ph = False
             return self.exit_codes.ERROR_NO_REMOTE_FOLDER
 
         self.ctx.ecutwfc = workchain.inputs.pw.parameters["SYSTEM"]["ecutwfc"]
         self.ctx.ecutrho = workchain.inputs.pw.parameters["SYSTEM"]["ecutrho"]
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_pressure.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/evaluate/_pressure.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/measure/__init__.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/measure/bands.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/measure/bands.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,17 @@
                 "degauss": self._DEGAUSS,
                 "occupations": self._OCCUPATIONS,
                 "smearing": self._SMEARING,
             },
             "ELECTRONS": {
                 "conv_thr": self._CONV_THR,
             },
+            "CONTROL": {
+                "calculation": "scf",
+            },
         }
 
         self.ctx.ecutwfc = self._ECUTWFC
 
         self.ctx.pw_parameters = update_dict(self.ctx.pw_parameters, parameters)
 
         self.logger.info(
@@ -183,14 +186,15 @@
                 "ecutrho": round(ecutrho),
             },
         }
         parameters = update_dict(parameters, self.ctx.pw_parameters)
 
         parameters_bands = update_dict(parameters, {})
         parameters_bands["SYSTEM"].pop("nbnd", None)
+        parameters_bands["CONTROL"]["calculation"] = "bands"
 
         inputs = {
             "structure": self.ctx.structure,
             "scf": {
                 "pw": {
                     "code": self.inputs.code,
                     "pseudos": pseudos,
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/measure/delta.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/measure/delta.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,35 +207,44 @@
         self._OCCUPATIONS = protocol["occupations"]
         self._SMEARING = protocol["smearing"]
         self._CONV_THR = protocol["electron_conv_thr"]
         self.ctx.kpoints_distance = self._KDISTANCE = protocol["kpoints_distance"]
         self.ctx.scale_count = self._SCALE_COUNT = protocol["scale_count"]
         self.ctx.scale_increment = self._SCALE_INCREMENT = protocol["scale_increment"]
 
+        # Set the hardcoded parameters
+        _disk_io = "nowf"
+
         # narrow the configuration list by protocol
         # this is used for test protocol which only has limited configurations to be verified
         clist = protocol.get("configurations", self.ctx.configuration_list)
         for key in list(self.ctx.structures.keys()):
             if key not in clist:
                 self.ctx.structures.pop(key)
 
         cutoff_control = get_protocol(
             category="control", name=self.inputs.cutoff_control.value
         )
         self._ECUTWFC = cutoff_control["max_wfc"]
 
         parameters = {
+            "CONTROL": {
+                "disk_io": _disk_io,
+            },
             "SYSTEM": {
                 "degauss": self._DEGAUSS,
                 "occupations": self._OCCUPATIONS,
                 "smearing": self._SMEARING,
             },
             "ELECTRONS": {
                 "conv_thr": self._CONV_THR,
             },
+            "CONTROL": {
+                "calculation": "scf",
+            },
         }
 
         self.ctx.ecutwfc = self._ECUTWFC
         self.ctx.ecutrho = self._ECUTWFC * 8
 
         self.ctx.pw_parameters = update_dict(self.ctx.pw_parameters, parameters)
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/verifications.py` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow/workflows/verifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         spec.input('pw_code', valid_type=orm.AbstractCode,
                     help='The `pw.x` code use for the `PwCalculation`.')
         spec.input('ph_code', valid_type=orm.AbstractCode,
                     help='The `ph.x` code use for the `PhCalculation`.')
         spec.input('pseudo', valid_type=UpfData, required=True,
                     help='Pseudopotential to be verified')
         spec.input('label', valid_type=orm.Str, required=False,
-                    help='label store for display as extra attribut.')
+                    help='label store for display as extra attributes.')
         spec.input('properties_list', valid_type=orm.List,
                     default=lambda: orm.List(list=DEFAULT_PROPERTIES_LIST),
                     help='The preperties will be calculated, passed as a list.')
         spec.input('options', valid_type=orm.Dict, required=False,
                     help='Optional `options`')
         spec.input('parallelization', valid_type=orm.Dict, required=False,
                     help='Parallelization options')
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/PKG-INFO` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-sssp-workflow
-Version: 3.0.2
+Version: 3.0.3
 Summary: Package for the AiiDA SSSP workflow
 Home-page: https://github.com/aiidateam/aiida-sssp-workflow
 Author: Jusong Yu
 Author-email: jusong.yu@epfl.ch
 License: MIT
 Project-URL: Bug Tracker, https://github.com/aiidateam/aiida-sssp-workflow/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/entry_points.txt` & `aiida_sssp_workflow-3.0.3/aiida_sssp_workflow.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/pseudo_parser/upf_parser/__init__.py` & `aiida_sssp_workflow-3.0.3/pseudo_parser/upf_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.2/setup.cfg` & `aiida_sssp_workflow-3.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aiida_sssp_workflow
-version = 3.0.2
+version = 3.0.3
 description = Package for the AiiDA SSSP workflow
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/aiidateam/aiida-sssp-workflow
 author = Jusong Yu
 author_email = jusong.yu@epfl.ch
 license = MIT
@@ -20,15 +20,15 @@
 project_urls = 
 	Bug Tracker = https://github.com/aiidateam/aiida-sssp-workflow/issues
 
 [options]
 packages = find:
 install_requires = 
 	aiida-core[atomic_tools]~=2.1
-	aiida-quantumespresso~=4.1
+	aiida-quantumespresso~=4.3.0
 python_requires = >=3.8
 include_package_data = True
 
 [options.packages.find]
 exclude = tests, test*
 
 [options.entry_points]
@@ -64,15 +64,15 @@
 [flake8]
 ignore = 
 	E501  # Line length handled by black.
 	W503  # Line break before binary operator, preferred formatting for black.
 	E203  # Whitespace before ':', preferred formatting for black.
 
 [bumpver]
-current_version = "3.0.2"
+current_version = "3.0.3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
```

### Comparing `aiida_sssp_workflow-3.0.2/tests/test_nightly.py` & `aiida_sssp_workflow-3.0.3/tests/test_nightly.py`

 * *Files identical despite different names*

