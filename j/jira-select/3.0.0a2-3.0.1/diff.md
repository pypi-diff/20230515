# Comparing `tmp/jira-select-3.0.0a2.tar.gz` & `tmp/jira-select-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira-select-3.0.0a2.tar", last modified: Wed Apr 12 03:59:59 2023, max compression
+gzip compressed data, was "jira-select-3.0.1.tar", last modified: Wed Apr 26 21:06:04 2023, max compression
```

## Comparing `jira-select-3.0.0a2.tar` & `jira-select-3.0.1.tar`

### file list

```diff
@@ -1,81 +1,143 @@
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.305309 jira-select-3.0.0a2/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3984 2023-04-12 03:59:59.305309 jira-select-3.0.0a2/PKG-INFO
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.301308 jira-select-3.0.0a2/jira_select/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       25 2023-04-12 03:59:42.000000 jira-select-3.0.0a2/jira_select/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       98 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/__main__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4180 2023-03-04 07:50:34.000000 jira-select-3.0.0a2/jira_select/cache.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4595 2023-04-10 16:55:25.000000 jira-select-3.0.0a2/jira_select/cmdline.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.301308 jira-select-3.0.0a2/jira_select/commands/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1815 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/build_query.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3473 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/configure.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4371 2023-04-09 01:41:06.000000 jira-select-3.0.0a2/jira_select/commands/functions.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2971 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/install_user_script.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      411 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/remove_instance.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4181 2023-04-10 03:27:31.000000 jira-select-3.0.0a2/jira_select/commands/run.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      899 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/run_script.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4031 2023-04-09 01:41:06.000000 jira-select-3.0.0a2/jira_select/commands/schema.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2706 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/setup_instance.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6891 2023-04-09 01:20:37.000000 jira-select-3.0.0a2/jira_select/commands/shell.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1687 2023-04-09 01:41:06.000000 jira-select-3.0.0a2/jira_select/commands/show_instances.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      759 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/store_password.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      442 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/constants.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      343 2023-03-04 07:50:34.000000 jira-select-3.0.0a2/jira_select/exceptions.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.301308 jira-select-3.0.0a2/jira_select/formatters/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/formatters/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      974 2023-04-09 01:20:37.000000 jira-select-3.0.0a2/jira_select/formatters/csv.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1895 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/formatters/html.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      706 2023-04-09 01:40:24.000000 jira-select-3.0.0a2/jira_select/formatters/json.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      386 2023-04-12 03:52:31.000000 jira-select-3.0.0a2/jira_select/formatters/raw.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1061 2023-01-26 02:12:26.000000 jira-select-3.0.0a2/jira_select/formatters/table.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      176 2023-04-09 01:20:37.000000 jira-select-3.0.0a2/jira_select/formatters/tsv.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.305309 jira-select-3.0.0a2/jira_select/functions/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      944 2023-03-24 16:42:35.000000 jira-select-3.0.0a2/jira_select/functions/estimate_to_days.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1010 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/extract.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1085 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/field_by_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1833 2023-04-09 01:20:37.000000 jira-select-3.0.0a2/jira_select/functions/flatten_changelog.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      261 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/flatten_list.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      427 2023-04-11 05:23:23.000000 jira-select-3.0.0a2/jira_select/functions/get_issue.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3339 2023-04-12 02:18:27.000000 jira-select-3.0.0a2/jira_select/functions/get_issue_snapshot_on_date.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      788 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/get_sprint_by_id.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3371 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/get_sprint_by_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2010 2023-04-11 05:15:10.000000 jira-select-3.0.0a2/jira_select/functions/interval_business_hours.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      859 2023-04-12 01:44:30.000000 jira-select-3.0.0a2/jira_select/functions/interval_matching.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      578 2023-04-10 23:51:45.000000 jira-select-3.0.0a2/jira_select/functions/interval_size.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      366 2023-04-09 01:37:57.000000 jira-select-3.0.0a2/jira_select/functions/json_dumps.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      628 2023-03-04 07:50:34.000000 jira-select-3.0.0a2/jira_select/functions/parse_date.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      776 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/parse_datetime.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      718 2023-04-09 01:20:37.000000 jira-select-3.0.0a2/jira_select/functions/simple_filter.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      592 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/simple_filter_any.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2834 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/sprint_details.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      473 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/sprint_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1574 2023-04-12 03:38:13.000000 jira-select-3.0.0a2/jira_select/functions/subquery.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      355 2023-04-10 04:56:24.000000 jira-select-3.0.0a2/jira_select/functions/union.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3454 2023-04-10 15:58:21.000000 jira-select-3.0.0a2/jira_select/functions/workdays_in_state.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10116 2023-04-12 02:18:19.000000 jira-select-3.0.0a2/jira_select/plugin.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    23021 2023-04-12 03:57:45.000000 jira-select-3.0.0a2/jira_select/query.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.305309 jira-select-3.0.0a2/jira_select/sources/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/sources/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2300 2023-03-04 07:50:34.000000 jira-select-3.0.0a2/jira_select/sources/boards.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3983 2023-04-12 03:22:28.000000 jira-select-3.0.0a2/jira_select/sources/issues.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3576 2023-03-04 07:50:34.000000 jira-select-3.0.0a2/jira_select/sources/sprints.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2254 2023-04-12 02:50:17.000000 jira-select-3.0.0a2/jira_select/types.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10349 2023-04-12 03:32:48.000000 jira-select-3.0.0a2/jira_select/utils.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.301308 jira-select-3.0.0a2/jira_select.egg-info/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3984 2023-04-12 03:59:59.000000 jira-select-3.0.0a2/jira_select.egg-info/PKG-INFO
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2322 2023-04-12 03:59:59.000000 jira-select-3.0.0a2/jira_select.egg-info/SOURCES.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2023-04-12 03:59:59.000000 jira-select-3.0.0a2/jira_select.egg-info/dependency_links.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2594 2023-04-12 03:59:59.000000 jira-select-3.0.0a2/jira_select.egg-info/entry_points.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2022-09-19 22:12:27.000000 jira-select-3.0.0a2/jira_select.egg-info/not-zip-safe
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      393 2023-04-12 03:59:59.000000 jira-select-3.0.0a2/jira_select.egg-info/requires.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       18 2023-04-12 03:59:59.000000 jira-select-3.0.0a2/jira_select.egg-info/top_level.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      775 2023-04-12 03:59:59.309309 jira-select-3.0.0a2/setup.cfg
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5718 2023-04-12 03:59:42.000000 jira-select-3.0.0a2/setup.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.305309 jira-select-3.0.0a2/tests/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/tests/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      892 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/tests/base.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      452 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/tests/conftest.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10342 2023-04-11 05:12:36.000000 jira-select-3.0.0a2/tests/test_functions.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    13320 2023-04-11 05:12:47.000000 jira-select-3.0.0a2/tests/test_query.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6901 2023-04-11 05:12:28.000000 jira-select-3.0.0a2/tests/test_utils.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.661804 jira-select-3.0.1/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      574 2023-04-26 21:05:57.000000 jira-select-3.0.1/.bumpversion.cfg
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1097 2023-03-04 07:50:34.000000 jira-select-3.0.1/.pre-commit-config.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      355 2023-04-26 21:00:29.000000 jira-select-3.0.1/MANIFEST.in
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3982 2023-04-26 21:06:04.661804 jira-select-3.0.1/PKG-INFO
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.645804 jira-select-3.0.1/docs/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      580 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/Makefile
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.641804 jira-select-3.0.1/docs/_build/
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.641804 jira-select-3.0.1/docs/_build/html/
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.649803 jira-select-3.0.1/docs/_build/html/_sources/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      104 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/api_documentation.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      116 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/appendix.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     7463 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/commands.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6018 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/examples.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3550 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/extending.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    16413 2023-03-04 03:10:17.000000 jira-select-3.0.1/docs/_build/html/_sources/functions.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4095 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/how_to.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1741 2023-03-04 06:42:17.000000 jira-select-3.0.1/docs/_build/html/_sources/index.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      829 2023-03-04 07:50:34.000000 jira-select-3.0.1/docs/_build/html/_sources/parameters.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10703 2023-03-04 06:39:28.000000 jira-select-3.0.1/docs/_build/html/_sources/query.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1110 2023-03-05 04:20:36.000000 jira-select-3.0.1/docs/_build/html/_sources/query_lifecycle.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      956 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/quickstart.rst.txt
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.649803 jira-select-3.0.1/docs/_build/html/_sources/source/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1658 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/source/jira_select.commands.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      903 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/source/jira_select.formatters.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1192 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/source/jira_select.functions.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1343 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/source/jira_select.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       88 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/source/modules.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      103 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/source/setup.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      559 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/source/tests.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4099 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/_build/html/_sources/troubleshooting.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      104 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/api_documentation.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       99 2023-04-12 19:20:42.000000 jira-select-3.0.1/docs/appendix.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     7463 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/commands.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5463 2023-04-26 21:05:57.000000 jira-select-3.0.1/docs/conf.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1028 2023-04-13 02:48:26.000000 jira-select-3.0.1/docs/evaluation_location.csv
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6051 2023-04-11 04:23:44.000000 jira-select-3.0.1/docs/examples.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3550 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/extending.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    20590 2023-04-12 04:17:05.000000 jira-select-3.0.1/docs/functions.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4124 2023-04-11 04:23:39.000000 jira-select-3.0.1/docs/how_to.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1758 2023-04-12 19:20:56.000000 jira-select-3.0.1/docs/index.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      787 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/make.bat
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      840 2023-04-11 04:20:52.000000 jira-select-3.0.1/docs/parameters.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    12629 2023-04-11 05:08:47.000000 jira-select-3.0.1/docs/query.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1171 2023-04-11 05:01:21.000000 jira-select-3.0.1/docs/query_lifecycle.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      956 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/quickstart.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       53 2023-03-05 04:28:37.000000 jira-select-3.0.1/docs/requirements.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      131 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/run.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.649803 jira-select-3.0.1/docs/source/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1658 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/source/jira_select.commands.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1240 2023-04-09 01:20:37.000000 jira-select-3.0.1/docs/source/jira_select.formatters.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1192 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/source/jira_select.functions.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1343 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/source/jira_select.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       88 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/source/modules.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      103 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/source/setup.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      559 2022-05-20 02:53:24.000000 jira-select-3.0.1/docs/source/tests.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4136 2023-04-12 04:16:44.000000 jira-select-3.0.1/docs/troubleshooting.rst
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.649803 jira-select-3.0.1/jira_select/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       22 2023-04-26 21:05:57.000000 jira-select-3.0.1/jira_select/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       98 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/__main__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4180 2023-03-04 07:50:34.000000 jira-select-3.0.1/jira_select/cache.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4595 2023-04-10 16:55:25.000000 jira-select-3.0.1/jira_select/cmdline.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.653804 jira-select-3.0.1/jira_select/commands/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/commands/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1815 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/commands/build_query.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3473 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/commands/configure.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4371 2023-04-09 01:41:06.000000 jira-select-3.0.1/jira_select/commands/functions.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2971 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/commands/install_user_script.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      411 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/commands/remove_instance.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4181 2023-04-10 03:27:31.000000 jira-select-3.0.1/jira_select/commands/run.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      899 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/commands/run_script.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4031 2023-04-09 01:41:06.000000 jira-select-3.0.1/jira_select/commands/schema.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2706 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/commands/setup_instance.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6891 2023-04-09 01:20:37.000000 jira-select-3.0.1/jira_select/commands/shell.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1687 2023-04-09 01:41:06.000000 jira-select-3.0.1/jira_select/commands/show_instances.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      759 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/commands/store_password.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      442 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/constants.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      343 2023-03-04 07:50:34.000000 jira-select-3.0.1/jira_select/exceptions.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.653804 jira-select-3.0.1/jira_select/formatters/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/formatters/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      974 2023-04-09 01:20:37.000000 jira-select-3.0.1/jira_select/formatters/csv.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1895 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/formatters/html.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      706 2023-04-09 01:40:24.000000 jira-select-3.0.1/jira_select/formatters/json.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      386 2023-04-12 03:52:31.000000 jira-select-3.0.1/jira_select/formatters/raw.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1061 2023-01-26 02:12:26.000000 jira-select-3.0.1/jira_select/formatters/table.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      176 2023-04-09 01:20:37.000000 jira-select-3.0.1/jira_select/formatters/tsv.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.657804 jira-select-3.0.1/jira_select/functions/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/functions/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      944 2023-03-24 16:42:35.000000 jira-select-3.0.1/jira_select/functions/estimate_to_days.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1010 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/functions/extract.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1085 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/functions/field_by_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1833 2023-04-09 01:20:37.000000 jira-select-3.0.1/jira_select/functions/flatten_changelog.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      261 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/functions/flatten_list.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      427 2023-04-11 05:23:23.000000 jira-select-3.0.1/jira_select/functions/get_issue.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3339 2023-04-12 02:18:27.000000 jira-select-3.0.1/jira_select/functions/get_issue_snapshot_on_date.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      788 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/functions/get_sprint_by_id.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3371 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/functions/get_sprint_by_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2010 2023-04-11 05:15:10.000000 jira-select-3.0.1/jira_select/functions/interval_business_hours.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      859 2023-04-12 01:44:30.000000 jira-select-3.0.1/jira_select/functions/interval_matching.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      578 2023-04-10 23:51:45.000000 jira-select-3.0.1/jira_select/functions/interval_size.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      366 2023-04-09 01:37:57.000000 jira-select-3.0.1/jira_select/functions/json_dumps.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      628 2023-03-04 07:50:34.000000 jira-select-3.0.1/jira_select/functions/parse_date.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      776 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/functions/parse_datetime.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      718 2023-04-09 01:20:37.000000 jira-select-3.0.1/jira_select/functions/simple_filter.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      592 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/functions/simple_filter_any.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2834 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/functions/sprint_details.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      473 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/functions/sprint_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1574 2023-04-12 03:38:13.000000 jira-select-3.0.1/jira_select/functions/subquery.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      355 2023-04-10 04:56:24.000000 jira-select-3.0.1/jira_select/functions/union.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3454 2023-04-10 15:58:21.000000 jira-select-3.0.1/jira_select/functions/workdays_in_state.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10116 2023-04-12 02:18:19.000000 jira-select-3.0.1/jira_select/plugin.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    23290 2023-04-13 02:51:26.000000 jira-select-3.0.1/jira_select/query.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.657804 jira-select-3.0.1/jira_select/sources/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.1/jira_select/sources/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2300 2023-03-04 07:50:34.000000 jira-select-3.0.1/jira_select/sources/boards.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3983 2023-04-12 03:22:28.000000 jira-select-3.0.1/jira_select/sources/issues.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3576 2023-03-04 07:50:34.000000 jira-select-3.0.1/jira_select/sources/sprints.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2254 2023-04-12 02:50:17.000000 jira-select-3.0.1/jira_select/types.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10641 2023-04-13 02:51:25.000000 jira-select-3.0.1/jira_select/utils.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.653804 jira-select-3.0.1/jira_select.egg-info/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3982 2023-04-26 21:06:04.000000 jira-select-3.0.1/jira_select.egg-info/PKG-INFO
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4048 2023-04-26 21:06:04.000000 jira-select-3.0.1/jira_select.egg-info/SOURCES.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2023-04-26 21:06:04.000000 jira-select-3.0.1/jira_select.egg-info/dependency_links.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2594 2023-04-26 21:06:04.000000 jira-select-3.0.1/jira_select.egg-info/entry_points.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2022-09-19 22:12:27.000000 jira-select-3.0.1/jira_select.egg-info/not-zip-safe
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      393 2023-04-26 21:06:04.000000 jira-select-3.0.1/jira_select.egg-info/requires.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       18 2023-04-26 21:06:04.000000 jira-select-3.0.1/jira_select.egg-info/top_level.txt
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.657804 jira-select-3.0.1/pyinstaller/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      829 2022-05-20 02:53:24.000000 jira-select-3.0.1/pyinstaller/Makefile
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2965 2022-05-20 02:53:24.000000 jira-select-3.0.1/pyinstaller/jira_select.exe.spec
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3160 2022-05-20 02:53:24.000000 jira-select-3.0.1/pyinstaller/jira_select.spec
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      163 2022-05-20 02:53:24.000000 jira-select-3.0.1/pyinstaller/requirements.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2843 2023-04-11 04:15:47.000000 jira-select-3.0.1/readme.md
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      393 2023-04-26 21:05:39.000000 jira-select-3.0.1/requirements.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      775 2023-04-26 21:06:04.661804 jira-select-3.0.1/setup.cfg
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5715 2023-04-26 21:05:57.000000 jira-select-3.0.1/setup.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-26 21:06:04.661804 jira-select-3.0.1/tests/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.1/tests/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      892 2022-05-20 02:53:24.000000 jira-select-3.0.1/tests/base.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      452 2022-05-20 02:53:24.000000 jira-select-3.0.1/tests/conftest.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10342 2023-04-11 05:12:36.000000 jira-select-3.0.1/tests/test_functions.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    13320 2023-04-11 05:12:47.000000 jira-select-3.0.1/tests/test_query.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6901 2023-04-11 05:12:28.000000 jira-select-3.0.1/tests/test_utils.py
```

### Comparing `jira-select-3.0.0a2/PKG-INFO` & `jira-select-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-select
-Version: 3.0.0a2
+Version: 3.0.1
 Summary: Easily run complex SQL-like queries far beyond what Jira's standard JQL query language can provide.
 Home-page: https://github.com/coddingtonbear/jira-select
 Author: Adam Coddington
 Author-email: me@adamcoddington.net
 License: MIT
 Project-URL: Issue Tracker, https://github.com/coddingtonbear/jira-select/issues
 Keywords: jira,csv,sql
```

### Comparing `jira-select-3.0.0a2/jira_select/cache.py` & `jira-select-3.0.1/jira_select/cache.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/cmdline.py` & `jira-select-3.0.1/jira_select/cmdline.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/commands/build_query.py` & `jira-select-3.0.1/jira_select/commands/build_query.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/commands/configure.py` & `jira-select-3.0.1/jira_select/commands/configure.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/commands/functions.py` & `jira-select-3.0.1/jira_select/commands/functions.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/commands/install_user_script.py` & `jira-select-3.0.1/jira_select/commands/install_user_script.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/commands/run.py` & `jira-select-3.0.1/jira_select/commands/run.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/commands/run_script.py` & `jira-select-3.0.1/jira_select/commands/run_script.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/commands/schema.py` & `jira-select-3.0.1/jira_select/commands/schema.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/commands/setup_instance.py` & `jira-select-3.0.1/jira_select/commands/setup_instance.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/commands/shell.py` & `jira-select-3.0.1/jira_select/commands/shell.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/commands/show_instances.py` & `jira-select-3.0.1/jira_select/commands/show_instances.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/commands/store_password.py` & `jira-select-3.0.1/jira_select/commands/store_password.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/formatters/csv.py` & `jira-select-3.0.1/jira_select/formatters/csv.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/formatters/html.py` & `jira-select-3.0.1/jira_select/formatters/html.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/formatters/json.py` & `jira-select-3.0.1/jira_select/formatters/json.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/formatters/table.py` & `jira-select-3.0.1/jira_select/formatters/table.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/estimate_to_days.py` & `jira-select-3.0.1/jira_select/functions/estimate_to_days.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/extract.py` & `jira-select-3.0.1/jira_select/functions/extract.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/field_by_name.py` & `jira-select-3.0.1/jira_select/functions/field_by_name.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/flatten_changelog.py` & `jira-select-3.0.1/jira_select/functions/flatten_changelog.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/get_issue_snapshot_on_date.py` & `jira-select-3.0.1/jira_select/functions/get_issue_snapshot_on_date.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/get_sprint_by_id.py` & `jira-select-3.0.1/jira_select/functions/get_sprint_by_id.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/get_sprint_by_name.py` & `jira-select-3.0.1/jira_select/functions/get_sprint_by_name.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/interval_business_hours.py` & `jira-select-3.0.1/jira_select/functions/interval_business_hours.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/interval_matching.py` & `jira-select-3.0.1/jira_select/functions/interval_matching.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/interval_size.py` & `jira-select-3.0.1/jira_select/functions/interval_size.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/parse_date.py` & `jira-select-3.0.1/jira_select/functions/parse_date.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/parse_datetime.py` & `jira-select-3.0.1/jira_select/functions/parse_datetime.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/simple_filter.py` & `jira-select-3.0.1/jira_select/functions/simple_filter.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/simple_filter_any.py` & `jira-select-3.0.1/jira_select/functions/simple_filter_any.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/sprint_details.py` & `jira-select-3.0.1/jira_select/functions/sprint_details.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/subquery.py` & `jira-select-3.0.1/jira_select/functions/subquery.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/functions/workdays_in_state.py` & `jira-select-3.0.1/jira_select/functions/workdays_in_state.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/plugin.py` & `jira-select-3.0.1/jira_select/plugin.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/query.py` & `jira-select-3.0.1/jira_select/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from .types import SchemaRow
 from .types import SelectFieldDefinition
 from .types import WhereParamDict
 from .utils import calculate_result_hash
 from .utils import evaluate_expression
 from .utils import expression_includes_group_by
 from .utils import find_missing_parameters
+from .utils import find_used_parameters
 from .utils import get_cache_path
 from .utils import get_field_data
 from .utils import get_row_dict
 from .utils import normalize_value
 from .utils import parse_select_definition
 from .utils import parse_sort_by_definition
 
@@ -450,15 +451,21 @@
                 __version__,
                 str(self.jira.client_info()),
                 str(self.query.from_),
                 str(self.query.where),
                 str(self.query.order_by),
                 str(self.query.limit),
                 str(self.query.expand),
-                str(self.parameters),
+                str(
+                    {
+                        key: value
+                        for key, value in self.parameters.items()
+                        if key in find_used_parameters("".join(self.query.where))
+                    }
+                ),
             ]
         )
 
         if self.query.cache and self._enable_cache:
             try:
                 min_recency, _ = self.query.cache
                 if min_recency is None:
```

### Comparing `jira-select-3.0.0a2/jira_select/sources/boards.py` & `jira-select-3.0.1/jira_select/sources/boards.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/sources/issues.py` & `jira-select-3.0.1/jira_select/sources/issues.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/sources/sprints.py` & `jira-select-3.0.1/jira_select/sources/sprints.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/types.py` & `jira-select-3.0.1/jira_select/types.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/jira_select/utils.py` & `jira-select-3.0.1/jira_select/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Mapping
 from typing import Optional
+from typing import Set
 from typing import Tuple
 from typing import Union
 
 import simpleeval
 from appdirs import user_config_dir
 from jira.resources import Resource
 from portion import Interval
@@ -337,14 +338,24 @@
     else:
         raise UnhandledConditionError(
             "Could not determine method of launching default "
             f"interpreter for platform {sys.platform}."
         )
 
 
+def find_used_parameters(expression: str) -> List[str]:
+    used_params: Set[str] = set()
+
+    expression_params = PARAM_FINDER.findall(expression)
+    for expression_param in expression_params:
+        used_params.add(expression_param)
+
+    return list(used_params)
+
+
 def find_missing_parameters(expression: str, known_params: List[str]) -> List[str]:
     missing_parameters: List[str] = []
 
     expression_params = PARAM_FINDER.findall(expression)
     for expression_param in expression_params:
         if expression_param not in known_params:
             missing_parameters.append(expression_param)
```

### Comparing `jira-select-3.0.0a2/jira_select.egg-info/PKG-INFO` & `jira-select-3.0.1/jira_select.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-select
-Version: 3.0.0a2
+Version: 3.0.1
 Summary: Easily run complex SQL-like queries far beyond what Jira's standard JQL query language can provide.
 Home-page: https://github.com/coddingtonbear/jira-select
 Author: Adam Coddington
 Author-email: me@adamcoddington.net
 License: MIT
 Project-URL: Issue Tracker, https://github.com/coddingtonbear/jira-select/issues
 Keywords: jira,csv,sql
```

### Comparing `jira-select-3.0.0a2/jira_select.egg-info/SOURCES.txt` & `jira-select-3.0.1/jira_select.egg-info/entry_points.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,53 @@
-setup.cfg
-setup.py
-jira_select/__init__.py
-jira_select/__main__.py
-jira_select/cache.py
-jira_select/cmdline.py
-jira_select/constants.py
-jira_select/exceptions.py
-jira_select/plugin.py
-jira_select/query.py
-jira_select/types.py
-jira_select/utils.py
-jira_select.egg-info/PKG-INFO
-jira_select.egg-info/SOURCES.txt
-jira_select.egg-info/dependency_links.txt
-jira_select.egg-info/entry_points.txt
-jira_select.egg-info/not-zip-safe
-jira_select.egg-info/requires.txt
-jira_select.egg-info/top_level.txt
-jira_select/commands/__init__.py
-jira_select/commands/build_query.py
-jira_select/commands/configure.py
-jira_select/commands/functions.py
-jira_select/commands/install_user_script.py
-jira_select/commands/remove_instance.py
-jira_select/commands/run.py
-jira_select/commands/run_script.py
-jira_select/commands/schema.py
-jira_select/commands/setup_instance.py
-jira_select/commands/shell.py
-jira_select/commands/show_instances.py
-jira_select/commands/store_password.py
-jira_select/formatters/__init__.py
-jira_select/formatters/csv.py
-jira_select/formatters/html.py
-jira_select/formatters/json.py
-jira_select/formatters/raw.py
-jira_select/formatters/table.py
-jira_select/formatters/tsv.py
-jira_select/functions/__init__.py
-jira_select/functions/estimate_to_days.py
-jira_select/functions/extract.py
-jira_select/functions/field_by_name.py
-jira_select/functions/flatten_changelog.py
-jira_select/functions/flatten_list.py
-jira_select/functions/get_issue.py
-jira_select/functions/get_issue_snapshot_on_date.py
-jira_select/functions/get_sprint_by_id.py
-jira_select/functions/get_sprint_by_name.py
-jira_select/functions/interval_business_hours.py
-jira_select/functions/interval_matching.py
-jira_select/functions/interval_size.py
-jira_select/functions/json_dumps.py
-jira_select/functions/parse_date.py
-jira_select/functions/parse_datetime.py
-jira_select/functions/simple_filter.py
-jira_select/functions/simple_filter_any.py
-jira_select/functions/sprint_details.py
-jira_select/functions/sprint_name.py
-jira_select/functions/subquery.py
-jira_select/functions/union.py
-jira_select/functions/workdays_in_state.py
-jira_select/sources/__init__.py
-jira_select/sources/boards.py
-jira_select/sources/issues.py
-jira_select/sources/sprints.py
-tests/__init__.py
-tests/base.py
-tests/conftest.py
-tests/test_functions.py
-tests/test_query.py
-tests/test_utils.py
+[console_scripts]
+jira-select = jira_select.cmdline:main
+
+[jira_select.commands]
+build-query = jira_select.commands.build_query:Command
+configure = jira_select.commands.configure:Command
+functions = jira_select.commands.functions:Command
+install-user-script = jira_select.commands.install_user_script:Command
+remove-instance = jira_select.commands.remove_instance:Command
+run-query = jira_select.commands.run:Command
+run-script = jira_select.commands.run_script:Command
+schema = jira_select.commands.schema:Command
+setup-instance = jira_select.commands.setup_instance:Command
+shell = jira_select.commands.shell:Command
+show-instances = jira_select.commands.show_instances:Command
+store-password = jira_select.commands.store_password:Command
+
+[jira_select.formatters]
+csv = jira_select.formatters.csv:Formatter
+html = jira_select.formatters.html:Formatter
+json = jira_select.formatters.json:Formatter
+raw = jira_select.formatters.raw:Formatter
+table = jira_select.formatters.table:Formatter
+tsv = jira_select.formatters.tsv:Formatter
+
+[jira_select.functions]
+estimate_to_days = jira_select.functions.estimate_to_days:Function
+extract = jira_select.functions.extract:Function
+field_by_name = jira_select.functions.field_by_name:Function
+flatten_changelog = jira_select.functions.flatten_changelog:Function
+flatten_list = jira_select.functions.flatten_list:Function
+get_issue = jira_select.functions.get_issue:Function
+get_issue_snapshot_on_date = jira_select.functions.get_issue_snapshot_on_date:Function
+get_sprint_by_id = jira_select.functions.get_sprint_by_id:Function
+get_sprint_by_name = jira_select.functions.get_sprint_by_name:Function
+interval_business_hours = jira_select.functions.interval_business_hours:Function
+interval_matching = jira_select.functions.interval_matching:Function
+interval_size = jira_select.functions.interval_size:Function
+json_dumps = jira_select.functions.json_dumps:Function
+parse_date = jira_select.functions.parse_date:Function
+parse_datetime = jira_select.functions.parse_datetime:Function
+simple_filter = jira_select.functions.simple_filter:Function
+simple_filter_any = jira_select.functions.simple_filter_any:Function
+sprint_details = jira_select.functions.sprint_details:Function
+sprint_name = jira_select.functions.sprint_name:Function
+subquery = jira_select.functions.subquery:Function
+union = jira_select.functions.union:Function
+workdays_in_state = jira_select.functions.workdays_in_state:Function
+
+[jira_select.sources]
+boards = jira_select.sources.boards:Source
+issues = jira_select.sources.issues:Source
+sprints = jira_select.sources.sprints:Source
```

### Comparing `jira-select-3.0.0a2/setup.cfg` & `jira-select-3.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/setup.py` & `jira-select-3.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="jira-select",
-    version="3.0.0.a2",
+    version="3.0.1",
     license="MIT",
     description=(
         "Easily run complex SQL-like queries far beyond what "
         "Jira's standard JQL query language can provide."
     ),
     long_description_content_type="text/markdown",
     long_description=read("readme.md"),
```

### Comparing `jira-select-3.0.0a2/tests/base.py` & `jira-select-3.0.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/tests/test_functions.py` & `jira-select-3.0.1/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/tests/test_query.py` & `jira-select-3.0.1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a2/tests/test_utils.py` & `jira-select-3.0.1/tests/test_utils.py`

 * *Files identical despite different names*

