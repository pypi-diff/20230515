# Comparing `tmp/miniwdl-1.9.0.tar.gz` & `tmp/miniwdl-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniwdl-1.9.0.tar", last modified: Sat Jan 28 08:19:28 2023, max compression
+gzip compressed data, was "miniwdl-1.9.1.tar", last modified: Sun Feb 26 10:21:14 2023, max compression
```

## Comparing `miniwdl-1.9.0.tar` & `miniwdl-1.9.1.tar`

### file list

```diff
@@ -1,192 +1,193 @@
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.723224 miniwdl-1.9.0/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      220 2022-04-25 00:03:54.000000 miniwdl-1.9.0/.coveragerc
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      100 2021-06-12 09:10:29.000000 miniwdl-1.9.0/.flake8
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.707224 miniwdl-1.9.0/.github/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      724 2021-06-12 09:10:29.000000 miniwdl-1.9.0/.github/pull_request_template.md
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.707224 miniwdl-1.9.0/.github/workflows/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     3463 2022-04-25 03:13:20.000000 miniwdl-1.9.0/.github/workflows/CI.yml
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     3345 2021-06-12 09:10:29.000000 miniwdl-1.9.0/.gitmodules
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       96 2021-06-12 09:10:29.000000 miniwdl-1.9.0/.pyre_configuration
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      294 2021-06-12 09:10:29.000000 miniwdl-1.9.0/.readthedocs.yml
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     3194 2021-06-12 09:10:29.000000 miniwdl-1.9.0/CONTRIBUTING.md
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1539 2022-08-05 10:28:39.000000 miniwdl-1.9.0/Dockerfile
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1084 2021-06-12 09:10:29.000000 miniwdl-1.9.0/LICENSE
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     3048 2023-01-28 05:55:04.000000 miniwdl-1.9.0/Makefile
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      770 2023-01-28 08:19:28.723224 miniwdl-1.9.0/PKG-INFO
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     4194 2023-01-28 08:05:27.000000 miniwdl-1.9.0/README.md
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.711224 miniwdl-1.9.0/WDL/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    73925 2023-01-28 05:55:04.000000 miniwdl-1.9.0/WDL/CLI.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     8192 2021-06-12 09:10:29.000000 miniwdl-1.9.0/WDL/Env.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    11426 2022-04-25 00:03:54.000000 miniwdl-1.9.0/WDL/Error.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    39503 2023-01-28 08:05:27.000000 miniwdl-1.9.0/WDL/Expr.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    48159 2023-01-28 08:05:27.000000 miniwdl-1.9.0/WDL/Lint.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    47540 2023-01-28 08:05:27.000000 miniwdl-1.9.0/WDL/StdLib.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    80105 2023-01-28 06:48:07.000000 miniwdl-1.9.0/WDL/Tree.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    21824 2023-01-28 08:05:27.000000 miniwdl-1.9.0/WDL/Type.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    26029 2023-01-28 05:55:04.000000 miniwdl-1.9.0/WDL/Value.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    11360 2021-11-28 02:55:39.000000 miniwdl-1.9.0/WDL/Walker.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    10824 2023-01-28 08:05:27.000000 miniwdl-1.9.0/WDL/Zip.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    12120 2022-04-25 00:03:54.000000 miniwdl-1.9.0/WDL/__init__.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       85 2021-06-12 09:10:29.000000 miniwdl-1.9.0/WDL/__main__.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    17887 2023-01-28 05:55:04.000000 miniwdl-1.9.0/WDL/_grammar.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    30547 2023-01-28 08:05:27.000000 miniwdl-1.9.0/WDL/_parser.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    30366 2022-08-05 10:28:39.000000 miniwdl-1.9.0/WDL/_util.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)        0 2022-04-25 00:03:54.000000 miniwdl-1.9.0/WDL/py.typed
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.711224 miniwdl-1.9.0/WDL/runtime/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     2700 2021-11-28 01:40:40.000000 miniwdl-1.9.0/WDL/runtime/__init__.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     4304 2022-04-25 00:03:54.000000 miniwdl-1.9.0/WDL/runtime/_statusbar.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.711224 miniwdl-1.9.0/WDL/runtime/backend/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)        0 2021-11-28 01:40:40.000000 miniwdl-1.9.0/WDL/runtime/backend/__init__.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    11428 2023-01-28 08:05:27.000000 miniwdl-1.9.0/WDL/runtime/backend/cli_subprocess.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    31078 2023-01-28 08:05:27.000000 miniwdl-1.9.0/WDL/runtime/backend/docker_swarm.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     5907 2023-01-28 08:05:27.000000 miniwdl-1.9.0/WDL/runtime/backend/podman.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     4751 2022-11-25 05:10:35.000000 miniwdl-1.9.0/WDL/runtime/backend/singularity.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     2416 2022-11-25 05:10:35.000000 miniwdl-1.9.0/WDL/runtime/backend/udocker.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    15632 2022-08-22 03:32:30.000000 miniwdl-1.9.0/WDL/runtime/cache.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    16773 2023-01-28 05:55:04.000000 miniwdl-1.9.0/WDL/runtime/config.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.711224 miniwdl-1.9.0/WDL/runtime/config_templates/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    16059 2023-01-28 08:05:27.000000 miniwdl-1.9.0/WDL/runtime/config_templates/default.cfg
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    15237 2022-08-22 03:32:30.000000 miniwdl-1.9.0/WDL/runtime/download.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     4798 2021-11-28 01:40:40.000000 miniwdl-1.9.0/WDL/runtime/error.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    41635 2023-01-28 05:55:04.000000 miniwdl-1.9.0/WDL/runtime/task.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    23399 2023-01-28 08:05:27.000000 miniwdl-1.9.0/WDL/runtime/task_container.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    46715 2023-01-28 08:05:27.000000 miniwdl-1.9.0/WDL/runtime/workflow.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.715224 miniwdl-1.9.0/docs/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     4866 2022-08-05 10:28:39.000000 miniwdl-1.9.0/docs/FAQ.md
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      604 2021-06-12 09:10:29.000000 miniwdl-1.9.0/docs/Makefile
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1068 2023-01-28 05:55:04.000000 miniwdl-1.9.0/docs/WDL.rst
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     7560 2021-06-12 09:10:29.000000 miniwdl-1.9.0/docs/add_functions.md
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     9558 2022-04-25 00:03:54.000000 miniwdl-1.9.0/docs/assert.md
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     4261 2021-11-28 01:40:40.000000 miniwdl-1.9.0/docs/check.rst
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     4974 2022-04-25 00:03:54.000000 miniwdl-1.9.0/docs/conf.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     8277 2022-11-02 08:51:54.000000 miniwdl-1.9.0/docs/getting_started.md
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      797 2022-08-22 03:32:30.000000 miniwdl-1.9.0/docs/index.rst
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    80175 2021-06-12 09:10:29.000000 miniwdl-1.9.0/docs/miniwdl-logo.png
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     8569 2023-01-28 05:55:04.000000 miniwdl-1.9.0/docs/runner_advanced.md
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     6761 2023-01-28 08:05:27.000000 miniwdl-1.9.0/docs/runner_backends.md
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      173 2021-06-12 09:10:29.000000 miniwdl-1.9.0/docs/runner_cli.rst
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    13637 2022-11-02 08:51:54.000000 miniwdl-1.9.0/docs/runner_reference.md
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     9631 2021-06-12 09:10:29.000000 miniwdl-1.9.0/docs/trace_identifiers.md
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    11049 2023-01-28 08:05:27.000000 miniwdl-1.9.0/docs/wdlviz.md
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     4692 2021-06-12 09:10:29.000000 miniwdl-1.9.0/docs/wdlviz_ex1.png
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    80838 2021-06-12 09:10:29.000000 miniwdl-1.9.0/docs/wdlviz_ex2.png
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      926 2022-08-22 03:32:30.000000 miniwdl-1.9.0/docs/zip.rst
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.715224 miniwdl-1.9.0/examples/
--rwxrwxr-x   0 mlin      (1000) mlin      (1000)     2758 2021-11-28 01:40:40.000000 miniwdl-1.9.0/examples/clean_download_cache.sh
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     2278 2021-11-28 01:40:40.000000 miniwdl-1.9.0/examples/clean_download_cache.t
--rwxrwxr-x   0 mlin      (1000) mlin      (1000)     4608 2021-06-12 09:10:29.000000 miniwdl-1.9.0/examples/paste_wdl_imports.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.715224 miniwdl-1.9.0/examples/plugin_log_task_usage/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     2133 2021-06-12 09:10:29.000000 miniwdl-1.9.0/examples/plugin_log_task_usage/miniwdl_log_task_usage.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      430 2021-06-12 09:10:29.000000 miniwdl-1.9.0/examples/plugin_log_task_usage/setup.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.715224 miniwdl-1.9.0/examples/plugin_s3_progressive_upload/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     8091 2023-01-28 05:55:04.000000 miniwdl-1.9.0/examples/plugin_s3_progressive_upload/miniwdl_s3_progressive_upload.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      643 2023-01-28 05:55:04.000000 miniwdl-1.9.0/examples/plugin_s3_progressive_upload/setup.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     3422 2023-01-28 05:55:04.000000 miniwdl-1.9.0/examples/plugin_s3_progressive_upload/test.t
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.715224 miniwdl-1.9.0/examples/plugin_task_omnibus/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     6894 2021-06-12 09:10:29.000000 miniwdl-1.9.0/examples/plugin_task_omnibus/miniwdl_task_omnibus_example.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      483 2021-06-12 09:10:29.000000 miniwdl-1.9.0/examples/plugin_task_omnibus/setup.py
--rwxrwxr-x   0 mlin      (1000) mlin      (1000)     2582 2021-06-12 09:10:29.000000 miniwdl-1.9.0/examples/run_with_custom_error.py
--rwxrwxr-x   0 mlin      (1000) mlin      (1000)     2797 2023-01-28 05:55:04.000000 miniwdl-1.9.0/examples/upload_output_files.sh
--rwxrwxr-x   0 mlin      (1000) mlin      (1000)     6525 2022-04-25 00:03:54.000000 miniwdl-1.9.0/examples/wdlviz.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.715224 miniwdl-1.9.0/miniwdl.egg-info/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      770 2023-01-28 08:19:27.000000 miniwdl-1.9.0/miniwdl.egg-info/PKG-INFO
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     4584 2023-01-28 08:19:28.000000 miniwdl-1.9.0/miniwdl.egg-info/SOURCES.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)        1 2023-01-28 08:19:27.000000 miniwdl-1.9.0/miniwdl.egg-info/dependency_links.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       41 2023-01-28 08:19:28.000000 miniwdl-1.9.0/miniwdl.egg-info/entry_points.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)        1 2021-06-27 08:22:31.000000 miniwdl-1.9.0/miniwdl.egg-info/not-zip-safe
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       46 2023-01-28 08:19:27.000000 miniwdl-1.9.0/miniwdl.egg-info/pbr.json
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      214 2023-01-28 08:19:28.000000 miniwdl-1.9.0/miniwdl.egg-info/requires.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)        4 2023-01-28 08:19:28.000000 miniwdl-1.9.0/miniwdl.egg-info/top_level.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      375 2022-08-22 03:32:30.000000 miniwdl-1.9.0/requirements.dev.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      355 2023-01-28 08:05:27.000000 miniwdl-1.9.0/requirements.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      807 2023-01-28 08:19:28.723224 miniwdl-1.9.0/setup.cfg
--rwxrwxr-x   0 mlin      (1000) mlin      (1000)      134 2021-06-12 09:10:29.000000 miniwdl-1.9.0/setup.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.715224 miniwdl-1.9.0/stubs/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      203 2021-06-12 09:10:29.000000 miniwdl-1.9.0/stubs/README.md
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.715224 miniwdl-1.9.0/stubs/argcomplete/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      134 2021-06-12 09:10:29.000000 miniwdl-1.9.0/stubs/argcomplete/__init__.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.719224 miniwdl-1.9.0/stubs/bullet/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)        0 2021-06-12 09:10:29.000000 miniwdl-1.9.0/stubs/bullet/__init__.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.719224 miniwdl-1.9.0/stubs/coloredlogs/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      325 2021-06-12 09:10:29.000000 miniwdl-1.9.0/stubs/coloredlogs/__init__.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.719224 miniwdl-1.9.0/stubs/docker/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     2809 2021-11-28 01:40:40.000000 miniwdl-1.9.0/stubs/docker/__init__.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.719224 miniwdl-1.9.0/stubs/importlib_metadata/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      271 2023-01-28 05:55:04.000000 miniwdl-1.9.0/stubs/importlib_metadata/__init__.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.719224 miniwdl-1.9.0/stubs/lark/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      406 2021-06-12 09:10:29.000000 miniwdl-1.9.0/stubs/lark/__init__.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       80 2021-06-12 09:10:29.000000 miniwdl-1.9.0/stubs/lark/exceptions.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.719224 miniwdl-1.9.0/stubs/psutil/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       76 2021-06-12 09:10:29.000000 miniwdl-1.9.0/stubs/psutil/__init__.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.719224 miniwdl-1.9.0/stubs/pygtail/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      319 2021-06-12 09:10:29.000000 miniwdl-1.9.0/stubs/pygtail/__init__.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.719224 miniwdl-1.9.0/stubs/pythonjsonlogger/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      282 2021-06-12 09:10:29.000000 miniwdl-1.9.0/stubs/pythonjsonlogger/jsonlogger.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.719224 miniwdl-1.9.0/stubs/regex/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      528 2023-01-28 05:55:04.000000 miniwdl-1.9.0/stubs/regex/__init__.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.719224 miniwdl-1.9.0/stubs/ruamel/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      168 2021-06-12 09:10:29.000000 miniwdl-1.9.0/stubs/ruamel/yaml.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.719224 miniwdl-1.9.0/stubs/xdg/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       85 2021-06-12 09:10:29.000000 miniwdl-1.9.0/stubs/xdg/__init__.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.719224 miniwdl-1.9.0/test_corpi/
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.703224 miniwdl-1.9.0/test_corpi/DataBiosphere/
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.703224 miniwdl-1.9.0/test_corpi/ENCODE-DCC/
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.703224 miniwdl-1.9.0/test_corpi/HumanCellAtlas/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      501 2021-06-12 09:10:29.000000 miniwdl-1.9.0/test_corpi/README.md
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.703224 miniwdl-1.9.0/test_corpi/biowdl/
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.703224 miniwdl-1.9.0/test_corpi/broadinstitute/
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.719224 miniwdl-1.9.0/test_corpi/contrived/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      466 2021-06-12 09:10:29.000000 miniwdl-1.9.0/test_corpi/contrived/check_quant.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1693 2021-06-12 09:10:29.000000 miniwdl-1.9.0/test_corpi/contrived/contrived.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)        0 2021-06-12 09:10:29.000000 miniwdl-1.9.0/test_corpi/contrived/emptier.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       19 2021-06-12 09:10:29.000000 miniwdl-1.9.0/test_corpi/contrived/empty.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      370 2021-06-12 09:10:29.000000 miniwdl-1.9.0/test_corpi/contrived/incomplete.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       81 2021-06-12 09:10:29.000000 miniwdl-1.9.0/test_corpi/contrived/incomplete_call.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      109 2021-06-12 09:10:29.000000 miniwdl-1.9.0/test_corpi/contrived/incomplete_import.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      356 2021-06-12 09:10:29.000000 miniwdl-1.9.0/test_corpi/contrived/issue120.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      538 2023-01-28 05:55:04.000000 miniwdl-1.9.0/test_corpi/contrived/issue596.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      382 2021-06-12 09:10:29.000000 miniwdl-1.9.0/test_corpi/contrived/issue81.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      330 2021-06-12 09:10:29.000000 miniwdl-1.9.0/test_corpi/contrived/issue82.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      376 2023-01-28 05:55:04.000000 miniwdl-1.9.0/test_corpi/contrived/scatter_collisions.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      629 2021-06-12 09:10:29.000000 miniwdl-1.9.0/test_corpi/contrived/tricky_outputs.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      498 2021-06-12 09:10:29.000000 miniwdl-1.9.0/test_corpi/contrived/unverified_struct.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      654 2023-01-28 05:55:04.000000 miniwdl-1.9.0/test_corpi/contrived/wdl1.1.wdl
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.707224 miniwdl-1.9.0/test_corpi/dnanexus/
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.707224 miniwdl-1.9.0/test_corpi/gatk-workflows/
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.723224 miniwdl-1.9.0/tests/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)        0 2021-06-12 09:10:29.000000 miniwdl-1.9.0/tests/__init__.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      108 2021-06-12 09:10:29.000000 miniwdl-1.9.0/tests/alyssa_ben.txt
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.723224 miniwdl-1.9.0/tests/applied/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      659 2021-06-12 09:10:29.000000 miniwdl-1.9.0/tests/applied/DVGLx.t
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1233 2021-06-12 09:10:29.000000 miniwdl-1.9.0/tests/applied/SARS-CoV-2.t
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      860 2021-06-12 09:10:29.000000 miniwdl-1.9.0/tests/applied/encode_atac_seq.t
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1230 2021-06-12 09:10:29.000000 miniwdl-1.9.0/tests/applied/getting_started.t
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     2820 2021-06-12 09:10:29.000000 miniwdl-1.9.0/tests/applied/skylab.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      790 2021-06-12 09:10:29.000000 miniwdl-1.9.0/tests/applied/skylab_bulk_rna.t
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      696 2021-06-12 09:10:29.000000 miniwdl-1.9.0/tests/applied/viral_assemble.t
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      749 2021-06-12 09:10:29.000000 miniwdl-1.9.0/tests/applied/viral_refbased.t
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     6700 2021-11-28 01:40:40.000000 miniwdl-1.9.0/tests/check.t
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      150 2021-06-12 09:10:29.000000 miniwdl-1.9.0/tests/context.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      827 2022-04-25 00:03:54.000000 miniwdl-1.9.0/tests/eval.t
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      602 2023-01-28 05:55:04.000000 miniwdl-1.9.0/tests/multi_line_strings.t
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     2646 2023-01-28 05:55:04.000000 miniwdl-1.9.0/tests/multi_line_strings.wdl
--rwxrwxr-x   0 mlin      (1000) mlin      (1000)      857 2021-06-12 09:10:29.000000 miniwdl-1.9.0/tests/no_docker_services.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1141 2023-01-28 05:55:04.000000 miniwdl-1.9.0/tests/podman.t
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    17307 2023-01-28 05:55:04.000000 miniwdl-1.9.0/tests/runner.t
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1435 2023-01-28 05:55:04.000000 miniwdl-1.9.0/tests/singularity.t
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1273 2023-01-28 05:55:04.000000 miniwdl-1.9.0/tests/task_env_inputs.wdl
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    26946 2023-01-28 05:55:04.000000 miniwdl-1.9.0/tests/test_0eval.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    66406 2022-08-22 03:32:30.000000 miniwdl-1.9.0/tests/test_1doc.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    20454 2022-04-25 00:03:54.000000 miniwdl-1.9.0/tests/test_2calls.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    20792 2023-01-28 08:05:27.000000 miniwdl-1.9.0/tests/test_3corpi.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    42892 2022-08-05 10:28:39.000000 miniwdl-1.9.0/tests/test_4taskrun.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    61219 2022-08-22 03:32:30.000000 miniwdl-1.9.0/tests/test_5stdlib.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    33941 2023-01-28 08:05:27.000000 miniwdl-1.9.0/tests/test_6workflowrun.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    47876 2023-01-28 08:05:27.000000 miniwdl-1.9.0/tests/test_7runner.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    23255 2021-11-28 01:40:40.000000 miniwdl-1.9.0/tests/test_8cache.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     2676 2022-08-05 10:28:39.000000 miniwdl-1.9.0/tests/test_cli_argcomplete.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1127 2023-01-28 05:55:04.000000 miniwdl-1.9.0/tests/udocker.t
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     2451 2023-01-28 08:05:27.000000 miniwdl-1.9.0/tests/zip.t
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 08:19:28.723224 miniwdl-1.9.0/tools_image/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      529 2022-06-03 09:57:05.000000 miniwdl-1.9.0/tools_image/Dockerfile
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1922 2021-11-28 01:40:40.000000 miniwdl-1.9.0/tools_image/README.md
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.552442 miniwdl-1.9.1/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      220 2022-04-25 00:03:54.000000 miniwdl-1.9.1/.coveragerc
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      100 2021-06-12 09:10:29.000000 miniwdl-1.9.1/.flake8
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.528442 miniwdl-1.9.1/.github/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      724 2021-06-12 09:10:29.000000 miniwdl-1.9.1/.github/pull_request_template.md
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.528442 miniwdl-1.9.1/.github/workflows/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     3463 2022-04-25 03:13:20.000000 miniwdl-1.9.1/.github/workflows/CI.yml
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     3345 2021-06-12 09:10:29.000000 miniwdl-1.9.1/.gitmodules
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       96 2021-06-12 09:10:29.000000 miniwdl-1.9.1/.pyre_configuration
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      294 2021-06-12 09:10:29.000000 miniwdl-1.9.1/.readthedocs.yml
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     3194 2021-06-12 09:10:29.000000 miniwdl-1.9.1/CONTRIBUTING.md
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1539 2023-02-26 10:03:27.000000 miniwdl-1.9.1/Dockerfile
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1084 2021-06-12 09:10:29.000000 miniwdl-1.9.1/LICENSE
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     3048 2023-01-28 05:55:04.000000 miniwdl-1.9.1/Makefile
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      770 2023-02-26 10:21:14.552442 miniwdl-1.9.1/PKG-INFO
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     4194 2023-01-28 08:05:27.000000 miniwdl-1.9.1/README.md
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.532442 miniwdl-1.9.1/WDL/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    73923 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/CLI.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     8192 2021-06-12 09:10:29.000000 miniwdl-1.9.1/WDL/Env.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    11426 2022-04-25 00:03:54.000000 miniwdl-1.9.1/WDL/Error.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    39500 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/Expr.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    49960 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/Lint.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    47536 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/StdLib.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    80101 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/Tree.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    21822 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/Type.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    26027 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/Value.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    11360 2021-11-28 02:55:39.000000 miniwdl-1.9.1/WDL/Walker.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    10824 2023-01-28 08:05:27.000000 miniwdl-1.9.1/WDL/Zip.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    12120 2022-04-25 00:03:54.000000 miniwdl-1.9.1/WDL/__init__.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       85 2021-06-12 09:10:29.000000 miniwdl-1.9.1/WDL/__main__.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    17889 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/_grammar.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    30547 2023-01-28 08:05:27.000000 miniwdl-1.9.1/WDL/_parser.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    30366 2022-08-05 10:28:39.000000 miniwdl-1.9.1/WDL/_util.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)        0 2022-04-25 00:03:54.000000 miniwdl-1.9.1/WDL/py.typed
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.532442 miniwdl-1.9.1/WDL/runtime/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     2700 2021-11-28 01:40:40.000000 miniwdl-1.9.1/WDL/runtime/__init__.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     4304 2022-04-25 00:03:54.000000 miniwdl-1.9.1/WDL/runtime/_statusbar.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.532442 miniwdl-1.9.1/WDL/runtime/backend/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)        0 2021-11-28 01:40:40.000000 miniwdl-1.9.1/WDL/runtime/backend/__init__.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    11427 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/runtime/backend/cli_subprocess.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    31078 2023-02-16 05:11:14.000000 miniwdl-1.9.1/WDL/runtime/backend/docker_swarm.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     5905 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/runtime/backend/podman.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     4750 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/runtime/backend/singularity.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     2414 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/runtime/backend/udocker.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    15632 2022-08-22 03:32:30.000000 miniwdl-1.9.1/WDL/runtime/cache.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    16771 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/runtime/config.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.532442 miniwdl-1.9.1/WDL/runtime/config_templates/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    16060 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/runtime/config_templates/default.cfg
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    15237 2022-08-22 03:32:30.000000 miniwdl-1.9.1/WDL/runtime/download.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     4798 2021-11-28 01:40:40.000000 miniwdl-1.9.1/WDL/runtime/error.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    41635 2023-01-28 05:55:04.000000 miniwdl-1.9.1/WDL/runtime/task.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    23399 2023-01-28 08:05:27.000000 miniwdl-1.9.1/WDL/runtime/task_container.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    46714 2023-02-26 10:03:27.000000 miniwdl-1.9.1/WDL/runtime/workflow.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.536442 miniwdl-1.9.1/docs/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     4866 2022-08-05 10:28:39.000000 miniwdl-1.9.1/docs/FAQ.md
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      604 2021-06-12 09:10:29.000000 miniwdl-1.9.1/docs/Makefile
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1068 2023-01-28 05:55:04.000000 miniwdl-1.9.1/docs/WDL.rst
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     7560 2021-06-12 09:10:29.000000 miniwdl-1.9.1/docs/add_functions.md
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     9558 2022-04-25 00:03:54.000000 miniwdl-1.9.1/docs/assert.md
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     4261 2021-11-28 01:40:40.000000 miniwdl-1.9.1/docs/check.rst
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     4974 2022-04-25 00:03:54.000000 miniwdl-1.9.1/docs/conf.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     8277 2022-11-02 08:51:54.000000 miniwdl-1.9.1/docs/getting_started.md
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      797 2022-08-22 03:32:30.000000 miniwdl-1.9.1/docs/index.rst
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    80175 2021-06-12 09:10:29.000000 miniwdl-1.9.1/docs/miniwdl-logo.png
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     8569 2023-01-28 05:55:04.000000 miniwdl-1.9.1/docs/runner_advanced.md
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     6761 2023-01-28 08:05:27.000000 miniwdl-1.9.1/docs/runner_backends.md
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      173 2021-06-12 09:10:29.000000 miniwdl-1.9.1/docs/runner_cli.rst
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    13637 2022-11-02 08:51:54.000000 miniwdl-1.9.1/docs/runner_reference.md
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     9631 2021-06-12 09:10:29.000000 miniwdl-1.9.1/docs/trace_identifiers.md
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    11049 2023-01-28 08:05:27.000000 miniwdl-1.9.1/docs/wdlviz.md
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     4692 2021-06-12 09:10:29.000000 miniwdl-1.9.1/docs/wdlviz_ex1.png
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    80838 2021-06-12 09:10:29.000000 miniwdl-1.9.1/docs/wdlviz_ex2.png
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      926 2022-08-22 03:32:30.000000 miniwdl-1.9.1/docs/zip.rst
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.536442 miniwdl-1.9.1/examples/
+-rwxrwxr-x   0 mlin      (1000) mlin      (1000)     2758 2021-11-28 01:40:40.000000 miniwdl-1.9.1/examples/clean_download_cache.sh
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     2278 2021-11-28 01:40:40.000000 miniwdl-1.9.1/examples/clean_download_cache.t
+-rwxrwxr-x   0 mlin      (1000) mlin      (1000)     4608 2021-06-12 09:10:29.000000 miniwdl-1.9.1/examples/paste_wdl_imports.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.536442 miniwdl-1.9.1/examples/plugin_log_task_usage/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     2133 2021-06-12 09:10:29.000000 miniwdl-1.9.1/examples/plugin_log_task_usage/miniwdl_log_task_usage.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      430 2021-06-12 09:10:29.000000 miniwdl-1.9.1/examples/plugin_log_task_usage/setup.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/examples/plugin_s3_progressive_upload/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     8091 2023-01-28 05:55:04.000000 miniwdl-1.9.1/examples/plugin_s3_progressive_upload/miniwdl_s3_progressive_upload.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      643 2023-01-28 05:55:04.000000 miniwdl-1.9.1/examples/plugin_s3_progressive_upload/setup.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     3422 2023-01-28 05:55:04.000000 miniwdl-1.9.1/examples/plugin_s3_progressive_upload/test.t
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/examples/plugin_task_omnibus/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     6894 2021-06-12 09:10:29.000000 miniwdl-1.9.1/examples/plugin_task_omnibus/miniwdl_task_omnibus_example.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      483 2021-06-12 09:10:29.000000 miniwdl-1.9.1/examples/plugin_task_omnibus/setup.py
+-rwxrwxr-x   0 mlin      (1000) mlin      (1000)     2582 2021-06-12 09:10:29.000000 miniwdl-1.9.1/examples/run_with_custom_error.py
+-rwxrwxr-x   0 mlin      (1000) mlin      (1000)     2797 2023-01-28 05:55:04.000000 miniwdl-1.9.1/examples/upload_output_files.sh
+-rwxrwxr-x   0 mlin      (1000) mlin      (1000)     6525 2022-04-25 00:03:54.000000 miniwdl-1.9.1/examples/wdlviz.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/miniwdl.egg-info/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      770 2023-02-26 10:21:13.000000 miniwdl-1.9.1/miniwdl.egg-info/PKG-INFO
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     4613 2023-02-26 10:21:14.000000 miniwdl-1.9.1/miniwdl.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)        1 2023-02-26 10:21:13.000000 miniwdl-1.9.1/miniwdl.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       41 2023-02-26 10:21:13.000000 miniwdl-1.9.1/miniwdl.egg-info/entry_points.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)        1 2021-06-27 08:22:31.000000 miniwdl-1.9.1/miniwdl.egg-info/not-zip-safe
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       46 2023-02-26 10:21:13.000000 miniwdl-1.9.1/miniwdl.egg-info/pbr.json
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      214 2023-02-26 10:21:13.000000 miniwdl-1.9.1/miniwdl.egg-info/requires.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)        4 2023-02-26 10:21:14.000000 miniwdl-1.9.1/miniwdl.egg-info/top_level.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      375 2023-02-26 10:03:27.000000 miniwdl-1.9.1/requirements.dev.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      355 2023-01-28 08:05:27.000000 miniwdl-1.9.1/requirements.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      807 2023-02-26 10:21:14.552442 miniwdl-1.9.1/setup.cfg
+-rwxrwxr-x   0 mlin      (1000) mlin      (1000)      134 2021-06-12 09:10:29.000000 miniwdl-1.9.1/setup.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/stubs/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      203 2021-06-12 09:10:29.000000 miniwdl-1.9.1/stubs/README.md
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/stubs/argcomplete/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      134 2021-06-12 09:10:29.000000 miniwdl-1.9.1/stubs/argcomplete/__init__.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/stubs/bullet/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)        0 2021-06-12 09:10:29.000000 miniwdl-1.9.1/stubs/bullet/__init__.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/stubs/coloredlogs/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      325 2021-06-12 09:10:29.000000 miniwdl-1.9.1/stubs/coloredlogs/__init__.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/stubs/docker/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     2809 2021-11-28 01:40:40.000000 miniwdl-1.9.1/stubs/docker/__init__.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/stubs/importlib_metadata/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      271 2023-01-28 05:55:04.000000 miniwdl-1.9.1/stubs/importlib_metadata/__init__.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/stubs/lark/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      406 2021-06-12 09:10:29.000000 miniwdl-1.9.1/stubs/lark/__init__.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       80 2021-06-12 09:10:29.000000 miniwdl-1.9.1/stubs/lark/exceptions.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/stubs/psutil/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       76 2021-06-12 09:10:29.000000 miniwdl-1.9.1/stubs/psutil/__init__.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/stubs/pygtail/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      319 2021-06-12 09:10:29.000000 miniwdl-1.9.1/stubs/pygtail/__init__.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/stubs/pythonjsonlogger/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      282 2021-06-12 09:10:29.000000 miniwdl-1.9.1/stubs/pythonjsonlogger/jsonlogger.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/stubs/regex/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      583 2023-02-26 10:03:27.000000 miniwdl-1.9.1/stubs/regex/__init__.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/stubs/ruamel/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      168 2021-06-12 09:10:29.000000 miniwdl-1.9.1/stubs/ruamel/yaml.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/stubs/xdg/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       85 2021-06-12 09:10:29.000000 miniwdl-1.9.1/stubs/xdg/__init__.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.540442 miniwdl-1.9.1/test_corpi/
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.524442 miniwdl-1.9.1/test_corpi/DataBiosphere/
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.524442 miniwdl-1.9.1/test_corpi/ENCODE-DCC/
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.524442 miniwdl-1.9.1/test_corpi/HumanCellAtlas/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      501 2021-06-12 09:10:29.000000 miniwdl-1.9.1/test_corpi/README.md
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.524442 miniwdl-1.9.1/test_corpi/biowdl/
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.524442 miniwdl-1.9.1/test_corpi/broadinstitute/
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.544442 miniwdl-1.9.1/test_corpi/contrived/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      466 2021-06-12 09:10:29.000000 miniwdl-1.9.1/test_corpi/contrived/check_quant.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1693 2021-06-12 09:10:29.000000 miniwdl-1.9.1/test_corpi/contrived/contrived.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)        0 2021-06-12 09:10:29.000000 miniwdl-1.9.1/test_corpi/contrived/emptier.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       19 2021-06-12 09:10:29.000000 miniwdl-1.9.1/test_corpi/contrived/empty.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      425 2023-02-26 10:03:27.000000 miniwdl-1.9.1/test_corpi/contrived/env.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      370 2021-06-12 09:10:29.000000 miniwdl-1.9.1/test_corpi/contrived/incomplete.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       81 2021-06-12 09:10:29.000000 miniwdl-1.9.1/test_corpi/contrived/incomplete_call.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      109 2021-06-12 09:10:29.000000 miniwdl-1.9.1/test_corpi/contrived/incomplete_import.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      356 2021-06-12 09:10:29.000000 miniwdl-1.9.1/test_corpi/contrived/issue120.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      523 2023-02-26 10:03:27.000000 miniwdl-1.9.1/test_corpi/contrived/issue596.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      382 2021-06-12 09:10:29.000000 miniwdl-1.9.1/test_corpi/contrived/issue81.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      330 2021-06-12 09:10:29.000000 miniwdl-1.9.1/test_corpi/contrived/issue82.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      376 2023-01-28 05:55:04.000000 miniwdl-1.9.1/test_corpi/contrived/scatter_collisions.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      629 2021-06-12 09:10:29.000000 miniwdl-1.9.1/test_corpi/contrived/tricky_outputs.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      498 2021-06-12 09:10:29.000000 miniwdl-1.9.1/test_corpi/contrived/unverified_struct.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      654 2023-01-28 05:55:04.000000 miniwdl-1.9.1/test_corpi/contrived/wdl1.1.wdl
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.524442 miniwdl-1.9.1/test_corpi/dnanexus/
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.524442 miniwdl-1.9.1/test_corpi/gatk-workflows/
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.548442 miniwdl-1.9.1/tests/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)        0 2021-06-12 09:10:29.000000 miniwdl-1.9.1/tests/__init__.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      108 2021-06-12 09:10:29.000000 miniwdl-1.9.1/tests/alyssa_ben.txt
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.552442 miniwdl-1.9.1/tests/applied/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      659 2021-06-12 09:10:29.000000 miniwdl-1.9.1/tests/applied/DVGLx.t
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1233 2021-06-12 09:10:29.000000 miniwdl-1.9.1/tests/applied/SARS-CoV-2.t
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      860 2021-06-12 09:10:29.000000 miniwdl-1.9.1/tests/applied/encode_atac_seq.t
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1230 2021-06-12 09:10:29.000000 miniwdl-1.9.1/tests/applied/getting_started.t
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     2820 2021-06-12 09:10:29.000000 miniwdl-1.9.1/tests/applied/skylab.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      790 2021-06-12 09:10:29.000000 miniwdl-1.9.1/tests/applied/skylab_bulk_rna.t
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      696 2021-06-12 09:10:29.000000 miniwdl-1.9.1/tests/applied/viral_assemble.t
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      749 2021-06-12 09:10:29.000000 miniwdl-1.9.1/tests/applied/viral_refbased.t
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     6700 2021-11-28 01:40:40.000000 miniwdl-1.9.1/tests/check.t
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      150 2021-06-12 09:10:29.000000 miniwdl-1.9.1/tests/context.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      827 2022-04-25 00:03:54.000000 miniwdl-1.9.1/tests/eval.t
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      602 2023-01-28 05:55:04.000000 miniwdl-1.9.1/tests/multi_line_strings.t
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     2646 2023-01-28 05:55:04.000000 miniwdl-1.9.1/tests/multi_line_strings.wdl
+-rwxrwxr-x   0 mlin      (1000) mlin      (1000)      857 2021-06-12 09:10:29.000000 miniwdl-1.9.1/tests/no_docker_services.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1141 2023-01-28 05:55:04.000000 miniwdl-1.9.1/tests/podman.t
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    17307 2023-01-28 05:55:04.000000 miniwdl-1.9.1/tests/runner.t
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1435 2023-01-28 05:55:04.000000 miniwdl-1.9.1/tests/singularity.t
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1273 2023-01-28 05:55:04.000000 miniwdl-1.9.1/tests/task_env_inputs.wdl
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    26946 2023-01-28 05:55:04.000000 miniwdl-1.9.1/tests/test_0eval.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    66406 2022-08-22 03:32:30.000000 miniwdl-1.9.1/tests/test_1doc.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    20454 2022-04-25 00:03:54.000000 miniwdl-1.9.1/tests/test_2calls.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    20793 2023-02-26 10:03:27.000000 miniwdl-1.9.1/tests/test_3corpi.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    42892 2022-08-05 10:28:39.000000 miniwdl-1.9.1/tests/test_4taskrun.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    61219 2022-08-22 03:32:30.000000 miniwdl-1.9.1/tests/test_5stdlib.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    33941 2023-01-28 08:05:27.000000 miniwdl-1.9.1/tests/test_6workflowrun.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    47876 2023-01-28 08:05:27.000000 miniwdl-1.9.1/tests/test_7runner.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    23255 2021-11-28 01:40:40.000000 miniwdl-1.9.1/tests/test_8cache.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     2676 2022-08-05 10:28:39.000000 miniwdl-1.9.1/tests/test_cli_argcomplete.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1127 2023-01-28 05:55:04.000000 miniwdl-1.9.1/tests/udocker.t
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     2451 2023-01-28 08:05:27.000000 miniwdl-1.9.1/tests/zip.t
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-26 10:21:14.552442 miniwdl-1.9.1/tools_image/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      529 2022-06-03 09:57:05.000000 miniwdl-1.9.1/tools_image/Dockerfile
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1922 2021-11-28 01:40:40.000000 miniwdl-1.9.1/tools_image/README.md
```

### Comparing `miniwdl-1.9.0/.github/pull_request_template.md` & `miniwdl-1.9.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/.github/workflows/CI.yml` & `miniwdl-1.9.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/.gitmodules` & `miniwdl-1.9.1/.gitmodules`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/CONTRIBUTING.md` & `miniwdl-1.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/Dockerfile` & `miniwdl-1.9.1/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # run the full test suite -- notice configuration needed for it to command the host dockerd
 #    docker run  \
 #       -v /var/run/docker.sock:/var/run/docker.sock --group-add $(stat -c %g /var/run/docker.sock)
 #       -v $(pwd):/home/wdler/miniwdl -v /tmp:/tmp \
 #       --rm -it miniwdl
 # or append 'bash' to that to enter interactive shell
 
-# start with ubuntu:18.04 plus some apt packages
-FROM ubuntu:18.04 as deps
+# start with ubuntu:20.04 plus some apt packages
+FROM ubuntu:20.04 as deps
 ENV LC_ALL C.UTF-8
 ENV LANG C.UTF-8
 RUN apt-get -qq update && DEBIAN_FRONTEND=noninteractive apt-get -qq install -y \
     python3-pip python3-setuptools tzdata wget zip git-core default-jre jq shellcheck docker.io
 RUN pip3 install -U pip  # due to infamous pyca/cryptography#5771
 
 # add and become 'wdler' user -- it's useful to run the test suite as some arbitrary uid, because
```

### Comparing `miniwdl-1.9.0/LICENSE` & `miniwdl-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/Makefile` & `miniwdl-1.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/PKG-INFO` & `miniwdl-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniwdl
-Version: 1.9.0
+Version: 1.9.1
 Summary: Workflow Description Language (WDL) local runner & developer toolkit
 Home-page: https://github.com/chanzuckerberg/miniwdl
 Author: CZI
 Author-email: security@chanzuckerberg.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `miniwdl-1.9.0/README.md` & `miniwdl-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/CLI.py` & `miniwdl-1.9.1/WDL/CLI.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
     s = "".join(" " for i in range(level * 4))
 
     first_descent = []
 
     def descend(dobj=None, first_descent=first_descent):
         # show lint for the node just prior to first descent beneath it
         if not first_descent and hasattr(obj, "lint"):
-            for (pos, cls, msg, suppressed) in sorted(obj.lint, key=lambda t: t[0]):
+            for pos, cls, msg, suppressed in sorted(obj.lint, key=lambda t: t[0]):
                 if not (suppress and str(cls) in suppress) and (show_all or not suppressed):
                     print(
                         f"{s}    (Ln {pos.line}, Col {pos.column}) {cls}{' (suppressed)' if suppressed else ''}, {msg}",
                         file=file,
                     )
                     if shown:
                         shown[0] += 1
```

### Comparing `miniwdl-1.9.0/WDL/Env.py` & `miniwdl-1.9.1/WDL/Env.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/Error.py` & `miniwdl-1.9.1/WDL/Error.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/Expr.py` & `miniwdl-1.9.1/WDL/Expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -664,15 +664,15 @@
         self,
         pos: SourcePosition,
         members: List[Tuple[str, Base]],
         struct_type_name: Optional[str] = None,
     ):
         super().__init__(pos)
         self.members = {}
-        for (k, v) in members:
+        for k, v in members:
             if k in self.members:
                 raise Error.MultipleDefinitions(self.pos, "duplicate keys " + k)
             self.members[k] = v
         self.struct_type_name = struct_type_name
         assert struct_type_name is None or isinstance(struct_type_name, str), str(struct_type_name)
 
     def __str__(self):
@@ -1122,15 +1122,14 @@
 
     @property
     def children(self) -> Iterable[SourceNode]:
         for arg in self.arguments:
             yield arg
 
     def _infer_type(self, type_env: Env.Bindings[Type.Base]) -> Type.Base:
-
         f = getattr(self._stdlib, self.function_name, None)
         if not f:
             raise Error.NoSuchFunction(self, self.function_name) from None
         assert isinstance(f, StdLib.Function)
         return f.infer_type(self)
 
     def _eval(self, env: Env.Bindings[Value.Base], stdlib: StdLib.Base) -> Value.Base:
```

### Comparing `miniwdl-1.9.0/WDL/Lint.py` & `miniwdl-1.9.1/WDL/Lint.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 import subprocess
 import tempfile
 import json
 import os
 import random
 import shutil
 from typing import Any, Optional, Union
+import regex
 from . import Error, Type, Env, Expr, Tree, StdLib, Walker, _util
 
 
 def _find_doc(obj: Error.SourceNode):
     "find the containing document"
     doc = obj
     while not isinstance(doc, Tree.Document):
@@ -777,14 +778,16 @@
         if not is_output and not getattr(obj, "referrers", []):
             # heuristic exceptions:
             # 1. File whose name suggests it's an hts index file; as these
             #    commonly need to be localized, but not explicitly used in task
             #    command
             # 2. dxWDL "native" task stubs, which declare inputs but leave
             #    command empty.
+            # 3. task declaration has "env" decorator and the command uses it
+            #    as an environment variable
             index_suffixes = [
                 "index",
                 "indexes",
                 "indices",
                 "idx",
                 "tbi",
                 "bai",
@@ -804,17 +807,37 @@
                     and sum(1 for sfx in index_suffixes if obj.name.lower().endswith(sfx))
                 )
                 or (
                     isinstance(pt, Tree.Task)
                     and pt.meta.get("type") == "native"
                     and pt.meta.get("id")
                 )
+                or self._used_as_command_env_var(obj)
             ):
                 self.add(obj, "nothing references {} {}".format(str(obj.type), obj.name))
 
+    def _used_as_command_env_var(self, decl: Tree.Decl) -> bool:
+        # Task input declarations with the "env" modifier are intended to be
+        # used as environment variables in the task command. False-positive
+        # UnusedDeclaration warnings might result because such references are
+        # not modeled in our WDL syntax tree.
+        # Avoid this by searching for apparent usage of the environment
+        # variable in string literal parts of the task command script. This
+        # isn't a perfect heuristic (e.g. it could be single-quoted within the
+        # script), but that's OK for lint warning purposes.
+        task = getattr(decl, "parent")
+        if not (isinstance(task, Tree.Task) and decl.decor.get("env", False)):
+            return False
+        pat = regex.compile(r"\$\{?" + decl.name + r"([^0-9A-Za-z_]|$)")
+        for part in task.command.parts:
+            if isinstance(part, str):
+                if pat.search(part):
+                    return True
+        return False
+
 
 @a_linter
 class UnusedCall(Linter):
     # the outputs of a Call are neither used nor propagated
 
     def call(self, obj: Tree.Call) -> Any:
         if obj.effective_outputs and not getattr(obj, "referrers", []):
@@ -935,20 +958,30 @@
                     obj,
                     "shellcheck failed on the task command; update shellcheck version or use --no-shellcheck "
                     "to suppress this warning",
                     obj.command.pos,
                 )
 
         if shellcheck_items:
+            env_decls = set(
+                decl.name
+                for decl in ((obj.inputs or []) + obj.postinputs)
+                if decl.decor.get("env", False)
+            )
             try:
                 shellcheck_items = json.loads(shellcheck_items)
                 assert isinstance(shellcheck_items, list)
 
                 # annotate on tree, adding appropriate offsets to line/column positions
                 for item in shellcheck_items:
+                    if item["code"] == 2154 and item["message"].split(" ")[0] in env_decls:
+                        # Suppress SC2154 "var is referenced but not assigned" specifically when
+                        # var corresponds to a declaration with the "env" modifier. ShellCheck
+                        # doesn't know that command expects this var to be set in its environment.
+                        continue
                     line = obj.command.pos.line + item["line"] - 1
                     column = col_offset + item["column"] - 1
                     self.add(
                         obj,
                         "SC{} {}".format(item["code"], item["message"]),
                         Error.SourcePosition(
                             uri=obj.command.pos.uri,
@@ -1023,15 +1056,14 @@
                     "array of non-optional items passed to " + obj.function_name,
                     obj.arguments[0].pos,
                 )
 
 
 @a_linter
 class UnknownRuntimeKey(Linter):
-
     # refs:
     # https://cromwell.readthedocs.io/en/develop/RuntimeAttributes/
     # https://github.com/broadinstitute/cromwell/blob/develop/wom/src/main/scala/wom/RuntimeAttributes.scala
     # https://github.com/broadinstitute/cromwell/blob/develop/supportedBackends/google/pipelines/common/src/main/scala/cromwell/backend/google/pipelines/common/PipelinesApiRuntimeAttributes.scala
     # https://github.com/broadinstitute/cromwell/blob/develop/supportedBackends/aws/src/main/scala/cromwell/backend/impl/aws/AwsBatchRuntimeAttributes.scala
     # https://github.com/openwdl/wdl/pull/315
     # https://github.com/dnanexus/dxWDL/blob/master/doc/ExpertOptions.md
```

### Comparing `miniwdl-1.9.0/WDL/StdLib.py` & `miniwdl-1.9.1/WDL/StdLib.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
     """
     Defines type signatures for functions only available in task output sections.
     (Implementations left to by overridden by the task runtime)
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        for (name, argument_types, return_type, F) in [
+        for name, argument_types, return_type, F in [
             ("stdout", [], Type.File(), _notimpl),
             ("stderr", [], Type.File(), _notimpl),
             ("glob", [Type.String()], Type.Array(Type.File()), _notimpl),
         ]:
             setattr(self, name, StaticFunction(name, argument_types, return_type, F))
 
 
@@ -402,15 +402,15 @@
         ),
         outfile,
     )
 
 
 def _serialize_map(map: Value.Map, outfile: BinaryIO) -> None:
     lines = []
-    for (k, v) in map.value:
+    for k, v in map.value:
         k = k.coerce(Type.String()).value
         v = v.coerce(Type.String()).value
         if "\n" in k or "\t" in k or "\n" in v or "\t" in v:
             raise ValueError(
                 "write_map(): keys & values must not contain tab or newline characters"
             )
         lines.append(Value.String(k + "\t" + v))
```

### Comparing `miniwdl-1.9.0/WDL/Tree.py` & `miniwdl-1.9.1/WDL/Tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1889,15 +1889,15 @@
     for imp in [
         imp for imp in doc.imports if imp.doc
     ]:  # imp.doc should be None only for certain legacy unit tests
         imported_structs = {}
         for stb in imp.doc.struct_typedefs:
             assert isinstance(stb, Env.Binding) and isinstance(stb.value, StructTypeDef)
             imported_structs[stb.name] = stb.value
-        for (name, alias) in imp.aliases:
+        for name, alias in imp.aliases:
             if name not in imported_structs:
                 raise Error.NoSuchMember(imp.pos, name)
             if alias in imported_structs:
                 raise Error.MultipleDefinitions(
                     imp.pos,
                     "struct type alias {} collides with another struct type in the imported document".format(
                         alias
@@ -1917,15 +1917,15 @@
                     ),
                 )
             except KeyError:
                 pass
             if alias != name:
                 imported_structs[alias] = imported_structs[name]
                 del imported_structs[name]
-        for (name, st) in imported_structs.items():
+        for name, st in imported_structs.items():
             existing = None
             try:
                 existing = doc.struct_typedefs[name]
                 if existing.type_id != st.type_id:
                     raise Error.MultipleDefinitions(
                         imp.pos,
                         "imported struct {} must be aliased because it collides with a struct {} document".format(
```

### Comparing `miniwdl-1.9.0/WDL/Type.py` & `miniwdl-1.9.1/WDL/Type.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,15 +443,15 @@
         return self.members.values()
 
 
 def _struct_type_id(members: Dict[str, Base]) -> str:
     # generates a content hash of the struct type definition, used to recognize
     # equivalent struct types going by different aliases
     ans = []
-    for (name, ty) in sorted(members.items()):
+    for name, ty in sorted(members.items()):
         if isinstance(ty, StructInstance):
             assert ty.members
             ty = _struct_type_id(ty.members) + ("?" if ty.optional else "")
         else:
             ty = str(ty)
         ans.append(name + " : " + ty)
     return "struct(" + ", ".join(ans) + ")"
```

### Comparing `miniwdl-1.9.0/WDL/Value.py` & `miniwdl-1.9.1/WDL/Value.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
         items = {}
         for k, v in self.value:
             items[str(k)] = str(v)
         return "{" + ", ".join(f"{k}: {v}" for k, v in items.items()) + "}"
 
     @property
     def children(self) -> Iterable[Base]:
-        for (k, v) in self.value:
+        for k, v in self.value:
             yield k
             yield v
 
     def coerce(self, desired_type: Optional[Type.Base] = None) -> Base:
         """"""
         if isinstance(desired_type, Type.Map) and desired_type != self.type:
             return Map(
```

### Comparing `miniwdl-1.9.0/WDL/Walker.py` & `miniwdl-1.9.1/WDL/Walker.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/Zip.py` & `miniwdl-1.9.1/WDL/Zip.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/__init__.py` & `miniwdl-1.9.1/WDL/__init__.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/_grammar.py` & `miniwdl-1.9.1/WDL/_grammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 scatter: "scatter" "(" CNAME "in" expr ")" "{" inner_workflow_element* "}"
 conditional: "if" "(" expr ")" "{" inner_workflow_element* "}"
 ?inner_workflow_element: any_decl | call | scatter | conditional
 
 call: "call" namespaced_ident ("after" CNAME)* _call_body? -> call
     | "call" namespaced_ident "as" CNAME ("after" CNAME)* _call_body? -> call_as
 namespaced_ident: CNAME ("." CNAME)*
-call_inputs: "input" ":" [call_input ("," call_input)*] ","?
+call_inputs: ["input" ":"] [call_input ("," call_input)*] ","?
 _call_body: "{" call_inputs? "}"
 call_input: CNAME ["=" expr]
 
 ?workflow_outputs: output_decls
 
 ///////////////////////////////////////////////////////////////////////////////////////////////////
 // task
```

### Comparing `miniwdl-1.9.0/WDL/_parser.py` & `miniwdl-1.9.1/WDL/_parser.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/_util.py` & `miniwdl-1.9.1/WDL/_util.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/runtime/__init__.py` & `miniwdl-1.9.1/WDL/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/runtime/_statusbar.py` & `miniwdl-1.9.1/WDL/runtime/_statusbar.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/runtime/backend/cli_subprocess.py` & `miniwdl-1.9.1/WDL/runtime/backend/cli_subprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,14 @@
         assert self._bind_input_files
         super().copy_input_files(logger)
         # now that files have been copied into the working dir, it won't be necessary to bind-mount
         # them individually
         self._bind_input_files = False
 
     def prepare_mounts(self) -> List[Tuple[str, str, bool]]:
-
         mounts = []
         # mount stdout, stderr, and working directory read/write
         self.touch_mount_point(self.host_stdout_txt())
         mounts.append(
             (os.path.join(self.container_dir, "stdout.txt"), self.host_stdout_txt(), True)
         )
         self.touch_mount_point(self.host_stderr_txt())
```

### Comparing `miniwdl-1.9.0/WDL/runtime/backend/docker_swarm.py` & `miniwdl-1.9.1/WDL/runtime/backend/docker_swarm.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/runtime/backend/podman.py` & `miniwdl-1.9.1/WDL/runtime/backend/podman.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         logger.info(
             _(
                 "podman invocation",
                 args=" ".join(shlex.quote(s) for s in (ans + [image])),
                 binds=len(mounts),
             )
         )
-        for (container_path, host_path, writable) in mounts:
+        for container_path, host_path, writable in mounts:
             if ":" in (container_path + host_path):
                 raise InputError("Podman input filenames cannot contain ':'")
             ans.append("-v")
             bind_arg = f"{host_path}:{container_path}"
             if not writable:
                 bind_arg += ":ro"
             ans.append(bind_arg)
```

### Comparing `miniwdl-1.9.0/WDL/runtime/backend/singularity.py` & `miniwdl-1.9.1/WDL/runtime/backend/singularity.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         Formulate `singularity run` command-line invocation
         """
 
         ans = self.cli_exe
         if logger.isEnabledFor(logging.DEBUG):
             ans.append("--verbose")
         ans += [
-            "run",
+            "exec",
             "--pwd",
             os.path.join(self.container_dir, "work"),
         ]
         if self.runtime_values.get("privileged", False) is True:
             logger.warning("runtime.privileged enabled (security & portability warning)")
             ans += ["--add-caps", "all"]
         ans += self.cfg.get_list("singularity", "run_options")
@@ -108,15 +108,15 @@
             _(
                 "singularity invocation",
                 args=" ".join(shlex.quote(s) for s in (ans + [image])),
                 binds=len(mounts),
                 tmpdir=tempdir,
             )
         )
-        for (container_path, host_path, writable) in mounts:
+        for container_path, host_path, writable in mounts:
             if ":" in (container_path + host_path):
                 raise InputError("Singularity input filenames cannot contain ':'")
             ans.append("--bind")
             bind_arg = f"{host_path}:{container_path}"
             if not writable:
                 bind_arg += ":ro"
             ans.append(bind_arg)
```

### Comparing `miniwdl-1.9.0/WDL/runtime/backend/udocker.py` & `miniwdl-1.9.1/WDL/runtime/backend/udocker.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,14 @@
         logger.info(
             _(
                 "udocker invocation",
                 args=" ".join(shlex.quote(s) for s in (ans + [image])),
                 binds=len(mounts),
             )
         )
-        for (container_path, host_path, _writable) in mounts:
+        for container_path, host_path, _writable in mounts:
             if ":" in (container_path + host_path):
                 raise InputError("udocker input filenames cannot contain ':'")
             ans.append("-v")
             ans.append(f"{host_path}:{container_path}")
         ans.append(image)
         return ans
```

### Comparing `miniwdl-1.9.0/WDL/runtime/cache.py` & `miniwdl-1.9.1/WDL/runtime/cache.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/runtime/config.py` & `miniwdl-1.9.1/WDL/runtime/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
             options |= set((section, key) for key in self._overrides.options(section))
         for section in self._options.sections():
             options |= set((section, key) for key in self._options.options(section))
         for section in self._defaults.sections():
             options |= set((section, key) for key in self._defaults.options(section))
 
         all = {}
-        for (section, key) in options:
+        for section, key in options:
             value = self.get(section, key)
             default_value = None
             if not defaults and self._defaults.has_option(section, key):
                 default_value = self._defaults.get(section, key)
                 default_value = _expand_env_var(_strip(default_value))
             if defaults or value != default_value:
                 all[section] = all.get(section, dict())
```

### Comparing `miniwdl-1.9.0/WDL/runtime/config_templates/default.cfg` & `miniwdl-1.9.1/WDL/runtime/config_templates/default.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -200,33 +200,33 @@
 # systems with low limits on the number of outstanding flocks.
 # (Opt-out new in v1.3.1)
 flock = true
 
 
 [download_aria2c]
 # see: https://github.com/chanzuckerberg/miniwdl/tree/main/tools_image
-docker = ghcr.io/miniwdl-ext/miniwdl-tools:Id_sha256_c519ec5aad2c8968329623049562dcf2b94cd4ea6d3a50085270629f6922cafc
+docker = ghcr.io/miniwdl-ext/miniwdl-tools:Id_sha256_e5e90788bf3720c5391a3206a3a59cec016f6f09415382de719e7317f67bbcf6
 
 
 [download_awscli]
 # If workflow inputs or generates s3:// URIs, load AWS credentials using boto3 on the miniwdl host.
 # Note: If running inside EC2, downloader & other tasks might be able assume an IAM role via the
 #       instance metadata service, regardless of this setting. You can set the environment variable
 #       AWS_EC2_METADATA_DISABLED=true to prevent this (or use iptables to block the endpoint IP).
 # Recommendation: use only trusted WDL and Docker images, if either host_credentials = true or an
 #                 EC2 instance profile is available.
 # Failing all of the above, public S3 URIs can always be used.
 host_credentials = false
 # see: https://github.com/chanzuckerberg/miniwdl/tree/main/tools_image
-docker = ghcr.io/miniwdl-ext/miniwdl-tools:Id_sha256_c519ec5aad2c8968329623049562dcf2b94cd4ea6d3a50085270629f6922cafc
+docker = ghcr.io/miniwdl-ext/miniwdl-tools:Id_sha256_e5e90788bf3720c5391a3206a3a59cec016f6f09415382de719e7317f67bbcf6
 
 
 [download_gsutil]
 # current version from https://github.com/GoogleCloudPlatform/cloud-sdk-docker/releases
-docker = gcr.io/google.com/cloudsdktool/cloud-sdk:412.0.0-slim
+docker = gcr.io/google.com/cloudsdktool/cloud-sdk:419.0.0-slim
 
 
 [call_cache]
 # Register task outputs for potential reuse by subsequent executions of the same task & inputs
 put = false
 # Enable use of previously-cached outputs
 get = false
@@ -263,15 +263,15 @@
 
 [singularity]
 # Singularity task runtime -- with `singularity` CLI already set up, set
 #     [task_scheduler] container_backend = singularity
 #
 # singularity executable and any desired global options
 exe = ["singularity"]
-# Configuration options to pass to `singularity run` invocations. Defaults for docker-like
+# Configuration options to pass to `singularity exec` invocations. Defaults for docker-like
 # isolation from the host.
 run_options = [
         "--containall",
         "--no-mount", "hostfs",
         "--fakeroot"
     ]
 # Where pulled images should be stored to save image construction time between
```

### Comparing `miniwdl-1.9.0/WDL/runtime/download.py` & `miniwdl-1.9.1/WDL/runtime/download.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/runtime/error.py` & `miniwdl-1.9.1/WDL/runtime/error.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/runtime/task.py` & `miniwdl-1.9.1/WDL/runtime/task.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/runtime/task_container.py` & `miniwdl-1.9.1/WDL/runtime/task_container.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/WDL/runtime/workflow.py` & `miniwdl-1.9.1/WDL/runtime/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -483,15 +483,14 @@
             array = [None]
     digits = math.ceil(math.log10(len(array))) if len(array) > 1 else 1
 
     # for each array element, schedule an instance of the body subgraph
     last_scatter_indices = None
     scatter_tags = _scatter_tags(array, max_tag)
     for i, array_i in enumerate(array):
-
         # scatter bookkeeping: format the index as a left-zero-padded string so that it'll sort
         # lexicographically in the desired order; bind the scatter variable name to the array value
         scatter_stack_i = scatter_stack
         if isinstance(array_i, Value.Base):
             assert isinstance(section, Tree.Scatter)
             str_i = str(i).zfill(digits)
             assert len(str_i) <= digits
```

### Comparing `miniwdl-1.9.0/docs/FAQ.md` & `miniwdl-1.9.1/docs/FAQ.md`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/Makefile` & `miniwdl-1.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/WDL.rst` & `miniwdl-1.9.1/docs/WDL.rst`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/add_functions.md` & `miniwdl-1.9.1/docs/add_functions.md`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/assert.md` & `miniwdl-1.9.1/docs/assert.md`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/check.rst` & `miniwdl-1.9.1/docs/check.rst`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/conf.py` & `miniwdl-1.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/getting_started.md` & `miniwdl-1.9.1/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/index.rst` & `miniwdl-1.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/miniwdl-logo.png` & `miniwdl-1.9.1/docs/miniwdl-logo.png`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/runner_advanced.md` & `miniwdl-1.9.1/docs/runner_advanced.md`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/runner_backends.md` & `miniwdl-1.9.1/docs/runner_backends.md`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/runner_reference.md` & `miniwdl-1.9.1/docs/runner_reference.md`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/trace_identifiers.md` & `miniwdl-1.9.1/docs/trace_identifiers.md`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/wdlviz.md` & `miniwdl-1.9.1/docs/wdlviz.md`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/wdlviz_ex1.png` & `miniwdl-1.9.1/docs/wdlviz_ex1.png`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/wdlviz_ex2.png` & `miniwdl-1.9.1/docs/wdlviz_ex2.png`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/docs/zip.rst` & `miniwdl-1.9.1/docs/zip.rst`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/examples/clean_download_cache.sh` & `miniwdl-1.9.1/examples/clean_download_cache.sh`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/examples/clean_download_cache.t` & `miniwdl-1.9.1/examples/clean_download_cache.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/examples/paste_wdl_imports.py` & `miniwdl-1.9.1/examples/paste_wdl_imports.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/examples/plugin_log_task_usage/miniwdl_log_task_usage.py` & `miniwdl-1.9.1/examples/plugin_log_task_usage/miniwdl_log_task_usage.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/examples/plugin_s3_progressive_upload/miniwdl_s3_progressive_upload.py` & `miniwdl-1.9.1/examples/plugin_s3_progressive_upload/miniwdl_s3_progressive_upload.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/examples/plugin_s3_progressive_upload/setup.py` & `miniwdl-1.9.1/examples/plugin_s3_progressive_upload/setup.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/examples/plugin_s3_progressive_upload/test.t` & `miniwdl-1.9.1/examples/plugin_s3_progressive_upload/test.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/examples/plugin_task_omnibus/miniwdl_task_omnibus_example.py` & `miniwdl-1.9.1/examples/plugin_task_omnibus/miniwdl_task_omnibus_example.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/examples/run_with_custom_error.py` & `miniwdl-1.9.1/examples/run_with_custom_error.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/examples/upload_output_files.sh` & `miniwdl-1.9.1/examples/upload_output_files.sh`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/examples/wdlviz.py` & `miniwdl-1.9.1/examples/wdlviz.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/miniwdl.egg-info/PKG-INFO` & `miniwdl-1.9.1/miniwdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniwdl
-Version: 1.9.0
+Version: 1.9.1
 Summary: Workflow Description Language (WDL) local runner & developer toolkit
 Home-page: https://github.com/chanzuckerberg/miniwdl
 Author: CZI
 Author-email: security@chanzuckerberg.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `miniwdl-1.9.0/miniwdl.egg-info/SOURCES.txt` & `miniwdl-1.9.1/miniwdl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 test_corpi/broadinstitute/gtex-pipeline
 test_corpi/broadinstitute/viral-ngs
 test_corpi/broadinstitute/warp
 test_corpi/contrived/check_quant.wdl
 test_corpi/contrived/contrived.wdl
 test_corpi/contrived/emptier.wdl
 test_corpi/contrived/empty.wdl
+test_corpi/contrived/env.wdl
 test_corpi/contrived/incomplete.wdl
 test_corpi/contrived/incomplete_call.wdl
 test_corpi/contrived/incomplete_import.wdl
 test_corpi/contrived/issue120.wdl
 test_corpi/contrived/issue596.wdl
 test_corpi/contrived/issue81.wdl
 test_corpi/contrived/issue82.wdl
```

### Comparing `miniwdl-1.9.0/setup.cfg` & `miniwdl-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/stubs/docker/__init__.py` & `miniwdl-1.9.1/stubs/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/stubs/regex/__init__.py` & `miniwdl-1.9.1/stubs/regex/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
     def sub(self, repl: str, string: str) -> str:
         ...
 
     def split(self, string: str) -> List[str]:
         ...
 
+    def search(self, string: str) -> Any:
+        ...
+
 def compile(pattern, flags=0, **kwargs) -> Pattern:
     ...
 
 def fullmatch(pat: str, string: str) -> Any:
     ...
 
 class Match:
```

### Comparing `miniwdl-1.9.0/test_corpi/contrived/contrived.wdl` & `miniwdl-1.9.1/test_corpi/contrived/contrived.wdl`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/test_corpi/contrived/issue596.wdl` & `miniwdl-1.9.1/test_corpi/contrived/issue596.wdl`

 * *Files 2% similar despite different names*

```diff
@@ -21,12 +21,11 @@
 }
 
 workflow w {
     input {
         File? f
     }
     call t {
-        input:
         s_in = f,
         struct1 = Struct1 { strings:[f, f] }
     }
 }
```

### Comparing `miniwdl-1.9.0/test_corpi/contrived/tricky_outputs.wdl` & `miniwdl-1.9.1/test_corpi/contrived/tricky_outputs.wdl`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/test_corpi/contrived/wdl1.1.wdl` & `miniwdl-1.9.1/test_corpi/contrived/wdl1.1.wdl`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/applied/DVGLx.t` & `miniwdl-1.9.1/tests/applied/DVGLx.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/applied/SARS-CoV-2.t` & `miniwdl-1.9.1/tests/applied/SARS-CoV-2.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/applied/encode_atac_seq.t` & `miniwdl-1.9.1/tests/applied/encode_atac_seq.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/applied/getting_started.t` & `miniwdl-1.9.1/tests/applied/getting_started.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/applied/skylab.py` & `miniwdl-1.9.1/tests/applied/skylab.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/applied/skylab_bulk_rna.t` & `miniwdl-1.9.1/tests/applied/skylab_bulk_rna.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/applied/viral_assemble.t` & `miniwdl-1.9.1/tests/applied/viral_assemble.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/applied/viral_refbased.t` & `miniwdl-1.9.1/tests/applied/viral_refbased.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/check.t` & `miniwdl-1.9.1/tests/check.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/eval.t` & `miniwdl-1.9.1/tests/eval.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/multi_line_strings.t` & `miniwdl-1.9.1/tests/multi_line_strings.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/multi_line_strings.wdl` & `miniwdl-1.9.1/tests/multi_line_strings.wdl`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/no_docker_services.py` & `miniwdl-1.9.1/tests/no_docker_services.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/podman.t` & `miniwdl-1.9.1/tests/podman.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/runner.t` & `miniwdl-1.9.1/tests/runner.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/singularity.t` & `miniwdl-1.9.1/tests/singularity.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/task_env_inputs.wdl` & `miniwdl-1.9.1/tests/task_env_inputs.wdl`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/test_0eval.py` & `miniwdl-1.9.1/tests/test_0eval.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/test_1doc.py` & `miniwdl-1.9.1/tests/test_1doc.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/test_2calls.py` & `miniwdl-1.9.1/tests/test_2calls.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/test_3corpi.py` & `miniwdl-1.9.1/tests/test_3corpi.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
         "_suppressions": 8,
         "UnusedImport": 4,
         "NameCollision": 27,
         "StringCoercion": 7,
         "FileCoercion": 3,
         "NonemptyCoercion": 1,
         "UnnecessaryQuantifier": 5,
-        "UnusedDeclaration": 2,
+        "UnusedDeclaration": 4,
         "IncompleteCall": 2,
         "SelectArray": 1,
         "MissingVersion": 7,
         "UnboundDeclaration": 1,
         "UnverifiedStruct": 3,
         "Deprecated": 2,
         "UnexpectedRuntimeValue": 1,
@@ -424,15 +424,15 @@
         "UnusedImport": 6,
         "NameCollision": 43,
         "StringCoercion": 13,
         "FileCoercion": 5,
         "OptionalCoercion": 10,
         "NonemptyCoercion": 2,
         "UnnecessaryQuantifier": 9,
-        "UnusedDeclaration": 9,
+        "UnusedDeclaration": 11,
         "IncompleteCall": 3,
         "ArrayCoercion": 2,
         "SelectArray": 4,
         "MissingVersion": 11,
         "UnboundDeclaration": 1,
         "UnverifiedStruct": 3,
         "Deprecated": 3,
```

### Comparing `miniwdl-1.9.0/tests/test_4taskrun.py` & `miniwdl-1.9.1/tests/test_4taskrun.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/test_5stdlib.py` & `miniwdl-1.9.1/tests/test_5stdlib.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/test_6workflowrun.py` & `miniwdl-1.9.1/tests/test_6workflowrun.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/test_7runner.py` & `miniwdl-1.9.1/tests/test_7runner.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/test_8cache.py` & `miniwdl-1.9.1/tests/test_8cache.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/test_cli_argcomplete.py` & `miniwdl-1.9.1/tests/test_cli_argcomplete.py`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/udocker.t` & `miniwdl-1.9.1/tests/udocker.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tests/zip.t` & `miniwdl-1.9.1/tests/zip.t`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tools_image/Dockerfile` & `miniwdl-1.9.1/tools_image/Dockerfile`

 * *Files identical despite different names*

### Comparing `miniwdl-1.9.0/tools_image/README.md` & `miniwdl-1.9.1/tools_image/README.md`

 * *Files identical despite different names*

