# Comparing `tmp/cycode-0.2.3.tar.gz` & `tmp/cycode-0.2.4.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-0.2.3.tar", last modified: Thu Mar 30 14:08:25 2023, max compression
+gzip compressed data, was "cycode-0.2.4.dev8.tar", max compression
```

## Comparing `cycode-0.2.3.tar` & `cycode-0.2.4.dev8.tar`

### file list

```diff
@@ -1,94 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.688124 cycode-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-30 14:07:59.000000 cycode-0.2.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)    32140 2023-03-30 14:08:25.688124 cycode-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31536 2023-03-30 14:07:59.000000 cycode-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-30 14:07:59.000000 cycode-0.2.3/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.684124 cycode-0.2.3/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.684124 cycode-0.2.3/cli/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/auth/auth_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/auth/auth_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/ci_integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    46536 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/code_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/cycode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.684124 cycode-0.2.3/cli/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/exceptions/custom_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.684124 cycode-0.2.3/cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.684124 cycode-0.2.3/cli/helpers/maven/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/helpers/maven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/helpers/maven/base_restore_maven_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/helpers/maven/restore_gradle_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/helpers/maven/restore_maven_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/helpers/sca_code_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.684124 cycode-0.2.3/cli/printers/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/printers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/printers/base_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/printers/json_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/printers/results_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/printers/table_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/printers/text_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.684124 cycode-0.2.3/cli/user_settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/user_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/user_settings/base_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/user_settings/config_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/user_settings/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/user_settings/credentials_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/user_settings/user_settings_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.688124 cycode-0.2.3/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/utils/path_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/utils/scan_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/utils/shell_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/utils/task_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/utils/yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-30 14:07:59.000000 cycode-0.2.3/cli/zip_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.688124 cycode-0.2.3/cyclient/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/config_dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/cycode_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/cycode_client_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/cycode_dev_based_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/cycode_token_based_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/scan_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.688124 cycode-0.2.3/cyclient/scan_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/scan_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/scan_config/scan_config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/scan_config/scan_config_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-30 14:07:59.000000 cycode-0.2.3/cyclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.688124 cycode-0.2.3/cycode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32140 2023-03-30 14:08:25.000000 cycode-0.2.3/cycode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-30 14:08:25.000000 cycode-0.2.3/cycode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 14:08:25.000000 cycode-0.2.3/cycode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 14:08:25.000000 cycode-0.2.3/cycode.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-30 14:08:25.000000 cycode-0.2.3/cycode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-30 14:08:25.000000 cycode-0.2.3/cycode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 14:08:25.000000 cycode-0.2.3/cycode.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 14:08:25.688124 cycode-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-03-30 14:07:59.000000 cycode-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.688124 cycode-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-30 14:07:59.000000 cycode-0.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.688124 cycode-0.2.3/tests/cyclient/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 14:07:59.000000 cycode-0.2.3/tests/cyclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-30 14:07:59.000000 cycode-0.2.3/tests/cyclient/test_scan_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-30 14:07:59.000000 cycode-0.2.3/tests/test_code_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-30 14:07:59.000000 cycode-0.2.3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-30 14:07:59.000000 cycode-0.2.3/tests/test_zip_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.688124 cycode-0.2.3/tests/user_settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 14:07:59.000000 cycode-0.2.3/tests/user_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-03-30 14:07:59.000000 cycode-0.2.3/tests/user_settings/test_configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-03-30 14:07:59.000000 cycode-0.2.3/tests/user_settings/test_user_settings_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:08:25.688124 cycode-0.2.3/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 14:07:59.000000 cycode-0.2.3/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-30 14:07:59.000000 cycode-0.2.3/tests/utils/test_path_utils.py
+-rw-r--r--   0        0        0    31536 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/README.md
+-rw-r--r--   0        0        0      102 2023-05-15 10:12:10.664827 cycode-0.2.4.dev8/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/auth/__init__.py
+-rw-r--r--   0        0        0     3076 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/auth/auth_command.py
+-rw-r--r--   0        0        0     4761 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/auth/auth_manager.py
+-rw-r--r--   0        0        0     1652 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/ci_integrations.py
+-rw-r--r--   0        0        0    47714 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/code_scanner.py
+-rw-r--r--   0        0        0      453 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/config.py
+-rw-r--r--   0        0        0      387 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     4994 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     1698 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/maven/__init__.py
+-rw-r--r--   0        0        0     2191 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0      992 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     2931 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     5835 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/sca_code_scanner.py
+-rw-r--r--   0        0        0     6734 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/main.py
+-rw-r--r--   0        0        0     1106 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/models.py
+-rw-r--r--   0        0        0      195 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0      356 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/base_printer.py
+-rw-r--r--   0        0        0      982 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     1068 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/results_printer.py
+-rw-r--r--   0        0        0     5670 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/table_printer.py
+-rw-r--r--   0        0        0     8749 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      533 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4348 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     6470 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     1908 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0     6853 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/user_settings/user_settings_commands.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0     2054 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0      195 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      910 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     1217 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2700 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      815 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      865 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/zip_file.py
+-rw-r--r--   0        0        0       57 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1708 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     2458 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      119 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      220 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     2706 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      543 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     1596 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     8126 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     6222 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/scan_config/__init__.py
+-rw-r--r--   0        0        0     1090 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/scan_config/scan_config_base.py
+-rw-r--r--   0        0        0     1021 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/scan_config/scan_config_creator.py
+-rw-r--r--   0        0        0      197 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/utils.py
+-rw-r--r--   0        0        0     1893 2023-05-15 10:12:10.660827 cycode-0.2.4.dev8/pyproject.toml
+-rw-r--r--   0        0        0    33354 1970-01-01 00:00:00.000000 cycode-0.2.4.dev8/PKG-INFO
```

### Comparing `cycode-0.2.3/PKG-INFO` & `cycode-0.2.4.dev8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: cycode
-Version: 0.2.3
-Summary: Perform secrets/iac scans for your sources using Cycode's engine
-Home-page: https://github.com/cycodehq-public/cycode-cli
-Author: Cycode
-Author-email: support@cycode.com
-License: MIT
-Keywords: secret-scan cycode devops token secret security cycode code
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 # Cycode CLI User Guide
 
 The Cycode Command Line Interface (CLI) is an application you can install on your local machine which can scan your locally stored repositories for any secrets or infrastructure as code misconfigurations.
 
 This guide will guide you through both installation and usage.
 
 # Table of Contents
@@ -711,8 +694,8 @@
 
 For example, to see options available for a Path Scan, you would simply enter:
 
 `cycode scan path --help`
 
 To see the options available for the ignore scan function, use this command:
 
-`cycode ignore --help`
+`cycode ignore --help`
```

### Comparing `cycode-0.2.3/README.md` & `cycode-0.2.4.dev8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,50 @@
+Metadata-Version: 2.1
+Name: cycode
+Version: 0.2.4.dev8
+Summary: Perform secrets/iac scans for your sources using Cycode's engine
+Home-page: https://github.com/cycodehq-public/cycode-cli
+License: MIT
+Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
+Author: Cycode
+Author-email: support@cycode.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: arrow (>=0.17.0,<0.18.0)
+Requires-Dist: binaryornot (>=0.4.4,<0.5.0)
+Requires-Dist: click (>=8.1.0,<8.2.0)
+Requires-Dist: colorama (>=0.4.3,<0.5.0)
+Requires-Dist: gitpython (>=3.1.30,<3.2.0)
+Requires-Dist: halo (==0.0.31)
+Requires-Dist: marshmallow (>=3.8.0,<3.9.0)
+Requires-Dist: pathspec (>=0.8.0,<0.9.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.24,<3.0)
+Requires-Dist: texttable (>=1.6.7,<1.7.0)
+Requires-Dist: typing (>=3.7.4.3,<3.8.0.0)
+Project-URL: Repository, https://github.com/cycodehq-public/cycode-cli
+Description-Content-Type: text/markdown
+
 # Cycode CLI User Guide
 
 The Cycode Command Line Interface (CLI) is an application you can install on your local machine which can scan your locally stored repositories for any secrets or infrastructure as code misconfigurations.
 
 This guide will guide you through both installation and usage.
 
 # Table of Contents
@@ -694,8 +737,8 @@
 
 For example, to see options available for a Path Scan, you would simply enter:
 
 `cycode scan path --help`
 
 To see the options available for the ignore scan function, use this command:
 
-`cycode ignore --help`
+`cycode ignore --help`
```

### Comparing `cycode-0.2.3/cli/auth/auth_manager.py` & `cycode-0.2.4.dev8/cycode/cli/auth/auth_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import time
 import webbrowser
 from requests import Request
 from typing import Optional
-from cli.exceptions.custom_exceptions import AuthProcessError
-from cli.utils.string_utils import generate_random_string, hash_string_to_sha256
-from cli.user_settings.configuration_manager import ConfigurationManager
-from cli.user_settings.credentials_manager import CredentialsManager
-from cyclient.auth_client import AuthClient
-from cyclient.models import ApiToken, ApiTokenGenerationPollingResponse
-from cyclient import logger
+
+from cycode.cli.exceptions.custom_exceptions import AuthProcessError
+from cycode.cli.utils.string_utils import generate_random_string, hash_string_to_sha256
+from cycode.cli.user_settings.configuration_manager import ConfigurationManager
+from cycode.cli.user_settings.credentials_manager import CredentialsManager
+from cycode.cyclient.auth_client import AuthClient
+from cycode.cyclient.models import ApiToken, ApiTokenGenerationPollingResponse
+from cycode.cyclient import logger
 
 
 class AuthManager:
     CODE_VERIFIER_LENGTH = 101
     POLLING_WAIT_INTERVAL_IN_SECONDS = 3
     POLLING_TIMEOUT_IN_SECONDS = 180
     FAILED_POLLING_STATUS = "Error"
@@ -80,14 +81,15 @@
         app_url = self.configuration_manager.get_cycode_app_url()
         login_url = f'{app_url}/account/sign-in'
         query_params = {
             'source': 'cycode_cli',
             'code_challenge': code_challenge,
             'session_id': session_id
         }
+        # TODO(MarshalX). Use auth_client instead and don't depend on "requests" lib here
         request = Request(url=login_url, params=query_params)
         return request.prepare().url
 
     def _generate_pkce_code_pair(self) -> (str, str):
         code_verifier = generate_random_string(self.CODE_VERIFIER_LENGTH)
         code_challenge = hash_string_to_sha256(code_verifier)
         return code_challenge, code_verifier
```

### Comparing `cycode-0.2.3/cli/ci_integrations.py` & `cycode-0.2.4.dev8/cycode/cli/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.3/cli/code_scanner.py` & `cycode-0.2.4.dev8/cycode/cli/code_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,39 @@
+from typing import Type, NamedTuple
+
 import click
 import json
 import logging
 import os
 import sys
 import time
 import traceback
 from platform import platform
 from uuid import uuid4, UUID
 from git import Repo, NULL_TREE, InvalidGitRepositoryError
 from sys import getsizeof
 
 from halo import Halo
 
-from cli.printers import ResultsPrinter
-from cli.models import Document, DocumentDetections, Severity
-from cli.ci_integrations import get_commit_range
-from cli.consts import *
-from cli.config import configuration_manager, config
-from cli.utils.path_utils import is_sub_path, is_binary_file, get_file_size, get_relevant_files_in_path, \
+from cycode.cli.printers import ResultsPrinter
+from cycode.cli.models import Document, DocumentDetections, Severity
+from cycode.cli.ci_integrations import get_commit_range
+from cycode.cli.consts import *
+from cycode.cli.config import configuration_manager
+from cycode.cli.utils.path_utils import is_sub_path, is_binary_file, get_file_size, get_relevant_files_in_path, \
     get_path_by_os, get_file_content
-from cli.utils.string_utils import get_content_size, is_binary_content
-from cli.utils.task_timer import TimeoutAfter
-from cli.utils import scan_utils
-from cli.user_settings.config_file_manager import ConfigFileManager
-from cli.zip_file import InMemoryZip
-from cli.exceptions.custom_exceptions import *
-from cyclient import logger
-from cyclient.models import *
-from cli.helpers import sca_code_scanner
+from cycode.cli.utils.string_utils import get_content_size, is_binary_content
+from cycode.cli.utils.task_timer import TimeoutAfter
+from cycode.cli.utils import scan_utils
+from cycode.cli.user_settings.config_file_manager import ConfigFileManager
+from cycode.cli.zip_file import InMemoryZip
+from cycode.cli.exceptions.custom_exceptions import *
+from cycode.cli.helpers import sca_code_scanner
+from cycode.cyclient import logger
+from cycode.cyclient.models import *
 
 start_scan_time = time.time()
 
 
 @click.command()
 @click.argument("path", nargs=1, type=click.STRING, required=True)
 @click.option('--branch', '-b',
@@ -813,42 +815,84 @@
 
 def _is_subpath_of_cycode_configuration_folder(filename: str) -> bool:
     return is_sub_path(configuration_manager.global_config_file_manager.get_config_directory_path(), filename) \
            or is_sub_path(configuration_manager.local_config_file_manager.get_config_directory_path(), filename) \
            or filename.endswith(ConfigFileManager.get_config_file_route())
 
 
+class CliScanError(NamedTuple):
+    soft_fail: bool
+    code: str
+    message: str
+
+
+CliScanErrors = Dict[Type[Exception], CliScanError]
+
+
 def _handle_exception(context: click.Context, e: Exception):
-    context.obj["did_fail"] = True
-    verbose = context.obj["verbose"]
-    if verbose:
+    context.obj['did_fail'] = True
+
+    if context.obj['verbose']:
         click.secho(f'Error: {traceback.format_exc()}', fg='red', nl=False)
-    if isinstance(e, (CycodeError, ScanAsyncError)):
-        click.secho('Cycode was unable to complete this scan. Please try again by executing the `cycode scan` command',
-                    fg='red', nl=False)
-        context.obj["soft_fail"] = True
-    elif isinstance(e, HttpUnauthorizedError):
-        click.secho('Unable to authenticate to Cycode, your token is either invalid or has expired. '
-                    'Please re-generate your token and reconfigure it by running the `cycode configure` command',
-                    fg='red', nl=False)
-        context.obj["soft_fail"] = True
-    elif isinstance(e, ZipTooLargeError):
-        click.secho('The path you attempted to scan exceeds the current maximum scanning size cap (10MB). '
-                    'Please try ignoring irrelevant paths using the ‘cycode ignore --by-path’ '
-                    'command and execute the scan again',
-                    fg='red', nl=False)
-        context.obj["soft_fail"] = True
-    elif isinstance(e, InvalidGitRepositoryError):
-        click.secho('The path you supplied does not correlate to a git repository. Should you still wish to scan '
-                    'this path, use: ‘cycode scan path <path>’',
-                    fg='red', nl=False)
-    elif isinstance(e, click.ClickException):
+
+    # TODO(MarshalX): Create global CLI errors database and move this
+    errors: CliScanErrors = {
+        NetworkError: CliScanError(
+            soft_fail=True,
+            code='cycode_error',
+            message='Cycode was unable to complete this scan. '
+                    'Please try again by executing the `cycode scan` command'
+        ),
+        ScanAsyncError: CliScanError(
+            soft_fail=True,
+            code='scan_error',
+            message='Cycode was unable to complete this scan. '
+                    'Please try again by executing the `cycode scan` command'
+        ),
+        HttpUnauthorizedError: CliScanError(
+            soft_fail=True,
+            code='auth_error',
+            message='Unable to authenticate to Cycode, your token is either invalid or has expired. '
+                    'Please re-generate your token and reconfigure it by running the `cycode configure` command'
+        ),
+        ZipTooLargeError: CliScanError(
+            soft_fail=True,
+            code='zip_too_large_error',
+            message='The path you attempted to scan exceeds the current maximum scanning size cap (10MB). '
+                    'Please try ignoring irrelevant paths using the ‘cycode ignore --by-path’ command '
+                    'and execute the scan again'
+        ),
+        InvalidGitRepositoryError: CliScanError(
+            soft_fail=False,
+            code='invalid_git_error',
+            message='The path you supplied does not correlate to a git repository. '
+                    'Should you still wish to scan this path, use: ‘cycode scan path <path>’'
+        ),
+    }
+
+    if type(e) in errors:
+        error = errors[type(e)]
+
+        if error.soft_fail is True:
+            context.obj['soft_fail'] = True
+
+        return _print_error(context, error)
+
+    if isinstance(e, click.ClickException):
         raise e
-    else:
-        raise click.ClickException(str(e))
+
+    raise click.ClickException(str(e))
+
+
+def _print_error(context: click.Context, error: CliScanError) -> None:
+    # TODO(MarshalX): Extend functionality of CLI printers and move this
+    if context.obj['output'] == 'text':
+        click.secho(error.message, fg='red', nl=False)
+    elif context.obj['output'] == 'json':
+        click.echo(json.dumps({'error': error.code, 'message': error.message}, ensure_ascii=False))
 
 
 def _report_scan_status(context: click.Context, scan_type: str, scan_id: str, scan_completed: bool,
                         output_detections_count: int, all_detections_count: int, files_to_scan_count: int,
                         zip_size: int, command_scan_type: str, error_message: Optional[str]):
     try:
         cycode_client = context.obj["client"]
```

### Comparing `cycode-0.2.3/cli/consts.py` & `cycode-0.2.4.dev8/cycode/cli/consts.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.3/cli/cycode.py` & `cycode-0.2.4.dev8/cycode/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 
 import click
 import sys
 
 from typing import List
 
-from cli.models import Severity
-from cli.config import config
-from cli import code_scanner, __version__
-from cyclient import logger
-from cyclient.scan_client import ScanClient
-from cli.user_settings.credentials_manager import CredentialsManager
-from cli.user_settings.configuration_manager import ConfigurationManager
-from cli.user_settings.user_settings_commands import set_credentials, add_exclusions
-from cli.auth.auth_command import authenticate
-from cli.utils import scan_utils
-from cyclient.scan_config.scan_config_creator import create_scan_client
+from cycode import __version__
+from cycode.cli.models import Severity
+from cycode.cli.config import config
+from cycode.cli import code_scanner
+from cycode.cli.user_settings.credentials_manager import CredentialsManager
+from cycode.cli.user_settings.configuration_manager import ConfigurationManager
+from cycode.cli.user_settings.user_settings_commands import set_credentials, add_exclusions
+from cycode.cli.auth.auth_command import authenticate
+from cycode.cli.utils import scan_utils
+from cycode.cyclient import logger
+from cycode.cyclient.scan_config.scan_config_creator import create_scan_client
 
 CONTEXT = dict()
 ISSUE_DETECTED_STATUS_CODE = 1
 NO_ISSUES_STATUS_CODE = 0
 
 
 @click.group(
@@ -56,15 +56,15 @@
               required=False)
 @click.option('--soft-fail',
               is_flag=True,
               default=False,
               help='Run scan without failing, always return a non-error status code',
               type=bool,
               required=False)
-@click.option('--output', default='text',
+@click.option('--output', default=None,
               help="""
               \b
               Specify the results output (text/json), 
               the default is text
               """,
               type=click.Choice(['text', 'json']))
 @click.option('--severity-threshold',
@@ -100,15 +100,17 @@
 
     if soft_fail:
         context.obj["soft_fail"] = soft_fail
     else:
         context.obj["soft_fail"] = config["soft_fail"]
 
     context.obj["scan_type"] = scan_type
-    context.obj["output"] = output
+    if output is not None:
+        # save backward compatability with old style command
+        context.obj["output"] = output
     context.obj["client"] = get_cycode_client(client_id, secret)
     context.obj["severity_threshold"] = severity_threshold
     context.obj["monitor"] = monitor
     context.obj["report"] = report
     _sca_scan_to_context(context, sca_scan)
 
     return 1
@@ -131,24 +133,33 @@
         "auth": authenticate
     },
     context_settings=CONTEXT
 )
 @click.option(
     "--verbose", "-v", is_flag=True, default=False, help="Show detailed logs",
 )
+@click.option(
+    '--output',
+    default='text',
+    help='Specify the output (text/json), the default is text',
+    type=click.Choice(['text', 'json'])
+)
 @click.version_option(__version__, prog_name="cycode")
 @click.pass_context
-def main_cli(context: click.Context, verbose: bool):
+def main_cli(context: click.Context, verbose: bool, output: str):
     context.ensure_object(dict)
     configuration_manager = ConfigurationManager()
+
     verbose = verbose or configuration_manager.get_verbose_flag()
-    context.obj["verbose"] = verbose
+    context.obj['verbose'] = verbose
     log_level = logging.DEBUG if verbose else logging.INFO
     logger.setLevel(log_level)
 
+    context.obj['output'] = output
+
 
 def get_cycode_client(client_id, client_secret):
     if not client_id or not client_secret:
         client_id, client_secret = _get_configured_credentials()
         if not client_id:
             raise click.ClickException("Cycode client id needed.")
         if not client_secret:
```

### Comparing `cycode-0.2.3/cli/exceptions/custom_exceptions.py` & `cycode-0.2.4.dev8/cycode/cli/exceptions/custom_exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,55 @@
+from requests import Response
+
+
 class CycodeError(Exception):
-    def __init__(self, status_code: int, error_message: str):
+    """Base class for all custom exceptions"""
+
+
+class NetworkError(CycodeError):
+    def __init__(self, status_code: int, error_message: str, response: Response):
         self.status_code = status_code
         self.error_message = error_message
+        self.response = response
         super().__init__(self.error_message)
 
     def __str__(self):
         return f'error occurred during the request. status code: {self.status_code}, error message: ' \
                f'{self.error_message}'
 
 
-class ScanAsyncError(Exception):
+class ScanAsyncError(CycodeError):
     def __init__(self, error_message: str):
         self.error_message = error_message
         super().__init__(self.error_message)
 
     def __str__(self):
         return f'error occurred during the scan. error message: {self.error_message}'
 
 
-class HttpUnauthorizedError(Exception):
-    def __init__(self, error_message: str):
+class HttpUnauthorizedError(CycodeError):
+    def __init__(self, error_message: str, response: Response):
         self.status_code = 401
         self.error_message = error_message
+        self.response = response
         super().__init__(self.error_message)
 
     def __str__(self):
         return 'Http Unauthorized Error'
 
 
-class ZipTooLargeError(Exception):
+class ZipTooLargeError(CycodeError):
     def __init__(self, size_limit: int):
         self.size_limit = size_limit
         super().__init__()
 
     def __str__(self):
         return f'The size of zip to scan is too large, size limit: {self.size_limit}'
 
 
-class AuthProcessError(Exception):
+class AuthProcessError(CycodeError):
     def __init__(self, error_message: str):
         self.error_message = error_message
         super().__init__()
 
     def __str__(self):
         return f'Something went wrong during the authentication process, error message: {self.error_message}'
```

### Comparing `cycode-0.2.3/cli/helpers/maven/base_restore_maven_dependencies.py` & `cycode-0.2.4.dev8/cycode/cli/helpers/maven/restore_maven_dependencies.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from abc import ABC, abstractmethod
-from typing import List, Optional, Dict
+from os import path
+from typing import List, Optional
 
 import click
 
-from cli.models import Document
-from cli.utils.path_utils import join_paths, get_file_dir
-from cli.utils.shell_executor import shell
-from cyclient import logger
+from cycode.cli.helpers.maven.base_restore_maven_dependencies import BaseRestoreMavenDependencies, build_dep_tree_path, \
+    execute_command
+from cycode.cli.models import Document
+from cycode.cli.utils.path_utils import get_file_dir, get_file_content, join_paths
 
+BUILD_MAVEN_FILE_NAME = 'pom.xml'
+MAVEN_CYCLONE_DEP_TREE_FILE_NAME = 'bom.json'
+MAVEN_DEP_TREE_FILE_NAME = 'bcde.mvndeps'
 
-def build_dep_tree_path(path: str, generated_file_name: str) -> str:
-    return join_paths(get_file_dir(path), generated_file_name)
-
-
-def execute_command(command: List, file_name: str, command_timeout: int) -> Optional[Dict]:
-    try:
-        dependencies = shell(command, command_timeout)
-    except Exception as e:
-        logger.debug('Failed to restore dependencies shell comment. %s',
-                     {'filename': file_name, 'exception': str(e)})
-        return None
-
-    return dependencies
-
-
-class BaseRestoreMavenDependencies(ABC):
 
+class RestoreMavenDependencies(BaseRestoreMavenDependencies):
     def __init__(self, context: click.Context, is_git_diff: bool,
                  command_timeout: int):
-        self.context = context
-        self.is_git_diff = is_git_diff
-        self.command_timeout = command_timeout
+        super().__init__(context, is_git_diff, command_timeout)
 
-    def restore(self, document: Document) -> Optional[Document]:
-        restore_dependencies_document = self.try_restore_dependencies(document)
-        return restore_dependencies_document
-
-    def get_manifest_file_path(self, document: Document) -> str:
-        return join_paths(self.context.params.get('path'), document.path) if self.context.obj.get(
-            'monitor') else document.path
-
-    @abstractmethod
     def is_project(self, document: Document) -> bool:
-        pass
+        return path.basename(document.path).split('/')[-1] == BUILD_MAVEN_FILE_NAME
 
-    @abstractmethod
     def get_command(self, manifest_file_path: str) -> List[str]:
-        pass
+        return ['mvn', 'org.cyclonedx:cyclonedx-maven-plugin:2.7.4:makeAggregateBom', '-f', manifest_file_path]
 
-    @abstractmethod
     def get_lock_file_name(self) -> str:
-        pass
+        return join_paths('target', MAVEN_CYCLONE_DEP_TREE_FILE_NAME)
 
     def try_restore_dependencies(self, document: Document) -> Optional[Document]:
+        restore_dependencies_document = super().try_restore_dependencies(document)
         manifest_file_path = self.get_manifest_file_path(document)
-        document = Document(build_dep_tree_path(document.path, self.get_lock_file_name()),
-                            execute_command(self.get_command(manifest_file_path), manifest_file_path,
-                                            self.command_timeout),
-                            self.is_git_diff)
-        return document
+        if document.content is None:
+            restore_dependencies_document = self.restore_from_secondary_command(document, manifest_file_path,
+                                                                                restore_dependencies_document)
+        else:
+            restore_dependencies_document.content = get_file_content(
+                join_paths(get_file_dir(manifest_file_path), self.get_lock_file_name()))
+
+        return restore_dependencies_document
+
+    def restore_from_secondary_command(self, document, manifest_file_path, restore_dependencies_document):
+        secondary_restore_command = create_secondary_restore_command(manifest_file_path)
+        backup_restore_content = execute_command(
+            secondary_restore_command,
+            manifest_file_path,
+            self.command_timeout)
+        restore_dependencies_document = Document(build_dep_tree_path(document.path, MAVEN_DEP_TREE_FILE_NAME),
+                                                 backup_restore_content,
+                                                 self.is_git_diff)
+        restore_dependencies = None
+        if restore_dependencies_document.content is not None:
+            restore_dependencies = restore_dependencies_document
+            restore_dependencies.content = get_file_content(MAVEN_DEP_TREE_FILE_NAME)
+
+        return restore_dependencies
+
+
+def create_secondary_restore_command(self, manifest_file_path):
+    return ['mvn', 'dependency:tree', '-B', '-DoutputType=text', '-f', manifest_file_path,
+            f'-DoutputFile={MAVEN_DEP_TREE_FILE_NAME}']
```

### Comparing `cycode-0.2.3/cli/helpers/maven/restore_gradle_dependencies.py` & `cycode-0.2.4.dev8/cycode/cli/helpers/maven/restore_gradle_dependencies.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 import click
 
-from cli.helpers.maven.base_restore_maven_dependencies import BaseRestoreMavenDependencies
-from cli.models import Document
+from cycode.cli.helpers.maven.base_restore_maven_dependencies import BaseRestoreMavenDependencies
+from cycode.cli.models import Document
 
 BUILD_GRADLE_FILE_NAME = 'build.gradle'
 BUILD_GRADLE_KTS_FILE_NAME = 'build.gradle.kts'
 BUILD_GRADLE_DEP_TREE_FILE_NAME = 'gradle-dependencies-generated.txt'
 
 
 class RestoreGradleDependencies(BaseRestoreMavenDependencies):
```

### Comparing `cycode-0.2.3/cli/helpers/sca_code_scanner.py` & `cycode-0.2.4.dev8/cycode/cli/helpers/sca_code_scanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 from typing import List, Optional, Dict
 
 import click
 from git import Repo, GitCommandError
 
-from cli.consts import *
-from cli.helpers.maven.restore_gradle_dependencies import RestoreGradleDependencies
-from cli.helpers.maven.restore_maven_dependencies import RestoreMavenDependencies
-from cli.models import Document
-from cli.utils.path_utils import get_file_dir, join_paths, get_file_content
-from cyclient import logger
+from cycode.cli.consts import *
+from cycode.cli.helpers.maven.restore_gradle_dependencies import RestoreGradleDependencies
+from cycode.cli.helpers.maven.restore_maven_dependencies import RestoreMavenDependencies
+from cycode.cli.models import Document
+from cycode.cli.utils.path_utils import get_file_dir, join_paths, get_file_content
+from cycode.cyclient import logger
 
 BUILD_GRADLE_FILE_NAME = 'build.gradle'
 BUILD_GRADLE_KTS_FILE_NAME = 'build.gradle.kts'
 BUILD_GRADLE_DEP_TREE_FILE_NAME = 'gradle-dependencies-generated.txt'
 BUILD_GRADLE_DEP_TREE_TIMEOUT = 180
```

### Comparing `cycode-0.2.3/cli/models.py` & `cycode-0.2.4.dev8/cycode/cli/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
 from typing import List
-from cyclient.models import Detection
+from cycode.cyclient.models import Detection
 
 
 class Document:
     def __init__(self, path: str, content: str, is_git_diff_format: bool = False, unique_id: str = None):
         self.path = path
         self.content = content
         self.is_git_diff_format = is_git_diff_format
```

### Comparing `cycode-0.2.3/cli/printers/json_printer.py` & `cycode-0.2.4.dev8/cycode/cli/printers/json_printer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from typing import List
 
 import click
 
-from cli.models import DocumentDetections
-from cli.printers.base_printer import BasePrinter
-from cyclient.models import DetectionSchema, Detection
+from cycode.cli.models import DocumentDetections
+from cycode.cli.printers.base_printer import BasePrinter
+from cycode.cyclient.models import DetectionSchema
 
 
 class JsonPrinter(BasePrinter):
 
     scan_id: str
 
     def __init__(self, context: click.Context):
```

### Comparing `cycode-0.2.3/cli/printers/results_printer.py` & `cycode-0.2.4.dev8/cycode/cli/printers/results_printer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import click
 from typing import List
 
-from cli.consts import SCA_SCAN_TYPE
-from cli.printers import JsonPrinter, TextPrinter
-from cli.models import DocumentDetections
-from cli.printers.table_printer import TablePrinter
+from cycode.cli.consts import SCA_SCAN_TYPE
+from cycode.cli.printers import JsonPrinter, TextPrinter
+from cycode.cli.models import DocumentDetections
+from cycode.cli.printers.table_printer import TablePrinter
 
 
 class ResultsPrinter:
     printers = {
         'text': TextPrinter,
         'json': JsonPrinter,
         'text_sca': TablePrinter
```

### Comparing `cycode-0.2.3/cli/printers/table_printer.py` & `cycode-0.2.4.dev8/cycode/cli/printers/table_printer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List, Dict
 
 import click
 from texttable import Texttable
 
-from cli.consts import LICENSE_COMPLIANCE_POLICY_ID, \
+from cycode.cli.consts import LICENSE_COMPLIANCE_POLICY_ID, \
     PACKAGE_VULNERABILITY_POLICY_ID
-from cli.models import DocumentDetections, Detection
-from cli.printers.base_printer import BasePrinter
+from cycode.cli.models import DocumentDetections, Detection
+from cycode.cli.printers.base_printer import BasePrinter
 
 SEVERITY_COLUMN = 'Severity'
 LICENSE_COLUMN = 'License'
 UPGRADE_COLUMN = 'Upgrade'
 REPOSITORY_COLUMN = 'Repository'
 PREVIEW_DETECTIONS_COMMON_HEADERS = ['File Path', 'Ecosystem', 'Dependency Name',
                                      'Direct Dependency',
```

### Comparing `cycode-0.2.3/cli/printers/text_printer.py` & `cycode-0.2.4.dev8/cycode/cli/printers/text_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-import click
 import math
 from typing import List, Optional
-from cli.printers.base_printer import BasePrinter
-from cli.models import DocumentDetections, Detection, Document
-from cli.config import config
-from cli.consts import SECRET_SCAN_TYPE, COMMIT_RANGE_BASED_COMMAND_SCAN_TYPES
-from cli.utils.string_utils import obfuscate_text
+
+import click
+
+from cycode.cli.printers.base_printer import BasePrinter
+from cycode.cli.models import DocumentDetections, Detection, Document
+from cycode.cli.config import config
+from cycode.cli.consts import SECRET_SCAN_TYPE, COMMIT_RANGE_BASED_COMMAND_SCAN_TYPES
+from cycode.cli.utils.string_utils import obfuscate_text
 
 
 class TextPrinter(BasePrinter):
     RED_COLOR_NAME = 'red'
     WHITE_COLOR_NAME = 'white'
     GREEN_COLOR_NAME = 'green'
```

### Comparing `cycode-0.2.3/cli/user_settings/base_file_manager.py` & `cycode-0.2.4.dev8/cycode/cli/user_settings/base_file_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from abc import ABC, abstractmethod
-from cli.utils.yaml_utils import update_file, read_file
+from cycode.cli.utils.yaml_utils import update_file, read_file
 
 
 class BaseFileManager(ABC):
 
     @abstractmethod
     def get_filename(self):
         pass
```

### Comparing `cycode-0.2.3/cli/user_settings/config_file_manager.py` & `cycode-0.2.4.dev8/cycode/cli/user_settings/config_file_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from typing import Optional, List, Dict
-from cli.user_settings.base_file_manager import BaseFileManager
-from cli.consts import CYCODE_CONFIGURATION_DIRECTORY
+
+from cycode.cli.user_settings.base_file_manager import BaseFileManager
+from cycode.cli.consts import CYCODE_CONFIGURATION_DIRECTORY
 
 
 class ConfigFileManager(BaseFileManager):
     CYCODE_HIDDEN_DIRECTORY: str = CYCODE_CONFIGURATION_DIRECTORY
     FILE_NAME: str = 'config.yaml'
 
     ENVIRONMENT_SECTION_NAME: str = 'environment'
```

### Comparing `cycode-0.2.3/cli/user_settings/configuration_manager.py` & `cycode-0.2.4.dev8/cycode/cli/user_settings/configuration_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from pathlib import Path
 from typing import Optional, Dict
-from cli.user_settings.config_file_manager import ConfigFileManager
-from cli.consts import *
+
+from cycode.cli.user_settings.config_file_manager import ConfigFileManager
+from cycode.cli.consts import *
 
 
 class ConfigurationManager:
     global_config_file_manager: ConfigFileManager
     local_config_file_manager: ConfigFileManager
 
     def __init__(self):
```

### Comparing `cycode-0.2.3/cli/user_settings/credentials_manager.py` & `cycode-0.2.4.dev8/cycode/cli/user_settings/credentials_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from pathlib import Path
-from cli.utils.yaml_utils import read_file
-from cli.config import CYCODE_CLIENT_ID_ENV_VAR_NAME, CYCODE_CLIENT_SECRET_ENV_VAR_NAME
-from cli.user_settings.base_file_manager import BaseFileManager
+
+from cycode.cli.utils.yaml_utils import read_file
+from cycode.cli.config import CYCODE_CLIENT_ID_ENV_VAR_NAME, CYCODE_CLIENT_SECRET_ENV_VAR_NAME
+from cycode.cli.user_settings.base_file_manager import BaseFileManager
 
 
 class CredentialsManager(BaseFileManager):
 
     HOME_PATH: str = Path.home()
     CYCODE_HIDDEN_DIRECTORY: str = '.cycode'
     FILE_NAME: str = 'credentials.yaml'
```

### Comparing `cycode-0.2.3/cli/user_settings/user_settings_commands.py` & `cycode-0.2.4.dev8/cycode/cli/user_settings/user_settings_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-import os.path
 import re
+import os.path
+from typing import Optional
 
 import click
-from typing import Optional
-from cli.utils.string_utils import obfuscate_text, hash_string_to_sha256
-from cli.utils.path_utils import get_absolute_path
-from cli.user_settings.credentials_manager import CredentialsManager
-from cli.config import configuration_manager, config
-from cli.consts import *
-from cyclient import logger
+
+from cycode.cli.utils.string_utils import obfuscate_text, hash_string_to_sha256
+from cycode.cli.utils.path_utils import get_absolute_path
+from cycode.cli.user_settings.credentials_manager import CredentialsManager
+from cycode.cli.config import configuration_manager, config
+from cycode.cli.consts import *
+from cycode.cyclient import logger
 
 CREDENTIALS_UPDATED_SUCCESSFULLY_MESSAGE = 'Successfully configured CLI credentials!'
 CREDENTIALS_ARE_SET_IN_ENVIRONMENT_VARIABLES_MESSAGE = 'Note that the credentials that already exist in environment' \
                                                        ' variables (CYCODE_CLIENT_ID and CYCODE_CLIENT_SECRET) take' \
                                                        ' precedent over these credentials; either update or remove ' \
                                                        'the environment variables.'
 credentials_manager = CredentialsManager()
```

### Comparing `cycode-0.2.3/cli/utils/path_utils.py` & `cycode-0.2.4.dev8/cycode/cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.3/cli/utils/shell_executor.py` & `cycode-0.2.4.dev8/cycode/cli/utils/shell_executor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Optional
 import subprocess
 import click
-from cyclient import logger
+from cycode.cyclient import logger
 
 TIMEOUT = 60
 
 
 def shell(command: List[str], timeout: int = TIMEOUT) -> Optional[str]:
     logger.debug(f"executing shell command: {' '.join(map(str, command))}")
     try:
```

### Comparing `cycode-0.2.3/cli/utils/string_utils.py` & `cycode-0.2.4.dev8/cycode/cli/utils/string_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import math
 import re
 import random
 import string
 from sys import getsizeof
 from binaryornot.check import is_binary_string
 
+
 def obfuscate_text(text: str) -> str:
     match_len = len(text)
     start_reveled_len = math.ceil(match_len / 8)
     end_reveled_len = match_len - (math.ceil(match_len / 8))
 
     obfuscated = obfuscate_regex.sub("*", text)
```

### Comparing `cycode-0.2.3/cli/utils/task_timer.py` & `cycode-0.2.4.dev8/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.3/cli/utils/yaml_utils.py` & `cycode-0.2.4.dev8/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.3/cli/zip_file.py` & `cycode-0.2.4.dev8/cycode/cli/zip_file.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.3/cyclient/config.py` & `cycode-0.2.4.dev8/cycode/cyclient/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import os
 import sys
 from urllib.parse import urlparse
 
-from cli.consts import *
-from cli.user_settings.configuration_manager import ConfigurationManager
+from cycode.cli.consts import *
+from cycode.cli.user_settings.configuration_manager import ConfigurationManager
 # set io encoding (for windows)
-from cyclient.config_dev import DEV_MODE_ENV_VAR_NAME, DEV_TENANT_ID_ENV_VAR_NAME
+from .config_dev import DEV_MODE_ENV_VAR_NAME, DEV_TENANT_ID_ENV_VAR_NAME
 
 sys.stdout.reconfigure(encoding='utf-8')
 sys.stderr.reconfigure(encoding='utf-8')
 
 # logs
 logging.basicConfig(
     stream=sys.stdout,
```

### Comparing `cycode-0.2.3/cyclient/cycode_dev_based_client.py` & `cycode-0.2.4.dev8/cycode/cyclient/cycode_dev_based_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from cyclient.config import dev_tenant_id
-from cyclient.cycode_client_base import CycodeClientBase
+from .config import dev_tenant_id
+from .cycode_client_base import CycodeClientBase
 
 """
 Send requests with api token
 """
 
 
 class CycodeDevBasedClient(CycodeClientBase):
```

### Comparing `cycode-0.2.3/cyclient/cycode_token_based_client.py` & `cycode-0.2.4.dev8/cycode/cyclient/cycode_token_based_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import arrow
-import requests
 from threading import Lock
-from cyclient.cycode_client import CycodeClient
 
-"""
-Send requests with api token
-"""
+import arrow
+
+from .cycode_client import CycodeClient
+
+
 class CycodeTokenBasedClient(CycodeClient):
+    """Send requests with api token"""
 
     def __init__(self, client_id: str, client_secret: str):
         super().__init__()
         self.client_secret = client_secret
         self.client_id = client_id
 
         self._api_token = None
@@ -25,27 +25,27 @@
             return self._api_token
 
     def refresh_api_token_if_needed(self) -> None:
         if self._api_token is None or self._expires_in is None or arrow.utcnow() >= self._expires_in:
             self.refresh_api_token()
 
     def refresh_api_token(self) -> None:
-        auth_response = requests.post(f"{self.api_url}/api/v1/auth/api-token",
-                                      json={
-                                          'clientId': self.client_id,
-                                          'secret': self.client_secret
-                                      })
-        auth_response.raise_for_status()
-
+        auth_response = self.post(
+            url_path=f'api/v1/auth/api-token',
+            body={'clientId': self.client_id, 'secret': self.client_secret}
+        )
         auth_response_data = auth_response.json()
+
         self._api_token = auth_response_data['token']
-        self._expires_in = arrow.utcnow().shift(
-            seconds=auth_response_data['expires_in'] * 0.8)
+        self._expires_in = arrow.utcnow().shift(seconds=auth_response_data['expires_in'] * 0.8)
 
-    def get_request_headers(self, additional_headers: dict = None):
+    def get_request_headers(self, additional_headers: dict = None) -> dict:
         headers = super().get_request_headers(additional_headers=additional_headers)
-        headers = self._add_auth_header(headers)
+
+        if not self.lock.locked():
+            headers = self._add_auth_header(headers)
+
         return headers
 
-    def _add_auth_header(self, headers: dict):
+    def _add_auth_header(self, headers: dict) -> dict:
         headers['Authorization'] = f'Bearer {self.api_token}'
         return headers
```

### Comparing `cycode-0.2.3/cyclient/models.py` & `cycode-0.2.4.dev8/cycode/cyclient/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from typing import List, Dict, Optional
 from marshmallow import Schema, fields, EXCLUDE, post_load
 
 
 class Detection(Schema):
-    def __init__(self, detection_type_id: str, type: str, message: str, detection_details: dict, detection_rule_id: str):
+    def __init__(self, detection_type_id: str, type: str, message: str, detection_details: dict,
+                 detection_rule_id: str, severity: Optional[str] = None):
         super().__init__()
         self.message = message
         self.type = type
+        self.severity = severity
         self.detection_type_id = detection_type_id
         self.detection_details = detection_details
         self.detection_rule_id = detection_rule_id
 
     def __repr__(self) -> str:
-        return (
-            "type:{0}, "
-            "message:{1}, "
-            "detection_details: {2}"
-            "detection_rule_id:{3}".format(self.type, self.message, repr(self.detection_details),
-                                           self.detection_rule_id)
-        )
+        return f'type:{self.type}, ' \
+               f'severity:{self.severity}, ' \
+               f'message:{self.message}, ' \
+               f'detection_details:{repr(self.detection_details)}, ' \
+               f'detection_rule_id:{self.detection_rule_id}'
 
 
 class DetectionSchema(Schema):
     class Meta:
         unknown = EXCLUDE
 
     message = fields.String()
     type = fields.String()
+    severity = fields.String(missing='High')
+    # TODO(MarshalX): Remove "missing" arg when IaC and Secrets scans will have classifications
     detection_type_id = fields.String()
     detection_details = fields.Dict()
     detection_rule_id = fields.String()
 
     @post_load
     def build_dto(self, data, **kwargs):
         return Detection(**data)
```

### Comparing `cycode-0.2.3/cyclient/scan_config/scan_config_base.py` & `cycode-0.2.4.dev8/cycode/cyclient/scan_config/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.3/cyclient/scan_config/scan_config_creator.py` & `cycode-0.2.4.dev8/cycode/cyclient/scan_config/scan_config_creator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from cyclient.config import dev_mode
-from cyclient.config_dev import DEV_CYCODE_API_URL
-from cyclient.cycode_dev_based_client import CycodeDevBasedClient
-from cyclient.cycode_token_based_client import CycodeTokenBasedClient
-from cyclient.scan_client import ScanClient
-from cyclient.scan_config.scan_config_base import DefaultScanConfig, DevScanConfig
+from ..config import dev_mode
+from ..config_dev import DEV_CYCODE_API_URL
+from ..cycode_dev_based_client import CycodeDevBasedClient
+from ..cycode_token_based_client import CycodeTokenBasedClient
+from ..scan_client import ScanClient
+from ..scan_config.scan_config_base import DefaultScanConfig, DevScanConfig
 
 
 def create_scan_client(client_id, client_secret):
     if dev_mode:
         scan_cycode_client, scan_config = create_scan_for_dev_env()
     else:
         scan_cycode_client, scan_config = create_scan(client_id, client_secret)
```

