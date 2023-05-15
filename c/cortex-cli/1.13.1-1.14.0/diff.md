# Comparing `tmp/cortex_cli-1.13.1.tar.gz` & `tmp/cortex_cli-1.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_cli-1.13.1.tar", last modified: Fri May  5 19:39:55 2023, max compression
+gzip compressed data, was "cortex_cli-1.14.0.tar", last modified: Mon May 15 20:18:38 2023, max compression
```

## Comparing `cortex_cli-1.13.1.tar` & `cortex_cli-1.14.0.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5211 2023-05-02 16:03:43.000000 cortex_cli-1.13.1/README.md
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-05-05 19:39:44.000000 cortex_cli-1.13.1/cortex_cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.13.1/cortex_cli/cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/cli/api/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.1/cortex_cli/cli/api/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3992 2023-05-02 16:03:43.000000 cortex_cli-1.13.1/cortex_cli/cli/api/github_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.13.1/cortex_cli/cli/api/http_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.13.1/cortex_cli/cli/cli_api_base.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.13.1/cortex_cli/cli/cli_api_base_config.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.13.1/cortex_cli/cli/clients.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2027 2023-05-02 16:03:43.000000 cortex_cli-1.13.1/cortex_cli/cli/configure.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.13.1/cortex_cli/cli/cortex_cli.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.13.1/cortex_cli/cli/generic_get.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.13.1/cortex_cli/cli/inferences.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    24829 2023-05-05 19:39:27.000000 cortex_cli-1.13.1/cortex_cli/cli/models.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-07 17:56:26.000000 cortex_cli-1.13.1/cortex_cli/cli/pipelines.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/core/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.1/cortex_cli/core/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4182 2023-04-17 18:14:34.000000 cortex_cli-1.13.1/cortex_cli/core/cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.13.1/cortex_cli/core/drift_checks.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-04-17 18:14:34.000000 cortex_cli-1.13.1/cortex_cli/core/ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/core/mlflow/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.1/cortex_cli/core/mlflow/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.13.1/cortex_cli/core/mlflow/mlflow_cortex.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/core/models/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.1/cortex_cli/core/models/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-04-20 17:50:53.000000 cortex_cli-1.13.1/cortex_cli/core/models/cortex_model.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/core/secrets_manager.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/model_templates/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-05-02 16:03:43.000000 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      322 2023-05-05 19:39:27.000000 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-05-02 16:03:43.000000 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      455 2023-05-05 19:39:27.000000 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli/tests/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.1/cortex_cli/tests/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.13.1/cortex_cli/tests/test_cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.13.1/cortex_cli/tests/test_ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/cortex_cli.egg-info/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-05-05 19:39:55.000000 cortex_cli-1.13.1/cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3123 2023-05-05 19:39:55.000000 cortex_cli-1.13.1/cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-05-05 19:39:55.000000 cortex_cli-1.13.1/cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-05-05 19:39:55.000000 cortex_cli-1.13.1/cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-05-05 19:39:55.000000 cortex_cli-1.13.1/cortex_cli.egg-info/requires.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-05-05 19:39:55.000000 cortex_cli-1.13.1/cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.13.1/pyproject.toml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-05-05 19:39:55.090288 cortex_cli-1.13.1/setup.cfg
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1076 2023-04-25 18:48:24.000000 cortex_cli-1.13.1/setup.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5733 2023-05-15 20:17:46.000000 cortex_cli-1.14.0/README.md
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.472183 cortex_cli-1.14.0/cortex_cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-05-15 20:17:46.000000 cortex_cli-1.14.0/cortex_cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.14.0/cortex_cli/cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/cli/api/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.14.0/cortex_cli/cli/api/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3992 2023-05-02 16:03:43.000000 cortex_cli-1.14.0/cortex_cli/cli/api/github_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.14.0/cortex_cli/cli/api/http_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.14.0/cortex_cli/cli/cli_api_base.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.14.0/cortex_cli/cli/cli_api_base_config.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3505 2023-05-15 20:17:46.000000 cortex_cli-1.14.0/cortex_cli/cli/cli_multipart_upload.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.14.0/cortex_cli/cli/clients.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2027 2023-05-02 16:03:43.000000 cortex_cli-1.14.0/cortex_cli/cli/configure.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      973 2023-05-15 20:17:46.000000 cortex_cli-1.14.0/cortex_cli/cli/cortex_cli.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.14.0/cortex_cli/cli/generic_get.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.14.0/cortex_cli/cli/inferences.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    24626 2023-05-15 20:17:46.000000 cortex_cli-1.14.0/cortex_cli/cli/models.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3259 2023-05-15 20:17:46.000000 cortex_cli-1.14.0/cortex_cli/cli/pipelines.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/core/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.14.0/cortex_cli/core/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4182 2023-04-17 18:14:34.000000 cortex_cli-1.14.0/cortex_cli/core/cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.14.0/cortex_cli/core/drift_checks.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-04-17 18:14:34.000000 cortex_cli-1.14.0/cortex_cli/core/ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/core/mlflow/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.14.0/cortex_cli/core/mlflow/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.14.0/cortex_cli/core/mlflow/mlflow_cortex.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/core/models/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.14.0/cortex_cli/core/models/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-04-20 17:50:53.000000 cortex_cli-1.14.0/cortex_cli/core/models/cortex_model.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/core/secrets_manager.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/model_templates/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-05-02 16:03:43.000000 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      322 2023-05-05 19:39:27.000000 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.472183 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-05-02 16:03:43.000000 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      455 2023-05-05 19:39:27.000000 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.472183 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli/tests/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.14.0/cortex_cli/tests/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.14.0/cortex_cli/tests/test_cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.14.0/cortex_cli/tests/test_ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/cortex_cli.egg-info/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-05-15 20:18:38.000000 cortex_cli-1.14.0/cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3162 2023-05-15 20:18:38.000000 cortex_cli-1.14.0/cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-05-15 20:18:38.000000 cortex_cli-1.14.0/cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-05-15 20:18:38.000000 cortex_cli-1.14.0/cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-05-15 20:18:38.000000 cortex_cli-1.14.0/cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-05-15 20:18:38.000000 cortex_cli-1.14.0/cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.14.0/pyproject.toml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-05-15 20:18:38.482183 cortex_cli-1.14.0/setup.cfg
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1076 2023-04-25 18:48:24.000000 cortex_cli-1.14.0/setup.py
```

### Comparing `cortex_cli-1.13.1/README.md` & `cortex_cli-1.14.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -31,54 +31,58 @@
 cortex-cli [resource] [action] [parameters ...]
 ```
 
 Resources include configure, clients, models, pipelines, and inferences.
 Actions include get, list, and create.
 Parameters are action+resource specific.
 
+### Configure
+The profile for the CLI must be configured before use. An API key needs to be generated from the Settings page in the Cortex UI.
+```
+$ cortex-cli configure
+Profile [default]:
+API Url [https://api.nearlyhuman.ai]:
+API Key []: nh_asdfasdfasdf1341234
+```
+
 ### Client
-*NOTE*: the default client is `demo`.  This can be modified by passing in `-c CLENT_NAME` to all commands, or to set the ENV variable 'CLIENT' to the client key.
 
-*Get a List of Clients*
+#### Get a List of Clients
+The registered profile may only associate with one client.  The get command returns information about their client license, profile, and name.
 ```
-$ cortex-cli clients list
+$ cortex-cli clients get
 
 [{'_id': '6317eceaeef27d972e86b4ff',
   'clientKey': 'demo',
   'createdDate': '2022-09-07T00:59:22.582Z',
   'description': 'The Cortex Demo Client',
   'experimentId': '1',
   'licensePlan': 'enterprise',
   'name': 'Demo',
   'supportEmail': 'karl.haviland@nearlyhuman.ai',
   'supportPhone': '717-111-2222',
   'updatedDate': '2022-09-07T00:59:22.582Z',
   'website': 'https://www.nearlhuman.ai'}]
 ```
 
-*Get a Client by ID*
-```
-$ cortex-cli clients get -i 6317eceaeef27d972e86b4ff
+### Models
 
-{'_id': '6317eceaeef27d972e86b4ff',
- 'clientKey': 'demo',
- 'createdDate': '2022-09-07T00:59:22.582Z',
- 'description': 'The Cortex Demo Client',
- 'experimentId': '1',
- 'licensePlan': 'enterprise',
- 'name': 'Demo',
- 'supportEmail': 'karl.haviland@nearlyhuman.ai',
- 'supportPhone': '717-111-2222',
- 'updatedDate': '2022-09-07T00:59:22.582Z',
- 'website': 'https://www.nearlhuman.ai'}
+#### Initialize a New Model
+*NOTE:* Only needed if you want to both create a brand new Cortex ready model and automatically register it with the server.  Start from the workspace directory where the model repo is going to be created locally.
+```
+$ cortex-cli models init -n my-demo-name
+```
 
+#### Register a Model*
+*NOTE:* Only needed if you have an existing Cortex Github repository and you want to register it with the server. First, cd to the model's local directory.
+```
+$ cortex-cli models register -n "My Demo Model" -r my-demo-name
 ```
 
-### Models
-*Get a List of Models*
+#### Get a List of Models
 ```
 $ cortex-cli models list
 
 [{'_id': '632b32731d2faa4ffbade76d',
   'clientKey': 'demo',
   'createdDate': '2022-09-20T15:49:06.882Z',
   'description': 'A model that is initialized through the Cortex CLI.',
@@ -98,60 +102,88 @@
   'repo': 'nmci-chat-3',
   'tags': [],
   'updatedDate': '2022-09-21T17:03:57.365Z'},
  ...
  ]
 ```
 
-*Get a Model By ID*
+#### Get a Model By ID
 ```
 $ cortex-cli models get -i 632b32731d2faa4ffbade76d
 {'_id': '632b32731d2faa4ffbade76d',
  'clientKey': 'demo',
  'createdDate': '2022-09-20T15:49:06.882Z',
  'description': 'A model that is initialized through the Cortex CLI.',
  'experimentId': '1',
  'name': 'nmci-chat-2',
  'organization': 'nearlyhuman',
  'repo': 'nmci-chat-2',
  'tags': [],
  'updatedDate': '2022-09-20T15:49:06.882Z'}
 ```
 
-*Run a Model's Pipeline*
+#### Run a Model's Pipeline
 *NOTE:* First, cd to the model's local directory.  Use the `-t` flag to set tracking against the Cortex server.  Otherwise it will simply train locally.
+A pipeline is a series of steps that the model performs to transform and validate data, train, and store the model artifact.  This pipeline displays in the
+Cortex UI where it can be deployed. The steps that define the pipeline are located in the 
 ```
-~/nh-models/github/financialchat$ cortex-cli models run -t
+$ cortex-cli models run -t
    + Found the model financialchat
    + Did not find existing pipeline for branch main
    + Pipeline Pending with id: 642c68841368f765a05fdb38
                 Loading module financialchat from ./src/financialchat/financialchat.py
    + Loaded pipeline steps
    + Download data completed successfully
    + Fit model completed successfully
    + Evaluate model completed successfully
    + Cleanup model params completed successfully
    > Saving pipeline artifacts...
    + Saved the pipeline artifacts to disk: (models/cortex/642c68841368f765a05fdb38)
    > Packing conda environment...
 Collecting packages...
-Packing environment at '/home/mattgroho/mambaforge/envs/financial_chat' to 'models/cortex/642c68841368f765a05fdb38/environment.tar.gz'
+Packing environment at '/home/user/mambaforge/envs/financial_chat' to 'models/cortex/642c68841368f765a05fdb38/environment.tar.gz'
 [########################################] | 100% Completed | 13.7s
    + Packed conda environment to disk: (models/cortex/642c68841368f765a05fdb38)
    > Uploading pipeline artifacts to Cortex...
    + Uploaded the pipeline artifacts to Cortex
    + Completed Cortex Pipeline Run
 ```
 
-*Initialize a New Model*
-*NOTE:* Only needed if you want to both create a brand new Cortex ready model and automatically register it with the server.  Start from the workspace directory where the model repo is going to be created locally.
+### Pipelines
+
+#### Get a List of Pipelines
+
 ```
-$ cortex-cli models init -n demo-digits-predictions-karl
+$ cortex-cli pipelines list
+
 ```
 
-*Register a Model*
-*NOTE:* Only needed if you have an existing Cortex Github repository and you want to register it with the server. First, cd to the model's local directory.
+#### Get a Pipeline by ID
 ```
-$ cortex-cli models register -n "Financial Chat" -r financial-chat
+$ cortex-cli pipelines get -i 134123413412341234
+
 ```
 
-### Pipelines
+#### Deploy a Pipeline
+```
+$ cortex-cli pipelines deploy -i 134123413412341234
+
+```
+
+#### Undeploy a Pipeline
+```
+$ cortex-cli pipelines undeploy -i 134123413412341234
+
+```
+
+### Inferences
+#### Get a List of Inferences
+```
+$ cortex-cli inferences list
+
+```
+
+#### Get an Inference by ID
+```
+$ cortex-cli inferences get -i 134123413412341234
+
+```
```

### Comparing `cortex_cli-1.13.1/cortex_cli/cli/api/github_api.py` & `cortex_cli-1.14.0/cortex_cli/cli/api/github_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/cli/api/http_api.py` & `cortex_cli-1.14.0/cortex_cli/cli/api/http_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/cli/cli_api_base.py` & `cortex_cli-1.14.0/cortex_cli/cli/cli_api_base.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/cli/cli_api_base_config.py` & `cortex_cli-1.14.0/cortex_cli/cli/cli_api_base_config.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/cli/configure.py` & `cortex_cli-1.14.0/cortex_cli/cli/configure.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/cli/cortex_cli.py` & `cortex_cli-1.14.0/cortex_cli/cli/cortex_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from cortex_cli.cli.configure import ConfigureCli
 from cortex_cli.cli.clients import ClientsCli
 from cortex_cli.cli.generic_get import GetCli
 from cortex_cli.cli.inferences import InferencesCli
 from cortex_cli.cli.models import ModelsCli
 from cortex_cli.cli.pipelines import PipelinesCli
 
+
 class CortexCli(Application):
     VERSION = cortex_cli.__version__
 
 
 def main():
     CortexCli.subcommand('configure', ConfigureCli)
     CortexCli.subcommand('clients', ClientsCli)
```

### Comparing `cortex_cli-1.13.1/cortex_cli/cli/generic_get.py` & `cortex_cli-1.14.0/cortex_cli/cli/generic_get.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/cli/inferences.py` & `cortex_cli-1.14.0/cortex_cli/cli/inferences.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/cli/models.py` & `cortex_cli-1.14.0/cortex_cli/cli/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 import conda_pack
 import traceback
 import os
 import os.path
 import mlflow
 import yaml
 import sys
+from tqdm import tqdm
 import os, shutil
 import importlib
 from datetime import datetime
 from mlflow.models.signature import infer_signature
 from os import walk
 
 from cortex_cli.cli.cli_api_base import CliApiBase
+from cortex_cli.cli.cli_multipart_upload import MultipartUpload
 
 import cortex_cli.core.mlflow.mlflow_cortex as mlflow_cortex
 from cortex_cli.core.ethics_checks import EthicsResult
 from cortex_cli.core.drift_checks import DriftResult
 from cortex_cli import __version__
 
 
@@ -707,41 +709,29 @@
 
         return f'Packed conda environment to disk: ({self._artifacts_dir})'
 
 
     def _upload_pipeline(self):
         self._info('Uploading pipeline artifacts to Cortex...')
 
-        file_names = []
         file_paths = []
 
         # Get files from pipeline run
         for root, dirs, files in os.walk(self._artifacts_dir):
             for file in files:
-                file_names.append(file)
                 file_paths.append(os.path.join(root, file))
 
-        body = {
-            'fileNames': file_names
-        }
-        
-        # Obtain individual file upload urls
-        upload_urls = requests.post(
-            f'{self._api_url}/pipelines/{self._pipeline_id}/files/upload',
-            headers=self._headers,
-            json=body
-        ).json()
-
-        # Upload each file individually
-        for i in range(len(file_names)):
-            with open(file_paths[i], 'rb') as f:
-                requests.put(
-                    upload_urls[i],
-                    data=f
-                )
+        for i in tqdm(range(len(file_paths))):
+            uploadable_file = MultipartUpload(
+                path = file_paths[i], 
+                endpoint = f'{self._api_url}/pipelines/{self._pipeline_id}/files/multipart',
+                headers = self._headers
+            )
+            
+            uploadable_file.upload()
         
         return f'Uploaded the pipeline artifacts to Cortex'
 
 
     def _instantiate_model(self):
         # LOAD DEPENDENCY MODULES (except model)
         for path, module in self._modules.items():
```

### Comparing `cortex_cli-1.13.1/cortex_cli/cli/pipelines.py` & `cortex_cli-1.14.0/cortex_cli/cli/pipelines.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import plumbum.cli
 from cortex_cli.cli.cli_api_base import CliApiBase
 import requests
 import mlflow
 import traceback
```

### Comparing `cortex_cli-1.13.1/cortex_cli/core/cortex_data.py` & `cortex_cli-1.14.0/cortex_cli/core/cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/core/drift_checks.py` & `cortex_cli-1.14.0/cortex_cli/core/drift_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/core/ethics_checks.py` & `cortex_cli-1.14.0/cortex_cli/core/ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/core/mlflow/mlflow_cortex.py` & `cortex_cli-1.14.0/cortex_cli/core/mlflow/mlflow_cortex.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/core/models/cortex_model.py` & `cortex_cli-1.14.0/cortex_cli/core/models/cortex_model.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/core/secrets_manager.py` & `cortex_cli-1.14.0/cortex_cli/core/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/.gitignore` & `cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/README.md` & `cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.14.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/.gitignore` & `cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/README.md` & `cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.14.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/tests/test_cortex_data.py` & `cortex_cli-1.14.0/cortex_cli/tests/test_cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli/tests/test_ethics_checks.py` & `cortex_cli-1.14.0/cortex_cli/tests/test_ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.1/cortex_cli.egg-info/SOURCES.txt` & `cortex_cli-1.14.0/cortex_cli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 cortex_cli.egg-info/dependency_links.txt
 cortex_cli.egg-info/entry_points.txt
 cortex_cli.egg-info/requires.txt
 cortex_cli.egg-info/top_level.txt
 cortex_cli/cli/__init__.py
 cortex_cli/cli/cli_api_base.py
 cortex_cli/cli/cli_api_base_config.py
+cortex_cli/cli/cli_multipart_upload.py
 cortex_cli/cli/clients.py
 cortex_cli/cli/configure.py
 cortex_cli/cli/cortex_cli.py
 cortex_cli/cli/generic_get.py
 cortex_cli/cli/inferences.py
 cortex_cli/cli/models.py
 cortex_cli/cli/pipelines.py
```

### Comparing `cortex_cli-1.13.1/setup.py` & `cortex_cli-1.14.0/setup.py`

 * *Files identical despite different names*

